# Comparing `tmp/stela_professional-0.4.0.tar.gz` & `tmp/stela_professional-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stela_professional-0.4.0.tar", last modified: Mon Apr  8 13:37:42 2024, max compression
+gzip compressed data, was "stela_professional-0.4.1.tar", last modified: Sat Apr 20 13:21:44 2024, max compression
```

## Comparing `stela_professional-0.4.0.tar` & `stela_professional-0.4.1.tar`

### file list

```diff
@@ -1,429 +1,429 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:41.976605 stela_professional-0.4.0/
--rw-rw-rw-   0        0        0    35803 2024-01-15 04:02:49.000000 stela_professional-0.4.0/LICENSE
--rw-rw-rw-   0        0        0      133 2024-01-21 05:12:11.000000 stela_professional-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1268 2024-04-08 13:37:41.973604 stela_professional-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       25 2024-01-15 04:02:49.000000 stela_professional-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.498560 stela_professional-0.4.0/accounts/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.0/accounts/__init__.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.0/accounts/admin.py
--rw-rw-rw-   0        0        0      154 2024-01-15 04:02:49.000000 stela_professional-0.4.0/accounts/apps.py
--rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.0/accounts/forms.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.521010 stela_professional-0.4.0/accounts/migrations/
--rw-rw-rw-   0        0        0     4062 2024-01-22 13:09:35.000000 stela_professional-0.4.0/accounts/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-01-22 13:09:35.000000 stela_professional-0.4.0/accounts/migrations/__init__.py
--rw-rw-rw-   0        0        0     4862 2024-01-16 08:21:22.000000 stela_professional-0.4.0/accounts/models.py
--rw-rw-rw-   0        0        0       63 2024-01-15 04:02:49.000000 stela_professional-0.4.0/accounts/tests.py
--rw-rw-rw-   0        0        0      370 2024-01-15 04:02:49.000000 stela_professional-0.4.0/accounts/token.py
--rw-rw-rw-   0        0        0     1836 2024-01-15 04:02:49.000000 stela_professional-0.4.0/accounts/urls.py
--rw-rw-rw-   0        0        0    10979 2024-01-15 04:02:49.000000 stela_professional-0.4.0/accounts/views.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.552075 stela_professional-0.4.0/cloud/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.0/cloud/__init__.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.0/cloud/admin.py
--rw-rw-rw-   0        0        0      148 2024-01-15 04:02:49.000000 stela_professional-0.4.0/cloud/apps.py
--rw-rw-rw-   0        0        0     3456 2024-01-15 04:02:49.000000 stela_professional-0.4.0/cloud/cart.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.557075 stela_professional-0.4.0/cloud/migrations/
--rw-rw-rw-   0        0        0     5564 2024-01-22 13:10:00.000000 stela_professional-0.4.0/cloud/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-01-22 13:10:00.000000 stela_professional-0.4.0/cloud/migrations/__init__.py
--rw-rw-rw-   0        0        0     3508 2024-01-15 04:02:49.000000 stela_professional-0.4.0/cloud/models.py
--rw-rw-rw-   0        0        0       63 2024-01-15 04:02:49.000000 stela_professional-0.4.0/cloud/tests.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.0/cloud/views.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.576755 stela_professional-0.4.0/geolocation/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.0/geolocation/__init__.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.0/geolocation/admin.py
--rw-rw-rw-   0        0        0      160 2024-01-15 04:02:49.000000 stela_professional-0.4.0/geolocation/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.583750 stela_professional-0.4.0/geolocation/migrations/
--rw-rw-rw-   0        0        0     6403 2024-01-22 13:10:12.000000 stela_professional-0.4.0/geolocation/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-01-22 13:10:12.000000 stela_professional-0.4.0/geolocation/migrations/__init__.py
--rw-rw-rw-   0        0        0      582 2024-01-15 04:02:49.000000 stela_professional-0.4.0/geolocation/models.py
--rw-rw-rw-   0        0        0       63 2024-01-15 04:02:49.000000 stela_professional-0.4.0/geolocation/tests.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.0/geolocation/views.py
--rw-rw-rw-   0        0        0       42 2024-04-08 13:37:41.977604 stela_professional-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1448 2024-04-08 13:35:35.000000 stela_professional-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.656732 stela_professional-0.4.0/stela_control/
--rw-rw-rw-   0        0        0        0 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/__init__.py
--rw-rw-rw-   0        0        0       34 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/admin.py
--rw-rw-rw-   0        0        0      163 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/apps.py
--rw-rw-rw-   0        0        0     7527 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/cart.py
--rw-rw-rw-   0        0        0      164 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/context_processors.py
--rw-rw-rw-   0        0        0      316 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/cron.py
--rw-rw-rw-   0        0        0    85813 2024-03-05 11:43:43.000000 stela_professional-0.4.0/stela_control/forms.py
--rw-rw-rw-   0        0        0      181 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.206530 stela_professional-0.4.0/stela_control/locale/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.207529 stela_professional-0.4.0/stela_control/locale/es/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.701704 stela_professional-0.4.0/stela_control/locale/es/LC_MESSAGES/
--rw-rw-rw-   0        0        0    55259 2024-02-19 18:04:13.000000 stela_professional-0.4.0/stela_control/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0   332194 2024-02-19 18:03:02.000000 stela_professional-0.4.0/stela_control/locale/es/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.792649 stela_professional-0.4.0/stela_control/migrations/
--rw-rw-rw-   0        0        0    89195 2024-01-22 13:10:23.000000 stela_professional-0.4.0/stela_control/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     5384 2024-01-22 16:02:46.000000 stela_professional-0.4.0/stela_control/migrations/0002_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     6120 2024-01-22 19:38:17.000000 stela_professional-0.4.0/stela_control/migrations/0003_rename_description_company_content_and_more.py
--rw-rw-rw-   0        0        0     5640 2024-01-22 21:09:07.000000 stela_professional-0.4.0/stela_control/migrations/0004_alter_billingrecipt_option_alter_company_address_and_more.py
--rw-rw-rw-   0        0        0     5424 2024-01-22 22:24:05.000000 stela_professional-0.4.0/stela_control/migrations/0005_rename_description_team_content_and_more.py
--rw-rw-rw-   0        0        0     7730 2024-01-31 12:37:18.000000 stela_professional-0.4.0/stela_control/migrations/0006_alter_bankstatement_bank_and_more.py
--rw-rw-rw-   0        0        0     5121 2024-01-31 16:03:17.000000 stela_professional-0.4.0/stela_control/migrations/0007_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     5644 2024-02-05 01:43:23.000000 stela_professional-0.4.0/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     5171 2024-02-05 07:46:11.000000 stela_professional-0.4.0/stela_control/migrations/0009_content_video_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     4962 2024-02-06 05:55:50.000000 stela_professional-0.4.0/stela_control/migrations/0010_resource_category_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     6460 2024-02-06 15:43:12.000000 stela_professional-0.4.0/stela_control/migrations/0011_resource_cover_taxid_pdf_file2_and_more.py
--rw-rw-rw-   0        0        0     5640 2024-02-06 17:11:41.000000 stela_professional-0.4.0/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     5323 2024-02-19 17:38:39.000000 stela_professional-0.4.0/stela_control/migrations/0013_content_cover_content_fecade_url_and_more.py
--rw-rw-rw-   0        0        0     5891 2024-02-20 23:29:50.000000 stela_professional-0.4.0/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     5039 2024-02-21 15:45:43.000000 stela_professional-0.4.0/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0        0 2024-01-22 13:10:23.000000 stela_professional-0.4.0/stela_control/migrations/__init__.py
--rw-rw-rw-   0        0        0    71703 2024-02-21 15:44:07.000000 stela_professional-0.4.0/stela_control/models.py
--rw-rw-rw-   0        0        0     2943 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/routers.py
--rw-rw-rw-   0        0        0   179088 2024-02-27 00:29:11.000000 stela_professional-0.4.0/stela_control/superfunctions.py
--rw-rw-rw-   0        0        0      410 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/tasks.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.210528 stela_professional-0.4.0/stela_control/templates/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:32.453751 stela_professional-0.4.0/stela_control/templates/stela_control/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:32.524709 stela_professional-0.4.0/stela_control/templates/stela_control/accounts/
--rw-rw-rw-   0        0        0      497 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/accounts/base.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:32.697476 stela_professional-0.4.0/stela_control/templates/stela_control/accounts/registration/
--rw-rw-rw-   0        0        0      227 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/accounts/registration/account_activation_email.html
--rw-rw-rw-   0        0        0       21 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/accounts/registration/activation_invalid.html
--rw-rw-rw-   0        0        0     1373 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/accounts/registration/confirmation_email.html
--rw-rw-rw-   0        0        0     3071 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/accounts/registration/register.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:33.085188 stela_professional-0.4.0/stela_control/templates/stela_control/accounts/user/
--rw-rw-rw-   0        0        0     1364 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/accounts/user/delete_user.html
--rw-rw-rw-   0        0        0     2956 2024-02-06 18:30:10.000000 stela_professional-0.4.0/stela_control/templates/stela_control/accounts/user/login.html
--rw-rw-rw-   0        0        0     2692 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html
--rw-rw-rw-   0        0        0     2043 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/accounts/user/password_reset_done.html
--rw-rw-rw-   0        0        0      629 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/accounts/user/password_reset_email.html
--rw-rw-rw-   0        0        0     2424 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/accounts/user/password_reset_form.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:33.118166 stela_professional-0.4.0/stela_control/templates/stela_control/analytics/
--rw-rw-rw-   0        0        0      757 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/analytics/analytics.html
--rw-rw-rw-   0        0        0      527 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/analytics/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:33.143151 stela_professional-0.4.0/stela_control/templates/stela_control/api/
--rw-rw-rw-   0        0        0     5932 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/api/main.html
--rw-rw-rw-   0        0        0     2883 2024-01-21 23:59:12.000000 stela_professional-0.4.0/stela_control/templates/stela_control/base.html
--rw-rw-rw-   0        0        0     4402 2024-01-22 14:53:11.000000 stela_professional-0.4.0/stela_control/templates/stela_control/base_content.html
--rw-rw-rw-   0        0        0     6768 2024-01-20 15:13:41.000000 stela_professional-0.4.0/stela_control/templates/stela_control/base_list.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:33.286063 stela_professional-0.4.0/stela_control/templates/stela_control/billing/
--rw-rw-rw-   0        0        0   253007 2024-03-18 11:50:23.000000 stela_professional-0.4.0/stela_control/templates/stela_control/billing/homebrew.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:33.828673 stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/
--rw-rw-rw-   0        0        0     1443 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/bill-data-customer.html
--rw-rw-rw-   0        0        0    30854 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/checkout.html
--rw-rw-rw-   0        0        0      906 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/data-customer.html
--rw-rw-rw-   0        0        0    56802 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/invoice-copy.html
--rw-rw-rw-   0        0        0    56693 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/invoice.html
--rw-rw-rw-   0        0        0     2875 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/order-placed.html
--rw-rw-rw-   0        0        0    48021 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/preview-recipt.html
--rw-rw-rw-   0        0        0     2750 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html
--rw-rw-rw-   0        0        0     3336 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/recipt-detail.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:33.910621 stela_professional-0.4.0/stela_control/templates/stela_control/booking-control/
--rw-rw-rw-   0        0        0     1992 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/booking-control/customer-detail.html
--rw-rw-rw-   0        0        0     4067 2024-01-22 14:58:02.000000 stela_professional-0.4.0/stela_control/templates/stela_control/booking-control/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:33.974581 stela_professional-0.4.0/stela_control/templates/stela_control/chatstela/
--rw-rw-rw-   0        0        0    30842 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/templates/stela_control/chatstela/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:34.124578 stela_professional-0.4.0/stela_control/templates/stela_control/content/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:34.180545 stela_professional-0.4.0/stela_control/templates/stela_control/content/comments/
--rw-rw-rw-   0        0        0     2254 2024-01-20 22:35:04.000000 stela_professional-0.4.0/stela_control/templates/stela_control/content/comments/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:34.226008 stela_professional-0.4.0/stela_control/templates/stela_control/content/docs/
--rw-rw-rw-   0        0        0    10531 2024-02-05 01:03:29.000000 stela_professional-0.4.0/stela_control/templates/stela_control/content/docs/main.html
--rw-rw-rw-   0        0        0     7438 2024-02-06 18:40:47.000000 stela_professional-0.4.0/stela_control/templates/stela_control/content/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:34.263984 stela_professional-0.4.0/stela_control/templates/stela_control/content/main/
--rw-rw-rw-   0        0        0     1003 2024-02-20 02:42:20.000000 stela_professional-0.4.0/stela_control/templates/stela_control/content/main/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:34.314954 stela_professional-0.4.0/stela_control/templates/stela_control/content/staff/
--rw-rw-rw-   0        0        0     7608 2024-02-05 04:12:54.000000 stela_professional-0.4.0/stela_control/templates/stela_control/content/staff/index.html
--rw-rw-rw-   0        0        0    26830 2024-02-23 19:08:09.000000 stela_professional-0.4.0/stela_control/templates/stela_control/content/stelastory.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:34.367921 stela_professional-0.4.0/stela_control/templates/stela_control/developer/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:34.567797 stela_professional-0.4.0/stela_control/templates/stela_control/developer/data-update/
--rw-rw-rw-   0        0        0      933 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/developer/data-update/modal1.html
--rw-rw-rw-   0        0        0      898 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/developer/data-update/modal2.html
--rw-rw-rw-   0        0        0      900 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/developer/data-update/modal3.html
--rw-rw-rw-   0        0        0      875 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/developer/data-update/modal4.html
--rw-rw-rw-   0        0        0    46793 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/developer/home.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.268564 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:34.610771 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/accounts/
--rw-rw-rw-   0        0        0      413 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/accounts/password_reset_email.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:34.743689 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/billing/
--rw-rw-rw-   0        0        0    21938 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html
--rw-rw-rw-   0        0        0    21903 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/billing/invoice.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:34.856392 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/contact/
--rw-rw-rw-   0        0        0    20096 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/contact/message_notification.html
--rw-rw-rw-   0        0        0     8454 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/contact/support_notification.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:34.902363 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/marketing/
--rw-rw-rw-   0        0        0    60992 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:34.931346 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/newsletter/
--rw-rw-rw-   0        0        0    21461 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:34.971321 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/orders/
--rw-rw-rw-   0        0        0    10226 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:35.195182 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/payments/
--rw-rw-rw-   0        0        0    27770 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/payments/billing_payment.html
--rw-rw-rw-   0        0        0     6930 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/payments/charges.html
--rw-rw-rw-   0        0        0    20151 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/payments/payment_notification.html
--rw-rw-rw-   0        0        0    20151 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/payments/sale_notification.html
--rw-rw-rw-   0        0        0     7266 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html
--rw-rw-rw-   0        0        0     7166 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/payments/withdrawals.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:35.221167 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/support/
--rw-rw-rw-   0        0        0    20072 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/support/support_notification.html
--rw-rw-rw-   0        0        0    22345 2024-02-23 19:07:47.000000 stela_professional-0.4.0/stela_control/templates/stela_control/home.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:35.266139 stela_professional-0.4.0/stela_control/templates/stela_control/inbox/
--rw-rw-rw-   0        0        0     2272 2024-01-21 15:59:26.000000 stela_professional-0.4.0/stela_control/templates/stela_control/inbox/index.html
--rw-rw-rw-   0        0        0    11555 2024-02-03 04:29:28.000000 stela_professional-0.4.0/stela_control/templates/stela_control/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.272564 stela_professional-0.4.0/stela_control/templates/stela_control/inventory/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:35.280131 stela_professional-0.4.0/stela_control/templates/stela_control/inventory/products/
--rw-rw-rw-   0        0        0        0 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/inventory/products/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:35.405055 stela_professional-0.4.0/stela_control/templates/stela_control/inventory/resources/
--rw-rw-rw-   0        0        0     2888 2024-01-18 21:03:25.000000 stela_professional-0.4.0/stela_control/templates/stela_control/inventory/resources/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:35.662894 stela_professional-0.4.0/stela_control/templates/stela_control/inventory/services/
--rw-rw-rw-   0        0        0     6806 2024-02-27 00:40:42.000000 stela_professional-0.4.0/stela_control/templates/stela_control/inventory/services/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:35.866770 stela_professional-0.4.0/stela_control/templates/stela_control/jobs/
--rw-rw-rw-   0        0        0     2265 2024-01-22 15:22:45.000000 stela_professional-0.4.0/stela_control/templates/stela_control/jobs/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:36.475130 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:36.550070 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/aboutemmerut/
--rw-rw-rw-   0        0        0     1694 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:36.590571 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/aboutsecondary/
--rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:36.609558 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/aboutstela/
--rw-rw-rw-   0        0        0     1381 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/aboutstela/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:36.780015 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/alerts/
--rw-rw-rw-   0        0        0      444 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/alerts/budget-alert.html
--rw-rw-rw-   0        0        0      384 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/alerts/budget-success.html
--rw-rw-rw-   0        0        0      404 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/alerts/cancel-recipt.html
--rw-rw-rw-   0        0        0      445 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/alerts/invoice-alert.html
--rw-rw-rw-   0        0        0      380 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/alerts/invoice-success.html
--rw-rw-rw-   0        0        0      471 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/alerts/payeed-recipt.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:36.799715 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/appstela/
--rw-rw-rw-   0        0        0     1806 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/appstela/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.283558 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/auth/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:36.825699 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/auth/pw_reset/
--rw-rw-rw-   0        0        0       45 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/auth/pw_reset/form_errors.html
--rw-rw-rw-   0        0        0      220 2024-01-20 02:10:43.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/auth/pw_reset/password_reset_form.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:36.846133 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/auth/signup/
--rw-rw-rw-   0        0        0      794 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html
--rw-rw-rw-   0        0        0      269 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/auth/signup/success_register.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:36.949076 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/billing/
--rw-rw-rw-   0        0        0     6947 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/billing/form-billing.html
--rw-rw-rw-   0        0        0    40487 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/billing/recipt-data.html
--rw-rw-rw-   0        0        0     3005 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/blog-feed.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:37.001575 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/categories/
--rw-rw-rw-   0        0        0      834 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/categories/modal4.html
--rw-rw-rw-   0        0        0      826 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/chatbox.html
--rw-rw-rw-   0        0        0      925 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/chatbox2.html
--rw-rw-rw-   0        0        0      143 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/city_data.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:37.022783 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/colors/
--rw-rw-rw-   0        0        0      857 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/colors/modal2.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:37.085863 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/contact/
--rw-rw-rw-   0        0        0     1088 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/contact/form.html
--rw-rw-rw-   0        0        0     1606 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/contact/modal.html
--rw-rw-rw-   0        0        0     1638 2024-01-22 20:05:28.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/dynamic-formset.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:37.106464 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/emmerutfooter/
--rw-rw-rw-   0        0        0     2233 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:37.162738 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/emmerutservices/
--rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html
--rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html
--rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html
--rw-rw-rw-   0        0        0      841 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/form-base.html
--rw-rw-rw-   0        0        0       64 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/form-errors.html
--rw-rw-rw-   0        0        0      924 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/formset-base-services.html
--rw-rw-rw-   0        0        0     1790 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/formset-base.html
--rw-rw-rw-   0        0        0     1569 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/formset.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.289555 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/handlers/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:37.238465 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/handlers/blog/
--rw-rw-rw-   0        0        0     1469 2024-01-30 20:17:44.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages-v1.html
--rw-rw-rw-   0        0        0      128 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/handlers/blog/empty-blog.html
--rw-rw-rw-   0        0        0      103 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/hashtags.html
--rw-rw-rw-   0        0        0      587 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/instagram-alert.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:37.275705 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/inventory/
--rw-rw-rw-   0        0        0     1778 2024-02-26 17:25:31.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:37.289696 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/job-application/
--rw-rw-rw-   0        0        0       45 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/job-application/error-form-v1.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:37.324067 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/linkzoneupdates/
--rw-rw-rw-   0        0        0      848 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.298550 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:37.810450 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/
--rw-rw-rw-   0        0        0     1067 2024-02-23 15:58:42.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html
--rw-rw-rw-   0        0        0     1467 2024-02-23 16:29:50.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html
--rw-rw-rw-   0        0        0     1650 2024-02-23 18:05:44.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html
--rw-rw-rw-   0        0        0     2732 2024-02-23 18:06:01.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html
--rw-rw-rw-   0        0        0     2540 2024-02-26 13:05:43.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html
--rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:06.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html
--rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:10.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html
--rw-rw-rw-   0        0        0     2887 2024-02-23 18:06:18.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html
--rw-rw-rw-   0        0        0     2593 2024-02-23 18:06:24.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html
--rw-rw-rw-   0        0        0     2296 2024-02-23 18:06:30.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html
--rw-rw-rw-   0        0        0     1639 2024-02-23 18:06:35.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html
--rw-rw-rw-   0        0        0     2587 2024-02-26 13:34:25.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:38.077163 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/
--rw-rw-rw-   0        0        0     1614 2024-02-23 18:04:43.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html
--rw-rw-rw-   0        0        0     3292 2024-02-23 18:04:45.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html
--rw-rw-rw-   0        0        0     3051 2024-02-23 18:04:50.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html
--rw-rw-rw-   0        0        0     1936 2024-02-23 18:04:55.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html
--rw-rw-rw-   0        0        0     2198 2024-02-23 18:05:01.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html
--rw-rw-rw-   0        0        0     2866 2024-02-23 18:05:07.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html
--rw-rw-rw-   0        0        0     2737 2024-02-23 18:05:12.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html
--rw-rw-rw-   0        0        0     2418 2024-02-23 18:05:17.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html
--rw-rw-rw-   0        0        0     1412 2024-02-23 18:07:47.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html
--rw-rw-rw-   0        0        0     2803 2024-02-23 18:05:27.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html
--rw-rw-rw-   0        0        0     1297 2024-02-23 15:56:06.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html
--rw-rw-rw-   0        0        0     1778 2024-02-23 16:29:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:38.372814 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/
--rw-rw-rw-   0        0        0     1069 2024-02-23 15:58:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html
--rw-rw-rw-   0        0        0     1464 2024-02-23 16:29:44.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html
--rw-rw-rw-   0        0        0     1962 2024-02-23 18:06:50.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html
--rw-rw-rw-   0        0        0     3022 2024-02-23 18:06:54.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html
--rw-rw-rw-   0        0        0     2878 2024-02-26 13:33:54.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html
--rw-rw-rw-   0        0        0     1740 2024-02-23 18:07:07.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html
--rw-rw-rw-   0        0        0     2080 2024-02-23 18:07:11.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html
--rw-rw-rw-   0        0        0     3148 2024-02-23 18:07:16.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html
--rw-rw-rw-   0        0        0     2631 2024-02-23 18:07:22.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html
--rw-rw-rw-   0        0        0     2489 2024-02-23 18:07:28.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html
--rw-rw-rw-   0        0        0     1929 2024-02-23 18:07:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html
--rw-rw-rw-   0        0        0     2616 2024-02-26 14:03:38.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:38.531734 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:38.572777 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/community/
--rw-rw-rw-   0        0        0      818 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/community/formdata.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:38.597455 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/content-pro-media/
--rw-rw-rw-   0        0        0     3209 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:38.672593 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/content-pro-update/
--rw-rw-rw-   0        0        0       83 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/content-pro-update/content.html
--rw-rw-rw-   0        0        0       84 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/content-pro-update/schedule.html
--rw-rw-rw-   0        0        0      986 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:38.696993 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ic-update/
--rw-rw-rw-   0        0        0      469 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ic-update/content.html
--rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:38.791276 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ig-analythics/
--rw-rw-rw-   0        0        0    25077 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html
--rw-rw-rw-   0        0        0     1667 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html
--rw-rw-rw-   0        0        0     1530 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html
--rw-rw-rw-   0        0        0     1849 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html
--rw-rw-rw-   0        0        0     1774 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html
--rw-rw-rw-   0        0        0     4485 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html
--rw-rw-rw-   0        0        0     5787 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:38.816260 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/meta-assets/
--rw-rw-rw-   0        0        0        0 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page-alert.html
--rw-rw-rw-   0        0        0      628 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:38.888216 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/page-analythics/
--rw-rw-rw-   0        0        0     1755 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html
--rw-rw-rw-   0        0        0     1960 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html
--rw-rw-rw-   0        0        0     1428 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:38.906901 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/smart-boost/
--rw-rw-rw-   0        0        0     2129 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:38.918897 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/stela-sight/
--rw-rw-rw-   0        0        0      268 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/stela-sight/data.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:38.976135 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/newcomer/
--rw-rw-rw-   0        0        0     4162 2024-02-06 04:01:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/newcomer/form.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.000644 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/newsletter/
--rw-rw-rw-   0        0        0      216 2024-01-31 02:03:43.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/newsletter/form.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.033412 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/post/
--rw-rw-rw-   0        0        0      846 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/post/list-modal.html
--rw-rw-rw-   0        0        0      850 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/post/main-modal.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.082320 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/
--rw-rw-rw-   0        0        0     1824 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/catalog-modal.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.193792 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/new/
--rw-rw-rw-   0        0        0      933 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/new/catalog-form.html
--rw-rw-rw-   0        0        0      872 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/new/category-form.html
--rw-rw-rw-   0        0        0      888 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/new/color-form.html
--rw-rw-rw-   0        0        0     1024 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/new/product-form.html
--rw-rw-rw-   0        0        0      855 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/new/size-form.html
--rw-rw-rw-   0        0        0      115 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/new/variant-form.html
--rw-rw-rw-   0        0        0      805 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/product-modal.html
--rw-rw-rw-   0        0        0      848 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/size-modal.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.318353 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/update/
--rw-rw-rw-   0        0        0      234 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/update/catalog-form.html
--rw-rw-rw-   0        0        0      287 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/update/category-form.html
--rw-rw-rw-   0        0        0      230 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/update/color-form.html
--rw-rw-rw-   0        0        0     1008 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/update/product-form.html
--rw-rw-rw-   0        0        0      228 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/update/size-form.html
--rw-rw-rw-   0        0        0      234 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/update/variant-form.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.356331 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/profile/
--rw-rw-rw-   0        0        0     1306 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/profile/dynamic-form.html
--rw-rw-rw-   0        0        0      200 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/profile/single-form.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.392387 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/projects/
--rw-rw-rw-   0        0        0     1698 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/projects/modal.html
--rw-rw-rw-   0        0        0      265 2024-01-18 10:44:28.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/remove-complete.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.424035 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/render/
--rw-rw-rw-   0        0        0      143 2024-01-21 14:42:59.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/render/city_data.html
--rw-rw-rw-   0        0        0      604 2024-01-18 10:28:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/single-form.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.324532 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.458064 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/
--rw-rw-rw-   0        0        0     1099 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html
--rw-rw-rw-   0        0        0     1265 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.495462 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/error_forms/
--rw-rw-rw-   0        0        0     1099 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html
--rw-rw-rw-   0        0        0     1265 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.561600 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/forms/
--rw-rw-rw-   0        0        0     1269 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html
--rw-rw-rw-   0        0        0     1097 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html
--rw-rw-rw-   0        0        0     1265 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.624164 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/update_forms/
--rw-rw-rw-   0        0        0     1156 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html
--rw-rw-rw-   0        0        0     1320 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.649263 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/staff/
--rw-rw-rw-   0        0        0     1947 2024-01-18 10:28:34.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/staff/form.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.729183 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/stela_story/
--rw-rw-rw-   0        0        0     3418 2024-02-21 15:38:13.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/stela_story/feed-item.html
--rw-rw-rw-   0        0        0     2001 2024-01-18 10:28:39.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.748350 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/stelafooter/
--rw-rw-rw-   0        0        0     2176 2024-01-18 10:28:39.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/stelafooter/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.769341 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/stelamedia/
--rw-rw-rw-   0        0        0     1695 2024-01-18 10:28:39.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/stelamedia/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.788740 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/stelapath/
--rw-rw-rw-   0        0        0     1337 2024-01-18 10:28:39.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/stelapath/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.862321 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/tables/
--rw-rw-rw-   0        0        0      663 2024-01-22 15:21:03.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/tables/bank_statements.html
--rw-rw-rw-   0        0        0      675 2024-01-22 15:22:21.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/tables/invoices.html
--rw-rw-rw-   0        0        0      675 2024-01-22 15:22:25.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/tables/retentions.html
--rw-rw-rw-   0        0        0      630 2024-01-22 15:21:30.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/tables/tax-return.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:39.880849 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/users/
--rw-rw-rw-   0        0        0      254 2024-01-19 18:04:36.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/users/suspend.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:40.018762 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/youtube/
--rw-rw-rw-   0        0        0      157 2024-01-18 10:28:39.000000 stela_professional-0.4.0/stela_control/templates/stela_control/load-data/youtube/video-preview.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.352042 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:40.093189 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/email-marketing/
--rw-rw-rw-   0        0        0     1543 2024-01-20 22:43:07.000000 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/email-marketing/email_list.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:40.429509 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/
--rw-rw-rw-   0        0        0    10789 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:31.356007 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/instagram/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:40.754346 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/
--rw-rw-rw-   0        0        0    13445 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:40.785388 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/
--rw-rw-rw-   0        0        0    23333 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:40.854801 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/
--rw-rw-rw-   0        0        0    34272 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:40.889016 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/page/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:40.936931 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/page/community/
--rw-rw-rw-   0        0        0    14156 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:41.033871 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/
--rw-rw-rw-   0        0        0    30243 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html
--rw-rw-rw-   0        0        0      248 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/update.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:41.059858 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/
--rw-rw-rw-   0        0        0     3162 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html
--rw-rw-rw-   0        0        0    12633 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html
--rw-rw-rw-   0        0        0    17640 2024-01-22 19:37:49.000000 stela_professional-0.4.0/stela_control/templates/stela_control/newcomer.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:41.136700 stela_professional-0.4.0/stela_control/templates/stela_control/orders/
--rw-rw-rw-   0        0        0     6171 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/orders/list_view.html
--rw-rw-rw-   0        0        0     8860 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/orders/order_update.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:41.280172 stela_professional-0.4.0/stela_control/templates/stela_control/payments/
--rw-rw-rw-   0        0        0    43167 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/payments/homebrew.html
--rw-rw-rw-   0        0        0     2687 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/payments/register-wallet.html
--rw-rw-rw-   0        0        0     4322 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/payments/wallet-list.html
--rw-rw-rw-   0        0        0     2831 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/payments/withdraw.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:41.302158 stela_professional-0.4.0/stela_control/templates/stela_control/prostela/
--rw-rw-rw-   0        0        0      153 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/prostela/chatbox.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:41.327897 stela_professional-0.4.0/stela_control/templates/stela_control/prostela-expert/
--rw-rw-rw-   0        0        0    34014 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/prostela-expert/index.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:41.358410 stela_professional-0.4.0/stela_control/templates/stela_control/reviews/
--rw-rw-rw-   0        0        0     2269 2024-01-20 22:29:12.000000 stela_professional-0.4.0/stela_control/templates/stela_control/reviews/reviews.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:41.396393 stela_professional-0.4.0/stela_control/templates/stela_control/support/
--rw-rw-rw-   0        0        0     6350 2024-01-18 22:16:16.000000 stela_professional-0.4.0/stela_control/templates/stela_control/support/case-detail.html
--rw-rw-rw-   0        0        0     2323 2024-01-18 14:01:39.000000 stela_professional-0.4.0/stela_control/templates/stela_control/support/list.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:41.861609 stela_professional-0.4.0/stela_control/templates/stela_control/users/
--rw-rw-rw-   0        0        0      339 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templates/stela_control/users/generic-user-handler.html
--rw-rw-rw-   0        0        0    11181 2024-01-22 21:22:30.000000 stela_professional-0.4.0/stela_control/templates/stela_control/users/profile.html
--rw-rw-rw-   0        0        0    12343 2024-02-06 16:52:33.000000 stela_professional-0.4.0/stela_control/templates/stela_control/users/users-control.html
--rw-rw-rw-   0        0        0     6472 2024-02-06 15:00:39.000000 stela_professional-0.4.0/stela_control/templates/stela_control/users/users.html
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:41.897585 stela_professional-0.4.0/stela_control/templatetags/
--rw-rw-rw-   0        0        0        0 2024-01-18 10:28:40.000000 stela_professional-0.4.0/stela_control/templatetags/__init__.py
--rw-rw-rw-   0        0        0     1428 2024-04-08 13:35:26.000000 stela_professional-0.4.0/stela_control/templatetags/stelatags.py
--rw-rw-rw-   0        0        0      507 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/tests.py
--rw-rw-rw-   0        0        0     1131 2024-01-18 10:28:32.000000 stela_professional-0.4.0/stela_control/tokenize.py
--rw-rw-rw-   0        0        0     7442 2024-02-20 00:40:50.000000 stela_professional-0.4.0/stela_control/urls.py
--rw-rw-rw-   0        0        0   270343 2024-03-18 11:42:47.000000 stela_professional-0.4.0/stela_control/views.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:37:41.941737 stela_professional-0.4.0/stela_professional.egg-info/
--rw-rw-rw-   0        0        0     1268 2024-04-08 13:37:29.000000 stela_professional-0.4.0/stela_professional.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    20476 2024-04-08 13:37:30.000000 stela_professional-0.4.0/stela_professional.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 13:37:29.000000 stela_professional-0.4.0/stela_professional.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      384 2024-04-08 13:37:29.000000 stela_professional-0.4.0/stela_professional.egg-info/requires.txt
--rw-rw-rw-   0        0        0       41 2024-04-08 13:37:29.000000 stela_professional-0.4.0/stela_professional.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:44.283244 stela_professional-0.4.1/
+-rw-rw-rw-   0        0        0    35803 2024-01-15 04:02:49.000000 stela_professional-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0      133 2024-01-21 05:12:11.000000 stela_professional-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1268 2024-04-20 13:21:44.279246 stela_professional-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2024-01-15 04:02:49.000000 stela_professional-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.462947 stela_professional-0.4.1/accounts/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.1/accounts/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.1/accounts/admin.py
+-rw-rw-rw-   0        0        0      154 2024-01-15 04:02:49.000000 stela_professional-0.4.1/accounts/apps.py
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.1/accounts/forms.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.475381 stela_professional-0.4.1/accounts/migrations/
+-rw-rw-rw-   0        0        0     4062 2024-01-22 13:09:35.000000 stela_professional-0.4.1/accounts/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 13:09:35.000000 stela_professional-0.4.1/accounts/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4862 2024-01-16 08:21:22.000000 stela_professional-0.4.1/accounts/models.py
+-rw-rw-rw-   0        0        0       63 2024-01-15 04:02:49.000000 stela_professional-0.4.1/accounts/tests.py
+-rw-rw-rw-   0        0        0      370 2024-01-15 04:02:49.000000 stela_professional-0.4.1/accounts/token.py
+-rw-rw-rw-   0        0        0     1836 2024-01-15 04:02:49.000000 stela_professional-0.4.1/accounts/urls.py
+-rw-rw-rw-   0        0        0    10979 2024-01-15 04:02:49.000000 stela_professional-0.4.1/accounts/views.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.496129 stela_professional-0.4.1/cloud/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.1/cloud/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.1/cloud/admin.py
+-rw-rw-rw-   0        0        0      148 2024-01-15 04:02:49.000000 stela_professional-0.4.1/cloud/apps.py
+-rw-rw-rw-   0        0        0     3456 2024-01-15 04:02:49.000000 stela_professional-0.4.1/cloud/cart.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.503124 stela_professional-0.4.1/cloud/migrations/
+-rw-rw-rw-   0        0        0     5564 2024-01-22 13:10:00.000000 stela_professional-0.4.1/cloud/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 13:10:00.000000 stela_professional-0.4.1/cloud/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3508 2024-01-15 04:02:49.000000 stela_professional-0.4.1/cloud/models.py
+-rw-rw-rw-   0        0        0       63 2024-01-15 04:02:49.000000 stela_professional-0.4.1/cloud/tests.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.1/cloud/views.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.521114 stela_professional-0.4.1/geolocation/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:02:49.000000 stela_professional-0.4.1/geolocation/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.1/geolocation/admin.py
+-rw-rw-rw-   0        0        0      160 2024-01-15 04:02:49.000000 stela_professional-0.4.1/geolocation/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.527733 stela_professional-0.4.1/geolocation/migrations/
+-rw-rw-rw-   0        0        0     6403 2024-01-22 13:10:12.000000 stela_professional-0.4.1/geolocation/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 13:10:12.000000 stela_professional-0.4.1/geolocation/migrations/__init__.py
+-rw-rw-rw-   0        0        0      582 2024-01-15 04:02:49.000000 stela_professional-0.4.1/geolocation/models.py
+-rw-rw-rw-   0        0        0       63 2024-01-15 04:02:49.000000 stela_professional-0.4.1/geolocation/tests.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:02:49.000000 stela_professional-0.4.1/geolocation/views.py
+-rw-rw-rw-   0        0        0       42 2024-04-20 13:21:44.283244 stela_professional-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1448 2024-04-20 13:18:54.000000 stela_professional-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.599039 stela_professional-0.4.1/stela_control/
+-rw-rw-rw-   0        0        0        0 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/__init__.py
+-rw-rw-rw-   0        0        0       34 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/admin.py
+-rw-rw-rw-   0        0        0      163 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/apps.py
+-rw-rw-rw-   0        0        0     7527 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/cart.py
+-rw-rw-rw-   0        0        0      164 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/context_processors.py
+-rw-rw-rw-   0        0        0      316 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/cron.py
+-rw-rw-rw-   0        0        0    85813 2024-03-05 11:43:43.000000 stela_professional-0.4.1/stela_control/forms.py
+-rw-rw-rw-   0        0        0      181 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.089000 stela_professional-0.4.1/stela_control/locale/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.089000 stela_professional-0.4.1/stela_control/locale/es/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.831964 stela_professional-0.4.1/stela_control/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    55259 2024-02-19 18:04:13.000000 stela_professional-0.4.1/stela_control/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0   332194 2024-02-19 18:03:02.000000 stela_professional-0.4.1/stela_control/locale/es/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.952309 stela_professional-0.4.1/stela_control/migrations/
+-rw-rw-rw-   0        0        0    89195 2024-01-22 13:10:23.000000 stela_professional-0.4.1/stela_control/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     5384 2024-01-22 16:02:46.000000 stela_professional-0.4.1/stela_control/migrations/0002_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     6120 2024-01-22 19:38:17.000000 stela_professional-0.4.1/stela_control/migrations/0003_rename_description_company_content_and_more.py
+-rw-rw-rw-   0        0        0     5640 2024-01-22 21:09:07.000000 stela_professional-0.4.1/stela_control/migrations/0004_alter_billingrecipt_option_alter_company_address_and_more.py
+-rw-rw-rw-   0        0        0     5424 2024-01-22 22:24:05.000000 stela_professional-0.4.1/stela_control/migrations/0005_rename_description_team_content_and_more.py
+-rw-rw-rw-   0        0        0     7730 2024-01-31 12:37:18.000000 stela_professional-0.4.1/stela_control/migrations/0006_alter_bankstatement_bank_and_more.py
+-rw-rw-rw-   0        0        0     5121 2024-01-31 16:03:17.000000 stela_professional-0.4.1/stela_control/migrations/0007_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     5644 2024-02-05 01:43:23.000000 stela_professional-0.4.1/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     5171 2024-02-05 07:46:11.000000 stela_professional-0.4.1/stela_control/migrations/0009_content_video_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     4962 2024-02-06 05:55:50.000000 stela_professional-0.4.1/stela_control/migrations/0010_resource_category_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     6460 2024-02-06 15:43:12.000000 stela_professional-0.4.1/stela_control/migrations/0011_resource_cover_taxid_pdf_file2_and_more.py
+-rw-rw-rw-   0        0        0     5640 2024-02-06 17:11:41.000000 stela_professional-0.4.1/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     5323 2024-02-19 17:38:39.000000 stela_professional-0.4.1/stela_control/migrations/0013_content_cover_content_fecade_url_and_more.py
+-rw-rw-rw-   0        0        0     5891 2024-02-20 23:29:50.000000 stela_professional-0.4.1/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     5039 2024-02-21 15:45:43.000000 stela_professional-0.4.1/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 13:10:23.000000 stela_professional-0.4.1/stela_control/migrations/__init__.py
+-rw-rw-rw-   0        0        0    71703 2024-02-21 15:44:07.000000 stela_professional-0.4.1/stela_control/models.py
+-rw-rw-rw-   0        0        0     2943 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/routers.py
+-rw-rw-rw-   0        0        0   179141 2024-04-20 13:17:23.000000 stela_professional-0.4.1/stela_control/superfunctions.py
+-rw-rw-rw-   0        0        0      410 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/tasks.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.091996 stela_professional-0.4.1/stela_control/templates/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:29.515726 stela_professional-0.4.1/stela_control/templates/stela_control/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:29.647644 stela_professional-0.4.1/stela_control/templates/stela_control/accounts/
+-rw-rw-rw-   0        0        0      497 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/accounts/base.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:29.858515 stela_professional-0.4.1/stela_control/templates/stela_control/accounts/registration/
+-rw-rw-rw-   0        0        0      227 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/accounts/registration/account_activation_email.html
+-rw-rw-rw-   0        0        0       21 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/accounts/registration/activation_invalid.html
+-rw-rw-rw-   0        0        0     1373 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/accounts/registration/confirmation_email.html
+-rw-rw-rw-   0        0        0     3071 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/accounts/registration/register.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:30.214502 stela_professional-0.4.1/stela_control/templates/stela_control/accounts/user/
+-rw-rw-rw-   0        0        0     1364 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/accounts/user/delete_user.html
+-rw-rw-rw-   0        0        0     2956 2024-02-06 18:30:10.000000 stela_professional-0.4.1/stela_control/templates/stela_control/accounts/user/login.html
+-rw-rw-rw-   0        0        0     2692 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html
+-rw-rw-rw-   0        0        0     2043 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/accounts/user/password_reset_done.html
+-rw-rw-rw-   0        0        0      629 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/accounts/user/password_reset_email.html
+-rw-rw-rw-   0        0        0     2424 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/accounts/user/password_reset_form.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:30.342954 stela_professional-0.4.1/stela_control/templates/stela_control/analytics/
+-rw-rw-rw-   0        0        0      757 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/analytics/analytics.html
+-rw-rw-rw-   0        0        0      527 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/analytics/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:30.489864 stela_professional-0.4.1/stela_control/templates/stela_control/api/
+-rw-rw-rw-   0        0        0     5932 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/api/main.html
+-rw-rw-rw-   0        0        0     2883 2024-01-21 23:59:12.000000 stela_professional-0.4.1/stela_control/templates/stela_control/base.html
+-rw-rw-rw-   0        0        0     4402 2024-01-22 14:53:11.000000 stela_professional-0.4.1/stela_control/templates/stela_control/base_content.html
+-rw-rw-rw-   0        0        0     6768 2024-01-20 15:13:41.000000 stela_professional-0.4.1/stela_control/templates/stela_control/base_list.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:30.804670 stela_professional-0.4.1/stela_control/templates/stela_control/billing/
+-rw-rw-rw-   0        0        0   253007 2024-03-18 11:50:23.000000 stela_professional-0.4.1/stela_control/templates/stela_control/billing/homebrew.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:31.883495 stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/
+-rw-rw-rw-   0        0        0     1443 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/bill-data-customer.html
+-rw-rw-rw-   0        0        0    30854 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/checkout.html
+-rw-rw-rw-   0        0        0      906 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/data-customer.html
+-rw-rw-rw-   0        0        0    56802 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/invoice-copy.html
+-rw-rw-rw-   0        0        0    56693 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/invoice.html
+-rw-rw-rw-   0        0        0     2875 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/order-placed.html
+-rw-rw-rw-   0        0        0    48021 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/preview-recipt.html
+-rw-rw-rw-   0        0        0     2750 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html
+-rw-rw-rw-   0        0        0     3336 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/recipt-detail.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:31.965445 stela_professional-0.4.1/stela_control/templates/stela_control/booking-control/
+-rw-rw-rw-   0        0        0     1992 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/booking-control/customer-detail.html
+-rw-rw-rw-   0        0        0     4067 2024-01-22 14:58:02.000000 stela_professional-0.4.1/stela_control/templates/stela_control/booking-control/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:32.130881 stela_professional-0.4.1/stela_control/templates/stela_control/chatstela/
+-rw-rw-rw-   0        0        0    30842 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/templates/stela_control/chatstela/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:32.315610 stela_professional-0.4.1/stela_control/templates/stela_control/content/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:32.392352 stela_professional-0.4.1/stela_control/templates/stela_control/content/comments/
+-rw-rw-rw-   0        0        0     2254 2024-01-20 22:35:04.000000 stela_professional-0.4.1/stela_control/templates/stela_control/content/comments/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:32.491680 stela_professional-0.4.1/stela_control/templates/stela_control/content/docs/
+-rw-rw-rw-   0        0        0    10531 2024-02-05 01:03:29.000000 stela_professional-0.4.1/stela_control/templates/stela_control/content/docs/main.html
+-rw-rw-rw-   0        0        0     7438 2024-02-06 18:40:47.000000 stela_professional-0.4.1/stela_control/templates/stela_control/content/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:32.584621 stela_professional-0.4.1/stela_control/templates/stela_control/content/main/
+-rw-rw-rw-   0        0        0     1003 2024-02-20 02:42:20.000000 stela_professional-0.4.1/stela_control/templates/stela_control/content/main/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:32.626595 stela_professional-0.4.1/stela_control/templates/stela_control/content/staff/
+-rw-rw-rw-   0        0        0     7608 2024-02-05 04:12:54.000000 stela_professional-0.4.1/stela_control/templates/stela_control/content/staff/index.html
+-rw-rw-rw-   0        0        0    26830 2024-02-23 19:08:09.000000 stela_professional-0.4.1/stela_control/templates/stela_control/content/stelastory.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:32.661575 stela_professional-0.4.1/stela_control/templates/stela_control/developer/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:32.846460 stela_professional-0.4.1/stela_control/templates/stela_control/developer/data-update/
+-rw-rw-rw-   0        0        0      933 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/developer/data-update/modal1.html
+-rw-rw-rw-   0        0        0      898 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/developer/data-update/modal2.html
+-rw-rw-rw-   0        0        0      900 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/developer/data-update/modal3.html
+-rw-rw-rw-   0        0        0      875 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/developer/data-update/modal4.html
+-rw-rw-rw-   0        0        0    46793 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/developer/home.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.125976 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:32.948313 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/accounts/
+-rw-rw-rw-   0        0        0      413 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/accounts/password_reset_email.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:33.168653 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/billing/
+-rw-rw-rw-   0        0        0    21938 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html
+-rw-rw-rw-   0        0        0    21903 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/billing/invoice.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:33.483420 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/contact/
+-rw-rw-rw-   0        0        0    20096 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/contact/message_notification.html
+-rw-rw-rw-   0        0        0     8454 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/contact/support_notification.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:33.838677 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/marketing/
+-rw-rw-rw-   0        0        0    60992 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:33.915441 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/newsletter/
+-rw-rw-rw-   0        0        0    21461 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:34.015375 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/orders/
+-rw-rw-rw-   0        0        0    10226 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:34.497604 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/payments/
+-rw-rw-rw-   0        0        0    27770 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/payments/billing_payment.html
+-rw-rw-rw-   0        0        0     6930 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/payments/charges.html
+-rw-rw-rw-   0        0        0    20151 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/payments/payment_notification.html
+-rw-rw-rw-   0        0        0    20151 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/payments/sale_notification.html
+-rw-rw-rw-   0        0        0     7266 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html
+-rw-rw-rw-   0        0        0     7166 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/payments/withdrawals.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:34.591475 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/support/
+-rw-rw-rw-   0        0        0    20072 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/support/support_notification.html
+-rw-rw-rw-   0        0        0    22345 2024-02-23 19:07:47.000000 stela_professional-0.4.1/stela_control/templates/stela_control/home.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:34.683456 stela_professional-0.4.1/stela_control/templates/stela_control/inbox/
+-rw-rw-rw-   0        0        0     2272 2024-01-21 15:59:26.000000 stela_professional-0.4.1/stela_control/templates/stela_control/inbox/index.html
+-rw-rw-rw-   0        0        0    11555 2024-02-03 04:29:28.000000 stela_professional-0.4.1/stela_control/templates/stela_control/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.148962 stela_professional-0.4.1/stela_control/templates/stela_control/inventory/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:34.746123 stela_professional-0.4.1/stela_control/templates/stela_control/inventory/products/
+-rw-rw-rw-   0        0        0        0 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/inventory/products/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:34.973277 stela_professional-0.4.1/stela_control/templates/stela_control/inventory/resources/
+-rw-rw-rw-   0        0        0     2888 2024-01-18 21:03:25.000000 stela_professional-0.4.1/stela_control/templates/stela_control/inventory/resources/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:35.515548 stela_professional-0.4.1/stela_control/templates/stela_control/inventory/services/
+-rw-rw-rw-   0        0        0     6806 2024-02-27 00:40:42.000000 stela_professional-0.4.1/stela_control/templates/stela_control/inventory/services/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:35.778731 stela_professional-0.4.1/stela_control/templates/stela_control/jobs/
+-rw-rw-rw-   0        0        0     2265 2024-01-22 15:22:45.000000 stela_professional-0.4.1/stela_control/templates/stela_control/jobs/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:36.370716 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:36.420724 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/aboutemmerut/
+-rw-rw-rw-   0        0        0     1694 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:36.438559 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/aboutsecondary/
+-rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:36.456544 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/aboutstela/
+-rw-rw-rw-   0        0        0     1381 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/aboutstela/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:36.599837 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/alerts/
+-rw-rw-rw-   0        0        0      444 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/alerts/budget-alert.html
+-rw-rw-rw-   0        0        0      384 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/alerts/budget-success.html
+-rw-rw-rw-   0        0        0      404 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/alerts/cancel-recipt.html
+-rw-rw-rw-   0        0        0      445 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/alerts/invoice-alert.html
+-rw-rw-rw-   0        0        0      380 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/alerts/invoice-success.html
+-rw-rw-rw-   0        0        0      471 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/alerts/payeed-recipt.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:36.617830 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/appstela/
+-rw-rw-rw-   0        0        0     1806 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/appstela/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.183964 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/auth/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:36.704276 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/auth/pw_reset/
+-rw-rw-rw-   0        0        0       45 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/auth/pw_reset/form_errors.html
+-rw-rw-rw-   0        0        0      220 2024-01-20 02:10:43.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/auth/pw_reset/password_reset_form.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:36.725262 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/auth/signup/
+-rw-rw-rw-   0        0        0      794 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html
+-rw-rw-rw-   0        0        0      269 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/auth/signup/success_register.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:36.786520 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/billing/
+-rw-rw-rw-   0        0        0     6947 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/billing/form-billing.html
+-rw-rw-rw-   0        0        0    40487 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/billing/recipt-data.html
+-rw-rw-rw-   0        0        0     3005 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/blog-feed.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:36.888026 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/categories/
+-rw-rw-rw-   0        0        0      834 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/categories/modal4.html
+-rw-rw-rw-   0        0        0      826 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/chatbox.html
+-rw-rw-rw-   0        0        0      925 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/chatbox2.html
+-rw-rw-rw-   0        0        0      143 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/city_data.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:36.906014 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/colors/
+-rw-rw-rw-   0        0        0      857 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/colors/modal2.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:36.941992 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/contact/
+-rw-rw-rw-   0        0        0     1088 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/contact/form.html
+-rw-rw-rw-   0        0        0     1606 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/contact/modal.html
+-rw-rw-rw-   0        0        0     1638 2024-01-22 20:05:28.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/dynamic-formset.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:37.299478 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/emmerutfooter/
+-rw-rw-rw-   0        0        0     2233 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:37.475122 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/emmerutservices/
+-rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html
+-rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html
+-rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html
+-rw-rw-rw-   0        0        0      841 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/form-base.html
+-rw-rw-rw-   0        0        0       64 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/form-errors.html
+-rw-rw-rw-   0        0        0      924 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/formset-base-services.html
+-rw-rw-rw-   0        0        0     1790 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/formset-base.html
+-rw-rw-rw-   0        0        0     1569 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/formset.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.218879 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/handlers/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:37.517630 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/handlers/blog/
+-rw-rw-rw-   0        0        0     1469 2024-01-30 20:17:44.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages-v1.html
+-rw-rw-rw-   0        0        0      128 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/handlers/blog/empty-blog.html
+-rw-rw-rw-   0        0        0      103 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/hashtags.html
+-rw-rw-rw-   0        0        0      587 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/instagram-alert.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:37.554449 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/inventory/
+-rw-rw-rw-   0        0        0     1778 2024-02-26 17:25:31.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:37.568248 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/job-application/
+-rw-rw-rw-   0        0        0       45 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/job-application/error-form-v1.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:37.611291 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/linkzoneupdates/
+-rw-rw-rw-   0        0        0      848 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.223874 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:38.050879 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/
+-rw-rw-rw-   0        0        0     1067 2024-02-23 15:58:42.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html
+-rw-rw-rw-   0        0        0     1467 2024-02-23 16:29:50.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html
+-rw-rw-rw-   0        0        0     1650 2024-02-23 18:05:44.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html
+-rw-rw-rw-   0        0        0     2732 2024-02-23 18:06:01.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html
+-rw-rw-rw-   0        0        0     2540 2024-02-26 13:05:43.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html
+-rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:06.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html
+-rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:10.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html
+-rw-rw-rw-   0        0        0     2887 2024-02-23 18:06:18.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html
+-rw-rw-rw-   0        0        0     2593 2024-02-23 18:06:24.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html
+-rw-rw-rw-   0        0        0     2296 2024-02-23 18:06:30.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html
+-rw-rw-rw-   0        0        0     1639 2024-02-23 18:06:35.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html
+-rw-rw-rw-   0        0        0     2587 2024-02-26 13:34:25.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:38.354051 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/
+-rw-rw-rw-   0        0        0     1614 2024-02-23 18:04:43.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html
+-rw-rw-rw-   0        0        0     3292 2024-02-23 18:04:45.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html
+-rw-rw-rw-   0        0        0     3051 2024-02-23 18:04:50.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html
+-rw-rw-rw-   0        0        0     1936 2024-02-23 18:04:55.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html
+-rw-rw-rw-   0        0        0     2198 2024-02-23 18:05:01.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html
+-rw-rw-rw-   0        0        0     2866 2024-02-23 18:05:07.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html
+-rw-rw-rw-   0        0        0     2737 2024-02-23 18:05:12.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html
+-rw-rw-rw-   0        0        0     2418 2024-02-23 18:05:17.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html
+-rw-rw-rw-   0        0        0     1412 2024-02-23 18:07:47.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html
+-rw-rw-rw-   0        0        0     2803 2024-02-23 18:05:27.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html
+-rw-rw-rw-   0        0        0     1297 2024-02-23 15:56:06.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html
+-rw-rw-rw-   0        0        0     1778 2024-02-23 16:29:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:38.808325 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/
+-rw-rw-rw-   0        0        0     1069 2024-02-23 15:58:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html
+-rw-rw-rw-   0        0        0     1464 2024-02-23 16:29:44.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html
+-rw-rw-rw-   0        0        0     1962 2024-02-23 18:06:50.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html
+-rw-rw-rw-   0        0        0     3022 2024-02-23 18:06:54.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html
+-rw-rw-rw-   0        0        0     2878 2024-02-26 13:33:54.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html
+-rw-rw-rw-   0        0        0     1740 2024-02-23 18:07:07.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html
+-rw-rw-rw-   0        0        0     2080 2024-02-23 18:07:11.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html
+-rw-rw-rw-   0        0        0     3148 2024-02-23 18:07:16.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html
+-rw-rw-rw-   0        0        0     2631 2024-02-23 18:07:22.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html
+-rw-rw-rw-   0        0        0     2546 2024-04-20 12:39:16.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html
+-rw-rw-rw-   0        0        0     1929 2024-02-23 18:07:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html
+-rw-rw-rw-   0        0        0     2616 2024-02-26 14:03:38.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:38.892603 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:38.933577 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/community/
+-rw-rw-rw-   0        0        0      818 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/community/formdata.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:38.946570 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/content-pro-media/
+-rw-rw-rw-   0        0        0     3209 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:38.981477 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/content-pro-update/
+-rw-rw-rw-   0        0        0       83 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/content-pro-update/content.html
+-rw-rw-rw-   0        0        0       84 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/content-pro-update/schedule.html
+-rw-rw-rw-   0        0        0      986 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:39.034502 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ic-update/
+-rw-rw-rw-   0        0        0      469 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ic-update/content.html
+-rw-rw-rw-   0        0        0     1379 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:39.169476 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ig-analythics/
+-rw-rw-rw-   0        0        0    25077 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html
+-rw-rw-rw-   0        0        0     1667 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html
+-rw-rw-rw-   0        0        0     1530 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html
+-rw-rw-rw-   0        0        0     1849 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html
+-rw-rw-rw-   0        0        0     1774 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html
+-rw-rw-rw-   0        0        0     4485 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html
+-rw-rw-rw-   0        0        0     5787 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:39.198673 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/meta-assets/
+-rw-rw-rw-   0        0        0        0 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page-alert.html
+-rw-rw-rw-   0        0        0      628 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:39.293904 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/page-analythics/
+-rw-rw-rw-   0        0        0     1755 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html
+-rw-rw-rw-   0        0        0     1960 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html
+-rw-rw-rw-   0        0        0     1428 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:39.433152 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/smart-boost/
+-rw-rw-rw-   0        0        0     2129 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:39.491276 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/stela-sight/
+-rw-rw-rw-   0        0        0      268 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/stela-sight/data.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:39.526605 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/newcomer/
+-rw-rw-rw-   0        0        0     4162 2024-02-06 04:01:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/newcomer/form.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:39.539596 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/newsletter/
+-rw-rw-rw-   0        0        0      216 2024-01-31 02:03:43.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/newsletter/form.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:39.569578 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/post/
+-rw-rw-rw-   0        0        0      846 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/post/list-modal.html
+-rw-rw-rw-   0        0        0      850 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/post/main-modal.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:39.615225 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/
+-rw-rw-rw-   0        0        0     1824 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/catalog-modal.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:39.899263 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/new/
+-rw-rw-rw-   0        0        0      933 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/new/catalog-form.html
+-rw-rw-rw-   0        0        0      872 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/new/category-form.html
+-rw-rw-rw-   0        0        0      888 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/new/color-form.html
+-rw-rw-rw-   0        0        0     1024 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/new/product-form.html
+-rw-rw-rw-   0        0        0      855 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/new/size-form.html
+-rw-rw-rw-   0        0        0      115 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/new/variant-form.html
+-rw-rw-rw-   0        0        0      805 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/product-modal.html
+-rw-rw-rw-   0        0        0      848 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/size-modal.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:40.113469 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/update/
+-rw-rw-rw-   0        0        0      234 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/update/catalog-form.html
+-rw-rw-rw-   0        0        0      287 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/update/category-form.html
+-rw-rw-rw-   0        0        0      230 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/update/color-form.html
+-rw-rw-rw-   0        0        0     1008 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/update/product-form.html
+-rw-rw-rw-   0        0        0      228 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/update/size-form.html
+-rw-rw-rw-   0        0        0      234 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/update/variant-form.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:40.204457 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/profile/
+-rw-rw-rw-   0        0        0     1306 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/profile/dynamic-form.html
+-rw-rw-rw-   0        0        0      200 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/profile/single-form.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:40.285461 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/projects/
+-rw-rw-rw-   0        0        0     1698 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/projects/modal.html
+-rw-rw-rw-   0        0        0      265 2024-01-18 10:44:28.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/remove-complete.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:40.340394 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/render/
+-rw-rw-rw-   0        0        0      143 2024-01-21 14:42:59.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/render/city_data.html
+-rw-rw-rw-   0        0        0      604 2024-01-18 10:28:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/single-form.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.310526 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:40.396665 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/
+-rw-rw-rw-   0        0        0     1099 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html
+-rw-rw-rw-   0        0        0     1265 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:40.440636 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/error_forms/
+-rw-rw-rw-   0        0        0     1099 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html
+-rw-rw-rw-   0        0        0     1265 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:40.566036 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/forms/
+-rw-rw-rw-   0        0        0     1269 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html
+-rw-rw-rw-   0        0        0     1097 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html
+-rw-rw-rw-   0        0        0     1265 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:40.637350 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/update_forms/
+-rw-rw-rw-   0        0        0     1156 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html
+-rw-rw-rw-   0        0        0     1320 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:40.715087 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/staff/
+-rw-rw-rw-   0        0        0     1947 2024-01-18 10:28:34.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/staff/form.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:40.826560 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/stela_story/
+-rw-rw-rw-   0        0        0     3418 2024-02-21 15:38:13.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/stela_story/feed-item.html
+-rw-rw-rw-   0        0        0     2001 2024-01-18 10:28:39.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:40.854577 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/stelafooter/
+-rw-rw-rw-   0        0        0     2176 2024-01-18 10:28:39.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/stelafooter/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:40.969309 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/stelamedia/
+-rw-rw-rw-   0        0        0     1695 2024-01-18 10:28:39.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/stelamedia/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:41.000590 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/stelapath/
+-rw-rw-rw-   0        0        0     1337 2024-01-18 10:28:39.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/stelapath/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:41.111719 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/tables/
+-rw-rw-rw-   0        0        0      663 2024-01-22 15:21:03.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/tables/bank_statements.html
+-rw-rw-rw-   0        0        0      675 2024-01-22 15:22:21.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/tables/invoices.html
+-rw-rw-rw-   0        0        0      675 2024-01-22 15:22:25.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/tables/retentions.html
+-rw-rw-rw-   0        0        0      630 2024-01-22 15:21:30.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/tables/tax-return.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:41.127710 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/users/
+-rw-rw-rw-   0        0        0      254 2024-01-19 18:04:36.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/users/suspend.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:41.155692 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/youtube/
+-rw-rw-rw-   0        0        0      157 2024-01-18 10:28:39.000000 stela_professional-0.4.1/stela_control/templates/stela_control/load-data/youtube/video-preview.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.332512 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:41.204689 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/email-marketing/
+-rw-rw-rw-   0        0        0     1543 2024-01-20 22:43:07.000000 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/email-marketing/email_list.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:41.710537 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/
+-rw-rw-rw-   0        0        0    10789 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:27.344316 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/instagram/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:42.261612 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/
+-rw-rw-rw-   0        0        0    13445 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:42.494695 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/
+-rw-rw-rw-   0        0        0    23333 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:42.691573 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/
+-rw-rw-rw-   0        0        0    34272 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:42.743541 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/page/
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:42.776527 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/page/community/
+-rw-rw-rw-   0        0        0    14156 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:42.894138 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/
+-rw-rw-rw-   0        0        0    30243 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html
+-rw-rw-rw-   0        0        0      248 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/update.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:42.913126 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/
+-rw-rw-rw-   0        0        0     3162 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html
+-rw-rw-rw-   0        0        0    12633 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html
+-rw-rw-rw-   0        0        0    17640 2024-01-22 19:37:49.000000 stela_professional-0.4.1/stela_control/templates/stela_control/newcomer.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:43.104168 stela_professional-0.4.1/stela_control/templates/stela_control/orders/
+-rw-rw-rw-   0        0        0     6171 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/orders/list_view.html
+-rw-rw-rw-   0        0        0     8860 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/orders/order_update.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:43.222339 stela_professional-0.4.1/stela_control/templates/stela_control/payments/
+-rw-rw-rw-   0        0        0    43167 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/payments/homebrew.html
+-rw-rw-rw-   0        0        0     2687 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/payments/register-wallet.html
+-rw-rw-rw-   0        0        0     4322 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/payments/wallet-list.html
+-rw-rw-rw-   0        0        0     2831 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/payments/withdraw.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:43.304287 stela_professional-0.4.1/stela_control/templates/stela_control/prostela/
+-rw-rw-rw-   0        0        0      153 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/prostela/chatbox.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:43.447123 stela_professional-0.4.1/stela_control/templates/stela_control/prostela-expert/
+-rw-rw-rw-   0        0        0    34014 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/prostela-expert/index.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:43.480101 stela_professional-0.4.1/stela_control/templates/stela_control/reviews/
+-rw-rw-rw-   0        0        0     2269 2024-01-20 22:29:12.000000 stela_professional-0.4.1/stela_control/templates/stela_control/reviews/reviews.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:43.554625 stela_professional-0.4.1/stela_control/templates/stela_control/support/
+-rw-rw-rw-   0        0        0     6350 2024-01-18 22:16:16.000000 stela_professional-0.4.1/stela_control/templates/stela_control/support/case-detail.html
+-rw-rw-rw-   0        0        0     2323 2024-01-18 14:01:39.000000 stela_professional-0.4.1/stela_control/templates/stela_control/support/list.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:44.217284 stela_professional-0.4.1/stela_control/templates/stela_control/users/
+-rw-rw-rw-   0        0        0      339 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templates/stela_control/users/generic-user-handler.html
+-rw-rw-rw-   0        0        0    11181 2024-01-22 21:22:30.000000 stela_professional-0.4.1/stela_control/templates/stela_control/users/profile.html
+-rw-rw-rw-   0        0        0    12343 2024-02-06 16:52:33.000000 stela_professional-0.4.1/stela_control/templates/stela_control/users/users-control.html
+-rw-rw-rw-   0        0        0     6472 2024-02-06 15:00:39.000000 stela_professional-0.4.1/stela_control/templates/stela_control/users/users.html
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:44.230276 stela_professional-0.4.1/stela_control/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-01-18 10:28:40.000000 stela_professional-0.4.1/stela_control/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     1428 2024-04-08 13:35:26.000000 stela_professional-0.4.1/stela_control/templatetags/stelatags.py
+-rw-rw-rw-   0        0        0      507 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/tests.py
+-rw-rw-rw-   0        0        0     1131 2024-01-18 10:28:32.000000 stela_professional-0.4.1/stela_control/tokenize.py
+-rw-rw-rw-   0        0        0     7442 2024-02-20 00:40:50.000000 stela_professional-0.4.1/stela_control/urls.py
+-rw-rw-rw-   0        0        0   270343 2024-03-18 11:42:47.000000 stela_professional-0.4.1/stela_control/views.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:21:44.276247 stela_professional-0.4.1/stela_professional.egg-info/
+-rw-rw-rw-   0        0        0     1268 2024-04-20 13:21:24.000000 stela_professional-0.4.1/stela_professional.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    20476 2024-04-20 13:21:26.000000 stela_professional-0.4.1/stela_professional.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 13:21:24.000000 stela_professional-0.4.1/stela_professional.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      384 2024-04-20 13:21:24.000000 stela_professional-0.4.1/stela_professional.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       41 2024-04-20 13:21:24.000000 stela_professional-0.4.1/stela_professional.egg-info/top_level.txt
```

### Comparing `stela_professional-0.4.0/LICENSE` & `stela_professional-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/PKG-INFO` & `stela_professional-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stela_professional
-Version: 0.4.0
+Version: 0.4.1
 Summary: All apps in one for business.
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `stela_professional-0.4.0/accounts/migrations/0001_initial.py` & `stela_professional-0.4.1/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/accounts/models.py` & `stela_professional-0.4.1/accounts/models.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/accounts/urls.py` & `stela_professional-0.4.1/accounts/urls.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/accounts/views.py` & `stela_professional-0.4.1/accounts/views.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/cloud/cart.py` & `stela_professional-0.4.1/cloud/cart.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/cloud/migrations/0001_initial.py` & `stela_professional-0.4.1/cloud/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/cloud/models.py` & `stela_professional-0.4.1/cloud/models.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/geolocation/migrations/0001_initial.py` & `stela_professional-0.4.1/geolocation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/geolocation/models.py` & `stela_professional-0.4.1/geolocation/models.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/setup.py` & `stela_professional-0.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 excluded_packages = [
     'core', 'core.*', 
     'linkzone', 'linkzone.*', 
 ]
 setup(
     name='stela_professional',
-    version='0.4.0',
+    version='0.4.1',
     packages=find_packages(exclude=excluded_packages),
     include_package_data=True,
     license='MIT',
     description='All apps in one for business.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

### Comparing `stela_professional-0.4.0/stela_control/cart.py` & `stela_professional-0.4.1/stela_control/cart.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/forms.py` & `stela_professional-0.4.1/stela_control/forms.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/locale/es/LC_MESSAGES/django.mo` & `stela_professional-0.4.1/stela_control/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/locale/es/LC_MESSAGES/django.po` & `stela_professional-0.4.1/stela_control/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/migrations/0001_initial.py` & `stela_professional-0.4.1/stela_control/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/migrations/0002_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_professional-0.4.1/stela_control/migrations/0002_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/migrations/0003_rename_description_company_content_and_more.py` & `stela_professional-0.4.1/stela_control/migrations/0003_rename_description_company_content_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/migrations/0004_alter_billingrecipt_option_alter_company_address_and_more.py` & `stela_professional-0.4.1/stela_control/migrations/0004_alter_billingrecipt_option_alter_company_address_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/migrations/0005_rename_description_team_content_and_more.py` & `stela_professional-0.4.1/stela_control/migrations/0005_rename_description_team_content_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/migrations/0006_alter_bankstatement_bank_and_more.py` & `stela_professional-0.4.1/stela_control/migrations/0006_alter_bankstatement_bank_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/migrations/0007_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_professional-0.4.1/stela_control/migrations/0007_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_professional-0.4.1/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/migrations/0009_content_video_alter_billingrecipt_option_and_more.py` & `stela_professional-0.4.1/stela_control/migrations/0009_content_video_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/migrations/0010_resource_category_alter_billingrecipt_option_and_more.py` & `stela_professional-0.4.1/stela_control/migrations/0010_resource_category_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/migrations/0011_resource_cover_taxid_pdf_file2_and_more.py` & `stela_professional-0.4.1/stela_control/migrations/0011_resource_cover_taxid_pdf_file2_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_professional-0.4.1/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/migrations/0013_content_cover_content_fecade_url_and_more.py` & `stela_professional-0.4.1/stela_control/migrations/0013_content_cover_content_fecade_url_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_professional-0.4.1/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_professional-0.4.1/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/models.py` & `stela_professional-0.4.1/stela_control/models.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/routers.py` & `stela_professional-0.4.1/stela_control/routers.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/superfunctions.py` & `stela_professional-0.4.1/stela_control/superfunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1867,21 +1867,22 @@
             content.delete()
             alert = render_to_string('stela_control/load-data/remove-complete.html', {})
             return JsonResponse({'success': alert})
 
         if form_id == "doc-form":
             update_form = request.POST.get('form-update')
             if update_form:
