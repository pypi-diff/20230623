# Comparing `tmp/cid-cmd-0.2.8.tar.gz` & `tmp/cid-cmd-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cid-cmd-0.2.8.tar", last modified: Mon Jan 16 15:43:42 2023, max compression
+gzip compressed data, was "cid-cmd-0.2.9.tar", last modified: Mon Jan 16 18:21:08 2023, max compression
```

## Comparing `cid-cmd-0.2.8.tar` & `cid-cmd-0.2.9.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.822487 cid-cmd-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-01-16 15:43:42.822487 cid-cmd-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.810487 cid-cmd-0.2.8/cid/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.810487 cid-cmd-0.2.8/cid/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.810487 cid-cmd-0.2.8/cid/builtin/core/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.810487 cid-cmd-0.2.8/cid/builtin/core/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.806487 cid-cmd-0.2.8/cid/builtin/core/data/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.810487 cid-cmd-0.2.8/cid/builtin/core/data/datasets/cid/
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/datasets/cid/compute.json
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/datasets/cid/ec2_running_cost.json
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/datasets/cid/s3_view.json
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/datasets/cid/summary_view.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.810487 cid-cmd-0.2.8/cid/builtin/core/data/datasets/co/
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/datasets/co/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.814487 cid-cmd-0.2.8/cid/builtin/core/data/datasets/kpi/
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/datasets/kpi/kpi_ebs_snap.json
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/datasets/kpi/kpi_ebs_storage_all.json
--rw-r--r--   0 runner    (1001) docker     (123)    20317 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/datasets/kpi/kpi_instance_all.json
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/datasets/kpi/kpi_s3_storage_all.json
--rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/datasets/kpi/kpi_tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.814487 cid-cmd-0.2.8/cid/builtin/core/data/datasets/shared/
--rw-r--r--   0 runner    (1001) docker     (123)    33424 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/datasets/shared/customer_all.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.814487 cid-cmd-0.2.8/cid/builtin/core/data/datasets/tao/
--rw-r--r--   0 runner    (1001) docker     (123)    67579 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/datasets/tao/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.814487 cid-cmd-0.2.8/cid/builtin/core/data/datasets/trends/
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/datasets/trends/daily_anomaly_detection.json
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/datasets/trends/monthly_anomaly_detection.json
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/datasets/trends/monthly_bill_by_account.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.814487 cid-cmd-0.2.8/cid/builtin/core/data/permissions/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/permissions/dashboard_permissions.json
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/permissions/dashboard_permissions_namespace.json
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/permissions/data_set_permissions.json
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/permissions/data_source_permissions.json
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/permissions/folder_permissions.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.810487 cid-cmd-0.2.8/cid/builtin/core/data/queries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.814487 cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/compute_savings_plan_eligible_spend.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ec2_running_cost.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ec2_running_cost_ri.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ec2_running_cost_sp.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ec2_running_cost_sp_ri.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ri_sp_mapping.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ri_sp_mapping_ri.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp_ri.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/s3.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/summary_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/summary_view_ri.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/summary_view_sp.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/summary_view_sp_ri.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.818487 cid-cmd-0.2.8/cid/builtin/core/data/queries/co/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/co/all_options.sql
--rw-r--r--   0 runner    (1001) docker     (123)    14711 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/co/auto_scale.json
--rw-r--r--   0 runner    (1001) docker     (123)    26157 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/co/auto_scale_options.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/co/ebs_volume.json
--rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/co/ebs_volume_options.sql
--rw-r--r--   0 runner    (1001) docker     (123)    18754 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/co/ec2_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    27437 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/co/ec2_instance_options.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/co/lambda.json
--rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/co/lambda_options.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.818487 cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/first_kpi_instance_mapping_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/kpi_ebs_snap_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/kpi_ebs_storage_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)    23793 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/kpi_instance_all_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)    22987 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRI.sql
--rw-r--r--   0 runner    (1001) docker     (123)    21969 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRISP.sql
--rw-r--r--   0 runner    (1001) docker     (123)    22847 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noSP.sql
--rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/kpi_s3_storage_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/last_kpi_tracker_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.818487 cid-cmd-0.2.8/cid/builtin/core/data/queries/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/shared/account_map.sql
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/shared/account_map_dummy.sql
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/shared/aws_accounts.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/shared/aws_regions.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/shared/aws_service_category_map.sql
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/shared/business_units_map.sql
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/shared/payer_account_name_map.sql
--rw-r--r--   0 runner    (1001) docker     (123)   142433 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/shared/ta_descriptions.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.818487 cid-cmd-0.2.8/cid/builtin/core/data/queries/tao/
--rw-r--r--   0 runner    (1001) docker     (123)    35595 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/tao/glue_table.json
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/tao/ta_org_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.822487 cid-cmd-0.2.8/cid/builtin/core/data/queries/trends/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/trends/daily_anomaly_detection.sql
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/trends/monthly_anomaly_detection.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/trends/monthly_bill_by_account.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/trends/monthly_bill_by_account_ri.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp_ri.sql
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/builtin/core/data/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    60769 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.822487 cid-cmd-0.2.8/cid/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/helpers/account_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/helpers/athena.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/helpers/cur.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/helpers/glue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.822487 cid-cmd-0.2.8/cid/helpers/quicksight/
--rw-r--r--   0 runner    (1001) docker     (123)    49795 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/helpers/quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/helpers/quicksight/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/helpers/quicksight/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/helpers/quicksight/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/helpers/quicksight/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/helpers/quicksight/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.822487 cid-cmd-0.2.8/cid/queries/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/queries/ahq-queries.json
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/queries/ri_present.sql
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/queries/sp_present.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/cid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 15:43:42.822487 cid-cmd-0.2.8/cid_cmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-01-16 15:43:42.000000 cid-cmd-0.2.8/cid_cmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-01-16 15:43:42.000000 cid-cmd-0.2.8/cid_cmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 15:43:42.000000 cid-cmd-0.2.8/cid_cmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-16 15:43:42.000000 cid-cmd-0.2.8/cid_cmd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-16 15:43:42.000000 cid-cmd-0.2.8/cid_cmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-16 15:43:42.000000 cid-cmd-0.2.8/cid_cmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-16 15:43:33.000000 cid-cmd-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-16 15:43:42.822487 cid-cmd-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.810700 cid-cmd-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-01-16 18:21:08.810700 cid-cmd-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.798700 cid-cmd-0.2.9/cid/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.798700 cid-cmd-0.2.9/cid/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.798700 cid-cmd-0.2.9/cid/builtin/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.798700 cid-cmd-0.2.9/cid/builtin/core/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.794700 cid-cmd-0.2.9/cid/builtin/core/data/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.798700 cid-cmd-0.2.9/cid/builtin/core/data/datasets/cid/
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/datasets/cid/compute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/datasets/cid/ec2_running_cost.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/datasets/cid/s3_view.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/datasets/cid/summary_view.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.798700 cid-cmd-0.2.9/cid/builtin/core/data/datasets/co/
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/datasets/co/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.798700 cid-cmd-0.2.9/cid/builtin/core/data/datasets/kpi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/datasets/kpi/kpi_ebs_snap.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/datasets/kpi/kpi_ebs_storage_all.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20317 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/datasets/kpi/kpi_instance_all.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/datasets/kpi/kpi_s3_storage_all.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/datasets/kpi/kpi_tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.798700 cid-cmd-0.2.9/cid/builtin/core/data/datasets/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)    33424 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/datasets/shared/customer_all.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.802700 cid-cmd-0.2.9/cid/builtin/core/data/datasets/tao/
+-rw-r--r--   0 runner    (1001) docker     (123)    67579 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/datasets/tao/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.802700 cid-cmd-0.2.9/cid/builtin/core/data/datasets/trends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/datasets/trends/daily_anomaly_detection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/datasets/trends/monthly_anomaly_detection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/datasets/trends/monthly_bill_by_account.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.802700 cid-cmd-0.2.9/cid/builtin/core/data/permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/permissions/dashboard_permissions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/permissions/dashboard_permissions_namespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/permissions/data_set_permissions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/permissions/data_source_permissions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/permissions/folder_permissions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.798700 cid-cmd-0.2.9/cid/builtin/core/data/queries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.802700 cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/compute_savings_plan_eligible_spend.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ec2_running_cost.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ec2_running_cost_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ec2_running_cost_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ec2_running_cost_sp_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ri_sp_mapping.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ri_sp_mapping_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/s3.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/summary_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/summary_view_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/summary_view_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/summary_view_sp_ri.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.802700 cid-cmd-0.2.9/cid/builtin/core/data/queries/co/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/co/all_options.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    14711 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/co/auto_scale.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26157 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/co/auto_scale_options.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/co/ebs_volume.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/co/ebs_volume_options.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    18754 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/co/ec2_instance.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27437 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/co/ec2_instance_options.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/co/lambda.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/co/lambda_options.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.806700 cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/first_kpi_instance_mapping_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/kpi_ebs_snap_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/kpi_ebs_storage_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    23793 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/kpi_instance_all_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    22987 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRI.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    21969 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRISP.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    22847 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noSP.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/kpi_s3_storage_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/last_kpi_tracker_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.806700 cid-cmd-0.2.9/cid/builtin/core/data/queries/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/shared/account_map.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/shared/account_map_dummy.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/shared/aws_accounts.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/shared/aws_regions.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/shared/aws_service_category_map.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/shared/business_units_map.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/shared/payer_account_name_map.sql
+-rw-r--r--   0 runner    (1001) docker     (123)   142433 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/shared/ta_descriptions.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.806700 cid-cmd-0.2.9/cid/builtin/core/data/queries/tao/
+-rw-r--r--   0 runner    (1001) docker     (123)    35595 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/tao/glue_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/tao/ta_org_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.806700 cid-cmd-0.2.9/cid/builtin/core/data/queries/trends/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/trends/daily_anomaly_detection.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/trends/monthly_anomaly_detection.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/trends/monthly_bill_by_account.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/trends/monthly_bill_by_account_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/builtin/core/data/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60837 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.806700 cid-cmd-0.2.9/cid/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/helpers/account_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/helpers/athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/helpers/cur.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/helpers/glue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.806700 cid-cmd-0.2.9/cid/helpers/quicksight/
+-rw-r--r--   0 runner    (1001) docker     (123)    49795 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/helpers/quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/helpers/quicksight/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/helpers/quicksight/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/helpers/quicksight/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/helpers/quicksight/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/helpers/quicksight/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.810700 cid-cmd-0.2.9/cid/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/queries/ahq-queries.json
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/queries/ri_present.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/queries/sp_present.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/cid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 18:21:08.810700 cid-cmd-0.2.9/cid_cmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-01-16 18:21:08.000000 cid-cmd-0.2.9/cid_cmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-01-16 18:21:08.000000 cid-cmd-0.2.9/cid_cmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 18:21:08.000000 cid-cmd-0.2.9/cid_cmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-16 18:21:08.000000 cid-cmd-0.2.9/cid_cmd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-16 18:21:08.000000 cid-cmd-0.2.9/cid_cmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-16 18:21:08.000000 cid-cmd-0.2.9/cid_cmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-16 18:20:59.000000 cid-cmd-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-16 18:21:08.810700 cid-cmd-0.2.9/setup.cfg
```

### Comparing `cid-cmd-0.2.8/LICENSE` & `cid-cmd-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/PKG-INFO` & `cid-cmd-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cid-cmd
-Version: 0.2.8
+Version: 0.2.9
 Summary: Cloud Intelligence Dashboards deployment helper tool
 Home-page: https://github.com/aws-samples/aws-cudos-framework-deployment
 Author: AWS CUDOS Team
 License: MIT
 Keywords: aws,cmd,cli,cost intelligence dashboards
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cid-cmd-0.2.8/README.md` & `cid-cmd-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/base.py` & `cid-cmd-0.2.9/cid/base.py`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/datasets/cid/compute.json` & `cid-cmd-0.2.9/cid/builtin/core/data/datasets/cid/compute.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/datasets/cid/ec2_running_cost.json` & `cid-cmd-0.2.9/cid/builtin/core/data/datasets/cid/ec2_running_cost.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/datasets/cid/s3_view.json` & `cid-cmd-0.2.9/cid/builtin/core/data/datasets/cid/s3_view.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/datasets/cid/summary_view.json` & `cid-cmd-0.2.9/cid/builtin/core/data/datasets/cid/summary_view.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/datasets/co/dataset.json` & `cid-cmd-0.2.9/cid/builtin/core/data/datasets/co/dataset.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/datasets/kpi/kpi_ebs_snap.json` & `cid-cmd-0.2.9/cid/builtin/core/data/datasets/kpi/kpi_ebs_snap.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/datasets/kpi/kpi_ebs_storage_all.json` & `cid-cmd-0.2.9/cid/builtin/core/data/datasets/kpi/kpi_ebs_storage_all.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/datasets/kpi/kpi_instance_all.json` & `cid-cmd-0.2.9/cid/builtin/core/data/datasets/kpi/kpi_instance_all.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/datasets/kpi/kpi_s3_storage_all.json` & `cid-cmd-0.2.9/cid/builtin/core/data/datasets/kpi/kpi_s3_storage_all.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/datasets/kpi/kpi_tracker.json` & `cid-cmd-0.2.9/cid/builtin/core/data/datasets/kpi/kpi_tracker.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/datasets/shared/customer_all.json` & `cid-cmd-0.2.9/cid/builtin/core/data/datasets/shared/customer_all.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/datasets/tao/dataset.json` & `cid-cmd-0.2.9/cid/builtin/core/data/datasets/tao/dataset.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/datasets/trends/daily_anomaly_detection.json` & `cid-cmd-0.2.9/cid/builtin/core/data/datasets/trends/daily_anomaly_detection.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/datasets/trends/monthly_anomaly_detection.json` & `cid-cmd-0.2.9/cid/builtin/core/data/datasets/trends/monthly_anomaly_detection.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/datasets/trends/monthly_bill_by_account.json` & `cid-cmd-0.2.9/cid/builtin/core/data/datasets/trends/monthly_bill_by_account.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/compute_savings_plan_eligible_spend.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/compute_savings_plan_eligible_spend.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ec2_running_cost.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ec2_running_cost.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ec2_running_cost_ri.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ec2_running_cost_ri.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ec2_running_cost_sp.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ec2_running_cost_sp.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ec2_running_cost_sp_ri.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ec2_running_cost_sp_ri.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ri_sp_mapping.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ri_sp_mapping.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ri_sp_mapping_ri.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ri_sp_mapping_ri.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp_ri.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp_ri.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/s3.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/s3.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/summary_view.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/summary_view.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/summary_view_ri.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/summary_view_ri.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/summary_view_sp.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/summary_view_sp.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/cid/summary_view_sp_ri.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/cid/summary_view_sp_ri.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/co/auto_scale.json` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/co/auto_scale.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/co/auto_scale_options.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/co/auto_scale_options.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/co/ebs_volume.json` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/co/ebs_volume.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/co/ebs_volume_options.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/co/ebs_volume_options.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/co/ec2_instance.json` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/co/ec2_instance.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/co/ec2_instance_options.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/co/ec2_instance_options.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/co/lambda.json` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/co/lambda.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/co/lambda_options.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/co/lambda_options.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/first_kpi_instance_mapping_view.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/first_kpi_instance_mapping_view.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/kpi_ebs_snap_view.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/kpi_ebs_snap_view.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/kpi_ebs_storage_view.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/kpi_ebs_storage_view.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/kpi_instance_all_view.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/kpi_instance_all_view.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRI.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRI.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRISP.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRISP.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noSP.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noSP.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/kpi_s3_storage_view.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/kpi_s3_storage_view.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/kpi/last_kpi_tracker_view.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/kpi/last_kpi_tracker_view.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/shared/aws_accounts.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/shared/aws_accounts.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/shared/aws_regions.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/shared/aws_regions.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/shared/aws_service_category_map.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/shared/aws_service_category_map.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/shared/ta_descriptions.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/shared/ta_descriptions.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/tao/glue_table.json` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/tao/glue_table.json`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/tao/ta_org_view.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/tao/ta_org_view.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/trends/daily_anomaly_detection.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/trends/daily_anomaly_detection.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/trends/monthly_anomaly_detection.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/trends/monthly_anomaly_detection.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/trends/monthly_bill_by_account.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/trends/monthly_bill_by_account.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/trends/monthly_bill_by_account_ri.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/trends/monthly_bill_by_account_ri.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp_ri.sql` & `cid-cmd-0.2.9/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp_ri.sql`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/builtin/core/data/resources.yaml` & `cid-cmd-0.2.9/cid/builtin/core/data/resources.yaml`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/cli.py` & `cid-cmd-0.2.9/cid/cli.py`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/common.py` & `cid-cmd-0.2.9/cid/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -793,20 +793,20 @@
 
             logger.debug("The dashboard is up-to-date")
             logger.debug(f"CID Version      {cid_version}")
             logger.debug(f"TemplateVersion  {dashboard.deployed_version} ")
         else:
             print(f"An update is available:")
             print("                   Deployed -> Latest")
