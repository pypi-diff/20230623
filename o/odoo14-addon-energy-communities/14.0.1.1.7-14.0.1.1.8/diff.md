# Comparing `tmp/odoo14-addon-energy_communities-14.0.1.1.7.tar.gz` & `tmp/odoo14-addon-energy_communities-14.0.1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo14-addon-energy_communities-14.0.1.1.7.tar", last modified: Thu Jun 22 16:32:29 2023, max compression
+gzip compressed data, was "odoo14-addon-energy_communities-14.0.1.1.8.tar", last modified: Fri Jun 23 13:40:45 2023, max compression
```

## Comparing `odoo14-addon-energy_communities-14.0.1.1.7.tar` & `odoo14-addon-energy_communities-14.0.1.1.8.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.379961 odoo14-addon-energy_communities-14.0.1.1.7/
--rw-r--r--   0 enrico    (1000) enrico    (1000)      508 2023-06-22 16:32:29.379961 odoo14-addon-energy_communities-14.0.1.1.7/PKG-INFO
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.373294 odoo14-addon-energy_communities-14.0.1.1.7/odoo/
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.373294 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.373294 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/
--rw-r--r--   0 enrico    (1000) enrico    (1000)      145 2023-05-09 13:44:13.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/__init__.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     2358 2023-06-22 11:57:48.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/__manifest__.py
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.373294 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/controllers/
--rw-r--r--   0 enrico    (1000) enrico    (1000)      116 2023-05-09 14:12:27.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/controllers/__init__.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)      240 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/controllers/controllers.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)    11669 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/controllers/website_subscription_main.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)    12263 2023-05-09 14:12:27.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/controllers/website_subscription_voluntary_share.py
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.376628 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/data/
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1900 2023-02-23 08:13:19.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/data/auth_oauth_provider_data.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1695 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/data/crm_lead_tag.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)      830 2023-05-09 13:44:13.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/data/ir_cron.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)    12993 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/data/mail_template_data.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)    20442 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/data/mail_template_update_data.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1931 2023-05-09 14:12:27.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/data/product_data.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)      825 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/data/utm_data.xml
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.376628 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/demo/
--rw-r--r--   0 enrico    (1000) enrico    (1000)     2663 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/demo/demo_data.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)      553 2023-05-09 13:44:13.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/hooks.py
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.376628 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n/
--rw-r--r--   0 enrico    (1000) enrico    (1000)    87886 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n/ca_ES.po
--rw-r--r--   0 enrico    (1000) enrico    (1000)    66501 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n/energy_communities.pot
--rw-r--r--   0 enrico    (1000) enrico    (1000)    88480 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n/es.po
--rw-r--r--   0 enrico    (1000) enrico    (1000)    88715 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n/eu_ES.po
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.376628 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n_extra/
--rw-r--r--   0 enrico    (1000) enrico    (1000)   126254 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n_extra/ca_ES.po
--rw-r--r--   0 enrico    (1000) enrico    (1000)   126891 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n_extra/es.po
--rw-r--r--   0 enrico    (1000) enrico    (1000)   125321 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n_extra/eu_ES.po
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.376628 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/
--rw-r--r--   0 enrico    (1000) enrico    (1000)      435 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/__init__.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)      591 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/account_chart_template.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     2755 2023-05-09 14:12:27.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/account_move.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     4078 2023-03-16 11:09:28.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/auth_oauth_provider.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)    11809 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/crm_lead.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     4270 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/landing_page.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     5117 2023-03-16 11:09:28.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/operation_request.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1489 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/product.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)    10097 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/res_company.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)      704 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/res_config_settings.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1608 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/res_partner.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     7365 2023-03-16 11:09:28.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/res_users.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)      139 2023-03-16 11:09:28.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/res_users_role.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     4466 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/subscription_request.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)      418 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/utm_source.py
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.376628 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/pywordpress_client/
--rw-r--r--   0 enrico    (1000) enrico    (1000)        0 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/pywordpress_client/__init__.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     2713 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/pywordpress_client/client.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)      967 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/pywordpress_client/exceptions.py
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.376628 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/pywordpress_client/resources/
--rw-r--r--   0 enrico    (1000) enrico    (1000)        0 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/pywordpress_client/resources/__init__.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)      543 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/pywordpress_client/resources/authenticate.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)      746 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/pywordpress_client/resources/landing_page.py
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.376628 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/security/
--rw-r--r--   0 enrico    (1000) enrico    (1000)      277 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/security/ir.model.access.csv
--rw-r--r--   0 enrico    (1000) enrico    (1000)     3371 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/security/ir_rule_data.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)     3645 2023-05-09 13:44:13.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/security/res_users_role_data.xml
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.379961 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/services/
--rw-r--r--   0 enrico    (1000) enrico    (1000)      162 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/services/__init__.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     5281 2023-03-16 11:09:28.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/services/ce_community_service.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     2596 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/services/ce_landing_service.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     8407 2023-03-16 11:09:28.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/services/ce_member_profile_service.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     6696 2023-03-16 11:09:28.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/services/ce_member_service.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     7655 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/services/crm_lead_service.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     8338 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/services/schemas.py
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.373294 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/static/
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.379961 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/static/description/
--rw-r--r--   0 enrico    (1000) enrico    (1000)     3721 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/static/description/icon.png
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.379961 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/tests/
--rw-r--r--   0 enrico    (1000) enrico    (1000)       30 2023-05-09 13:44:13.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/tests/__init__.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)      975 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/tests/common.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)      793 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/tests/common_service.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1875 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/tests/test_crm_lead_service.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     3347 2023-05-09 13:44:13.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/tests/test_res_company.py
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.379961 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1322 2023-02-23 08:13:19.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/auth_oauth_views.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)     3354 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/ce_views.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)     3734 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/crm_lead_views.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)     2356 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/landing_page_view.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1889 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/menus.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)     3279 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/res_company_views.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1004 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/res_config_settings.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)      798 2023-03-16 11:09:28.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/res_partner_views.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)      630 2023-03-16 11:09:28.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/res_users_role_view.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)      656 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/res_users_view.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)     2054 2023-05-09 14:12:27.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/subscription_request_view.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1510 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/utm_views.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)      953 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/view_users_form.xml
--rw-r--r--   0 enrico    (1000) enrico    (1000)    19913 2023-06-19 10:18:40.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/website_subscription_template.xml
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.379961 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/wizards/
--rw-r--r--   0 enrico    (1000) enrico    (1000)       41 2023-02-16 11:43:59.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/wizards/__init__.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     5119 2023-05-09 13:44:13.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/wizards/multicompany_easy_creation.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1598 2023-05-09 13:44:13.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-06-22 16:32:29.379961 odoo14-addon-energy_communities-14.0.1.1.7/odoo14_addon_energy_communities.egg-info/
--rw-rw-r--   0 enrico    (1000) enrico    (1000)      508 2023-06-22 16:32:29.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo14_addon_energy_communities.egg-info/PKG-INFO
--rw-rw-r--   0 enrico    (1000) enrico    (1000)     4688 2023-06-22 16:32:29.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo14_addon_energy_communities.egg-info/SOURCES.txt
--rw-rw-r--   0 enrico    (1000) enrico    (1000)        1 2023-06-22 16:32:29.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo14_addon_energy_communities.egg-info/dependency_links.txt
--rw-rw-r--   0 enrico    (1000) enrico    (1000)        1 2023-06-22 10:46:23.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo14_addon_energy_communities.egg-info/not-zip-safe
--rw-rw-r--   0 enrico    (1000) enrico    (1000)      965 2023-06-22 16:32:29.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo14_addon_energy_communities.egg-info/requires.txt
--rw-rw-r--   0 enrico    (1000) enrico    (1000)        5 2023-06-22 16:32:29.000000 odoo14-addon-energy_communities-14.0.1.1.7/odoo14_addon_energy_communities.egg-info/top_level.txt
--rw-r--r--   0 enrico    (1000) enrico    (1000)       38 2023-06-22 16:32:29.379961 odoo14-addon-energy_communities-14.0.1.1.7/setup.cfg
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1243 2023-06-22 11:55:45.000000 odoo14-addon-energy_communities-14.0.1.1.7/setup.py
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.317739 odoo14-addon-energy_communities-14.0.1.1.8/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      462 2023-06-23 13:40:45.317739 odoo14-addon-energy_communities-14.0.1.1.8/PKG-INFO
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.301739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.301739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.305739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      145 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     2358 2023-06-23 13:40:08.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/__manifest__.py
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.305739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/controllers/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      116 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/controllers/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      240 2023-05-09 15:31:03.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/controllers/controllers.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    11669 2023-06-23 13:36:24.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/controllers/website_subscription_main.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    12263 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/controllers/website_subscription_voluntary_share.py
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.305739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/data/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1900 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/data/auth_oauth_provider_data.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1695 2023-05-09 15:31:03.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/data/crm_lead_tag.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      830 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/data/ir_cron.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    12993 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/data/mail_template_data.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    20442 2023-06-23 13:36:24.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/data/mail_template_update_data.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1931 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/data/product_data.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      825 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/data/utm_data.xml
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.305739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/demo/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     2663 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/demo/demo_data.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      553 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/hooks.py
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.309739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    87886 2023-06-23 13:36:24.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n/ca_ES.po
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    66501 2023-06-23 13:36:24.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n/energy_communities.pot
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    88480 2023-06-23 13:36:24.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n/es.po
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    88715 2023-06-23 13:36:24.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n/eu_ES.po
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.309739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n_extra/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)   126254 2023-06-23 13:36:24.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n_extra/ca_ES.po
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)   126891 2023-06-23 13:36:24.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n_extra/es.po
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)   125321 2023-06-23 13:36:24.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n_extra/eu_ES.po
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.309739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      435 2023-06-14 10:42:12.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      591 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/account_chart_template.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     2755 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/account_move.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     4078 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/auth_oauth_provider.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    11809 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/crm_lead.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     4270 2023-06-23 13:36:24.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/landing_page.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     5117 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/operation_request.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1489 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/product.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    10097 2023-06-14 10:42:12.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/res_company.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      704 2023-06-14 10:42:12.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/res_config_settings.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1608 2023-06-23 13:36:24.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/res_partner.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     7365 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/res_users.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      139 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/res_users_role.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     4466 2023-06-23 13:36:24.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/subscription_request.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      418 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/utm_source.py
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.313739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/pywordpress_client/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)        0 2023-06-14 10:42:12.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/pywordpress_client/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     2713 2023-06-14 10:42:12.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/pywordpress_client/client.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      967 2023-06-14 10:42:12.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/pywordpress_client/exceptions.py
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.313739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/pywordpress_client/resources/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)        0 2023-06-14 10:42:12.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/pywordpress_client/resources/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      543 2023-06-14 10:42:12.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/pywordpress_client/resources/authenticate.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      746 2023-06-14 10:42:12.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/pywordpress_client/resources/landing_page.py
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.313739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/security/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      277 2023-06-14 10:42:12.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/security/ir.model.access.csv
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     3371 2023-06-14 10:42:12.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/security/ir_rule_data.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     3645 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/security/res_users_role_data.xml
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.313739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/services/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      162 2023-06-14 10:42:12.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/services/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     5281 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/services/ce_community_service.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     2596 2023-06-23 13:36:24.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/services/ce_landing_service.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     8407 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/services/ce_member_profile_service.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     6696 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/services/ce_member_service.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     7655 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/services/crm_lead_service.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     8338 2023-06-14 10:42:12.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/services/schemas.py
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.305739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/static/
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.313739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/static/description/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     3721 2023-05-09 15:31:03.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/static/description/icon.png
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.313739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/tests/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)       30 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/tests/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      975 2023-05-09 15:31:03.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/tests/common.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      793 2023-05-09 15:31:03.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/tests/common_service.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1875 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/tests/test_crm_lead_service.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     3347 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/tests/test_res_company.py
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.317739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1322 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/auth_oauth_views.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     3354 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/ce_views.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     3734 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/crm_lead_views.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     2356 2023-06-23 13:36:24.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/landing_page_view.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1889 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/menus.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     3279 2023-06-14 10:42:12.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/res_company_views.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1004 2023-06-14 10:42:12.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/res_config_settings.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      798 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/res_partner_views.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      630 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/res_users_role_view.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      656 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/res_users_view.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     2054 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/subscription_request_view.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1510 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/utm_views.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      953 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/view_users_form.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    19913 2023-06-23 13:36:24.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/website_subscription_template.xml
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.317739 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/wizards/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)       41 2023-05-09 15:31:03.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/wizards/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     5119 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/wizards/multicompany_easy_creation.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1598 2023-05-15 12:39:43.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml
+drwxrwsr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-23 13:40:45.317739 odoo14-addon-energy_communities-14.0.1.1.8/odoo14_addon_energy_communities.egg-info/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      462 2023-06-23 13:40:45.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo14_addon_energy_communities.egg-info/PKG-INFO
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     4688 2023-06-23 13:40:45.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo14_addon_energy_communities.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-06-23 13:40:45.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo14_addon_energy_communities.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-06-23 13:40:45.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo14_addon_energy_communities.egg-info/not-zip-safe
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      965 2023-06-23 13:40:45.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo14_addon_energy_communities.egg-info/requires.txt
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)        5 2023-06-23 13:40:45.000000 odoo14-addon-energy_communities-14.0.1.1.8/odoo14_addon_energy_communities.egg-info/top_level.txt
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)       38 2023-06-23 13:40:45.317739 odoo14-addon-energy_communities-14.0.1.1.8/setup.cfg
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1243 2023-06-23 13:37:23.000000 odoo14-addon-energy_communities-14.0.1.1.8/setup.py
```

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/__manifest__.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/__manifest__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': "Energy Community",
-    'version': '14.0.1.1.7',
+    'version': '14.0.1.1.8',
     'depends': [
         'account',
         'cooperator_account_banking_mandate',
         'account_lock_date_update',
         'account_multicompany_easy_creation',
         'cooperator_account_payment',
         'account_payment_order',
```

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/controllers/website_subscription_main.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/controllers/website_subscription_main.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/controllers/website_subscription_voluntary_share.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/controllers/website_subscription_voluntary_share.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/data/auth_oauth_provider_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/data/auth_oauth_provider_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/data/crm_lead_tag.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/data/crm_lead_tag.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/data/ir_cron.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/data/ir_cron.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/data/mail_template_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/data/mail_template_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/data/mail_template_update_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/data/mail_template_update_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/data/product_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/data/product_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/data/utm_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/data/utm_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/demo/demo_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/demo/demo_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/hooks.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/hooks.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n/ca_ES.po` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n/ca_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n/energy_communities.pot` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n/energy_communities.pot`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n/es.po` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n/es.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n/eu_ES.po` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n/eu_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n_extra/ca_ES.po` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n_extra/ca_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n_extra/es.po` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n_extra/es.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/i18n_extra/eu_ES.po` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/i18n_extra/eu_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/account_chart_template.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/account_chart_template.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/account_move.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/account_move.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/auth_oauth_provider.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/auth_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/crm_lead.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/crm_lead.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/landing_page.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/landing_page.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/operation_request.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/operation_request.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/product.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/product.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/res_company.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/res_company.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/res_config_settings.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/res_config_settings.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/res_partner.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/res_partner.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/res_users.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/res_users.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/models/subscription_request.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/models/subscription_request.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/pywordpress_client/client.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/pywordpress_client/client.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/pywordpress_client/exceptions.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/pywordpress_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/pywordpress_client/resources/authenticate.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/pywordpress_client/resources/authenticate.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/pywordpress_client/resources/landing_page.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/pywordpress_client/resources/landing_page.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/security/ir_rule_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/security/ir_rule_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/security/res_users_role_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/security/res_users_role_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/services/ce_community_service.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/services/ce_community_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/services/ce_landing_service.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/services/ce_landing_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/services/ce_member_profile_service.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/services/ce_member_profile_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/services/ce_member_service.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/services/ce_member_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/services/crm_lead_service.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/services/crm_lead_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/services/schemas.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/services/schemas.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/static/description/icon.png` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/static/description/icon.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/tests/common.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/tests/common.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/tests/common_service.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/tests/common_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/tests/test_crm_lead_service.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/tests/test_crm_lead_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/tests/test_res_company.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/tests/test_res_company.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/auth_oauth_views.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/auth_oauth_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/ce_views.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/ce_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/crm_lead_views.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/crm_lead_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/landing_page_view.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/landing_page_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/menus.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/menus.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/res_company_views.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/res_company_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/res_config_settings.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/res_config_settings.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/res_partner_views.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/res_partner_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/res_users_role_view.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/res_users_role_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/res_users_view.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/res_users_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/subscription_request_view.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/subscription_request_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/utm_views.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/utm_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/view_users_form.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/view_users_form.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/views/website_subscription_template.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/views/website_subscription_template.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/wizards/multicompany_easy_creation.py` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/wizards/multicompany_easy_creation.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo14_addon_energy_communities.egg-info/SOURCES.txt` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo14_addon_energy_communities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/odoo14_addon_energy_communities.egg-info/requires.txt` & `odoo14-addon-energy_communities-14.0.1.1.8/odoo14_addon_energy_communities.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 odoo14-addon-auth_oidc
 odoo14-addon-base_rest
 odoo14-addon-base_technical_features
 odoo14-addon-base_user_role
 odoo14-addon-base_user_role_company
 odoo14-addon-community-maps==14.0.0.1.6.dev1
 odoo14-addon-cooperator
-odoo14-addon-cooperator-account-banking-mandate==14.0.1.0.2
+odoo14-addon-cooperator-account-banking-mandate==14.0.1.0.3
 odoo14-addon-cooperator-account-payment==14.0.1.0.1
 odoo14-addon-crm-metadata-rest-api==14.0.1.0.1
 odoo14-addon-crm-metadata==14.0.1.0.0
 odoo14-addon-crm-rest-api==14.0.1.0.1
 odoo14-addon-l10n-es-aeat-sii-oca==14.0.2.8.1
 odoo14-addon-l10n_es_aeat
 odoo14-addon-l10n_es_cooperator
```