-                form=PolicyForm(request.POST, instance=update_form)
+                policy=SitePolicy.objects.get(pk=update_form)
+                form=PolicyForm(request.POST, instance=policy)
                 get_formset = inlineformset_factory(
                     SitePolicy, LegalProvision, 
                     form=LegalProvitionForm,
                     extra=0, can_delete=True,
                 )
-                formset=get_formset(request.POST, prefix='terms', instance=update_form)
+                formset=get_formset(request.POST, prefix='terms', instance=policy)
                 if all([form.is_valid(),
                         formset.is_valid(),
                     ]):
                     policy = form.save(commit=False)
                     policy.owner = author
                     policy.lang = lang
                     policy.save()
```

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/accounts/registration/confirmation_email.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/accounts/registration/confirmation_email.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/accounts/registration/register.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/accounts/registration/register.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/accounts/user/delete_user.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/accounts/user/delete_user.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/accounts/user/login.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/accounts/user/login.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/accounts/user/password_reset_done.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/accounts/user/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/accounts/user/password_reset_email.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/accounts/user/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/accounts/user/password_reset_form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/accounts/user/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/analytics/analytics.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/analytics/analytics.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/analytics/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/analytics/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/api/main.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/api/main.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/base.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/base.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/base_content.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/base_content.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/base_list.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/base_list.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/billing/homebrew.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/billing/homebrew.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/bill-data-customer.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/bill-data-customer.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/checkout.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/checkout.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/data-customer.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/data-customer.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/invoice-copy.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/invoice-copy.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/invoice.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/invoice.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/order-placed.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/order-placed.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/preview-recipt.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/preview-recipt.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/billing/sections/recipt-detail.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/billing/sections/recipt-detail.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/booking-control/customer-detail.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/booking-control/customer-detail.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/booking-control/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/booking-control/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/chatstela/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/chatstela/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/content/comments/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/content/comments/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/content/docs/main.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/content/docs/main.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/content/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/content/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/content/main/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/content/main/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/content/staff/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/content/staff/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/content/stelastory.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/content/stelastory.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/developer/data-update/modal1.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/developer/data-update/modal1.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/developer/data-update/modal2.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/developer/data-update/modal2.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/developer/data-update/modal3.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/developer/data-update/modal3.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/developer/data-update/modal4.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/developer/data-update/modal4.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/developer/home.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/developer/home.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/billing/invoice.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/billing/invoice.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/contact/message_notification.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/contact/message_notification.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/contact/support_notification.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/contact/support_notification.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/payments/billing_payment.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/payments/billing_payment.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/payments/charges.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/payments/charges.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/payments/payment_notification.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/payments/payment_notification.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/payments/sale_notification.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/payments/sale_notification.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/payments/withdrawals.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/payments/withdrawals.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/emails-template/support/support_notification.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/emails-template/support/support_notification.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/home.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/home.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/inbox/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/inbox/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/inventory/resources/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/inventory/resources/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/inventory/services/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/inventory/services/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/jobs/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/jobs/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/aboutstela/modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/aboutstela/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/appstela/modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/appstela/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/billing/form-billing.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/billing/form-billing.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/billing/recipt-data.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/billing/recipt-data.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/blog-feed.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/blog-feed.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/categories/modal4.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/categories/modal4.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/chatbox.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/chatbox.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/chatbox2.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/chatbox2.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/colors/modal2.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/colors/modal2.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/contact/form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/contact/form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/contact/modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/contact/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/dynamic-formset.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/dynamic-formset.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/form-base.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/form-base.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/formset-base-services.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/formset-base-services.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/formset-base.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/formset-base.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/formset.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/formset.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages-v1.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages-v1.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/instagram-alert.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/instagram-alert.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html`

 * *Files 7% similar despite different names*