-            print(f"  CID Version      {cid_version: <9}   {cid_version_latest: <6}")
-            print(f"  TemplateVersion  {template_version: <9}   {template_version_latest: <6}")
+            print(f"  CID Version      {str(cid_version): <9}   {str(cid_version_latest): <6}")
+            print(f"  TemplateVersion  {str(dashboard.deployedTemplate.version): <9}   {dashboard.latest_version: <6}")
 
             logger.debug("An update is available")
-            logger.debug(f"CID Version      {cid_version: <9} --> {cid_version_latest: <6}")
-            logger.debug(f"TemplateVersion  {template_version: <9} -->  {template_version_latest: <6}")
+            logger.debug(f"CID Version      {str(cid_version): <9} --> {str(cid_version_latest): <6}")
+            logger.debug(f"TemplateVersion  {str(dashboard.deployedTemplate.version): <9} -->  {dashboard.latest_version: <6}")
 
         # Check if version are compatible
         compatible = None
         try:
             compatible = dashboard.sourceTemplate.cid_version.compatible_versions(dashboard.deployedTemplate.cid_version)
         except ValueError as e:
             logger.info(e)
```

### Comparing `cid-cmd-0.2.8/cid/export.py` & `cid-cmd-0.2.9/cid/export.py`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/helpers/account_map.py` & `cid-cmd-0.2.9/cid/helpers/account_map.py`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/helpers/athena.py` & `cid-cmd-0.2.9/cid/helpers/athena.py`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/helpers/cur.py` & `cid-cmd-0.2.9/cid/helpers/cur.py`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/helpers/glue.py` & `cid-cmd-0.2.9/cid/helpers/glue.py`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/helpers/quicksight/__init__.py` & `cid-cmd-0.2.9/cid/helpers/quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/helpers/quicksight/dashboard.py` & `cid-cmd-0.2.9/cid/helpers/quicksight/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,27 +119,28 @@
             cid_version = "N/A"
 
         try:
             cid_version_latest = self.sourceTemplate.cid_version if isinstance(self.sourceTemplate, CidQsTemplate) else "N/A"
         except ValueError:
             logger.debug("The latest version of the dashboard could not be retrieved")
             cid_version_latest = "N/A"
-            print(f"  CID Version {cid_version}")
+            print(f"  CID Version     {cid_version}")
             print(f"  TemplateVersion {self.deployed_version} ")
 
+        if self.latest:
             logger.debug("The dashboard is up-to-date")
             logger.debug(f"CID Version {cid_version}")
             logger.debug(f"TemplateVersion {self.deployed_version} ")
         else:
-            print(f"  CID Version {cid_version: <9} --> {cid_version_latest: <6}")
-            print(f"  TemplateVersion {self.deployed_version: <9} --> {self.latest_version: <6}")
+            print(f"  CID Version     {str(cid_version): <6} --> {str(cid_version_latest): <6}")
+            print(f"  TemplateVersion {str(self.deployed_version): <6} --> {str(self.latest_version): <6}")
 
             logger.debug("An update is available")
-            logger.debug(f"CID Version      {cid_version: <9} --> {cid_version_latest: <6}")
-            logger.debug(f"TemplateVersion  {self.deployed_version: <9} -->  {self.latest_version: <6}")
+            logger.debug(f"CID Version      {str(cid_version): <9} --> {str(cid_version_latest): <6}")
+            logger.debug(f"TemplateVersion  {str(self.deployed_version): <9} -->  {str(self.latest_version): <6}")
             
         if self.datasets:
             print(f"  Datasets: {', '.join(sorted(self.datasets.keys()))}")
         print('\n')
         if click.confirm('Display dashboard raw data?'):
             print(json.dumps(self.raw, indent=4, sort_keys=True, default=str))
```