### Comparing `odoo14-addon-energy_communities-14.0.1.1.7/setup.py` & `odoo14-addon-energy_communities-14.0.1.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     setup_requires=['setuptools-odoo'],
     odoo_addon={
         "depends_override": {
             "account_lock_date_update": "odoo14-addon-account-lock-date-update==14.0.2.0.1.dev10",
             "account_reconciliation_widget": "odoo14-addon-account-reconciliation-widget==14.0.2.0.2",
             "community_maps": "odoo14-addon-community-maps==14.0.0.1.6.dev1",
             "cooperator_account_payment": "odoo14-addon-cooperator-account-payment==14.0.1.0.1",
-            "cooperator_account_banking_mandate": "odoo14-addon-cooperator-account-banking-mandate==14.0.1.0.2",
+            "cooperator_account_banking_mandate": "odoo14-addon-cooperator-account-banking-mandate==14.0.1.0.3",
             "crm_metadata": "odoo14-addon-crm-metadata==14.0.1.0.0",
             "crm_metadata_rest_api": "odoo14-addon-crm-metadata-rest-api==14.0.1.0.1",
             "crm_rest_api": "odoo14-addon-crm-rest-api==14.0.1.0.1",
             "l10n_es_aeat_sii_oca": "odoo14-addon-l10n-es-aeat-sii-oca==14.0.2.8.1",
             "mail_multicompany": "odoo14-addon-mail-multicompany==14.0.0.1.1.dev2",
             "metadata": "odoo14-addon-metadata==14.0.0.0.1",
             "partner_multi_company": "odoo14-addon-partner-multi-company==14.0.1.0.1.dev4",
```