```diff
@@ -46,9 +46,10 @@
     </div>
     <div class="d-flex justify-content-between my-3">
         <button class="btn-clear" onclick="addFormset()" type="button"><i class="fa-solid fa-plus"></i> {% trans "Add" %}</button>
         <button class="btn-clear" onclick="clearFormset()" type="button"><i class="fa-solid fa-minus"></i> {% trans "Remove" %}</button>
     </div> 
 </div>
 <p class="response-footer text-link fw-bold oxanium"></p>
-<input type="hidden" name="form-id" value="apps-form"> 
+<input type="hidden" name="form-id" value={{form_name}}>
+<input type="hidden" name="section" value={{section}}>
 <input type="hidden" name="form-url" value="/validations/content/">
```

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/community/formdata.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/community/formdata.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/newcomer/form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/newcomer/form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/post/list-modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/post/list-modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/post/main-modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/post/main-modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/catalog-modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/catalog-modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/new/catalog-form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/new/catalog-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/new/category-form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/new/category-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/new/color-form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/new/color-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/new/product-form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/new/product-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/new/size-form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/new/size-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/product-modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/product-modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/size-modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/size-modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/products/update/product-form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/products/update/product-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/profile/dynamic-form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/profile/dynamic-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/projects/modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/projects/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/single-form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/single-form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/staff/form.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/staff/form.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/stela_story/feed-item.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/stela_story/feed-item.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/stelafooter/modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/stelafooter/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/stelamedia/modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/stelamedia/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/stelapath/modal.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/stelapath/modal.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/tables/bank_statements.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/tables/bank_statements.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/tables/invoices.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/tables/invoices.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/tables/retentions.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/tables/retentions.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/load-data/tables/tax-return.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/load-data/tables/tax-return.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/marketing/email-marketing/email_list.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/marketing/email-marketing/email_list.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/newcomer.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/newcomer.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/orders/list_view.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/orders/list_view.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/orders/order_update.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/orders/order_update.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/payments/homebrew.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/payments/homebrew.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/payments/register-wallet.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/payments/register-wallet.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/payments/wallet-list.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/payments/wallet-list.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/payments/withdraw.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/payments/withdraw.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/prostela-expert/index.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/prostela-expert/index.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/reviews/reviews.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/reviews/reviews.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/support/case-detail.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/support/case-detail.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/support/list.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/support/list.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/users/profile.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/users/profile.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/users/users-control.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/users/users-control.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templates/stela_control/users/users.html` & `stela_professional-0.4.1/stela_control/templates/stela_control/users/users.html`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/templatetags/stelatags.py` & `stela_professional-0.4.1/stela_control/templatetags/stelatags.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/tokenize.py` & `stela_professional-0.4.1/stela_control/tokenize.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/urls.py` & `stela_professional-0.4.1/stela_control/urls.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_control/views.py` & `stela_professional-0.4.1/stela_control/views.py`

 * *Files identical despite different names*

### Comparing `stela_professional-0.4.0/stela_professional.egg-info/PKG-INFO` & `stela_professional-0.4.1/stela_professional.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stela_professional
-Version: 0.4.0
+Version: 0.4.1
 Summary: All apps in one for business.
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `stela_professional-0.4.0/stela_professional.egg-info/SOURCES.txt` & `stela_professional-0.4.1/stela_professional.egg-info/SOURCES.txt`

 * *Files identical despite different names*