### Comparing `cid-cmd-0.2.8/cid/helpers/quicksight/dataset.py` & `cid-cmd-0.2.9/cid/helpers/quicksight/dataset.py`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/helpers/quicksight/datasource.py` & `cid-cmd-0.2.9/cid/helpers/quicksight/datasource.py`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/helpers/quicksight/template.py` & `cid-cmd-0.2.9/cid/helpers/quicksight/template.py`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/logger.py` & `cid-cmd-0.2.9/cid/logger.py`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/plugin.py` & `cid-cmd-0.2.9/cid/plugin.py`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid/utils.py` & `cid-cmd-0.2.9/cid/utils.py`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/cid_cmd.egg-info/PKG-INFO` & `cid-cmd-0.2.9/cid_cmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cid-cmd
-Version: 0.2.8
+Version: 0.2.9
 Summary: Cloud Intelligence Dashboards deployment helper tool
 Home-page: https://github.com/aws-samples/aws-cudos-framework-deployment
 Author: AWS CUDOS Team
 License: MIT
 Keywords: aws,cmd,cli,cost intelligence dashboards
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cid-cmd-0.2.8/cid_cmd.egg-info/SOURCES.txt` & `cid-cmd-0.2.9/cid_cmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cid-cmd-0.2.8/setup.cfg` & `cid-cmd-0.2.9/setup.cfg`

 * *Files identical despite different names*

