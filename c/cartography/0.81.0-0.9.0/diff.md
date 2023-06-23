# Comparing `tmp/cartography-0.81.0.tar.gz` & `tmp/cartography-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cartography-0.81.0.tar", last modified: Fri Jun 23 16:41:39 2023, max compression
+gzip compressed data, was "dist/cartography-0.9.0.tar", last modified: Mon Aug 19 22:00:36 2019, max compression
```

## Comparing `cartography-0.81.0.tar` & `cartography-0.9.0.tar`

### file list

```diff
@@ -1,361 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.160813 cartography-0.81.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-23 16:41:29.000000 cartography-0.81.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-23 16:41:29.000000 cartography-0.81.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-23 16:41:39.160813 cartography-0.81.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-23 16:41:29.000000 cartography-0.81.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.112810 cartography-0.81.0/cartography/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28833 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.112810 cartography-0.81.0/cartography/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.112810 cartography-0.81.0/cartography/client/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/client/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/client/aws/iam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.112810 cartography-0.81.0/cartography/client/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/client/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10805 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/client/core/tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.112810 cartography-0.81.0/cartography/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/indexes.cypher
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.112810 cartography-0.81.0/cartography/data/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.116810 cartography-0.81.0/cartography/data/jobs/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/analysis/aws_ec2_asset_exposure.json
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/analysis/aws_ec2_iaminstance.json
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/analysis/aws_ec2_iaminstanceprofile.json
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/analysis/aws_ec2_keypair_analysis.json
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/analysis/aws_eks_asset_exposure.json
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/analysis/aws_foreign_accounts.json
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/analysis/aws_lambda_ecr.json
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/analysis/aws_s3acl_analysis.json
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/analysis/gcp_compute_asset_inet_exposure.json
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/analysis/gcp_gke_asset_exposure.json
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/analysis/gcp_gke_basic_auth.json
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/analysis/gsuite_human_link.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.132811 cartography-0.81.0/cartography/data/jobs/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_account_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_apigateway_details.json
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_dns_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_account_access_key_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_apigateway_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_config_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_ec2_launch_configurations_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_ec2_launch_templates_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_ec2_security_groupinfo_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_ecr_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_ecs_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_eks_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_elastic_ip_addresses_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_elasticache_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_es_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_groups_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_groups_membership_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_groups_policy_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_inspector_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_internet_gateways_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_kms_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_lambda_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_principals_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_rds_clusters_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_rds_instances_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_rds_snapshots_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_redshift_clusters_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_reserved_instances_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_roles_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_roles_policy_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_s3_acl_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_s3_buckets_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_secrets_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_securityhub_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_snapshots_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_sqs_queues_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_ssm_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_tags_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_tgw_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_users_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_vpc_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_vpc_peering_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_ingest_ec2_auto_scaling_groups_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_ingest_load_balancers_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_ingest_load_balancers_v2_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_ingest_network_interfaces_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_ingest_subnets_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_kms_details.json
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_post_ingestion_principals_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/aws_s3_details.json
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/azure_cosmosdb_cassandra_keyspace_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/azure_cosmosdb_cors_details.json
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/azure_cosmosdb_mongodb_database_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/azure_cosmosdb_sql_database_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/azure_cosmosdb_table_resources_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/azure_database_account_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/azure_import_disks_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/azure_import_snapshots_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/azure_import_virtual_machines_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/azure_sql_server_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/azure_storage_account_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/azure_subscriptions_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/azure_tenant_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/crowdstrike_import_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/crxcavator_import_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/digitalocean_droplet_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/digitalocean_project_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/gcp_compute_firewall_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/gcp_compute_forwarding_rules_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/gcp_compute_instance_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/gcp_compute_vpc_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/gcp_compute_vpc_subnet_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/gcp_crm_folder_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/gcp_crm_organization_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/gcp_crm_project_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/gcp_dns_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/gcp_gke_cluster_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/gcp_storage_bucket_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/github_repos_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/github_users_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/gsuite_ingest_groups_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/gsuite_ingest_users_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/jamf_import_computers_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/kubernetes_import_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/oci_import_compartments_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/oci_import_groups_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/oci_import_groups_membership_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/oci_import_policies_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/oci_import_users_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/oci_tenancy_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/okta_groups_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/okta_import_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/jobs/cleanup/pagerduty_import_cleanup.json
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/data/permission_relationships.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.132811 cartography-0.81.0/cartography/driftdetect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/driftdetect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/driftdetect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/driftdetect/add_shortcut.py
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/driftdetect/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/driftdetect/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/driftdetect/detect_deviations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/driftdetect/get_states.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/driftdetect/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/driftdetect/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/driftdetect/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/driftdetect/shortcut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/driftdetect/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/driftdetect/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.132811 cartography-0.81.0/cartography/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/graph/cleanupbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/graph/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/graph/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    20108 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/graph/querybuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/graph/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.136811 cartography-0.81.0/cartography/intel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.140812 cartography-0.81.0/cartography/intel/aws/
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/dynamodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.140812 cartography-0.81.0/cartography/intel/aws/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/auto_scaling_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/elastic_ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/internet_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/key_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/launch_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/load_balancer_v2s.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/load_balancers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/network_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/reserved_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/security_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/tgw.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ec2/vpc_peerings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ecr.py
--rw-r--r--   0 runner    (1001) docker     (123)    23654 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/eks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/elasticache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/emr.py
--rw-r--r--   0 runner    (1001) docker     (123)    32347 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)    12491 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/kms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)    14792 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/permission_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/rds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/resourcegroupstaggingapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/route53.py
--rw-r--r--   0 runner    (1001) docker     (123)    26381 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/secretsmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/securityhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/ssm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.140812 cartography-0.81.0/cartography/intel/aws/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/aws/util/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.144812 cartography-0.81.0/cartography/intel/azure/
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/azure/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    41275 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/azure/cosmosdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    32865 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/azure/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    27393 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/azure/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/azure/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/azure/tenant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.144812 cartography-0.81.0/cartography/intel/azure/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/azure/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/azure/util/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.144812 cartography-0.81.0/cartography/intel/bigfix/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/bigfix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/bigfix/computers.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/create_indexes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.144812 cartography-0.81.0/cartography/intel/crowdstrike/
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/crowdstrike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/crowdstrike/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/crowdstrike/spotlight.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/crowdstrike/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.144812 cartography-0.81.0/cartography/intel/crxcavator/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/crxcavator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13797 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/crxcavator/crxcavator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.144812 cartography-0.81.0/cartography/intel/cve/
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/cve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/cve/feed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.144812 cartography-0.81.0/cartography/intel/digitalocean/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/digitalocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/digitalocean/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/digitalocean/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/digitalocean/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/dns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.148812 cartography-0.81.0/cartography/intel/duo/
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/duo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/duo/api_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/duo/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/duo/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/duo/phones.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/duo/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/duo/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/duo/web_authn_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.148812 cartography-0.81.0/cartography/intel/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48333 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/gcp/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/gcp/crm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/gcp/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/gcp/gke.py
--rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/gcp/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.148812 cartography-0.81.0/cartography/intel/github/
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21768 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/github/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/github/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/github/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/github/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.148812 cartography-0.81.0/cartography/intel/gsuite/
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/gsuite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/gsuite/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.148812 cartography-0.81.0/cartography/intel/jamf/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/jamf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/jamf/computers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/jamf/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.152812 cartography-0.81.0/cartography/intel/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/kubernetes/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/kubernetes/pods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/kubernetes/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/kubernetes/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/kubernetes/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.152812 cartography-0.81.0/cartography/intel/lastpass/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/lastpass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/lastpass/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.152812 cartography-0.81.0/cartography/intel/oci/
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/oci/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/oci/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.152812 cartography-0.81.0/cartography/intel/okta/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/okta/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/okta/awssaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/okta/factors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/okta/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/okta/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/okta/origins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/okta/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/okta/sync_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/okta/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/okta/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.156813 cartography-0.81.0/cartography/intel/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/pagerduty/escalation_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/pagerduty/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/pagerduty/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/pagerduty/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/pagerduty/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/intel/pagerduty/vendors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.156813 cartography-0.81.0/cartography/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.156813 cartography-0.81.0/cartography/models/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.156813 cartography-0.81.0/cartography/models/aws/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/aws/dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/aws/dynamodb/gsi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/aws/dynamodb/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.156813 cartography-0.81.0/cartography/models/aws/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/aws/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/aws/ec2/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/aws/ec2/instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/aws/ec2/keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/aws/ec2/networkinterfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/aws/ec2/reservations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/aws/ec2/securitygroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/aws/ec2/subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/aws/ec2/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/aws/emr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.156813 cartography-0.81.0/cartography/models/bigfix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/bigfix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/bigfix/bigfix_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/bigfix/bigfix_root.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.156813 cartography-0.81.0/cartography/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/core/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/core/relationships.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.160813 cartography-0.81.0/cartography/models/duo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/duo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/duo/api_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/duo/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/duo/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/duo/phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/duo/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/duo/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/duo/web_authn_credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.160813 cartography-0.81.0/cartography/models/github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/github/teams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.160813 cartography-0.81.0/cartography/models/lastpass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/lastpass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/lastpass/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/models/lastpass/user.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-06-23 16:41:29.000000 cartography-0.81.0/cartography/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:41:39.112810 cartography-0.81.0/cartography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-23 16:41:39.000000 cartography-0.81.0/cartography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-06-23 16:41:39.000000 cartography-0.81.0/cartography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:41:39.000000 cartography-0.81.0/cartography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-23 16:41:39.000000 cartography-0.81.0/cartography.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-23 16:41:39.000000 cartography-0.81.0/cartography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 16:41:39.000000 cartography-0.81.0/cartography.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-23 16:41:39.160813 cartography-0.81.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-23 16:41:29.000000 cartography-0.81.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      790 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4155 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      266 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography.egg-info/entry_points.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      800 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/intel/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      622 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/intel/create_indexes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3710 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/dns.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/intel/gcp/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36591 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/intel/gcp/compute.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10522 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/gcp/crm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6271 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/gcp/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/intel/aws/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40016 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/intel/aws/ec2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18590 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/intel/aws/iam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11252 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/aws/s3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4305 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/intel/aws/organizations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11158 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/aws/rds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5709 2019-08-19 22:00:00.000000 cartography-0.9.0/cartography/intel/aws/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8037 2019-08-19 22:00:00.000000 cartography-0.9.0/cartography/intel/aws/elasticsearch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3874 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/aws/dynamodb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8699 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/aws/route53.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/intel/crxcavator/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9294 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/intel/crxcavator/crxcavator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1671 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/crxcavator/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1417 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/intel/analysis.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/data/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/data/jobs/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/data/jobs/analysis/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2498 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/analysis/aws_s3acl_analysis.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3659 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/analysis/gcp_compute_asset_inet_exposure.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2057 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/analysis/aws_ec2_asset_exposure.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/data/jobs/analysis/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/data/jobs/cleanup/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      553 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_roles_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      263 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_post_ingestion_principals_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      531 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_post_ingestion_dns_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      344 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_roles_policy_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      775 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_ec2_key_pairs_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      715 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/crxcavator_import_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      329 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_groups_membership_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1551 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_vpc_peering_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      348 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_s3_details.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2120 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_firewall_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      342 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_account_access_key_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3098 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_instance_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1478 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_ingest_ec2_auto_scaling_groups_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1592 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_ec2_security_groupinfo_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_ec2_instances_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      587 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_es_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1039 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_vpc_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      685 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/gcp_crm_organization_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2992 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_rds_instances_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      620 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_dns_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      680 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_account_dns_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      272 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_account_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      957 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_dynamodb_tables_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      296 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_s3_buckets_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      294 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_users_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      304 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_principals_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      537 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_groups_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      543 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_policies_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      346 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_groups_policy_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/data/jobs/cleanup/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1988 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_ingest_load_balancers_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1790 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_vpc_subnet_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1059 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/gcp_crm_project_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      551 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_s3_acl_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1058 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/gcp_crm_folder_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1096 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_vpc_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/data/jobs/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2190 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/indexes.cypher
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8239 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      101 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/__main__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/graph/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/graph/job.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1230 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/graph/context.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2923 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/graph/statement.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/graph/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1667 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/config.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/driftdetect/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      929 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/driftdetect/util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1554 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/driftdetect/storage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1411 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/driftdetect/reporter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2377 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/driftdetect/add_shortcut.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1028 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/driftdetect/serializers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9175 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/driftdetect/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      125 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/driftdetect/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5400 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/driftdetect/get_states.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2840 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/driftdetect/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/driftdetect/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      371 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/driftdetect/shortcut.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      807 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/driftdetect/model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3994 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/driftdetect/detect_deviations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5796 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/sync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      790 2019-08-19 22:00:36.000000 cartography-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18556 2019-08-19 21:58:38.000000 cartography-0.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2019-08-19 22:00:36.000000 cartography-0.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1876 2019-08-19 21:59:57.000000 cartography-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `cartography-0.81.0/PKG-INFO` & `cartography-0.9.0/cartography.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: cartography
-Version: 0.81.0
+Version: 0.9.0
 Summary: Explore assets and their relationships across your technical infrastructure.
 Home-page: https://www.github.com/lyft/cartography
 Maintainer: Lyft
 Maintainer-email: security@lyft.com
 License: apache2
+Description: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE
-
-file: README.md
```

### Comparing `cartography-0.81.0/cartography/data/jobs/analysis/aws_ec2_asset_exposure.json` & `cartography-0.9.0/cartography/data/jobs/analysis/aws_ec2_asset_exposure.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8958333333333334%*

 * *Differences: {"'statements'": '{0: {\'query\': "MATCH (n) where EXISTS(n.exposed_internet) AND labels(n) IN '*

 * *                 "['AutoScalingGroup', 'EC2Instance', 'LoadBalancer'] WITH n LIMIT {LIMIT_SIZE} "*

 * *                 'REMOVE n.exposed_internet, n.exposed_internet_type return COUNT(*) as '*

 * *                 'TotalCompleted"}, 1: {\'query\': "MATCH (:IpRange{id: '*

 * *                 "'0.0.0.0/0'})-[:MEMBER_OF_IP_RULE]->(:IpPermissionInbound)-[:MEMBER_OF_EC2_SECURITY_GROUP]->(group:EC2SecurityGroup)<-[:MEMBER_OF_EC2_S […]*

```diff
@@ -1,34 +1,26 @@
 {
     "name": "AWS asset internet exposure",
     "statements": [
         {
             "iterationsize": 1000,
             "iterative": true,
-            "query": "MATCH (n) where n.exposed_internet IS NOT NULL AND labels(n) IN ['AutoScalingGroup', 'EC2Instance', 'LoadBalancer', 'LoadBalancerV2'] WITH n LIMIT $LIMIT_SIZE REMOVE n.exposed_internet, n.exposed_internet_type return COUNT(*) as TotalCompleted"
+            "query": "MATCH (n) where EXISTS(n.exposed_internet) AND labels(n) IN ['AutoScalingGroup', 'EC2Instance', 'LoadBalancer'] WITH n LIMIT {LIMIT_SIZE} REMOVE n.exposed_internet, n.exposed_internet_type return COUNT(*) as TotalCompleted"
         },
         {
             "iterative": false,
-            "query": "MATCH (:IpRange{id: '0.0.0.0/0'})-[:MEMBER_OF_IP_RULE]->(:IpPermissionInbound)-[:MEMBER_OF_EC2_SECURITY_GROUP]->(group:EC2SecurityGroup)<-[:MEMBER_OF_EC2_SECURITY_GROUP|NETWORK_INTERFACE*..2]-(instance:EC2Instance)\nWITH instance\nWHERE (instance.publicipaddress IS NOT NULL) AND (instance.exposed_internet_type IS NULL) OR (NOT 'direct' IN instance.exposed_internet_type)\nSET instance.exposed_internet = true, instance.exposed_internet_type = coalesce(instance.exposed_internet_type , []) + 'direct';"
-        },
-        {
-            "iterative": false,
-            "query": "MATCH (cidr:IpRange{range:'0.0.0.0/0'})\u2014->(perm:IpPermissionInbound)\u2014->(sg:EC2SecurityGroup)<-[:MEMBER_OF_EC2_SECURITY_GROUP]-(elbv2:LoadBalancerV2{scheme: 'internet-facing'})\u2014->(listener:ELBV2Listener)\nWHERE listener.port>=perm.fromport AND listener.port<=perm.toport\nSET elbv2.exposed_internet = true"
+            "query": "MATCH (:IpRange{id: '0.0.0.0/0'})-[:MEMBER_OF_IP_RULE]->(:IpPermissionInbound)-[:MEMBER_OF_EC2_SECURITY_GROUP]->(group:EC2SecurityGroup)<-[:MEMBER_OF_EC2_SECURITY_GROUP|NETWORK_INTERFACE*..2]-(instance:EC2Instance)\nWITH instance\nWHERE (EXISTS(instance.publicdnsname) AND instance.publicdnsname <> '') AND (NOT EXISTS(instance.exposed_internet_type)) OR (NOT 'direct' IN instance.exposed_internet_type)\nSET instance.exposed_internet = true, instance.exposed_internet_type = coalesce(instance.exposed_internet_type , []) + 'direct';"
         },
         {
             "iterative": false,
             "query": "MATCH (cidr:IpRange{range:'0.0.0.0/0'})\u2014->(perm:IpPermissionInbound)\u2014->(sg:EC2SecurityGroup)<-[:SOURCE_SECURITY_GROUP]-(elb:LoadBalancer{scheme: 'internet-facing'})\u2014->(listener:ELBListener)\nWHERE listener.port>=perm.fromport AND listener.port<=perm.toport\nSET elb.exposed_internet = true"
         },
         {
             "iterative": false,
-            "query": "MATCH (elb:LoadBalancer{exposed_internet: true})-[:EXPOSE]->(e:EC2Instance)\nWITH e\nWHERE (e.exposed_internet_type IS NULL) OR (NOT 'elb' IN e.exposed_internet_type)\nSET e.exposed_internet = true, e.exposed_internet_type = coalesce(e.exposed_internet_type, []) + 'elb'"
-        },
-        {
-            "iterative": false,
-            "query": "MATCH (elbv2:LoadBalancerV2{exposed_internet: true})-[:EXPOSE]->(e:EC2Instance)\nWITH e\nWHERE (e.exposed_internet_type IS NULL) OR (NOT 'elbv2' IN e.exposed_internet_type)\nSET e.exposed_internet = true, e.exposed_internet_type = coalesce(e.exposed_internet_type, []) + 'elbv2'"
+            "query": "MATCH (elb:LoadBalancer{exposed_internet: true})-[:EXPOSE]->(e:EC2Instance)\nWITH e\nWHERE (NOT EXISTS(e.exposed_internet_type)) OR (NOT 'elb' IN e.exposed_internet_type)\nSET e.exposed_internet = true, e.exposed_internet_type = coalesce(e.exposed_internet_type, []) + 'elb'"
         },
         {
             "iterative": false,
-            "query": "MATCH (instance:EC2Instance{exposed_internet: true})-[:MEMBER_AUTO_SCALE_GROUP]->(asg:AutoScalingGroup)\nWITH distinct instance.exposed_internet_type as types, asg\nUNWIND types as type\nWITH type, asg\nWHERE asg.exposed_internet_type IS NULL OR (NOT type IN asg.exposed_internet_type)\nSET asg.exposed_internet = true, asg.exposed_internet_type = coalesce(asg.exposed_internet_type, []) + type;"
+            "query": "MATCH (instance:EC2Instance{exposed_internet: true})-[:MEMBER_AUTO_SCALE_GROUP]->(asg:AutoScalingGroup)\nWITH distinct instance.exposed_internet_type as types, asg\nUNWIND types as type\nWITH type, asg\nWHERE NOT EXISTS(asg.exposed_internet_type) OR (NOT type IN asg.exposed_internet_type)\nSET asg.exposed_internet = true, asg.exposed_internet_type = coalesce(asg.exposed_internet_type, []) + type;"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/analysis/aws_s3acl_analysis.json` & `cartography-0.9.0/cartography/data/jobs/analysis/aws_s3acl_analysis.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'statements'": '{0: {\'query\': "MATCH '*

 * *                 '(acl:S3Acl)-[:APPLIES_TO]->(bucket:S3Bucket)<-[:RESOURCE]-(aws:AWSAccount{id: '*

 * *                 '{AWS_ID}})\\nWHERE acl.uri IN '*

 * *                 "['http://acs.amazonaws.com/groups/global/AllUsers', "*

 * *                 "'http://acs.amazonaws.com/groups/global/AuthenticatedUsers'] AND acl.permission "*

 * *                 "= 'READ'\\nSET bucket.anonymous_access = true, bucket.anonymous_actions = "*

 * *                 "coalesce(bucket.anonymous_actions, [] […]*

```diff
@@ -1,25 +1,25 @@
 {
     "name": "AWS S3 Acl exposure analysis",
     "statements": [
         {
             "iterative": false,
-            "query": "MATCH (acl:S3Acl)-[:APPLIES_TO]->(bucket:S3Bucket)<-[:RESOURCE]-(aws:AWSAccount{id: $AWS_ID})\nWHERE acl.uri IN ['http://acs.amazonaws.com/groups/global/AllUsers', 'http://acs.amazonaws.com/groups/global/AuthenticatedUsers'] AND acl.permission = 'READ'\nSET bucket.anonymous_access = true, bucket.anonymous_actions = coalesce(bucket.anonymous_actions, []) + ['s3:ListBucket', 's3:ListBucketVersions', 's3:ListBucketMultipartUploads']"
+            "query": "MATCH (acl:S3Acl)-[:APPLIES_TO]->(bucket:S3Bucket)<-[:RESOURCE]-(aws:AWSAccount{id: {AWS_ID}})\nWHERE acl.uri IN ['http://acs.amazonaws.com/groups/global/AllUsers', 'http://acs.amazonaws.com/groups/global/AuthenticatedUsers'] AND acl.permission = 'READ'\nSET bucket.anonymous_access = true, bucket.anonymous_actions = coalesce(bucket.anonymous_actions, []) + ['s3:ListBucket', 's3:ListBucketVersions', 's3:ListBucketMultipartUploads']"
         },
         {
             "iterative": false,
-            "query": "MATCH (acl:S3Acl)-[:APPLIES_TO]->(bucket:S3Bucket)<-[:RESOURCE]-(aws:AWSAccount{id: $AWS_ID})\nWHERE acl.uri IN ['http://acs.amazonaws.com/groups/global/AllUsers', 'http://acs.amazonaws.com/groups/global/AuthenticatedUsers'] AND acl.permission = 'WRITE'\nAND (acl.ownerid = acl.granteeid)\nSET bucket.anonymous_access = true, bucket.anonymous_actions = coalesce(bucket.anonymous_actions, []) + ['s3:DeleteObjectVersion']"
+            "query": "MATCH (acl:S3Acl)-[:APPLIES_TO]->(bucket:S3Bucket)<-[:RESOURCE]-(aws:AWSAccount{id: {AWS_ID}})\nWHERE acl.uri IN ['http://acs.amazonaws.com/groups/global/AllUsers', 'http://acs.amazonaws.com/groups/global/AuthenticatedUsers'] AND acl.permission = 'WRITE'\nAND (acl.ownerid = acl.granteeid)\nSET bucket.anonymous_access = true, bucket.anonymous_actions = coalesce(bucket.anonymous_actions, []) + ['s3:DeleteObjectVersion']"
         },
         {
             "iterative": false,
-            "query": "MATCH (acl:S3Acl)-[:APPLIES_TO]->(bucket:S3Bucket)<-[:RESOURCE]-(aws:AWSAccount{id: $AWS_ID})\nWHERE acl.uri IN ['http://acs.amazonaws.com/groups/global/AllUsers', 'http://acs.amazonaws.com/groups/global/AuthenticatedUsers'] AND acl.permission = 'READ_ACP'\nSET bucket.anonymous_access = true, bucket.anonymous_actions = coalesce(bucket.anonymous_actions, []) + ['s3:DeleteObjectVersion']"
+            "query": "MATCH (acl:S3Acl)-[:APPLIES_TO]->(bucket:S3Bucket)<-[:RESOURCE]-(aws:AWSAccount{id: {AWS_ID}})\nWHERE acl.uri IN ['http://acs.amazonaws.com/groups/global/AllUsers', 'http://acs.amazonaws.com/groups/global/AuthenticatedUsers'] AND acl.permission = 'READ_ACP'\nSET bucket.anonymous_access = true, bucket.anonymous_actions = coalesce(bucket.anonymous_actions, []) + ['s3:DeleteObjectVersion']"
         },
         {
             "iterative": false,
-            "query": "MATCH (acl:S3Acl)-[:APPLIES_TO]->(bucket:S3Bucket)<-[:RESOURCE]-(aws:AWSAccount{id: $AWS_ID})\nWHERE acl.uri IN ['http://acs.amazonaws.com/groups/global/AllUsers', 'http://acs.amazonaws.com/groups/global/AuthenticatedUsers'] AND acl.permission = 'WRITE_ACP'\nSET bucket.anonymous_access = true, bucket.anonymous_actions = coalesce(bucket.anonymous_actions, []) + ['s3:PutBucketAcl']"
+            "query": "MATCH (acl:S3Acl)-[:APPLIES_TO]->(bucket:S3Bucket)<-[:RESOURCE]-(aws:AWSAccount{id: {AWS_ID}})\nWHERE acl.uri IN ['http://acs.amazonaws.com/groups/global/AllUsers', 'http://acs.amazonaws.com/groups/global/AuthenticatedUsers'] AND acl.permission = 'WRITE_ACP'\nSET bucket.anonymous_access = true, bucket.anonymous_actions = coalesce(bucket.anonymous_actions, []) + ['s3:PutBucketAcl']"
         },
         {
             "iterative": false,
-            "query": "MATCH (acl:S3Acl)-[:APPLIES_TO]->(bucket:S3Bucket)<-[:RESOURCE]-(aws:AWSAccount{id: $AWS_ID})\nWHERE acl.uri IN ['http://acs.amazonaws.com/groups/global/AllUsers', 'http://acs.amazonaws.com/groups/global/AuthenticatedUsers'] AND acl.permission = 'FULL_CONTROL'\nSET bucket.anonymous_access = true, bucket.anonymous_actions = coalesce(bucket.anonymous_actions, []) + ['s3:ListBucket', 's3:ListBucketVersions', 's3:ListBucketMultipartUploads', 's3:PutObject', 's3:DeleteObject', 's3:DeleteObjectVersion', 's3:PutBucketAcl']"
+            "query": "MATCH (acl:S3Acl)-[:APPLIES_TO]->(bucket:S3Bucket)<-[:RESOURCE]-(aws:AWSAccount{id: {AWS_ID}})\nWHERE acl.uri IN ['http://acs.amazonaws.com/groups/global/AllUsers', 'http://acs.amazonaws.com/groups/global/AuthenticatedUsers'] AND acl.permission = 'FULL_CONTROL'\nSET bucket.anonymous_access = true, bucket.anonymous_actions = coalesce(bucket.anonymous_actions, []) + ['s3:ListBucket', 's3:ListBucketVersions', 's3:ListBucketMultipartUploads', 's3:PutObject', 's3:DeleteObject', 's3:DeleteObjectVersion', 's3:PutBucketAcl']"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/analysis/gsuite_human_link.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_s3_acl_cleanup.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6458333333333334%*

 * *Differences: {"'name'": "'cleanup S3Acl'",*

 * * "'statements'": "{0: {'query': 'MATCH (:AWSAccount{id: "*

 * *                 '{AWS_ID}})-[:RESOURCE]->(:S3Bucket)<-[:APPLIES_TO]-(n:S3Acl) WHERE n.lastupdated '*

 * *                 '<> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as '*

 * *                 "TotalCompleted', 'iterative': True, 'iterationsize': 100}, 1: {'query': 'MATCH "*

 * *                 '(a:S3Acl) WHERE NOT (a)-[:APPLIES_TO]->(:S3Bucket) WITH a LIMIT {LIMIT_SIZE} '*

 * *                 "DETACH DEL […]*

```diff
@@ -1,14 +1,15 @@
 {
-    "name": "GSuite user map to Human",
+    "name": "cleanup S3Acl",
     "statements": [
         {
-            "iterative": false,
-            "query": "MATCH (human:Human), (guser:GSuiteUser) WHERE human.email = guser.email MERGE (human)-[r:IDENTITY_GSUITE]->(guser) ON CREATE SET r.firstseen = $UPDATE_TAG SET r.lastupdated = $UPDATE_TAG"
+            "iterationsize": 100,
+            "iterative": true,
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(:S3Bucket)<-[:APPLIES_TO]-(n:S3Acl) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:Human)-[r:IDENTITY_GSUITE]->(:GSuiteUser) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r) return COUNT(*) as TotalCompleted"
+            "query": "MATCH (a:S3Acl) WHERE NOT (a)-[:APPLIES_TO]->(:S3Bucket) WITH a LIMIT {LIMIT_SIZE} DETACH DELETE (a) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_account_access_key_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/gcp_crm_organization_cleanup.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6875%*

 * *Differences: {"'name'": "'cleanup GCP Organizations'",*

 * * "'statements'": "{0: {'query': 'MATCH (n:GCPOrganization) WHERE n.lastupdated <> {UPDATE_TAG} "*

 * *                 "WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted', "*

 * *                 "'__comment__': 'Remove GCP organizations that are out of date.'}, 1: {'query': "*

 * *                 "'MATCH (:GCPOrganization)-[r:RESOURCE]->(:GCPProject) WHERE r.lastupdated <> "*

 * *                 '{UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return CO […]*

```diff
@@ -1,17 +1,17 @@
 {
-    "name": "cleanup AccountAccessKey",
+    "name": "cleanup GCP Organizations",
     "statements": [
         {
-            "__comment__": "cleanup access keys that are attached to users",
+            "__comment__": "Remove GCP organizations that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:AccountAccessKey)<-[:AWS_ACCESS_KEY]-(:AWSUser)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:GCPOrganization) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
-            "__comment__": "cleanup access keys that no longer attached to users, such as when a user no longer exists",
+            "__comment__": "Remove GCP Organization relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:AccountAccessKey) WHERE NOT (n)<-[:AWS_ACCESS_KEY]-(:AWSUser) AND n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:GCPOrganization)-[r:RESOURCE]->(:GCPProject) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_apigateway_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_ec2_security_groupinfo_cleanup.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6302083333333334%*

 * *Differences: {"'name'": "'cleanup EC2SecurityGroup|IpRule|IpRange'",*

 * * "'statements'": "{0: {'query': 'MATCH (n:EC2SecurityGroup)<-[:RESOURCE]-(:AWSAccount{id: "*

 * *                 '{AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH '*

 * *                 "DELETE (n) return COUNT(*) as TotalCompleted'}, 1: {'query': 'MATCH "*

 * *                 '(n:IpRule)-[:MEMBER_OF_EC2_SECURITY_GROUP]->(:EC2SecurityGroup)<-[:RESOURCE]-(:AWSAccount{id: '*

 * *                 '{AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TA […]*

```diff
@@ -1,45 +1,30 @@
 {
-    "name": "cleanup APIGateway",
+    "name": "cleanup EC2SecurityGroup|IpRule|IpRange",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:APIGatewayClientCertificate)<-[:HAS_CERTIFICATE]-(:APIGatewayStage)<-[:ASSOCIATED_WITH]-(:APIGatewayRestAPI)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:EC2SecurityGroup)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:APIGatewayClientCertificate)<-[r:HAS_CERTIFICATE]-(:APIGatewayStage)<-[:ASSOCIATED_WITH]-(:APIGatewayRestAPI)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (n:IpRule)-[:MEMBER_OF_EC2_SECURITY_GROUP]->(:EC2SecurityGroup)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:APIGatewayStage)<-[:ASSOCIATED_WITH]-(:APIGatewayRestAPI)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:IpRange)-[:MEMBER_OF_IP_RULE]->(:IpRule)-[:MEMBER_OF_EC2_SECURITY_GROUP]->(:EC2SecurityGroup)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:APIGatewayStage)<-[r:ASSOCIATED_WITH]-(:APIGatewayRestAPI)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:IpRule)-[r:MEMBER_OF_EC2_SECURITY_GROUP]->(:EC2SecurityGroup)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:APIGatewayResource)<-[:RESOURCE]-(:APIGatewayRestAPI)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (:APIGatewayResource)<-[r:RESOURCE]-(:APIGatewayRestAPI)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (n:APIGatewayRestAPI)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (:APIGatewayRestAPI)<-[r:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:IpRange)-[r:MEMBER_OF_IP_RULE]->(:IpRule)-[:MEMBER_OF_EC2_SECURITY_GROUP]->(:EC2SecurityGroup)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_config_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_roles_cleanup.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6388888888888888%*

 * *Differences: {"'name'": "'cleanup AWSRole'",*

 * * "'statements'": "{0: {'query': 'MATCH (:AWSAccount{id: {AWS_ID}})-[:AWS_ROLE]->(n:AWSRole) WHERE "*

 * *                 'n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return '*

 * *                 "COUNT(*) as TotalCompleted'}, 1: {'query': 'MATCH (:AWSAccount{id: "*

 * *                 '{AWS_ID}})-[:AWS_ROLE]->(:AWSRole)-[r]->(:AWSPrincipal) WHERE r.lastupdated <> '*

 * *                 '{UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as '*

 * *     […]*

```diff
@@ -1,20 +1,15 @@
 {
-    "name": "cleanup AWS Config",
+    "name": "cleanup AWSRole",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(n:AWSConfigurationRecorder) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:AWS_ROLE]->(n:AWSRole) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(n:AWSConfigDeliveryChannel) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(n:AWSConfigRule) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:AWS_ROLE]->(:AWSRole)-[r]->(:AWSPrincipal) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_ec2_launch_templates_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_dns_cleanup.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7083333333333334%*

 * *Differences: {"'name'": "'cleanup AWS DNS'",*

 * * "'statements'": "{0: {'query': 'MATCH (n:AWSDNSZone)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) "*

 * *                 'WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) '*

 * *                 "return COUNT(*) as TotalCompleted'}, 1: {'query': 'MATCH "*

 * *                 '()<-[r:DNS_POINTS_TO]-(:AWSDNSRecord)-[:MEMBER_OF_DNS_ZONE]->(:AWSDNSZone)<-[:RESOURCE]-(:AWSAccount{id: '*

 * *                 '{AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LI […]*

```diff
@@ -1,15 +1,15 @@
 {
-    "name": "cleanup LaunchTemplate",
+    "name": "cleanup AWS DNS",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:LaunchTemplateVersion)<-[:VERSION]-(:LaunchTemplate)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:AWSDNSZone)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:LaunchTemplate)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH ()<-[r:DNS_POINTS_TO]-(:AWSDNSRecord)-[:MEMBER_OF_DNS_ZONE]->(:AWSDNSZone)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_ec2_security_groupinfo_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_vpc_cleanup.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7083333333333334%*

 * *Differences: {"'name'": "'cleanup AWS VPC information'",*

 * * "'statements'": "{0: {'query': 'MATCH "*

 * *                 '(n:CidrBlock)<-[:BLOCK_ASSOCIATION]-(:AWSVpc)<-[:RESOURCE]-(:AWSAccount{id: '*

 * *                 '{AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH '*

 * *                 "DELETE (n) return COUNT(*) as TotalCompleted'}, 1: {'query': 'MATCH "*

 * *                 '(:CidrBlock)<-[r:BLOCK_ASSOCIATION]-(:AWSVpc)<-[:RESOURCE]-(:AWSAccount{id: '*

 * *                 '{AWS_ID}}) WHERE r.lastupdate […]*

```diff
@@ -1,25 +1,25 @@
 {
-    "name": "cleanup EC2SecurityGroup|IpRule|IpRange",
+    "name": "cleanup AWS VPC information",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:IpRule)-[:MEMBER_OF_EC2_SECURITY_GROUP]->(:EC2SecurityGroup)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:CidrBlock)<-[:BLOCK_ASSOCIATION]-(:AWSVpc)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:IpRange)-[:MEMBER_OF_IP_RULE]->(:IpRule)-[:MEMBER_OF_EC2_SECURITY_GROUP]->(:EC2SecurityGroup)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:CidrBlock)<-[r:BLOCK_ASSOCIATION]-(:AWSVpc)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:IpRule)-[r:MEMBER_OF_EC2_SECURITY_GROUP]->(:EC2SecurityGroup)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (n:AWSVpc)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:IpRange)-[r:MEMBER_OF_IP_RULE]->(:IpRule)-[:MEMBER_OF_EC2_SECURITY_GROUP]->(:EC2SecurityGroup)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:AWSVpc)<-[r:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_ecr_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_ec2_key_pairs_cleanup.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.625%*

 * *Differences: {"'name'": "'cleanup EC2KeyPair'",*

 * * "'statements'": "{0: {'query': 'MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(n:EC2KeyPair) "*

 * *                 'WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) '*

 * *                 "return COUNT(*) as TotalCompleted'}, 1: {'query': 'MATCH "*

 * *                 '(:EC2Instance)<-[r:SSH_LOGIN_TO]-(:EC2KeyPair) WHERE r.lastupdated <> '*

 * *                 '{UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as '*

 * *                 "TotalC […]*

```diff
@@ -1,30 +1,20 @@
 {
-    "name": "cleanup ECRImage|IMAGE|ECRRepositoryImage|REPO_IMAGE|ECRRepository",
+    "name": "cleanup EC2KeyPair",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:ECRRepository)-[:REPO_IMAGE]->(:ECRRepositoryImage)-[:IMAGE]->(n:ECRImage) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(n:EC2KeyPair) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:ECRRepository)-[:REPO_IMAGE]->(:ECRRepositoryImage)-[r:IMAGE]->(:ECRImage) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:EC2Instance)<-[r:SSH_LOGIN_TO]-(:EC2KeyPair) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:ECRRepository)-[:REPO_IMAGE]->(n:ECRRepositoryImage) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:ECRRepository)-[r:REPO_IMAGE]->(:ECRRepositoryImage) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(n:ECRRepository) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[r:RESOURCE]->(:EC2KeyPair) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_ecs_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_vpc_peering_cleanup.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.65625%*

 * *Differences: {"'name'": "'cleanup AWS VPC information'",*

 * * "'statements'": "{0: {'query': 'MATCH "*

 * *                 '(n:AWSCidrBlock)<-[:BLOCK_ASSOCIATION]-(:AWSVpc)<-[:RESOURCE]-(:AWSAccount{foreign: '*

 * *                 'true}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH '*

 * *                 "DELETE (n) return COUNT(*) as TotalCompleted'}, 1: {'query': 'MATCH "*

 * *                 '(:AWSCidrBlock)<-[r:BLOCK_ASSOCIATION]-(:AWSVpc)<-[:RESOURCE]-(:AWSAccount{foreign: '*

 * *                 'true}) WHERE r.la […]*

```diff
@@ -1,45 +1,35 @@
 {
-    "name": "cleanup ECS",
+    "name": "cleanup AWS VPC information",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:ECSCluster)-[:HAS_CONTAINER_INSTANCE]->(:ECSContainerInstance)-[r:HAS_TASK]->(:ECSTask) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (n:AWSCidrBlock)<-[:BLOCK_ASSOCIATION]-(:AWSVpc)<-[:RESOURCE]-(:AWSAccount{foreign: true}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:ECSCluster)-[:HAS_CONTAINER_INSTANCE]->(n:ECSContainerInstance) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSCidrBlock)<-[r:BLOCK_ASSOCIATION]-(:AWSVpc)<-[:RESOURCE]-(:AWSAccount{foreign: true}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:ECSCluster)-[:HAS_SERVICE]->(n:ECSService) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:AWSVpc)<-[:RESOURCE]-(:AWSAccount{foreign: true}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:ECSCluster)-[:HAS_TASK]->(:ECSTask)-[:HAS_CONTAINER]->(n:ECSContainer) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSVpc)<-[r:RESOURCE]-(:AWSAccount{foreign: true}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:ECSCluster)-[:HAS_TASK]->(n:ECSTask) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSVpc)-[r:VPC_PEERING]-(:AWSVpc) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:ECSTaskDefinition)-[:HAS_CONTAINER_DEFINITION]->(n:ECSContainerDefinition) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(n:ECSTaskDefinition) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(n:ECSCluster) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:AWSAccount{foreign: true}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_elastic_ip_addresses_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/crxcavator_import_cleanup.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.65625%*

 * *Differences: {"'name'": "'cleanup CRXcavator extensions'",*

 * * "'statements'": "{0: {'query': 'MATCH (n:ChromeExtension) WHERE n.lastupdated <> {UPDATE_TAG} "*

 * *                 "WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted'}, "*

 * *                 "1: {'query': 'MATCH (n:GSuiteUser) WHERE n.lastupdated <> {UPDATE_TAG} WITH n "*

 * *                 "LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted'}, 2: "*

 * *                 "{'query': 'MATCH (GSuiteUser)-[r:INSTALLS]->(:ChromeExt […]*

```diff
@@ -1,25 +1,20 @@
 {
-    "name": "cleanup EC2 Elastic IP Addresses",
+    "name": "cleanup CRXcavator extensions",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:ElasticIpAddress)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:ChromeExtension) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:ElasticIpAddress)<-[r:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (n:GSuiteUser) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:ElasticIpAddress)<-[r:ELASTIC_IP_ADDRESS]-(:EC2Instance)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (:ElasticIpAddress)<-[r:ELASTIC_IP_ADDRESS]-(:NetworkInterface)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (GSuiteUser)-[r:INSTALLS]->(:ChromeExtension) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_es_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_groups_cleanup.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6822916666666667%*

 * *Differences: {"'name'": "'cleanup AWSGroup'",*

 * * "'statements'": "{0: {'query': 'MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(n:AWSGroup) WHERE "*

 * *                 'n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return '*

 * *                 "COUNT(*) as TotalCompleted'}, 1: {'query': 'MATCH (:AWSAccount{id: "*

 * *                 '{AWS_ID}})-[r:AWS_GROUP]->(:AWSGroup) WHERE r.lastupdated <> {UPDATE_TAG} WITH r '*

 * *                 "LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted', delet […]*

```diff
@@ -1,16 +1,15 @@
 {
-    "name": "cleanup ESDomain|DNSRecord",
+    "name": "cleanup AWSGroup",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(n:ESDomain) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(n:AWSGroup) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
-            "__comment__": "Clean up DNSRecords pointing to ESDomains within the current AWS account",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:ESDomain)<-[:DNS_POINTS_TO]-(n:DNSRecord) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[r:AWS_GROUP]->(:AWSGroup) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_rds_clusters_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_rds_instances_cleanup.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5803571428571428%*

 * *Differences: {"'name'": "'cleanup RDSInstance'",*

 * * "'statements'": "{4: {'query': 'MATCH (:RDSInstance)<-[r:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) "*

 * *                 'WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return '*

 * *                 "COUNT(*) as TotalCompleted', '__comment__': 'If an RDS instance still exists but "*

 * *                 'is no longer associated with its old AWS Account, delete the relationship '*

 * *                 "between them.'}, 5: {'query': 'MATCH "*

 * *                 '(:EC2Sec […]*

```diff
@@ -1,23 +1,47 @@
 {
-    "name": "cleanup RDSCluster",
+    "name": "cleanup RDSInstance",
     "statements": [
         {
-            "__comment__": "Delete RDS clusters that no longer exist and DETACH them from all nodes they were previously connected to.",
+            "__comment__": "Delete DBSubnetGroups that no longer exist and DETACH them from their RDS instances.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:RDSCluster)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (sng:DBSubnetGroup)<-[:MEMBER_OF_DB_SUBNET_GROUP]-(:RDSInstance)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE sng.lastupdated <> {UPDATE_TAG} WITH sng LIMIT {LIMIT_SIZE} DETACH DELETE (sng) return COUNT(*) as TotalCompleted"
         },
         {
-            "__comment__": "If an RDS cluster still exists but is no longer associated with its old AWS Account, delete the relationship between them.",
+            "__comment__": "Delete the link between orphaned DB Subnet Groups and their RDS Instances.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:RDSCluster)<-[r:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:DBSubnetGroup)<-[r:MEMBER_OF_DB_SUBNET_GROUP]-(:RDSInstance)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
-            "__comment__": "If an RDS instance still exists and is no longer a member of an RDS cluster, delete the relationship between them.",
+            "__comment__": "Delete the link between orphaned DB Subnet Groups and their EC2 Subnets.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:RDSCluster)<-[r:IS_CLUSTER_MEMBER_OF]-(:RDSInstance)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:EC2Subnet)<-[r:RESOURCE]-(:DBSubnetGroup)<-[:MEMBER_OF_DB_SUBNET_GROUP]-(:RDSInstance)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
+        },
+        {
+            "__comment__": "Delete RDS instances that no longer exist and DETACH them from all nodes they were previously connected to.",
+            "iterationsize": 100,
+            "iterative": true,
+            "query": "MATCH (n:RDSInstance)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
+        },
+        {
+            "__comment__": "If an RDS instance still exists but is no longer associated with its old AWS Account, delete the relationship between them.",
+            "iterationsize": 100,
+            "iterative": true,
+            "query": "MATCH (:RDSInstance)<-[r:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
+        },
+        {
+            "__comment__": "If an RDS instance still exists and is no longer a part of its old EC2SecurityGroup, delete the relationship between them.",
+            "iterationsize": 100,
+            "iterative": true,
+            "query": "MATCH (:EC2SecurityGroup)<-[r:MEMBER_OF_EC2_SECURITY_GROUP]-(:RDSInstance)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
+        },
+        {
+            "__comment__": "If an RDS instance still exists and is no longer a read replica of another RDS instance, delete the relationship between them.",
+            "iterationsize": 100,
+            "iterative": true,
+            "query": "MATCH (:RDSInstance)<-[r:IS_READ_REPLICA_OF]-(:RDSInstance)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_rds_snapshots_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_vpc_subnet_cleanup.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6125%*

 * *Differences: {"'name'": "'cleanup GCP Instances'",*

 * * "'statements'": "{2: {'query': 'MATCH (:GCPNetworkInterface)-[r:PART_OF_SUBNET]-(:GCPSubnet) "*

 * *                 'WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return '*

 * *                 "COUNT(*) as TotalCompleted', '__comment__': 'Remove GCP "*

 * *                 "NetworkInterface-to-Subnet relationships that are out of date.'}, 3: {'query': "*

 * *                 "'MATCH (n:GCPNicAccessConfig) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT "*

 * *     […]*

```diff
@@ -1,23 +1,35 @@
 {
-    "name": "cleanup RDSSnapshot",
+    "name": "cleanup GCP Instances",
     "statements": [
         {
-            "__comment__": "Delete RDS snapshots that no longer exist and DETACH them from all nodes they were previously connected to.",
+            "__comment__": "Delete GCP Subnets that no longer exist and detach them from all previously connected nodes.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:RDSSnapshot)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:GCPSubnet) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
-            "__comment__": "If an RDS snapshot still exists but is no longer associated with its old AWS Account, delete the relationship between them.",
+            "__comment__": "Remove GCP VPC-to-Subnet relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:RDSSnapshot)<-[r:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPSubnet)<-[r:RESOURCE]-(:GCPVpc) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
-            "__comment__": "If an RDS snapshot still exists and is no longer a member of an RDS instance, delete the relationship between them.",
+            "__comment__": "Remove GCP NetworkInterface-to-Subnet relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:RDSInstance)<-[r:IS_SNAPSHOT_SOURCE]-(:RDSSnapshot)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPNetworkInterface)-[r:PART_OF_SUBNET]-(:GCPSubnet) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
+        },
+        {
+            "__comment__": "Remove GCP Network Interface Access Configs that no longer exist and detach them from all previously connected nodes.",
+            "iterationsize": 100,
+            "iterative": true,
+            "query": "MATCH (n:GCPNicAccessConfig) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
+        },
+        {
+            "__comment__": "Remove GCP NetworkInterface-to-NicAccessConfig relationships that are out of date.",
+            "iterationsize": 100,
+            "iterative": true,
+            "query": "MATCH (:GCPNicAccessConfig)-[r:RESOURCE]-(:GCPNetworkInterface) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_reserved_instances_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_dynamodb_tables_cleanup.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6388888888888888%*

 * *Differences: {"'name'": "'cleanup DynamoDBTable'",*

 * * "'statements'": "{1: {'query': 'MATCH "*

 * *                 '(g:DynamoDBGlobalSecondaryIndex)<-[:GLOBAL_SECONDARY_INDEX]-(:DynamoDBTable)<-[:RESOURCE]-(:AWSAccount{id: '*

 * *                 '{AWS_ID}}) WHERE g.lastupdated <> {UPDATE_TAG} WITH g LIMIT {LIMIT_SIZE} DETACH '*

 * *                 "DELETE (g) return COUNT(*) as TotalCompleted'}, 2: {'query': 'MATCH "*

 * *                 '(:DynamoDBGlobalSecondaryIndex)<-[r:GLOBAL_SECONDARY_INDEX]-(:DynamoDBTable)<-[:RESOURCE]-(:AWSAccou […]*

```diff
@@ -1,15 +1,20 @@
 {
-    "name": "cleanup EC2 Reserved Instances",
+    "name": "cleanup DynamoDBTable",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:EC2ReservedInstance)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:DynamoDBTable)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:EC2ReservedInstance)<-[r:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (g:DynamoDBGlobalSecondaryIndex)<-[:GLOBAL_SECONDARY_INDEX]-(:DynamoDBTable)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE g.lastupdated <> {UPDATE_TAG} WITH g LIMIT {LIMIT_SIZE} DETACH DELETE (g) return COUNT(*) as TotalCompleted"
+        },
+        {
+            "iterationsize": 100,
+            "iterative": true,
+            "query": "MATCH (:DynamoDBGlobalSecondaryIndex)<-[r:GLOBAL_SECONDARY_INDEX]-(:DynamoDBTable)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_sqs_queues_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_es_cleanup.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6822916666666667%*

 * *Differences: {"'name'": "'cleanup ESDomain|DNSRecord'",*

 * * "'statements'": "{0: {'query': 'MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(n:ESDomain) WHERE "*

 * *                 'n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return '*

 * *                 "COUNT(*) as TotalCompleted'}, 1: {'query': 'MATCH (:AWSAccount{id: "*

 * *                 '{AWS_ID}})-[:RESOURCE]->(:ESDomain)<-[:DNS_POINTS_TO]-(n:DNSRecord) WHERE '*

 * *                 'n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELET […]*

```diff
@@ -1,16 +1,15 @@
 {
-    "name": "cleanup SQSQueue",
+    "name": "cleanup ESDomain|DNSRecord",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(q:SQSQueue) WHERE q.lastupdated <> $UPDATE_TAG WITH q LIMIT $LIMIT_SIZE DETACH DELETE (q)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(n:ESDomain) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
-            "__comment__": "Cleanup HAS_DEADLETTER_QUEUE for queues that no longer have a deadletter queue.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:SQSQueue)-[r:HAS_DEADLETTER_QUEUE]->(:SQSQueue) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(:ESDomain)<-[:DNS_POINTS_TO]-(n:DNSRecord) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_ssm_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_account_dns_cleanup.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6041666666666667%*

 * *Differences: {"'name'": "'cleanup AWS resources linked to current account'",*

 * * "'statements'": "{0: {'query': 'MATCH "*

 * *                 '(n:AWSDNSRecord)-[:MEMBER_OF_DNS_ZONE]->(:AWSDNSZone)<-[:RESOURCE]-(:AWSAccount{id: '*

 * *                 '{AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH '*

 * *                 "DELETE (n) return COUNT(*) as TotalCompleted'}, 1: {'query': 'MATCH "*

 * *                 '()<-[r:DNS_POINTS_TO]-(:AWSDNSRecord)-[:MEMBER_OF_DNS_ZONE]->(:AWSDNSZone)<-[:RESOURCE]-(:AWSAcco […]*

```diff
@@ -1,25 +1,15 @@
 {
-    "name": "cleanup SSM",
+    "name": "cleanup AWS resources linked to current account",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(n:SSMInstanceInformation) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:AWSDNSRecord)-[:MEMBER_OF_DNS_ZONE]->(:AWSDNSZone)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:EC2Instance)-[r:HAS_INFORMATION]->(:SSMInstanceInformation) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(n:SSMInstancePatch) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:EC2Instance)-[r:HAS_PATCH]->(:SSMInstancePatch) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH ()<-[r:DNS_POINTS_TO]-(:AWSDNSRecord)-[:MEMBER_OF_DNS_ZONE]->(:AWSDNSZone)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DETACH DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_import_vpc_peering_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_ingest_ec2_auto_scaling_groups_cleanup.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6302083333333334%*

 * *Differences: {"'name'": "'cleanup EC2Instance|EC2SecurityGroup'",*

 * * "'statements'": "{0: {'query': 'MATCH (n:AutoScalingGroup)<-[:RESOURCE]-(:AWSAccount{id: "*

 * *                 '{AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH '*

 * *                 "DELETE (n) return COUNT(*) as TotalCompleted'}, 1: {'query': 'MATCH "*

 * *                 '(:AWSAccount{id: '*

 * *                 '{AWS_ID}})-[:RESOURCE]->(:AutoScalingGroup)-[:VPC_IDENTIFIER]->(n:EC2Subnet) '*

 * *                 'WHERE n.lastupdated <> {UPD […]*

```diff
@@ -1,45 +1,30 @@
 {
-    "name": "cleanup AWS VPC information",
+    "name": "cleanup EC2Instance|EC2SecurityGroup",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:AWSVpc)<-[:ACCEPTER_VPC]-(n:AWSPeeringConnection) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:AutoScalingGroup)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:AWSVpc)<-[:REQUESTER_VPC]-(n:AWSPeeringConnection) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(:AutoScalingGroup)-[:VPC_IDENTIFIER]->(n:EC2Subnet) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:AWSCidrBlock)<-[:BLOCK_ASSOCIATION]-(:AWSVpc)<-[:RESOURCE]-(:AWSAccount{foreign: true, id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(:AutoScalingGroup)-[r:VPC_IDENTIFIER]->(:EC2Subnet) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSCidrBlock)<-[r:BLOCK_ASSOCIATION]-(:AWSVpc)<-[:RESOURCE]-(:AWSAccount{foreign: true, id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(:EC2Instance)-[r:MEMBER_AUTO_SCALE_GROUP]->(:AutoScalingGroup) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:AWSVpc)<-[:RESOURCE]-(:AWSAccount{foreign: true, id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (:AWSVpc)<-[r:RESOURCE]-(:AWSAccount{foreign: true, id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (:AWSVpc)-[r:VPC_PEERING]-(:AWSVpc)<-[:RESOURCE]-(:AWSAccount{foreign: true, id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (n:AWSAccount{foreign: true, id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(:EC2Instance)-[r:MEMBER_OF_EC2_SECURITY_GROUP]->(:EC2SecurityGroup) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_ingest_ec2_auto_scaling_groups_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_ingest_load_balancers_cleanup.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7083333333333333%*

 * *Differences: {"'name'": "'cleanup LoadBalancer'",*

 * * "'statements'": "{0: {'query': 'MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(n:LoadBalancer) "*

 * *                 'WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) '*

 * *                 "return COUNT(*) as TotalCompleted'}, 1: {'query': 'MATCH (:AWSAccount{id: "*

 * *                 '{AWS_ID}})-[:RESOURCE]->(:LoadBalancer)-[r:SUBNET]->(:EC2Subnet) WHERE '*

 * *                 'r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return […]*

```diff
@@ -1,40 +1,40 @@
 {
-    "name": "cleanup EC2Instance|EC2SecurityGroup",
+    "name": "cleanup LoadBalancer",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:AutoScalingGroup)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(n:LoadBalancer) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:AutoScalingGroup)-[:VPC_IDENTIFIER]->(n:EC2Subnet) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(:LoadBalancer)-[r:SUBNET]->(:EC2Subnet) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:AutoScalingGroup)-[r:VPC_IDENTIFIER]->(:EC2Subnet) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(:LoadBalancer)-[r:MEMBER_OF_EC2_SECURITY_GROUP]->(:EC2SecurityGroup) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:EC2Instance)-[r:MEMBER_AUTO_SCALE_GROUP]->(:AutoScalingGroup) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(:LoadBalancer)-[r:SOURCE_SECURITY_GROUP]->(:EC2SecurityGroup) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:EC2Instance)-[r:MEMBER_OF_EC2_SECURITY_GROUP]->(:EC2SecurityGroup) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(:LoadBalancer)-[r:EXPOSE]->(:EC2Instance) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:LaunchTemplate)<-[r:HAS_LAUNCH_TEMPLATE]-(:AutoScalingGroup)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(:LoadBalancer)-[:ELB_LISTENER]->(n:ELBListener) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:LaunchConfiguration)<-[r:HAS_LAUNCH_CONFIG]-(:AutoScalingGroup)<-[:RESOURCE]-(:AWSAccount{id: $AWS_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(:LoadBalancer)-[r:ELB_LISTENER]->(:ELBListener) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_ingest_load_balancers_v2_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_ec2_instances_cleanup.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6388888888888888%*

 * *Differences: {"'name'": "'cleanup EC2Instance|EC2Subnet|NetworkInterface'",*

 * * "'statements'": "{3: {'query': 'MATCH "*

 * *                 '(:EC2Subnet)<-[r:PART_OF_SUBNET]-(:EC2Instance)<-[:RESOURCE]-(:AWSAccount{id: '*

 * *                 '{AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE '*

 * *                 "(r) return COUNT(*) as TotalCompleted'}, 4: {'query': 'MATCH (:AWSAccount{id: "*

 * *                 '{AWS_ID}})-[:RESOURCE]->(:EC2Instance)-[r:MEMBER_OF_EC2_RESERVATION]->(:EC2Reservation) '*

 * *     […]*

```diff
@@ -1,35 +1,50 @@
 {
-    "name": "cleanup LoadBalancerV2",
+    "name": "cleanup EC2Instance|EC2Subnet|NetworkInterface",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(n:LoadBalancerV2) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:EC2Reservation)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:LoadBalancerV2)-[r:SUBNET]->(:EC2Subnet) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (n:EC2Instance)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:LoadBalancerV2)-[r:MEMBER_OF_EC2_SECURITY_GROUP]->(:EC2SecurityGroup) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (n:EC2Subnet)<-[:PART_OF_SUBNET]-(:EC2Instance)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:LoadBalancerV2)-[r:EXPOSE]->(:EC2Instance) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:EC2Subnet)<-[r:PART_OF_SUBNET]-(:EC2Instance)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:LoadBalancerV2)-[:ELBV2_LISTENER]->(n:ELBV2Listener) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(:EC2Instance)-[r:MEMBER_OF_EC2_RESERVATION]->(:EC2Reservation) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:LoadBalancerV2)-[r:ELBV2_LISTENER]->(:ELBV2Listener) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(:EC2Instance)-[r:MEMBER_OF_EC2_SECURITY_GROUP]->(:EC2SecurityGroup) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
+        },
+        {
+            "iterationsize": 100,
+            "iterative": true,
+            "query": "MATCH (n:NetworkInterface)<-[:NETWORK_INTERFACE]-(:EC2Instance)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
+        },
+        {
+            "iterationsize": 100,
+            "iterative": true,
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(:EC2Instance)-[r:NETWORK_INTERFACE]->(:NetworkInterface) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
+        },
+        {
+            "iterationsize": 100,
+            "iterative": true,
+            "query": "MATCH (:NetworkInterface)-[r:MEMBER_OF_EC2_SECURITY_GROUP]->(:EC2SecurityGroup)<-[:RESOURCE]-(:AWSAccount{id: {AWS_ID}}) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/aws_ingest_subnets_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_policies_cleanup.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7083333333333334%*

 * *Differences: {"'name'": "'cleanup AWSPolicy'",*

 * * "'statements'": "{0: {'query': 'MATCH (:AWSAccount{id: {AWS_ID}})-[:AWS_POLICY]->(n:AWSPolicy) "*

 * *                 'WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) '*

 * *                 "return COUNT(*) as TotalCompleted'}, 1: {'query': 'MATCH (:AWSAccount{id: "*

 * *                 '{AWS_ID}})-[r:AWS_POLICY]->(:AWSPolicy) WHERE r.lastupdated <> {UPDATE_TAG} WITH '*

 * *                 "r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted'} […]*

```diff
@@ -1,15 +1,15 @@
 {
-    "name": "cleanup Subnet",
+    "name": "cleanup AWSPolicy",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:AWSVpc)<-[r:MEMBER_OF_AWS_VPC]-(n:EC2Subnet) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[:AWS_POLICY]->(n:AWSPolicy) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(:AWSVpc)<-[r:MEMBER_OF_AWS_VPC]-(:EC2Subnet) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:AWSAccount{id: {AWS_ID}})-[r:AWS_POLICY]->(:AWSPolicy) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/azure_cosmosdb_cassandra_keyspace_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/gcp_crm_project_cleanup.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6171875%*

 * *Differences: {"'name'": "'cleanup GCP Projects'",*

 * * "'statements'": "{0: {'query': 'MATCH (n:GCPProject) WHERE n.lastupdated <> {UPDATE_TAG} WITH n "*

 * *                 "LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted', "*

 * *                 "'__comment__': 'Delete GCP Projects that no longer exist and detach them from "*

 * *                 "all previously connected nodes.'}, 1: {'query': 'MATCH "*

 * *                 '(:GCPProject)<-[r:RESOURCE]-(:GCPFolder) WHERE r.lastupdated <> {UPDATE_TAG} '*

 * *              […]*

```diff
@@ -1,25 +1,23 @@
 {
-    "name": "cleanup Azure CosmosDB Cassandra Keyspace",
+    "name": "cleanup GCP Projects",
     "statements": [
         {
+            "__comment__": "Delete GCP Projects that no longer exist and detach them from all previously connected nodes.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:AzureCosmosDBCassandraTable)<-[:CONTAINS]-(:AzureCosmosDBCassandraKeyspace)<-[:CONTAINS]-(:AzureDatabaseAccount)<-[:RESOURCE]-(:AzureSubscription{id: $AZURE_SUBSCRIPTION_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:GCPProject) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
+            "__comment__": "Remove GCP Project-to-Folder relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:AzureCosmosDBCassandraTable)<-[r:CONTAINS]-(:AzureCosmosDBCassandraKeyspace)<-[:CONTAINS]-(:AzureDatabaseAccount)<-[:RESOURCE]-(:AzureSubscription{id: $AZURE_SUBSCRIPTION_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPProject)<-[r:RESOURCE]-(:GCPFolder) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
+            "__comment__": "Remove GCP Project-to-Organization relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:AzureCosmosDBCassandraKeyspace)<-[:CONTAINS]-(:AzureDatabaseAccount)<-[:RESOURCE]-(:AzureSubscription{id: $AZURE_SUBSCRIPTION_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (:AzureCosmosDBCassandraKeyspace)<-[r:CONTAINS]-(:AzureDatabaseAccount)<-[:RESOURCE]-(:AzureSubscription{id: $AZURE_SUBSCRIPTION_ID}) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPProject)<-[r:RESOURCE]-(:GCPOrganization) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/digitalocean_droplet_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_vpc_cleanup.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.625%*

 * *Differences: {"'name'": "'cleanup GCP Instances'",*

 * * "'statements'": "{1: {'query': 'MATCH (:GCPVpc)<-[r:RESOURCE]-(:GCPProject) WHERE r.lastupdated "*

 * *                 '<> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as '*

 * *                 "TotalCompleted', '__comment__': 'Remove GCP VPC-to-Project relationships that "*

 * *                 "are out of date.'}, 2: {'query': 'MATCH "*

 * *                 '(:GCPInstance)-[r:MEMBER_OF_GCP_VPC]->(:GCPVpc) WHERE r.lastupdated <> '*

 * *                 '{UPDATE_TAG} WIT […]*

```diff
@@ -1,17 +1,23 @@
 {
-    "name": "cleanup DigitalOcean Droplets",
+    "name": "cleanup GCP Instances",
     "statements": [
         {
-            "__comment__": "Delete DigitalOcean Droplets that no longer exist and detach them from all previously connected nodes.",
+            "__comment__": "Delete GCP VPCs that no longer exist and detach them from all previously connected nodes.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:DODroplet{account_id: $DO_ACCOUNT_ID}) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:GCPVpc) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
-            "__comment__": "Remove DigitalOcean Project-to-Droplet relationships that are out of date.",
+            "__comment__": "Remove GCP VPC-to-Project relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:DODroplet)<-[r:RESOURCE]-(:DOProject) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPVpc)<-[r:RESOURCE]-(:GCPProject) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
+        },
+        {
+            "__comment__": "Remove GCP Instance-to-VPC relationships that are out of date.",
+            "iterationsize": 100,
+            "iterative": true,
+            "query": "MATCH (:GCPInstance)-[r:MEMBER_OF_GCP_VPC]->(:GCPVpc) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/gcp_compute_firewall_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_firewall_cleanup.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'statements'": "{0: {'query': 'MATCH (n:GCPFirewall) WHERE n.lastupdated <> {UPDATE_TAG} WITH n "*

 * *                 "LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted'}, 1: "*

 * *                 "{'query': 'MATCH (:GCPFirewall)<-[r:RESOURCE]-(:GCPVpc) WHERE r.lastupdated <> "*

 * *                 '{UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as '*

 * *                 "TotalCompleted'}, 2: {'query': 'MATCH "*

 * *                 '(:GCPFirewall)-[r:HAS_TARGET_TAG]-(:GCPTag) WHERE r […]*

```diff
@@ -1,41 +1,41 @@
 {
     "name": "cleanup GCP Instances",
     "statements": [
         {
             "__comment__": "Delete GCP Firewalls that no longer exist and detach them from all previously connected nodes.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:GCPFirewall) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:GCPFirewall) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "__comment__": "Remove GCP VPC-to-Firewall relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:GCPFirewall)<-[r:RESOURCE]-(:GCPVpc) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPFirewall)<-[r:RESOURCE]-(:GCPVpc) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "__comment__": "Remove GCP Firewall-to-Tag relationships that are out of date. Deleting the tag itself is taken care of in GCP instance cleanup.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:GCPFirewall)-[r:HAS_TARGET_TAG]-(:GCPTag) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPFirewall)-[r:HAS_TARGET_TAG]-(:GCPTag) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "__comment__": "Delete GCP Ip Rules that no longer exist and detach them from all previously connected nodes.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:GCPIpRule) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:GCPIpRule) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "__comment__": "Remove GCP Firewall-to-IpRule relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:GCPFirewall)<-[r:ALLOWED_BY|DENIED_BY]-(:GcpIpRule) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPFirewall)<-[r:ALLOWED_BY|DENIED_BY]-(:GcpIpRule) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "__comment__": "Remove GCP IpRule-to-IpRange relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:GCPIpRule)<-[r:MEMBER_OF_IP_RULE]-(:IpRange) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPIpRule)<-[r:MEMBER_OF_IP_RULE]-(:IpRange) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/gcp_compute_instance_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_instance_cleanup.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'statements'": "{0: {'query': 'MATCH (n:GCPInstance) WHERE n.lastupdated <> {UPDATE_TAG} WITH n "*

 * *                 "LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted'}, 1: "*

 * *                 "{'query': 'MATCH (:GCPInstance)<-[r:RESOURCE]-(:GCPProject) WHERE r.lastupdated "*

 * *                 '<> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as '*

 * *                 "TotalCompleted'}, 2: {'query': 'MATCH (n:GCPNetworkInterface) WHERE "*

 * *                 'n.lastupdated <>  […]*

```diff
@@ -1,59 +1,59 @@
 {
     "name": "cleanup GCP Instances",
     "statements": [
         {
             "__comment__": "Delete GCP Instances that no longer exist and detach them from all previously connected nodes.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:GCPInstance) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:GCPInstance) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "__comment__": "Remove GCP Instance-to-Project relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:GCPInstance)<-[r:RESOURCE]-(:GCPProject) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPInstance)<-[r:RESOURCE]-(:GCPProject) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "__comment__": "Remove GCP Network Interfaces and detach them from all previously connected nodes.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:GCPNetworkInterface) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:GCPNetworkInterface) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "__comment__": "Remove GCP Instance-to-NetworkInterface relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:GCPInstance)-[r:NETWORK_INTERFACE]-(:GCPNetworkInterface) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPInstance)-[r:NETWORK_INTERFACE]-(:GCPNetworkInterface) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "__comment__": "Remove GCP Instance-to-NetworkInterface relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:GCPInstance)-[r:NETWORK_INTERFACE]-(:GCPNetworkInterface) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPInstance)-[r:NETWORK_INTERFACE]-(:GCPNetworkInterface) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "__comment__": "Remove GCP Subnets that no longer exist and detach them from all previously connected nodes.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:GCPSubnet) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:GCPSubnet) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "__comment__": "Remove GCP Network Tags that no longer exist and detach them from all previously connected nodes.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:GCPNetworkTag) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:GCPNetworkTag) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "__comment__": "Remove GCP Instance-to-Tag relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:GCPInstance)-[r:TAGGED]-(:GCPNetworkTag) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPInstance)-[r:TAGGED]-(:GCPNetworkTag) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "__comment__": "Remove GCP VPC-to-Tag relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:GCPVpc)<-[r:DEFINED_IN]-(:GCPNetworkTag) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPVpc)<-[r:DEFINED_IN]-(:GCPNetworkTag) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/gcp_crm_folder_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/gcp_crm_folder_cleanup.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'statements'": "{0: {'query': 'MATCH (n:GCPFolder) WHERE n.lastupdated <> {UPDATE_TAG} WITH n "*

 * *                 "LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted'}, 1: "*

 * *                 "{'query': 'MATCH (:GCPFolder)-[r:RESOURCE]-(:GCPFolder) WHERE r.lastupdated <> "*

 * *                 '{UPDATE_TAG} WITH distinct r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as '*

 * *                 "TotalCompleted'}, 2: {'query': 'MATCH "*

 * *                 '(:GCPFolder)<-[r:RESOURCE]-(:GCPOrganization […]*

```diff
@@ -1,23 +1,23 @@
 {
     "name": "cleanup GCP Folders",
     "statements": [
         {
             "__comment__": "Delete GCPFolders that no longer exist and detach them from all previously connected nodes",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:GCPFolder) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:GCPFolder) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "__comment__": "Remove GCP Folder-to-Folder relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:GCPFolder)-[r:RESOURCE]-(:GCPFolder) WHERE r.lastupdated <> $UPDATE_TAG WITH distinct r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPFolder)-[r:RESOURCE]-(:GCPFolder) WHERE r.lastupdated <> {UPDATE_TAG} WITH distinct r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         },
         {
             "__comment__": "Remove GCP Folder-to-Organization relationships that are out of date.",
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (:GCPFolder)<-[r:RESOURCE]-(:GCPOrganization) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH (:GCPFolder)<-[r:RESOURCE]-(:GCPOrganization) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/data/jobs/cleanup/github_users_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_post_ingestion_dns_cleanup.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6041666666666667%*

 * *Differences: {"'name'": "'cleanup AWS resources after all accounts are ingested'",*

 * * "'statements'": "{0: {'query': 'MATCH (n:DNSRecord) WHERE n.lastupdated <> {UPDATE_TAG} WITH n "*

 * *                 "LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted'}, 1: "*

 * *                 "{'query': 'MATCH ()<-[r:DNS_POINTS_TO]-(:DNSRecord) WHERE r.lastupdated <> "*

 * *                 '{UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as '*

 * *                 "TotalCompleted'}, delete: [1, 0]}"}*

```diff
@@ -1,25 +1,15 @@
 {
-    "name": "cleanup GitHub users data",
+    "name": "cleanup AWS resources after all accounts are ingested",
     "statements": [
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:GitHubUser) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
+            "query": "MATCH (n:DNSRecord) WHERE n.lastupdated <> {UPDATE_TAG} WITH n LIMIT {LIMIT_SIZE} DETACH DELETE (n) return COUNT(*) as TotalCompleted"
         },
         {
             "iterationsize": 100,
             "iterative": true,
-            "query": "MATCH (n:GitHubOrganization) WHERE n.lastupdated <> $UPDATE_TAG WITH n LIMIT $LIMIT_SIZE DETACH DELETE (n)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (:GitHubUser)-[r:OWNER]->(:GitHubRepository) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
-        },
-        {
-            "iterationsize": 100,
-            "iterative": true,
-            "query": "MATCH (:GitHubUser)-[r:MEMBER_OF]->(:GitHubOrganization) WHERE r.lastupdated <> $UPDATE_TAG WITH r LIMIT $LIMIT_SIZE DELETE (r)"
+            "query": "MATCH ()<-[r:DNS_POINTS_TO]-(:DNSRecord) WHERE r.lastupdated <> {UPDATE_TAG} WITH r LIMIT {LIMIT_SIZE} DELETE (r) return COUNT(*) as TotalCompleted"
         }
     ]
 }
```

### Comparing `cartography-0.81.0/cartography/driftdetect/add_shortcut.py` & `cartography-0.9.0/cartography/driftdetect/add_shortcut.py`

 * *Files identical despite different names*

### Comparing `cartography-0.81.0/cartography/driftdetect/cli.py` & `cartography-0.9.0/cartography/driftdetect/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,10 +235,10 @@
     """
     Entrypoint for the default cartography command line interface.
 
     :rtype: int
     :return: The return code.
     """
     logging.basicConfig(level=logging.INFO)
-    logging.getLogger('neo4j').setLevel(logging.WARNING)
+    logging.getLogger('neo4j.bolt').setLevel(logging.WARNING)
     argv = argv if argv is not None else sys.argv[1:]
     return CLI(prog="cartography-detectdrift").main(argv)
```

### Comparing `cartography-0.81.0/cartography/driftdetect/config.py` & `cartography-0.9.0/cartography/driftdetect/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from typing import Optional
-
-
 class UpdateConfig:
     """
     A common interface for the drift-detection update configuration.
 
     All fields defined on this class must be present on a configuration object. Fields documented as required must
     contain valid values. Fields documented as optional may contain None, in which case drift-detection will choose a
     sensible default value for that piece of configuration.
@@ -17,18 +14,18 @@
     :param neo4j_user: User name for a Neo4j graph database service. Optional.
     :type neo4j_password: string
     :param neo4j_password: Password for a Neo4j graph database service. Optional.
     """
 
     def __init__(
         self,
-        drift_detection_directory: str,
-        neo4j_uri: str,
-        neo4j_user: Optional[str] = None,
-        neo4j_password: Optional[str] = None,
+        drift_detection_directory,
+        neo4j_uri,
+        neo4j_user=None,
+        neo4j_password=None,
     ):
         self.neo4j_uri = neo4j_uri
         self.neo4j_user = neo4j_user
         self.neo4j_password = neo4j_password
         self.drift_detection_directory = drift_detection_directory
 
 
@@ -45,21 +42,21 @@
     :param start_state: Filename (without the directory prefix) of the earlier state to be compared with. Required.
     :type end_state: string
     :param end_state: Filename (without the directory prefix) of the later state to be compared with. Required.
     """
 
     def __init__(
         self,
-        query_directory: str,
-        start_state: str,
-        end_state: str,
+        query_directory,
+        start_state,
+        end_state,
     ):
-        self.query_directory: str = query_directory
-        self.start_state: str = start_state
-        self.end_state: str = end_state
+        self.query_directory = query_directory
+        self.start_state = start_state
+        self.end_state = end_state
 
 
 class AddShortcutConfig:
     """
     A common interface for the drift-detection add-shortcut configuration.
 
     All fields defined on this class must be present on a configuration object. Fields documented as required must
@@ -71,14 +68,14 @@
     :param shortcut: Name of shortcut to access the file. Required.
     :type filename: string
     :param filename: Filename (without the directory prefix) of the state to be shortcut. Required.
     """
 
     def __init__(
         self,
-        query_directory: str,
-        shortcut: str,
-        filename: str,
+        query_directory,
+        shortcut,
+        filename,
     ):
-        self.query_directory: str = query_directory
-        self.shortcut: str = shortcut
-        self.filename: str = filename
+        self.query_directory = query_directory
+        self.shortcut = shortcut
+        self.filename = filename
```

### Comparing `cartography-0.81.0/cartography/driftdetect/detect_deviations.py` & `cartography-0.9.0/cartography/driftdetect/detect_deviations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import logging
 import os
-from typing import List
-from typing import Union
 
 from marshmallow import ValidationError
 
-from cartography.driftdetect.config import GetDriftConfig
-from cartography.driftdetect.model import State
 from cartography.driftdetect.reporter import report_drift
 from cartography.driftdetect.serializers import ShortcutSchema
 from cartography.driftdetect.serializers import StateSchema
 from cartography.driftdetect.storage import FileSystem
 from cartography.driftdetect.util import valid_directory
 
 logger = logging.getLogger(__name__)
 
 
-def run_drift_detection(config: GetDriftConfig) -> None:
+def run_drift_detection(config):
     try:
         if not valid_directory(config.query_directory):
             logger.error("Invalid Drift Detection Directory")
             return
         state_serializer = StateSchema()
         shortcut_serializer = ShortcutSchema()
         shortcut_data = FileSystem.load(os.path.join(config.query_directory, "shortcut.json"))
@@ -59,15 +55,15 @@
             config.end_state,
             err,
             config.query_directory,
         )
         logger.exception(msg)
 
 
-def perform_drift_detection(start_state: State, end_state: State):
+def perform_drift_detection(start_state, end_state):
     """
     Returns differences (additions and missing results) between two States.
 
     :type start_state: State
     :param start_state: The earlier state chronologically to be compared to.
     :type end_state: State
     :param end_state: The later state chronologically to be compared to.
@@ -81,31 +77,29 @@
     if start_state.properties != end_state.properties:
         raise ValueError("State properties do not match.")
     new_results = compare_states(start_state, end_state)
     missing_results = compare_states(end_state, start_state)
     return new_results, missing_results
 
 
-def compare_states(start_state: State, end_state: State):
+def compare_states(start_state, end_state):
     """
     Helper function for comparing differences between two States.
 
     :type start_state: State
     :param start_state: The earlier state chronologically to be compared to.
     :type end_state: State
     :param end_state: The later state chronologically to be compared to.
     :return: list of tuples of differences between states in the form (dictionary, State object)
     """
     differences = []
-    # Use set for faster membership check
-    start_state_results = {tuple(res) for res in start_state.results}
     for result in end_state.results:
-        if tuple(result) in start_state_results:
+        if result in start_state.results:
             continue
-        drift: List[Union[str, List[str]]] = []
+        drift = []
         for field in result:
             value = field.split("|")
             if len(value) > 1:
                 drift.append(value)
             else:
                 drift.append(field)
         differences.append(drift)
```

### Comparing `cartography-0.81.0/cartography/driftdetect/get_states.py` & `cartography-0.9.0/cartography/driftdetect/get_states.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 import logging
 import os.path
 import time
-from typing import Any
-from typing import Dict
-from typing import List
 
-import neo4j.exceptions
+import neobolt.exceptions
 from marshmallow import ValidationError
-from neo4j import GraphDatabase
+from neo4j.v1 import GraphDatabase
 
-from cartography.client.core.tx import read_list_of_dicts_tx
 from cartography.driftdetect.add_shortcut import add_shortcut
-from cartography.driftdetect.config import UpdateConfig
-from cartography.driftdetect.model import State
 from cartography.driftdetect.serializers import ShortcutSchema
 from cartography.driftdetect.serializers import StateSchema
 from cartography.driftdetect.storage import FileSystem
 from cartography.driftdetect.util import valid_directory
 
 logger = logging.getLogger(__name__)
 
 
-def run_get_states(config: UpdateConfig) -> None:
+def run_get_states(config):
     """
     Handles neo4j errors and then updates detectors.
 
     :type config: Config Object
     :param config: Config Object from CLI
     :return:
     """
@@ -36,26 +30,26 @@
     if config.neo4j_user or config.neo4j_password:
         neo4j_auth = (config.neo4j_user, config.neo4j_password)
     try:
         neo4j_driver = GraphDatabase.driver(
             config.neo4j_uri,
             auth=neo4j_auth,
         )
-    except neo4j.exceptions.ServiceUnavailable as e:
+    except neobolt.exceptions.ServiceUnavailable as e:
         logger.debug("Error occurred during Neo4j connect.", exc_info=True)
         logger.error(
             (
                 "Unable to connect to Neo4j using the provided URI '%s', an error occurred: '%s'. Make sure the "
                 "Neo4j server is running and accessible from your network."
             ),
             config.neo4j_uri,
             e,
         )
         return
-    except neo4j.exceptions.AuthError as e:
+    except neobolt.exceptions.AuthError as e:
         logger.debug("Error occurred during Neo4j auth.", exc_info=True)
         if not neo4j_auth:
             logger.error(
                 (
                     "Unable to auth to Neo4j, an error occurred: '%s'. driftdetect attempted to connect to Neo4j "
                     "without any auth. Check your Neo4j server settings to see if auth is required and, if it is, "
                     "provide driftdetect with a valid username and password."
@@ -88,25 +82,19 @@
                 )
                 logger.exception(msg)
             except KeyError as err:
                 msg = f"Could not find {err} field in state template for directory {query_directory}."
                 logger.exception(msg)
             except FileNotFoundError as err:
                 logger.exception(err)
-            except neo4j.exceptions.CypherSyntaxError as err:
+            except neobolt.exceptions.CypherSyntaxError as err:
                 logger.exception(err)
 
 
-def get_query_state(
-        session: neo4j.Session,
-        query_directory: str,
-        state_serializer: StateSchema,
-        storage,
-        filename: str,
-) -> State:
+def get_query_state(session, query_directory, state_serializer, storage, filename):
     """
     Gets the most recent state of a query.
 
     :type session: neo4j session.
     :param session: neo4j session to connect to.
     :type query_directory: String.
     :param query_directory: Path to query directory.
@@ -123,39 +111,35 @@
     get_state(session, state)
     new_state_data = state_serializer.dump(state)
     fp = os.path.join(query_directory, filename)
     storage.write(new_state_data, fp)
     return state
 
 
-def get_state(session: neo4j.Session, state: State) -> None:
+def get_state(session, state):
     """
     Connects to a neo4j session, runs the validation query, then saves the results to a state.
 
     :type session: neo4j session
     :param session: Graph session to pull infrastructure information from.
     :type state: State
     :param state: State to be updated.
     :return:
     """
 
-    new_results: List[Dict[str, Any]] = session.read_transaction(
-        read_list_of_dicts_tx,
-        state.validation_query,
-    )
+    new_results = session.run(state.validation_query)
     logger.debug(f"Updating results for {state.name}")
 
-    # The keys will be the same across all items in the returned list
-    state.properties = list(new_results[0].keys())
+    state.properties = new_results.keys()
     results = []
 
     for record in new_results:
         values = []
         for field in record.values():
             if isinstance(field, list):
-                s = "|".join(sorted(str(i) for i in field))
+                s = "|".join(sorted([str(i) for i in field]))
                 values.append(s)
             else:
                 values.append(str(field))
         results.append(values)
 
-    state.results = sorted(results)
+    state.results = results
```

### Comparing `cartography-0.81.0/cartography/driftdetect/model.py` & `cartography-0.9.0/cartography/driftdetect/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from typing import List
 
 logger = logging.getLogger(__name__)
 
 
 class State:
     """
     The default object which stores query information.
@@ -16,17 +15,17 @@
     :param properties: List of keys in order that the cypher query will return.
     :type results: List of List of Strings
     :param results: List of all results of running the validation query
     """
 
     def __init__(
             self,
-            name: str,
-            validation_query: str,
-            properties: List[str],
-            results: List[List[str]],
+            name,
+            validation_query,
+            properties,
+            results,
     ):
 
-        self.name: str = name
-        self.validation_query: str = validation_query
-        self.properties: List[str] = properties
-        self.results: List[List[str]] = results
+        self.name = name
+        self.validation_query = validation_query
+        self.properties = properties
+        self.results = results
```

### Comparing `cartography-0.81.0/cartography/driftdetect/reporter.py` & `cartography-0.9.0/cartography/driftdetect/reporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 def report_drift_new(results, state_properties):
     """
     Prints new additions in Query Results between two states.
 
     :type results: List of List of Strings.
     :param results: Deviation information.
     :return: None
```

### Comparing `cartography-0.81.0/cartography/driftdetect/serializers.py` & `cartography-0.9.0/cartography/driftdetect/serializers.py`

 * *Files identical despite different names*

### Comparing `cartography-0.81.0/cartography/driftdetect/storage.py` & `cartography-0.9.0/cartography/driftdetect/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def load(cls, file_path):
         """
         Loads a JSON object (dict) from a file.
         :type file_path: string.
         :param file_path: Filepath for the file.
         :return: Dictionary in JSON format.
         """
-        with open(file_path) as json_file:
+        with open(file_path, 'r') as json_file:
             data = json.load(json_file)
         return data
 
     @classmethod
     def write(cls, data, file_path):
         """
         Writes a JSON object (dict) to a file.
```

### Comparing `cartography-0.81.0/cartography/driftdetect/util.py` & `cartography-0.9.0/cartography/driftdetect/util.py`

 * *Files identical despite different names*

### Comparing `cartography-0.81.0/cartography/graph/context.py` & `cartography-0.9.0/cartography/graph/context.py`

 * *Files identical despite different names*

### Comparing `cartography-0.81.0/cartography/intel/analysis.py` & `cartography-0.9.0/cartography/intel/analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import logging
 import pathlib
 
-import neo4j
-
-from cartography.config import Config
 from cartography.graph.job import GraphJob
 
+
 logger = logging.getLogger(__name__)
 
 
-def run(neo4j_session: neo4j.Session, config: Config) -> None:
+def run(neo4j_session, config):
     analysis_job_directory_path = config.analysis_job_directory
     if not analysis_job_directory_path:
         logger.info("Skipping analysis because no job path was provided.")
         return
     analysis_job_directory = pathlib.Path(analysis_job_directory_path)
     if not analysis_job_directory.exists():
         logger.warning(
```

### Comparing `cartography-0.81.0/cartography/intel/aws/apigateway.py` & `cartography-0.9.0/cartography/intel/aws/s3.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,379 +1,327 @@
+import hashlib
 import json
 import logging
-from typing import Any
-from typing import Dict
-from typing import List
-from typing import Optional
-from typing import Tuple
-
-import boto3
-import botocore
-import neo4j
+
 from botocore.exceptions import ClientError
 from policyuniverse.policy import Policy
 
-from cartography.util import aws_handle_regions
+from cartography.util import run_analysis_job
 from cartography.util import run_cleanup_job
-from cartography.util import timeit
 
 logger = logging.getLogger(__name__)
 
 
-@timeit
-@aws_handle_regions
-def get_apigateway_rest_apis(boto3_session: boto3.session.Session, region: str) -> List[Dict]:
-    client = boto3_session.client('apigateway', region_name=region)
-    paginator = client.get_paginator('get_rest_apis')
-    apis: List[Any] = []
-    for page in paginator.paginate():
-        apis.extend(page['items'])
-    return apis
-
-
-@timeit
-@aws_handle_regions
-def get_rest_api_details(
-        boto3_session: boto3.session.Session, rest_apis: List[Dict], region: str,
-) -> List[Tuple[Any, Any, Any, Any, Any]]:
-    """
-    Iterates over all API Gateway REST APIs.
-    """
-    client = boto3_session.client('apigateway', region_name=region)
-    apis = []
-    for api in rest_apis:
-        stages = get_rest_api_stages(api, client)
-        # clientcertificate id is given by the api stage
-        certificate = get_rest_api_client_certificate(stages, client)  # type: ignore
-        resources = get_rest_api_resources(api, client)
-        policy = get_rest_api_policy(api, client)
-        apis.append((api['id'], stages, certificate, resources, policy))
-    return apis
+def get_s3_bucket_list(session):
+    client = session.client('s3')
+    # NOTE no paginator available for this operation
+    return client.list_buckets()
 
 
-@timeit
-def get_rest_api_stages(api: Dict, client: botocore.client.BaseClient) -> List[Any]:
+def get_s3_bucket_details(session, bucket_data):
     """
-    Gets the REST API Stage Resources.
+    Iterates over all S3 buckets. Yields bucket name (string) and pairs of S3 bucket policies (JSON) and ACLs (JSON)
     """
-    try:
-        stages = client.get_stages(restApiId=api['id'])
-    except ClientError as e:
-        logger.warning(f'Failed to retrieve Stages for Api Id - {api["id"]} - {e}')
-        raise
-
-    return stages['item']
+    client = session.client('s3')
+    for bucket in bucket_data['Buckets']:
+        acl = get_acl(bucket, client)
+        policy = get_policy(bucket, client)
+        yield bucket['Name'], acl, policy
 
 
-@timeit
-def get_rest_api_client_certificate(stages: Dict, client: botocore.client.BaseClient) -> Optional[Any]:
+def get_policy(bucket, client):
     """
-    Gets the current ClientCertificate resource if present, else returns None.
-    """
-    response = None
-    for stage in stages:
-        if 'clientCertificateId' in stage:
-            try:
-                response = client.get_client_certificate(clientCertificateId=stage['clientCertificateId'])
-                response['stageName'] = stage['stageName']
-            except ClientError as e:
-                logger.warning(f"Failed to retrive Client Certificate for Stage {stage['stageName']} - {e}")
-                raise
+    Gets the S3 bucket policy. Returns policy string or None if no policy
+    """
+    try:
+        policy = client.get_bucket_policy(Bucket=bucket['Name'])
+    except ClientError as e:
+        # no policy is defined for this bucket
+        if "NoSuchBucketPolicy" in e.args[0]:
+            policy = None
+        elif "AccessDenied" in e.args[0]:
+            logger.warning("Access denied trying to retrieve S3 bucket {} policy".format(bucket['Name']))
+            policy = None
         else:
-            return []
-
-    return response
+            raise
+    return policy
 
 
-@timeit
-def get_rest_api_resources(api: Dict, client: botocore.client.BaseClient) -> List[Any]:
+def get_acl(bucket, client):
     """
-    Gets the collection of Resource resources.
+    Gets the S3 bucket ACL. Returns ACL string
     """
-    resources: List[Any] = []
-    paginator = client.get_paginator('get_resources')
-    response_iterator = paginator.paginate(restApiId=api['id'])
-    for page in response_iterator:
-        resources.extend(page['items'])
-
-    return resources
+    try:
+        acl = client.get_bucket_acl(Bucket=bucket['Name'])
+    except ClientError as e:
+        if "AccessDenied" in e.args[0]:
+            logger.warning("Failed to retrieve S3 bucket {} ACL - Access Denied".format(bucket['Name']))
+            return None
+        elif "NoSuchBucket" in e.args[0]:
+            logger.warning("Failed to retrieve S3 bucket {} ACL - No Such Bucket".format(bucket['Name']))
+            return None
+        else:
+            raise
+    return acl
 
 
-@timeit
-def get_rest_api_policy(api: Dict, client: botocore.client.BaseClient) -> List[Any]:
+def _load_s3_acls(session, acls, aws_account_id, update_tag):
     """
-    Gets the REST API policy. Returns policy string or None if no policy is present.
+    Ingest S3 ACL into neo4j.
     """
-    policy = api['policy'] if 'policy' in api and api['policy'] else None
-    return policy
-
-
-@timeit
-def load_apigateway_rest_apis(
-    neo4j_session: neo4j.Session, rest_apis: List[Dict], region: str, current_aws_account_id: str,
-    aws_update_tag: int,
-) -> None:
-    """
-    Ingest the details of API Gateway REST APIs into neo4j.
-    """
-    ingest_rest_apis = """
-    UNWIND $rest_apis_list AS r
-    MERGE (rest_api:APIGatewayRestAPI{id:r.id})
-    ON CREATE SET rest_api.firstseen = timestamp(),
-    rest_api.createddate = r.createdDate
-    SET rest_api.version = r.version,
-    rest_api.minimumcompressionsize = r.minimumCompressionSize,
-    rest_api.disableexecuteapiendpoint = r.disableExecuteApiEndpoint,
-    rest_api.lastupdated = $aws_update_tag,
-    rest_api.region = $Region
-    WITH rest_api
-    MATCH (aa:AWSAccount{id: $AWS_ACCOUNT_ID})
-    MERGE (aa)-[r:RESOURCE]->(rest_api)
+    ingest_acls = """
+    UNWIND {acls} AS acl
+    MERGE (a:S3Acl{id: acl.id})
+    ON CREATE SET a.firstseen = timestamp(), a.owner = acl.owner, a.ownerid = acl.ownerid, a.type = acl.type,
+    a.displayname = acl.displayname, a.granteeid = acl.granteeid, a.uri = acl.uri, a.permission = acl.permission
+    SET a.lastupdated = {UpdateTag}
+    WITH a,acl MATCH (s3:S3Bucket{name: acl.bucket})
+    MERGE (a)-[r:APPLIES_TO]->(s3)
     ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $aws_update_tag
+    SET r.lastupdated = {UpdateTag}
     """
 
-    # neo4j does not accept datetime objects and values. This loop is used to convert
-    # these values to string.
-    for api in rest_apis:
-        api['createdDate'] = str(api['createdDate']) if 'createdDate' in api else None
-
-    neo4j_session.run(
-        ingest_rest_apis,
-        rest_apis_list=rest_apis,
-        aws_update_tag=aws_update_tag,
-        Region=region,
-        AWS_ACCOUNT_ID=current_aws_account_id,
+    session.run(
+        ingest_acls,
+        acls=acls,
+        UpdateTag=update_tag,
+    )
+
+    # implement the acl permission
+    # https://docs.aws.amazon.com/AmazonS3/latest/dev/acl-overview.html#permissions
+    run_analysis_job(
+        'aws_s3acl_analysis.json',
+        session,
+        {'AWS_ID': aws_account_id},
     )
 
 
-@timeit
-def _load_apigateway_policies(
-        neo4j_session: neo4j.Session, policies: List, update_tag: int,
-) -> None:
+def _load_s3_policies(session, policies, update_tag):
     """
-    Ingest API Gateway REST API policy results into neo4j.
+    Ingest S3 policy results into neo4j.
     """
+    # NOTE we use the coalesce function so appending works when the value is null initially
     ingest_policies = """
-    UNWIND $policies as policy
-    MATCH (r:APIGatewayRestAPI) where r.name = policy.api_id
-    SET r.anonymous_access = (coalesce(r.anonymous_access, false) OR policy.internet_accessible),
-    r.anonymous_actions = coalesce(r.anonymous_actions, []) + policy.accessible_actions,
-    r.lastupdated = $UpdateTag
+    UNWIND {policies} AS policy
+    MATCH (s:S3Bucket) where s.name = policy.bucket
+    SET s.anonymous_access = (coalesce(s.anonymous_access, false) OR policy.internet_accessible),
+    s.anonymous_actions = coalesce(s.anonymous_actions, []) + policy.accessible_actions,
+    s.lastupdated = {UpdateTag}
     """
 
-    neo4j_session.run(
+    session.run(
         ingest_policies,
         policies=policies,
         UpdateTag=update_tag,
     )
 
 
-def _set_default_values(neo4j_session: neo4j.Session, aws_account_id: str) -> None:
+def _set_default_values(session, aws_account_id):
     set_defaults = """
-    MATCH (:AWSAccount{id: $AWS_ID})-[:RESOURCE]->(restApi:APIGatewayRestAPI)
-    where restApi.anonymous_actions IS NULL
-    SET restApi.anonymous_access = false, restApi.anonymous_actions = []
+    MATCH (:AWSAccount{id: {AWS_ID}})-[:RESOURCE]->(s:S3Bucket) where NOT EXISTS(s.anonymous_actions)
+    SET s.anonymous_access = false, s.anonymous_actions = []
     """
 
-    neo4j_session.run(
+    session.run(
         set_defaults,
         AWS_ID=aws_account_id,
     )
 
 
-@timeit
-def _load_apigateway_stages(
-        neo4j_session: neo4j.Session, stages: List, update_tag: int,
-) -> None:
-    """
-    Ingest the Stage resource details into neo4j.
-    """
-    ingest_stages = """
-    UNWIND $stages_list AS stage
-    MERGE (s:APIGatewayStage{id: stage.arn})
-    ON CREATE SET s.firstseen = timestamp(), s.stagename = stage.stageName,
-    s.createddate = stage.createdDate
-    SET s.deploymentid = stage.deploymentId,
-    s.clientcertificateid = stage.clientCertificateId,
-    s.cacheclusterenabled = stage.cacheClusterEnabled,
-    s.cacheclusterstatus = stage.cacheClusterStatus,
-    s.tracingenabled = stage.tracingEnabled,
-    s.webaclarn = stage.webAclArn,
-    s.lastupdated = $UpdateTag
-    WITH s, stage
-    MATCH (rest_api:APIGatewayRestAPI{id: stage.apiId})
-    MERGE (rest_api)-[r:ASSOCIATED_WITH]->(s)
-    ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $UpdateTag
+def load_s3_details(session, s3_details_iter, aws_account_id, update_tag):
+    """
+    Create dictionaries for all bucket ACLs and all bucket policies so we can import them in a single query for each
     """
+    acls = []
+    policies = []
+    for bucket, acl, policy in s3_details_iter:
+        if acl is None:
+            continue
+        parsed_acls = parse_acl(acl, bucket, aws_account_id)
+        if parsed_acls:
+            acls.extend(parsed_acls)
+        else:
+            continue
+        parsed_policy = parse_policy(bucket, policy)
+        if parsed_policy is not None:
+            policies.append(parsed_policy)
 
-    # neo4j does not accept datetime objects and values. This loop is used to convert
-    # these values to string.
-    for stage in stages:
-        stage['createdDate'] = str(stage['createdDate'])
-        stage['arn'] = "arn:aws:apigateway:::" + stage['apiId'] + "/" + stage['stageName']
-
-    neo4j_session.run(
-        ingest_stages,
-        stages_list=stages,
-        UpdateTag=update_tag,
+    # cleanup existing policy properties set on S3 Buckets
+    run_cleanup_job(
+        'aws_s3_details.json',
+        session,
+        {'UPDATE_TAG': update_tag, 'AWS_ID': aws_account_id},
     )
 
+    _load_s3_acls(session, acls, aws_account_id, update_tag)
+    _load_s3_policies(session, policies, update_tag)
+    _set_default_values(session, aws_account_id)
+
+
+def parse_policy(bucket, policy):
+    """
+    Uses PolicyUniverse to parse S3 policies and returns the internet accessibility results
+    """
+    # policy is not required, so may be None
+    # policy JSON format. Note condition can be any JSON statement so will need to import as-is
+    # policy is a very complex format, so the policyuniverse library will be used for parsing out important data
+    # ...metadata...
+    # "Policy" :
+    # {
+    #     "Version": "2012-10-17",
+    #     {
+    #         "Statement": [
+    #             {
+    #                 "Effect": "Allow",
+    #                 "Principal": "*",
+    #                 "Action": "s3:GetObject",
+    #                 "Resource": "arn:aws:s3:::MyBucket/*"
+    #             },
+    #             {
+    #                 "Effect": "Deny",
+    #                 "Principal": "*",
+    #                 "Action": "s3:GetObject",
+    #                 "Resource": "arn:aws:s3:::MyBucket/MySecretFolder/*"
+    #             },
+    #             {
+    #                 "Effect": "Allow",
+    #                 "Principal": {
+    #                     "AWS": "arn:aws:iam::123456789012:root"
+    #                 },
+    #                 "Action": [
+    #                     "s3:DeleteObject",
+    #                     "s3:PutObject"
+    #                 ],
+    #                 "Resource": "arn:aws:s3:::MyBucket/*"
+    #             }
+    #         ]
+    #     }
+    # }
+    if policy is not None:
+        # get just the policy element and convert to JSON because boto3 returns this as string
+        policy = Policy(json.loads(policy['Policy']))
+        if policy.is_internet_accessible():
+            return {
+                "bucket": bucket,
+                "internet_accessible": True,
+                "accessible_actions": list(policy.internet_accessible_actions()),
+            }
+        else:
+            return None
+    else:
+        return None
 
-@timeit
-def _load_apigateway_certificates(
-        neo4j_session: neo4j.Session, certificates: List, update_tag: int,
-) -> None:
-    """
-    Ingest the API Gateway Client Certificate details into neo4j.
-    """
-    ingest_certificates = """
-    UNWIND $certificates_list as certificate
-    MERGE (c:APIGatewayClientCertificate{id: certificate.clientCertificateId})
-    ON CREATE SET c.firstseen = timestamp(), c.createddate = certificate.createdDate
-    SET c.lastupdated = $UpdateTag, c.expirationdate = certificate.expirationDate
-    WITH c, certificate
-    MATCH (stage:APIGatewayStage{id: certificate.stageArn})
-    MERGE (stage)-[r:HAS_CERTIFICATE]->(c)
-    ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $UpdateTag
-    """
-
-    # neo4j does not accept datetime objects and values. This loop is used to convert
-    # these values to string.
-    for certificate in certificates:
-        certificate['createdDate'] = str(certificate['createdDate'])
-        certificate['expirationDate'] = str(certificate.get('expirationDate'))
-        certificate['stageArn'] = "arn:aws:apigateway:::" + certificate['apiId'] + "/" + certificate['stageName']
-
-    neo4j_session.run(
-        ingest_certificates,
-        certificates_list=certificates,
-        UpdateTag=update_tag,
-    )
 
+def parse_acl(acl, bucket, aws_account_id):
+    """ Parses the AWS ACL object and returns a dict of the relevant data """
+    # ACL JSON looks like
+    # ...metadata...
+    # {
+    #     "Grants": [
+    #         {
+    #             "Grantee": {
+    #                 "DisplayName": "string",
+    #                 "EmailAddress": "string",
+    #                 "ID": "string",
+    #                 "Type": "CanonicalUser" | "AmazonCustomerByEmail" | "Group",
+    #                 "URI": "string"
+    #             },
+    #             "Permission": "FULL_CONTROL" | "WRITE" | "WRITE_ACP" | "READ" | "READ_ACP"
+    #         }
+    #              ...
+    #     ],
+    #     "Owner": {
+    #         "DisplayName": "string",
+    #         "ID": "string"
+    #     }
+    # }
+    acl_list = []
+    for grant in acl['Grants']:
+        parsed_acl = None
+        if grant['Grantee']['Type'] == 'CanonicalUser':
+            parsed_acl = {
+                "bucket": bucket,
+                "owner": acl['Owner'].get('DisplayName', "none"),
+                "ownerid": acl['Owner'].get('ID', "none"),
+                "type": grant['Grantee']['Type'],
+                "displayname": grant['Grantee'].get('DisplayName', "none"),
+                "granteeid": grant['Grantee'].get('ID', "none"),
+                "uri": "",
+                "permission": grant.get('Permission', "none"),
+            }
+        elif grant['Grantee']['Type'] == 'Group':
+            parsed_acl = {
+                "bucket": bucket,
+                "owner": acl['Owner'].get('DisplayName', "none"),
+                "ownerid": acl['Owner'].get('ID', "none"),
+                "type": grant['Grantee']['Type'],
+                "displayname": "",
+                "granteeid": "",
+                "uri": grant['Grantee'].get('URI', "none"),
+                "permission": grant.get('Permission', "none"),
+            }
+        else:
+            logger.warning("Unexpected grant type: %s", grant['Grantee']['Type'])
+            continue
 
-@timeit
-def _load_apigateway_resources(
-        neo4j_session: neo4j.Session, resources: List, update_tag: int,
-) -> None:
-    """
-    Ingest the API Gateway Resource details into neo4j.
-    """
-    ingest_resources = """
-    UNWIND $resources_list AS res
-    MERGE (s:APIGatewayResource{id: res.id})
-    ON CREATE SET s.firstseen = timestamp()
-    SET s.path = res.path,
-    s.pathpart = res.pathPart,
-    s.parentid = res.parentId,
-    s.lastupdated =$UpdateTag
-    WITH s, res
-    MATCH (rest_api:APIGatewayRestAPI{id: res.apiId})
-    MERGE (rest_api)-[r:RESOURCE]->(s)
+        # TODO this can be replaced with a string join
+        id_data = "{}:{}:{}:{}:{}:{}:{}:{}".format(
+            aws_account_id,
+            parsed_acl['owner'],
+            parsed_acl['ownerid'],
+            parsed_acl['type'],
+            parsed_acl['displayname'],
+            parsed_acl['granteeid'],
+            parsed_acl['uri'],
+            parsed_acl['permission'],
+        )
+
+        parsed_acl['id'] = hashlib.sha256(id_data.encode("utf8")).hexdigest()
+        acl_list.append(parsed_acl)
+
+    return acl_list
+
+
+def load_s3_buckets(session, data, current_aws_account_id, aws_update_tag):
+    ingest_bucket = """
+    MERGE (bucket:S3Bucket{name: {BucketName}})
+    ON CREATE SET bucket.firstseen = timestamp(), bucket.creationdate = {CreationDate}
+    SET bucket.lastupdated = {aws_update_tag}
+    WITH bucket
+    MATCH (owner:AWSAccount{id: {AWS_ACCOUNT_ID}})
+    MERGE (owner)-[r:RESOURCE]->(bucket)
     ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $UpdateTag
+    SET r.lastupdated = {aws_update_tag}
     """
 
-    neo4j_session.run(
-        ingest_resources,
-        resources_list=resources,
-        UpdateTag=update_tag,
-    )
+    # The owner data returned by the API maps to the aws account nickname and not the IAM user
+    # there doesn't seem to be a way to retreive the mapping but we can get the current context account
+    # so we map to that directly
 
+    for bucket in data["Buckets"]:
+        session.run(
+            ingest_bucket,
+            BucketName=bucket["Name"],
+            CreationDate=str(bucket["CreationDate"]),
+            AWS_ACCOUNT_ID=current_aws_account_id,
+            aws_update_tag=aws_update_tag,
+        )
 
-@timeit
-def load_rest_api_details(
-        neo4j_session: neo4j.Session, stages_certificate_resources: List[Tuple[Any, Any, Any, Any, Any]],
-        aws_account_id: str, update_tag: int,
-) -> None:
-    """
-    Create dictionaries for Stages, Client certificates, policies and Resource resources
-    so we can import them in a single query
-    """
-    stages: List[Dict] = []
-    certificates: List[Dict] = []
-    resources: List[Dict] = []
-    policies: List = []
-    for api_id, stage, certificate, resource, policy in stages_certificate_resources:
-        parsed_policy = parse_policy(api_id, policy)
-        if parsed_policy is not None:
-            policies.append(parsed_policy)
-        if len(stage) > 0:
-            for s in stage:
-                s['apiId'] = api_id
-            stages.extend(stage)
-        if len(resource) > 0:
-            for r in resource:
-                r['apiId'] = api_id
-            resources.extend(resource)
-        if certificate:
-            certificate['apiId'] = api_id
-            certificates.append(certificate)
 
-    # cleanup existing properties
-    run_cleanup_job(
-        'aws_apigateway_details.json',
-        neo4j_session,
-        {'UPDATE_TAG': update_tag, 'AWS_ID': aws_account_id},
-    )
+def cleanup_s3_buckets(session, common_job_parameters):
+    run_cleanup_job('aws_import_s3_buckets_cleanup.json', session, common_job_parameters)
 
-    _load_apigateway_policies(neo4j_session, policies, update_tag)
-    _load_apigateway_stages(neo4j_session, stages, update_tag)
-    _load_apigateway_certificates(neo4j_session, certificates, update_tag)
-    _load_apigateway_resources(neo4j_session, resources, update_tag)
-    _set_default_values(neo4j_session, aws_account_id)
 
+def cleanup_s3_bucket_acl_and_policy(session, common_job_parameters):
+    run_cleanup_job('aws_import_s3_acl_cleanup.json', session, common_job_parameters)
 
-@timeit
-def parse_policy(api_id: str, policy: Policy) -> Optional[Dict[Any, Any]]:
-    """
-    Uses PolicyUniverse to parse API Gateway REST API policy and returns the internet accessibility results
-    """
 
-    if policy is not None:
-        # unescape doubly escapped JSON
-        policy = policy.replace("\\", "")
-        try:
-            policy = Policy(json.loads(policy))
-            if policy.is_internet_accessible():
-                return {
-                    "api_id": api_id,
-                    "internet_accessible": True,
-                    "accessible_actions": list(policy.internet_accessible_actions()),
-                }
-            else:
-                return None
-        except json.JSONDecodeError:
-            logger.warn(f"failed to decode policy json : {policy}")
-            return None
-    else:
-        return None
+def sync(neo4j_session, boto3_session, current_aws_account_id, aws_update_tag, common_job_parameters):
+    logger.info("Syncing S3 for account '%s'.", current_aws_account_id)
+    bucket_data = get_s3_bucket_list(boto3_session)
 
+    load_s3_buckets(neo4j_session, bucket_data, current_aws_account_id, aws_update_tag)
+    cleanup_s3_buckets(neo4j_session, common_job_parameters)
 
-@timeit
-def cleanup(neo4j_session: neo4j.Session, common_job_parameters: Dict) -> None:
-    run_cleanup_job('aws_import_apigateway_cleanup.json', neo4j_session, common_job_parameters)
-
-
-@timeit
-def sync_apigateway_rest_apis(
-    neo4j_session: neo4j.Session, boto3_session: boto3.session.Session, region: str, current_aws_account_id: str,
-    aws_update_tag: int,
-) -> None:
-    rest_apis = get_apigateway_rest_apis(boto3_session, region)
-    load_apigateway_rest_apis(neo4j_session, rest_apis, region, current_aws_account_id, aws_update_tag)
-
-    stages_certificate_resources = get_rest_api_details(boto3_session, rest_apis, region)
-    load_rest_api_details(neo4j_session, stages_certificate_resources, current_aws_account_id, aws_update_tag)
-
-
-@timeit
-def sync(
-    neo4j_session: neo4j.Session, boto3_session: boto3.session.Session, regions: List[str], current_aws_account_id: str,
-    update_tag: int, common_job_parameters: Dict,
-) -> None:
-    for region in regions:
-        logger.info(f"Syncing AWS APIGateway Rest APIs for region '{region}' in account '{current_aws_account_id}'.")
-        sync_apigateway_rest_apis(neo4j_session, boto3_session, region, current_aws_account_id, update_tag)
-    cleanup(neo4j_session, common_job_parameters)
+    acl_and_policy_data_iter = get_s3_bucket_details(boto3_session, bucket_data)
+    load_s3_details(neo4j_session, acl_and_policy_data_iter, current_aws_account_id, aws_update_tag)
+    cleanup_s3_bucket_acl_and_policy(neo4j_session, common_job_parameters)
```

### Comparing `cartography-0.81.0/cartography/intel/aws/dynamodb.py` & `cartography-0.9.0/cartography/intel/aws/dynamodb.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,129 +1,90 @@
 import logging
-from typing import Any
-from typing import Dict
-from typing import List
-
-import boto3
-import neo4j
-
-from cartography.client.core.tx import load
-from cartography.graph.job import GraphJob
-from cartography.intel.aws.ec2.util import get_botocore_config
-from cartography.models.aws.dynamodb.gsi import DynamoDBGSISchema
-from cartography.models.aws.dynamodb.tables import DynamoDBTableSchema
-from cartography.stats import get_stats_client
-from cartography.util import aws_handle_regions
-from cartography.util import merge_module_sync_metadata
-from cartography.util import timeit
+
+from cartography.util import run_cleanup_job
 
 logger = logging.getLogger(__name__)
-stat_handler = get_stats_client(__name__)
 
 
-@timeit
-@aws_handle_regions
-def get_dynamodb_tables(boto3_session: boto3.session.Session, region: str) -> List[Dict]:
-    client = boto3_session.client('dynamodb', region_name=region, config=get_botocore_config())
+def get_dynamodb_tables(session, region):
+    client = session.client('dynamodb', region_name=region)
     paginator = client.get_paginator('list_tables')
     dynamodb_tables = []
     for page in paginator.paginate():
         for table_name in page['TableNames']:
             dynamodb_tables.append(client.describe_table(TableName=table_name))
-    return dynamodb_tables
+    return {'Tables': dynamodb_tables}
+
+
+def load_dynamodb_tables(session, data, region, current_aws_account_id, aws_update_tag):
+    ingest_table = """
+    MERGE (table:DynamoDBTable{id: {Arn}})
+    ON CREATE SET table.firstseen = timestamp(), table.arn = {Arn}, table.name = {TableName},
+    table.region = {Region}
+    SET table.lastupdated = {aws_update_tag}, table.rows = {Rows}, table.size = {Size},
+    table.provisioned_throughput_read_capacity_units = {ProvisionedThroughputReadCapacityUnits},
+    table.provisioned_throughput_write_capacity_units = {ProvisionedThroughputWriteCapacityUnits}
+    WITH table
+    MATCH (owner:AWSAccount{id: {AWS_ACCOUNT_ID}})
+    MERGE (owner)-[r:RESOURCE]->(table)
+    ON CREATE SET r.firstseen = timestamp()
+    SET r.lastupdated = {aws_update_tag}
+    """
+
+    for table in data["Tables"]:
+        session.run(
+            ingest_table,
+            Arn=table['Table']['TableArn'],
+            Region=region,
+            ProvisionedThroughputReadCapacityUnits=table['Table']['ProvisionedThroughput']['ReadCapacityUnits'],
+            ProvisionedThroughputWriteCapacityUnits=table['Table']['ProvisionedThroughput']['WriteCapacityUnits'],
+            Size=table['Table']['TableSizeBytes'],
+            TableName=table['Table']['TableName'],
+            Rows=table['Table']['ItemCount'],
+            AWS_ACCOUNT_ID=current_aws_account_id,
+            aws_update_tag=aws_update_tag,
+        )
+        load_gsi(session, table, region, current_aws_account_id, aws_update_tag)
+
+
+def load_gsi(session, table, region, current_aws_account_id, aws_update_tag):
+    ingest_gsi = """
+    MERGE (gsi:DynamoDBGlobalSecondaryIndex{id: {Arn}})
+    ON CREATE SET gsi.firstseen = timestamp(), gsi.arn = {Arn}, gsi.name = {GSIName},
+    gsi.region = {Region}
+    SET gsi.lastupdated = {aws_update_tag},
+    gsi.provisioned_throughput_read_capacity_units = {ProvisionedThroughputReadCapacityUnits},
+    gsi.provisioned_throughput_write_capacity_units = {ProvisionedThroughputWriteCapacityUnits}
+    WITH gsi
+    MATCH (table:DynamoDBTable{arn: {TableArn}})
+    MERGE (table)-[r:GLOBAL_SECONDARY_INDEX]->(gsi)
+    ON CREATE SET r.firstseen = timestamp()
+    SET r.lastupdated = {aws_update_tag}
+    """
+
+    for gsi in table['Table'].get('GlobalSecondaryIndexes', []):
+        session.run(
+            ingest_gsi,
+            TableArn=table['Table']['TableArn'],
+            Arn=gsi['IndexArn'],
+            Region=region,
+            ProvisionedThroughputReadCapacityUnits=gsi['ProvisionedThroughput']['ReadCapacityUnits'],
+            ProvisionedThroughputWriteCapacityUnits=gsi['ProvisionedThroughput']['WriteCapacityUnits'],
+            GSIName=gsi['IndexName'],
+            AWS_ACCOUNT_ID=current_aws_account_id,
+            aws_update_tag=aws_update_tag,
+        )
 
 
-@timeit
-def transform_dynamodb_tables(dynamodb_tables: List, region: str) -> Any:
-    ddb_table_data: List[Dict[str, Any]] = []
-    ddb_gsi_data: List[Dict[str, Any]] = []
-
-    for table in dynamodb_tables:
-        ddb_table_data.append({
-            'Arn': table['Table']['TableArn'],
-            'TableName': table['Table']['TableName'],
-            'Region': region,
-            'Rows': table['Table']['ItemCount'],
-            'Size': table['Table']['TableSizeBytes'],
-            'ProvisionedThroughputReadCapacityUnits': table['Table']['ProvisionedThroughput']['ReadCapacityUnits'],
-            'ProvisionedThroughputWriteCapacityUnits': table['Table']['ProvisionedThroughput']['WriteCapacityUnits'],
-        })
-        for gsi in table['Table'].get('GlobalSecondaryIndexes', []):
-            ddb_gsi_data.append({
-                'Arn': gsi['IndexArn'],
-                'TableArn': table['Table']['TableArn'],
-                'Region': region,
-                'ProvisionedThroughputReadCapacityUnits': gsi['ProvisionedThroughput']['ReadCapacityUnits'],
-                'ProvisionedThroughputWriteCapacityUnits': gsi['ProvisionedThroughput']['WriteCapacityUnits'],
-                'GSIName': gsi['IndexName'],
-            })
-    return ddb_table_data, ddb_gsi_data
-
-
-@timeit
-def load_dynamodb_tables(
-    neo4j_session: neo4j.Session, tables_data: List[Dict[str, Any]], region: str, current_aws_account_id: str,
-    aws_update_tag: int,
-) -> None:
-    logger.info(f"Loading Dynamo DB tables {len(tables_data)} for region '{region}' into graph.")
-    load(
-        neo4j_session,
-        DynamoDBTableSchema(),
-        tables_data,
-        lastupdated=aws_update_tag,
-        Region=region,
-        AWS_ID=current_aws_account_id,
-    )
-
-
-@timeit
-def load_dynamodb_gsi(
-    neo4j_session: neo4j.Session, gsi_data: List[Dict[str, Any]], region: str, current_aws_account_id: str,
-    aws_update_tag: int,
-) -> None:
-    logger.info(f"Loading Dynamo DB GSI {len(gsi_data)} for region '{region}' into graph.")
-    load(
-        neo4j_session,
-        DynamoDBGSISchema(),
-        gsi_data,
-        lastupdated=aws_update_tag,
-        Region=region,
-        AWS_ID=current_aws_account_id,
-    )
-
-
-@timeit
-def cleanup_dynamodb_tables(neo4j_session: neo4j.Session, common_job_parameters: Dict) -> None:
-    GraphJob.from_node_schema(DynamoDBTableSchema(), common_job_parameters).run(neo4j_session)
-    GraphJob.from_node_schema(DynamoDBGSISchema(), common_job_parameters).run(neo4j_session)
+def cleanup_dynamodb_tables(session, common_job_parameters):
+    run_cleanup_job('aws_import_dynamodb_tables_cleanup.json', session, common_job_parameters)
 
 
-@timeit
 def sync_dynamodb_tables(
-    neo4j_session: neo4j.Session, boto3_session: boto3.session.Session, regions: List[str], current_aws_account_id: str,
-    aws_update_tag: int, common_job_parameters: Dict,
-) -> None:
+    session, boto3_session, regions, current_aws_account_id, aws_update_tag,
+    common_job_parameters,
+):
     for region in regions:
         logger.info("Syncing DynamoDB for region in '%s' in account '%s'.", region, current_aws_account_id)
-        dynamodb_tables = get_dynamodb_tables(boto3_session, region)
-        ddb_table_data, ddb_gsi_data = transform_dynamodb_tables(dynamodb_tables, region)
-        load_dynamodb_tables(neo4j_session, ddb_table_data, region, current_aws_account_id, aws_update_tag)
-        load_dynamodb_gsi(neo4j_session, ddb_gsi_data, region, current_aws_account_id, aws_update_tag)
-    cleanup_dynamodb_tables(neo4j_session, common_job_parameters)
-
-
-@timeit
-def sync(
-    neo4j_session: neo4j.Session, boto3_session: boto3.session.Session, regions: List[str], current_aws_account_id: str,
-    update_tag: int, common_job_parameters: Dict,
-) -> None:
-    sync_dynamodb_tables(
-        neo4j_session, boto3_session, regions, current_aws_account_id, update_tag, common_job_parameters,
-    )
-    merge_module_sync_metadata(
-        neo4j_session,
-        group_type='AWSAccount',
-        group_id=current_aws_account_id,
-        synced_type='DynamoDBTable',
-        update_tag=update_tag,
-        stat_handler=stat_handler,
-    )
+        data = get_dynamodb_tables(boto3_session, region)
+        load_dynamodb_tables(session, data, region, current_aws_account_id, aws_update_tag)
+    cleanup_dynamodb_tables(session, common_job_parameters)
```

### Comparing `cartography-0.81.0/cartography/intel/aws/elasticsearch.py` & `cartography-0.9.0/cartography/intel/aws/elasticsearch.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,80 @@
 import json
 import logging
-from typing import Dict
-from typing import List
 
-import boto3
 import botocore.config
-import neo4j
 from policyuniverse.policy import Policy
 
 from cartography.intel.dns import ingest_dns_record_by_fqdn
-from cartography.util import aws_handle_regions
 from cartography.util import run_cleanup_job
-from cartography.util import timeit
 
 logger = logging.getLogger(__name__)
 
+# TODO get this programmatically
+# https://docs.aws.amazon.com/general/latest/gr/rande.html#elasticsearch-service-regions
+es_regions = [
+    'us-east-2',
+    'us-east-1',
+    'us-west-1',
+    'us-west-2',
+    'ap-northeast-1',
+    'ap-northeast-2',
+    'ap-south-1',
+    'ap-southeast-1',
+    'ca-central-1',
+    # 'cn-northwest-1',  -- intentionally ignored. need specific token
+    'eu-central-1',
+    'eu-west-1',
+    'eu-west-2',
+    'eu-west-3',
+    'sa-east-1',
+    # 'us-gov-west-1', -- intentionally ignored, need specific token
+]
+
 
 # TODO memoize this
-def _get_botocore_config() -> botocore.config.Config:
+def _get_botocore_config():
     return botocore.config.Config(
         retries={
             'max_attempts': 8,
         },
     )
 
 
-@timeit
-@aws_handle_regions
-def _get_es_domains(client: botocore.client.BaseClient) -> List[Dict]:
+def _get_es_domains(client):
     """
     Get ES domains.
 
     :param client: ES boto client
     :return: list of ES domains
     """
     data = client.list_domain_names()
     domain_names = [d['DomainName'] for d in data.get('DomainNames', [])]
     # NOTE describe_elasticsearch_domains takes at most 5 domain names
     domain_name_chunks = [domain_names[i:i + 5] for i in range(0, len(domain_names), 5)]
-    domains: List[Dict] = []
+    domains = []
     for domain_name_chunk in domain_name_chunks:
         chunk_data = client.describe_elasticsearch_domains(DomainNames=domain_name_chunk)
         domains.extend(chunk_data['DomainStatusList'])
     return domains
 
 
-@timeit
-def _load_es_domains(
-    neo4j_session: neo4j.Session, domain_list: List[Dict], aws_account_id: str, aws_update_tag: int,
-) -> None:
+def _load_es_domains(session, domain_list, aws_account_id, aws_update_tag):
     """
     Ingest Elastic Search domains
 
-    :param neo4j_session: Neo4j session object
+    :param session: Neo4j session object
     :param aws_account_id: The AWS account related to the domains
     :param domains: Domain list to ingest
     """
     ingest_records = """
-    UNWIND $Records as record
+    UNWIND {Records} as record
     MERGE (es:ESDomain{id: record.DomainId})
     ON CREATE SET es.firstseen = timestamp(), es.arn = record.ARN, es.domainid = record.DomainId
-    SET es.lastupdated = $aws_update_tag, es.deleted = record.Deleted, es.created = record.created,
+    SET es.lastupdated = {aws_update_tag}, es.deleted = record.Deleted, es.created = record.created,
     es.endpoint = record.Endpoint, es.elasticsearch_version = record.ElasticsearchVersion,
     es.elasticsearch_cluster_config_instancetype = record.ElasticsearchClusterConfig.InstanceType,
     es.elasticsearch_cluster_config_instancecount = record.ElasticsearchClusterConfig.InstanceCount,
     es.elasticsearch_cluster_config_dedicatedmasterenabled = record.ElasticsearchClusterConfig.DedicatedMasterEnabled,
     es.elasticsearch_cluster_config_zoneawarenessenabled = record.ElasticsearchClusterConfig.ZoneAwarenessEnabled,
     es.elasticsearch_cluster_config_dedicatedmastertype = record.ElasticsearchClusterConfig.DedicatedMasterType,
     es.elasticsearch_cluster_config_dedicatedmastercount = record.ElasticsearchClusterConfig.DedicatedMasterCount,
@@ -73,149 +83,136 @@
     es.ebs_options_volumesize = record.EBSOptions.VolumeSize,
     es.ebs_options_iops = record.EBSOptions.Iops,
     es.encryption_at_rest_options_enabled = record.EncryptionAtRestOptions.Enabled,
     es.encryption_at_rest_options_kms_key_id = record.EncryptionAtRestOptions.KmsKeyId,
     es.log_publishing_options_cloudwatch_log_group_arn = record.LogPublishingOptions.CloudWatchLogsLogGroupArn,
     es.log_publishing_options_enabled = record.LogPublishingOptions.Enabled
     WITH es
-    MATCH (account:AWSAccount{id: $AWS_ACCOUNT_ID})
+    MATCH (account:AWSAccount{id: {AWS_ACCOUNT_ID}})
     MERGE (account)-[r:RESOURCE]->(es)
     ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $aws_update_tag
+    SET r.lastupdated = {aws_update_tag}
     """
 
     # TODO this is a hacky workaround -- neo4j doesn't accept datetime objects and this section of the object
     # TODO contains one. we really shouldn't be sending the entire object to neo4j
     for d in domain_list:
         del d['ServiceSoftwareOptions']
 
-    neo4j_session.run(
+    session.run(
         ingest_records,
         Records=domain_list,
         AWS_ACCOUNT_ID=aws_account_id,
         aws_update_tag=aws_update_tag,
     )
 
     for domain in domain_list:
         domain_id = domain["DomainId"]
-        _link_es_domains_to_dns(neo4j_session, domain_id, domain, aws_update_tag)
-        _link_es_domain_vpc(neo4j_session, domain_id, domain, aws_update_tag)
-        _process_access_policy(neo4j_session, domain_id, domain)
+        _link_es_domains_to_dns(session, domain_id, domain, aws_update_tag)
+        _link_es_domain_vpc(session, domain_id, domain, aws_update_tag)
+        _process_access_policy(session, domain_id, domain)
 
 
-@timeit
-def _link_es_domains_to_dns(
-    neo4j_session: neo4j.Session, domain_id: str, domain_data: Dict, aws_update_tag: int,
-) -> None:
+def _link_es_domains_to_dns(session, domain_id, domain_data, aws_update_tag):
     """
     Link the ES domain to its DNS FQDN endpoint and create associated nodes in the graph
     if needed
 
-    :param neo4j_session: Neo4j session object
+    :param session: Neo4j session object
     :param domain_id: ES domain id
     :param domain_data: domain data
     """
     # TODO add support for endpoints to this method
     if domain_data.get("Endpoint"):
-        ingest_dns_record_by_fqdn(
-            neo4j_session, aws_update_tag, domain_data["Endpoint"], domain_id,
-            record_label="ESDomain", dns_node_additional_label="AWSDNSRecord",
-        )
+        ingest_dns_record_by_fqdn(session, aws_update_tag, domain_data["Endpoint"], domain_id)
     else:
         logger.debug(f"No es endpoint data for domain id {domain_id}")
 
 
-@timeit
-def _link_es_domain_vpc(neo4j_session: neo4j.Session, domain_id: str, domain_data: Dict, aws_update_tag: int) -> None:
+def _link_es_domain_vpc(session, domain_id, domain_data, aws_update_tag):
     """
     Link the ES domain to its DNS FQDN endpoint and create associated nodes in the graph
     if needed
 
-    :param neo4j_session: Neo4j session object
+    :param session: Neo4j session object
     :param domain_id: ES domain id
     :param domain_data: domain data
     """
     ingest_subnet = """
-    MATCH (es:ESDomain{id: $DomainId})
+    MATCH (es:ESDomain{id: {DomainId}})
     WITH es
-    UNWIND $SubnetList as subnet_id
+    UNWIND {SubnetList} as subnet_id
         MATCH (subnet_node:EC2Subnet{id: subnet_id})
         MERGE (es)-[r:PART_OF_SUBNET]->(subnet_node)
         ON CREATE SET r.firstseen = timestamp()
-        SET r.lastupdated = $aws_update_tag
+        SET r.lastupdated = {aws_update_tag}
     """
 
     ingest_sec_groups = """
-    MATCH (es:ESDomain{id: $DomainId})
+    MATCH (es:ESDomain{id: {DomainId}})
     WITH es
-    UNWIND $SecGroupList as ecsecgroup_id
+    UNWIND {SecGroupList} as ecsecgroup_id
         MATCH (group_node:EC2SecurityGroup{id: ecsecgroup_id})
         MERGE (es)-[r:MEMBER_OF_EC2_SECURITY_GROUP]->(group_node)
         ON CREATE SET r.firstseen = timestamp()
-        SET r.lastupdated = $aws_update_tag
+        SET r.lastupdated = {aws_update_tag}
     """
     # TODO we really shouldn't be sending full objects to Neo4j
     if domain_data.get("VPCOptions"):
         vpc_data = domain_data["VPCOptions"]
         subnetList = vpc_data.get("SubnetIds", [])
         groupList = vpc_data.get("SecurityGroupIds", [])
 
         if len(subnetList) > 0:
-            neo4j_session.run(
+            session.run(
                 ingest_subnet,
                 DomainId=domain_id,
                 SubnetList=subnetList,
                 aws_update_tag=aws_update_tag,
             )
 
         if len(groupList) > 0:
-            neo4j_session.run(
+            session.run(
                 ingest_sec_groups,
                 DomainId=domain_id,
                 SecGroupList=groupList,
                 aws_update_tag=aws_update_tag,
             )
 
 
-@timeit
-def _process_access_policy(neo4j_session: neo4j.Session, domain_id: str, domain_data: Dict) -> None:
+def _process_access_policy(session, domain_id, domain_data):
     """
     Link the ES domain to its DNS FQDN endpoint and create associated nodes in the graph
     if needed
 
-    :param neo4j_session: Neo4j session object
+    :param session: Neo4j session object
     :param domain_id: ES domain id
     :param domain_data: domain data
     """
-    tag_es = "MATCH (es:ESDomain{id: $DomainId}) SET es.exposed_internet = $InternetExposed"
+    tag_es = "MATCH (es:ESDomain{id: {DomainId}}) SET es.exposed_internet = {InternetExposed}"
 
     exposed_internet = False
 
     if domain_data.get("Endpoint") and domain_data.get("AccessPolicies"):
         policy = Policy(json.loads(domain_data['AccessPolicies']))
         if policy.is_internet_accessible():
             exposed_internet = True
 
-    neo4j_session.run(tag_es, DomainId=domain_id, InternetExposed=exposed_internet)
+    session.run(tag_es, DomainId=domain_id, InternetExposed=exposed_internet)
 
 
-@timeit
-def cleanup(neo4j_session: neo4j.Session, update_tag: int, aws_account_id: int) -> None:
+def cleanup(session, update_tag, aws_account_id):
     run_cleanup_job(
         'aws_import_es_cleanup.json',
-        neo4j_session,
+        session,
         {'UPDATE_TAG': update_tag, 'AWS_ID': aws_account_id},
     )
 
 
-@timeit
-def sync(
-    neo4j_session: neo4j.Session, boto3_session: boto3.session.Session, regions: List[str], current_aws_account_id: str,
-    update_tag: int, common_job_parameters: Dict,
-) -> None:
-    for region in regions:
-        logger.info("Syncing Elasticsearch Service for region '%s' in account '%s'.", region, current_aws_account_id)
+def sync(neo4j_session, boto3_session, aws_account_id, update_tag):
+    for region in es_regions:
+        logger.info("Syncing Elasticsearch Service for region '%s' in account '%s'.", region, aws_account_id)
         client = boto3_session.client('es', region_name=region, config=_get_botocore_config())
         data = _get_es_domains(client)
-        _load_es_domains(neo4j_session, data, current_aws_account_id, update_tag)
+        _load_es_domains(neo4j_session, data, aws_account_id, update_tag)
 
-    cleanup(neo4j_session, update_tag, current_aws_account_id)  # type: ignore
+    cleanup(neo4j_session, update_tag, aws_account_id)
```

### Comparing `cartography-0.81.0/cartography/intel/aws/organizations.py` & `cartography-0.9.0/cartography/intel/aws/organizations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,69 @@
 import logging
-from typing import Dict
 
 import boto3
 import botocore.exceptions
-import neo4j
 
-from cartography.util import timeit
+from cartography.util import run_cleanup_job
 
 logger = logging.getLogger(__name__)
 
 
-def get_account_from_arn(arn: str) -> str:
+def get_account_from_arn(arn):
     # TODO use policyuniverse to parse ARN?
     return arn.split(":")[4]
 
 
-def get_caller_identity(boto3_session: boto3.session.Session) -> Dict:
-    client = boto3_session.client('sts')
+def get_caller_identity(session):
+    client = session.client('sts')
     return client.get_caller_identity()
 
 
-def get_current_aws_account_id(boto3_session: boto3.session.Session) -> Dict:
-    return get_caller_identity(boto3_session)['Account']
+def get_current_aws_account_id(session):
+    return get_caller_identity(session)['Account']
 
 
-def get_aws_account_default(boto3_session: boto3.session.Session) -> Dict:
+def get_aws_account_default(session):
     try:
-        return {boto3_session.profile_name: get_current_aws_account_id(boto3_session)}
+        return {"default": get_current_aws_account_id(session)}
     except (botocore.exceptions.BotoCoreError, botocore.exceptions.ClientError) as e:
         logger.debug("Error occurred getting default AWS account number.", exc_info=True)
         logger.error(
             (
                 "Unable to get AWS account number, an error occurred: '%s'. Make sure your AWS credentials are "
                 "configured correctly, your AWS config file is valid, and your credentials have the SecurityAudit "
                 "policy attached."
             ),
             e,
         )
         return {}
 
 
-def get_aws_accounts_from_botocore_config(boto3_session: boto3.session.Session) -> Dict:
+def get_aws_accounts_from_botocore_config(session):
     d = {}
-    for profile_name in boto3_session.available_profiles:
+    for profile_name in session.available_profiles:
         if profile_name == 'default':
             logger.debug("Skipping AWS profile 'default'.")
             continue
         try:
-            profile_boto3_session = boto3.Session(profile_name=profile_name)
+            boto3_session = boto3.Session(profile_name=profile_name)
         except (botocore.exceptions.BotoCoreError, botocore.exceptions.ClientError) as e:
             logger.debug("Error occurred calling boto3.Session() with profile_name '%s'.", profile_name, exc_info=True)
             logger.error(
                 (
                     "Unable to initialize an AWS session using profile '%s', an error occurred: '%s'. Make sure your "
                     "AWS credentials are configured correctly, your AWS config file is valid, and your credentials "
                     "have the SecurityAudit policy attached."
                 ),
                 profile_name,
                 e,
             )
             continue
         try:
-            d[profile_name] = get_current_aws_account_id(profile_boto3_session)
+            d[profile_name] = get_current_aws_account_id(boto3_session)
         except (botocore.exceptions.BotoCoreError, botocore.exceptions.ClientError) as e:
             logger.debug(
                 "Error occurred getting AWS account number with profile_name '%s'.",
                 profile_name,
                 exc_info=True,
             )
             logger.error(
@@ -82,39 +80,39 @@
             "Discovered AWS account '%s' associated with configured profile '%s'.",
             d[profile_name],
             profile_name,
         )
     return d
 
 
-def load_aws_accounts(
-    neo4j_session: neo4j.Session, aws_accounts: Dict, aws_update_tag: int,
-    common_job_parameters: Dict,
-) -> None:
+def load_aws_accounts(neo4j_session, aws_accounts, aws_update_tag, common_job_parameters):
     query = """
-    MERGE (aa:AWSAccount{id: $ACCOUNT_ID})
+    MERGE (aa:AWSAccount{id: {ACCOUNT_ID}})
     ON CREATE SET aa.firstseen = timestamp()
-    SET aa.lastupdated = $aws_update_tag, aa.name = $ACCOUNT_NAME, aa.inscope=true
-    REMOVE aa.foreign
+    SET aa.lastupdated = {aws_update_tag}, aa.name = {ACCOUNT_NAME}
     WITH aa
-    MERGE (root:AWSPrincipal{arn: $RootArn})
+    MERGE (root:AWSPrincipal{arn: {RootArn}})
     ON CREATE SET root.firstseen = timestamp(), root.type = 'AWS'
-    SET root.lastupdated = $aws_update_tag
+    SET root.lastupdated = {aws_update_tag}
     WITH aa, root
     MERGE (aa)-[r:RESOURCE]->(root)
     ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $aws_update_tag;
+    SET r.lastupdated = {aws_update_tag};
     """
     for account_name, account_id in aws_accounts.items():
         root_arn = f'arn:aws:iam::{account_id}:root'
         neo4j_session.run(
             query,
             ACCOUNT_ID=account_id,
             ACCOUNT_NAME=account_name,
             RootArn=root_arn,
             aws_update_tag=aws_update_tag,
         )
 
 
-@timeit
-def sync(neo4j_session: neo4j.Session, accounts: Dict, update_tag: int, common_job_parameters: Dict) -> None:
-    load_aws_accounts(neo4j_session, accounts, update_tag, common_job_parameters)
+def cleanup(neo4j_session, common_job_parameters):
+    run_cleanup_job('aws_account_cleanup.json', neo4j_session, common_job_parameters)
+
+
+def sync(neo4j_session, accounts, aws_update_tag, common_job_parameters):
+    load_aws_accounts(neo4j_session, accounts, aws_update_tag, common_job_parameters)
+    cleanup(neo4j_session, common_job_parameters)
```

### Comparing `cartography-0.81.0/cartography/intel/gcp/__init__.py` & `cartography-0.9.0/cartography/intel/gcp/crm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,268 +1,247 @@
-import json
+# Google Compute Resource Manager
+# https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy
 import logging
-from collections import namedtuple
-from typing import Dict
-from typing import List
-from typing import Set
-
-import googleapiclient.discovery
-import neo4j
-from googleapiclient.discovery import Resource
-from oauth2client.client import ApplicationDefaultCredentialsError
-from oauth2client.client import GoogleCredentials
-
-from cartography.config import Config
-from cartography.intel.gcp import compute
-from cartography.intel.gcp import crm
-from cartography.intel.gcp import dns
-from cartography.intel.gcp import gke
-from cartography.intel.gcp import storage
-from cartography.util import run_analysis_job
-from cartography.util import timeit
 
-logger = logging.getLogger(__name__)
-Resources = namedtuple('Resources', 'compute container crm_v1 crm_v2 dns storage serviceusage')
+from googleapiclient.discovery import HttpError
+
+from cartography.util import run_cleanup_job
 
-# Mapping of service short names to their full names as in docs. See https://developers.google.com/apis-explorer,
-# and https://cloud.google.com/service-usage/docs/reference/rest/v1/services#ServiceConfig
-Services = namedtuple('Services', 'compute storage gke dns')
-service_names = Services(
-    compute='compute.googleapis.com',
-    storage='storage.googleapis.com',
-    gke='container.googleapis.com',
-    dns='dns.googleapis.com',
-)
+logger = logging.getLogger(__name__)
 
 
-def _get_crm_resource_v1(credentials: GoogleCredentials) -> Resource:
+def get_gcp_organizations(crm_v1):
     """
-    Instantiates a Google Compute Resource Manager v1 resource object to call the Resource Manager API.
-    See https://cloud.google.com/resource-manager/reference/rest/.
-    :param credentials: The GoogleCredentials object
-    :return: A CRM v1 resource object
+    Return list of GCP organizations that the crm_v1 resource object has permissions to access.
+    Returns empty list if we are unable to enumerate organizations for any reason.
+    :param crm_v1: The Compute Resource Manager v1 resource object created by `googleapiclient.discovery.build()`.
+    See https://googleapis.github.io/google-api-python-client/docs/epy/googleapiclient.discovery-module.html#build.
+    :return: List of GCP Organizations. See https://cloud.google.com/resource-manager/reference/rest/v1/organizations.
     """
-    # cache_discovery=False to suppress extra warnings.
-    # See https://github.com/googleapis/google-api-python-client/issues/299#issuecomment-268915510 and related issues
-    return googleapiclient.discovery.build('cloudresourcemanager', 'v1', credentials=credentials, cache_discovery=False)
+    try:
+        req = crm_v1.organizations().search(body={})
+        res = req.execute()
+        return res.get('organizations', [])
+    except HttpError as e:
+        logger.warning("HttpError occurred in crm.get_gcp_organizations(), returning empty list. Details: %r", e)
+        return []
 
 
-def _get_crm_resource_v2(credentials: GoogleCredentials) -> Resource:
-    """
-    Instantiates a Google Compute Resource Manager v2 resource object to call the Resource Manager API.
-    We need a v2 resource object to query for GCP folders.
-    :param credentials: The GoogleCredentials object
-    :return: A CRM v2 resource object
+def get_gcp_folders(crm_v2):
+    """
+    Return list of GCP folders that the crm_v2 resource object has permissions to access.
+    Returns empty list if we are unable to enumerate folders for any reason.
+    :param crm_v2: The Compute Resource Manager v2 resource object created by `googleapiclient.discovery.build()`.
+    See https://googleapis.github.io/google-api-python-client/docs/epy/googleapiclient.discovery-module.html#build.
+    :return: List of GCP folders. See https://cloud.google.com/resource-manager/reference/rest/v2/folders/list.
     """
-    return googleapiclient.discovery.build('cloudresourcemanager', 'v2', credentials=credentials, cache_discovery=False)
+    try:
+        req = crm_v2.folders().search(body={})
+        res = req.execute()
+        return res.get('folders', [])
+    except HttpError as e:
+        logger.warning("HttpError occurred in crm.get_gcp_folders(), returning empty list. Details: %r", e)
+        return []
 
 
-def _get_compute_resource(credentials: GoogleCredentials) -> Resource:
-    """
-    Instantiates a Google Compute resource object to call the Compute API. This is used to pull zone, instance, and
-    networking data. See https://cloud.google.com/compute/docs/reference/rest/v1/.
-    :param credentials: The GoogleCredentials object
-    :return: A Compute resource object
+def get_gcp_projects(crm_v1):
+    """
+    Return list of GCP projects that the crm_v1 resource object has permissions to access.
+    Returns empty list if we are unable to enumerate projects for any reason.
+    :param crm_v1: The Compute Resource Manager v1 resource object created by `googleapiclient.discovery.build()`.
+    See https://googleapis.github.io/google-api-python-client/docs/epy/googleapiclient.discovery-module.html#build.
+    :return: List of GCP projects. See https://cloud.google.com/resource-manager/reference/rest/v2/projects/list.
     """
-    return googleapiclient.discovery.build('compute', 'v1', credentials=credentials, cache_discovery=False)
+    try:
+        req = crm_v1.projects().list()
+        res = req.execute()
+        return res.get('projects', [])
+    except HttpError as e:
+        logger.warning("HttpError occurred in crm.get_gcp_projects(), returning empty list. Details: %r", e)
+        return []
 
 
-def _get_storage_resource(credentials: GoogleCredentials) -> Resource:
+def load_gcp_organizations(neo4j_session, data, gcp_update_tag):
     """
-    Instantiates a Google Cloud Storage resource object to call the Storage API.
-    This is used to pull bucket metadata and IAM Policies
-    as well as list buckets in a specified project.
-    See https://cloud.google.com/storage/docs/json_api/.
-    :param credentials: The GoogleCredentials object
-    :return: A Storage resource object
+    Ingest the GCP organizations to Neo4j
+    :param neo4j_session: The Neo4j session
+    :param data: List of organizations; output from crm.get_gcp_organizations()
+    :param gcp_update_tag: The timestamp value to set our new Neo4j nodes with
+    :return: Nothing
     """
-    return googleapiclient.discovery.build('storage', 'v1', credentials=credentials, cache_discovery=False)
+    query = """
+    MERGE (org:GCPOrganization{id:{OrgName}})
+    ON CREATE SET org.firstseen = timestamp()
+    SET org.orgname = {OrgName},
+    org.displayname = {DisplayName},
+    org.lifecyclestate = {LifecycleState},
+    org.lastupdated = {gcp_update_tag}
+    """
+    for org_object in data:
+        neo4j_session.run(
+            query,
+            OrgName=org_object['name'],
+            DisplayName=org_object.get('displayName', None),
+            LifecycleState=org_object.get('lifecycleState', None),
+            gcp_update_tag=gcp_update_tag,
+        )
 
 
-def _get_container_resource(credentials: GoogleCredentials) -> Resource:
+def load_gcp_folders(neo4j_session, data, gcp_update_tag):
     """
-    Instantiates a Google Cloud Container resource object to call the
-    Container API. See: https://cloud.google.com/kubernetes-engine/docs/reference/rest/v1/.
-
-    :param credentials: The GoogleCredentials object
-    :return: A Container resource object
+    Ingest the GCP folders to Neo4j
+    :param neo4j_session: The Neo4j session
+    :param data: List of folders; output from crm.get_gcp_folders()
+    :param gcp_update_tag: The timestamp value to set our new Neo4j nodes with
+    :return: Nothing
     """
-    return googleapiclient.discovery.build('container', 'v1', credentials=credentials, cache_discovery=False)
+    for folder in data:
+        # Get the correct parent type.
+        # Parents of folders can only be GCPOrganizations or other folders, see
+        # https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy
+        if folder['parent'].startswith("organizations"):
+            query = "MATCH (parent:GCPOrganization{id:{ParentId}})"
+        elif folder['parent'].startswith("folders"):
+            query = """
+            MERGE (parent:GCPFolder{id:{ParentId}})
+            ON CREATE SET parent.firstseen = timestamp()
+            """
+        query += """
+        MERGE (folder:GCPFolder{id:{FolderName}})
+        ON CREATE SET folder.firstseen = timestamp()
+        SET folder.foldername = {FolderName},
+        folder.displayname = {DisplayName},
+        folder.lifecyclestate = {LifecycleState},
+        folder.lastupdated = {gcp_update_tag}
+        WITH parent, folder
+        MERGE (parent)-[r:RESOURCE]->(folder)
+        ON CREATE SET r.firstseen = timestamp()
+        SET r.lastupdated = {gcp_update_tag}
+        """
+        neo4j_session.run(
+            query,
+            ParentId=folder['parent'],
+            FolderName=folder['name'],
+            DisplayName=folder.get('displayName', None),
+            LifecycleState=folder.get('lifecycleState', None),
+            gcp_update_tag=gcp_update_tag,
+        )
 
 
-def _get_dns_resource(credentials: GoogleCredentials) -> Resource:
+def load_gcp_projects(neo4j_session, data, gcp_update_tag):
     """
-    Instantiates a Google Cloud DNS resource object to call the
-    Container API. See: https://cloud.google.com/dns/docs/reference/v1/.
-
-    :param credentials: The GoogleCredentials object
-    :return: A DNS resource object
+    Ingest the GCP projects to Neo4j
+    :param neo4j_session: The Neo4j session
+    :param data: List of GCP projects; output from crm.get_gcp_projects()
+    :param gcp_update_tag: The timestamp value to set our new Neo4j nodes with
+    :return: Nothing
     """
-    return googleapiclient.discovery.build('dns', 'v1', credentials=credentials, cache_discovery=False)
+    for project in data:
+        if project.get('parent', None):
+            if project['parent']['type'] == "organization":
+                query = """
+                MERGE (parent:GCPOrganization{id:{ParentId}})
+                ON CREATE SET parent.firstseen = timestamp()
+                """
+                parentid = f"organizations/{project['parent']['id']}"
+            elif project['parent']['type'] == "folder":
+                query = """
+                MERGE (parent:GCPFolder{id:{ParentId}})
+                ON CREATE SET parent.firstseen = timestamp()
+                """
+                parentid = f"folders/{project['parent']['id']}"
+        query += """
+        MERGE (project:GCPProject{id:{ProjectId}})
+        ON CREATE SET project.firstseen = timestamp()
+        SET project.projectid = {ProjectId},
+        project.displayname = {DisplayName},
+        project.lifecyclestate = {LifecycleState},
+        project.lastupdated = {gcp_update_tag}
+        WITH parent, project
+        MERGE (parent)-[r:RESOURCE]->(project)
+        ON CREATE SET r.firstseen = timestamp()
+        SET r.lastupdated = {gcp_update_tag}
+        """
+        neo4j_session.run(
+            query,
+            ParentId=parentid,
+            ProjectId=project['projectId'],
+            DisplayName=project.get('name', None),
+            LifecycleState=project.get('lifecycleState', None),
+            gcp_update_tag=gcp_update_tag,
+        )
 
 
-def _get_serviceusage_resource(credentials: GoogleCredentials) -> Resource:
+def cleanup_gcp_organizations(session, common_job_parameters):
     """
-    Instantiates a serviceusage resource object.
-    See: https://cloud.google.com/service-usage/docs/reference/rest/v1/operations/list.
-
-    :param credentials: The GoogleCredentials object
-    :return: A serviceusage resource object
+    Remove stale GCP organizations and their relationships
+    :param session: The Neo4j session
+    :param common_job_parameters: Parameters to carry to the cleanup job
+    :return: Nothing
     """
-    return googleapiclient.discovery.build('serviceusage', 'v1', credentials=credentials, cache_discovery=False)
+    run_cleanup_job('gcp_crm_organization_cleanup.json', session, common_job_parameters)
 
 
-def _initialize_resources(credentials: GoogleCredentials) -> Resource:
+def cleanup_gcp_folders(session, common_job_parameters):
     """
-    Create namedtuple of all resource objects necessary for GCP data gathering.
-    :param credentials: The GoogleCredentials object
-    :return: namedtuple of all resource objects
+    Remove stale GCP folders and their relationships
+    :param session: The Neo4j session
+    :param common_job_parameters: Parameters to carry to the cleanup job
+    :return: Nothing
     """
-    return Resources(
-        crm_v1=_get_crm_resource_v1(credentials),
-        crm_v2=_get_crm_resource_v2(credentials),
-        compute=_get_compute_resource(credentials),
-        storage=_get_storage_resource(credentials),
-        container=_get_container_resource(credentials),
-        serviceusage=_get_serviceusage_resource(credentials),
-        dns=_get_dns_resource(credentials),
-    )
+    run_cleanup_job('gcp_crm_folder_cleanup.json', session, common_job_parameters)
 
 
-def _services_enabled_on_project(serviceusage: Resource, project_id: str) -> Set:
+def cleanup_gcp_projects(session, common_job_parameters):
     """
-    Return a list of all Google API services that are enabled on the given project ID.
-    See https://cloud.google.com/service-usage/docs/reference/rest/v1/services/list for data shape.
-    :param serviceusage: the serviceusage resource provider. See https://cloud.google.com/service-usage/docs/overview.
-    :param project_id: The project ID number to sync.  See  the `projectId` field in
-    https://cloud.google.com/resource-manager/reference/rest/v1/projects
-    :return: A set of services that are enabled on the project
+    Remove stale GCP projects and their relationships
+    :param session: The Neo4j session
+    :param common_job_parameters: Parameters to carry to the cleanup job
+    :return: Nothing
     """
-    try:
-        req = serviceusage.services().list(parent=f'projects/{project_id}', filter='state:ENABLED')
-        res = req.execute()
-        if 'services' in res:
-            return {svc['config']['name'] for svc in res['services']}
-        else:
-            return set()
-    except googleapiclient.discovery.HttpError as http_error:
-        http_error = json.loads(http_error.content.decode('utf-8'))
-        # This is set to log-level `info` because Google creates many projects under the hood that cartography cannot
-        # audit (e.g. adding a script to a Google spreadsheet causes a project to get created) and we don't need to emit
-        # a warning for these projects.
-        logger.info(
-            f"HttpError when trying to get enabled services on project {project_id}. "
-            f"Code: {http_error['error']['code']}, Message: {http_error['error']['message']}. "
-            f"Skipping.",
-        )
-        return set()
+    run_cleanup_job('gcp_crm_project_cleanup.json', session, common_job_parameters)
 
 
-def _sync_single_project(
-    neo4j_session: neo4j.Session, resources: Resource, project_id: str, gcp_update_tag: int,
-    common_job_parameters: Dict,
-) -> None:
+def sync_gcp_organizations(session, crm_v1, gcp_update_tag, common_job_parameters):
     """
-    Handles graph sync for a single GCP project.
-    :param neo4j_session: The Neo4j session
-    :param resources: namedtuple of the GCP resource objects
-    :param project_id: The project ID number to sync.  See  the `projectId` field in
-    https://cloud.google.com/resource-manager/reference/rest/v1/projects
+    Get GCP organization data using the CRM v1 resource object, load the data to Neo4j, and clean up stale nodes.
+    :param session: The Neo4j session
+    :param crm_v1: The Compute Resource Manager v1 resource object created by `googleapiclient.discovery.build()`.
+    See https://googleapis.github.io/google-api-python-client/docs/epy/googleapiclient.discovery-module.html#build.
     :param gcp_update_tag: The timestamp value to set our new Neo4j nodes with
-    :param common_job_parameters: Other parameters sent to Neo4j
+    :param common_job_parameters: Parameters to carry to the Neo4j jobs
     :return: Nothing
     """
-    # Determine the resources available on the project.
-    enabled_services = _services_enabled_on_project(resources.serviceusage, project_id)
-    if service_names.compute in enabled_services:
-        compute.sync(neo4j_session, resources.compute, project_id, gcp_update_tag, common_job_parameters)
-    if service_names.storage in enabled_services:
-        storage.sync_gcp_buckets(neo4j_session, resources.storage, project_id, gcp_update_tag, common_job_parameters)
-    if service_names.gke in enabled_services:
-        gke.sync_gke_clusters(neo4j_session, resources.container, project_id, gcp_update_tag, common_job_parameters)
-    if service_names.dns in enabled_services:
-        dns.sync(neo4j_session, resources.dns, project_id, gcp_update_tag, common_job_parameters)
-
-
-def _sync_multiple_projects(
-    neo4j_session: neo4j.Session, resources: Resource, projects: List[Dict],
-    gcp_update_tag: int, common_job_parameters: Dict,
-) -> None:
-    """
-    Handles graph sync for multiple GCP projects.
-    :param neo4j_session: The Neo4j session
-    :param resources: namedtuple of the GCP resource objects
-    :param: projects: A list of projects. At minimum, this list should contain a list of dicts with the key "projectId"
-     defined; so it would look like this: [{"projectId": "my-project-id-12345"}].
-    This is the returned data from `crm.get_gcp_projects()`.
-    See https://cloud.google.com/resource-manager/reference/rest/v1/projects.
+    logger.debug("Syncing GCP organizations")
+    data = get_gcp_organizations(crm_v1)
+    load_gcp_organizations(session, data, gcp_update_tag)
+    cleanup_gcp_organizations(session, common_job_parameters)
+
+
+def sync_gcp_folders(session, crm_v2, gcp_update_tag, common_job_parameters):
+    """
+    Get GCP folder data using the CRM v2 resource object, load the data to Neo4j, and clean up stale nodes.
+    :param session: The Neo4j session
+    :param crm_v2: The Compute Resource Manager v2 resource object created by `googleapiclient.discovery.build()`.
+    See https://googleapis.github.io/google-api-python-client/docs/epy/googleapiclient.discovery-module.html#build.
     :param gcp_update_tag: The timestamp value to set our new Neo4j nodes with
-    :param common_job_parameters: Other parameters sent to Neo4j
+    :param common_job_parameters: Parameters to carry to the Neo4j jobs
     :return: Nothing
     """
-    logger.info("Syncing %d GCP projects.", len(projects))
-    crm.sync_gcp_projects(neo4j_session, projects, gcp_update_tag, common_job_parameters)
-
-    for project in projects:
-        project_id = project['projectId']
-        logger.info("Syncing GCP project %s.", project_id)
-        _sync_single_project(neo4j_session, resources, project_id, gcp_update_tag, common_job_parameters)
+    logger.debug("Syncing GCP folders")
+    folders = get_gcp_folders(crm_v2)
+    load_gcp_folders(session, folders, gcp_update_tag)
+    cleanup_gcp_folders(session, common_job_parameters)
 
 
-@timeit
-def start_gcp_ingestion(neo4j_session: neo4j.Session, config: Config) -> None:
+def sync_gcp_projects(session, projects, gcp_update_tag, common_job_parameters):
     """
-    Starts the GCP ingestion process by initializing Google Application Default Credentials, creating the necessary
-    resource objects, listing all GCP organizations and projects available to the GCP identity, and supplying that
-    context to all intel modules.
-    :param neo4j_session: The Neo4j session
-    :param config: A `cartography.config` object
+    Load a given list of GCP project data to Neo4j and clean up stale nodes.
+    :param session: The Neo4j session
+    :param projects: List of GCP projects; output from crm.get_gcp_projects()
+    :param gcp_update_tag: The timestamp value to set our new Neo4j nodes with
+    :param common_job_parameters: Parameters to carry to the Neo4j jobs
     :return: Nothing
     """
-    common_job_parameters = {
-        "UPDATE_TAG": config.update_tag,
-    }
-    try:
-        # Explicitly use Application Default Credentials.
-        # See https://oauth2client.readthedocs.io/en/latest/source/
-        #             oauth2client.client.html#oauth2client.client.OAuth2Credentials
-        credentials = GoogleCredentials.get_application_default()
-    except ApplicationDefaultCredentialsError as e:
-        logger.debug("Error occurred calling GoogleCredentials.get_application_default().", exc_info=True)
-        logger.error(
-            (
-                "Unable to initialize Google Compute Platform creds. If you don't have GCP data or don't want to load "
-                "GCP data then you can ignore this message. Otherwise, the error code is: %s "
-                "Make sure your GCP credentials are configured correctly, your credentials file (if any) is valid, and "
-                "that the identity you are authenticating to has the securityReviewer role attached."
-            ),
-            e,
-        )
-        return
-
-    resources = _initialize_resources(credentials)
-
-    # If we don't have perms to pull Orgs or Folders from GCP, we will skip safely
-    crm.sync_gcp_organizations(neo4j_session, resources.crm_v1, config.update_tag, common_job_parameters)
-    crm.sync_gcp_folders(neo4j_session, resources.crm_v2, config.update_tag, common_job_parameters)
-
-    projects = crm.get_gcp_projects(resources.crm_v1)
-
-    _sync_multiple_projects(neo4j_session, resources, projects, config.update_tag, common_job_parameters)
-
-    run_analysis_job(
-        'gcp_compute_asset_inet_exposure.json',
-        neo4j_session,
-        common_job_parameters,
-    )
-
-    run_analysis_job(
-        'gcp_gke_asset_exposure.json',
-        neo4j_session,
-        common_job_parameters,
-    )
-
-    run_analysis_job(
-        'gcp_gke_basic_auth.json',
-        neo4j_session,
-        common_job_parameters,
-    )
+    logger.debug("Syncing GCP projects")
+    load_gcp_projects(session, projects, gcp_update_tag)
+    cleanup_gcp_projects(session, common_job_parameters)
```

### Comparing `cartography-0.81.0/cartography/intel/gcp/compute.py` & `cartography-0.9.0/cartography/intel/gcp/compute.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 # Google Compute Engine API-centric functions
 # https://cloud.google.com/compute/docs/concepts
 import json
 import logging
 from collections import namedtuple
-from string import Template
-from typing import Any
-from typing import Dict
-from typing import List
-from typing import Optional
-from typing import Set
 
-import neo4j
 from googleapiclient.discovery import HttpError
-from googleapiclient.discovery import Resource
 
 from cartography.util import run_cleanup_job
-from cartography.util import timeit
 
 logger = logging.getLogger(__name__)
 InstanceUriPrefix = namedtuple('InstanceUriPrefix', 'zone_name project_id')
 
 
-def _get_error_reason(http_error: HttpError) -> str:
+def _get_error_reason(http_error):
     """
     Helper function to get an error reason out of the googleapiclient's HttpError object
     This function copies the structure of
     https://github.com/googleapis/google-api-python-client/blob/1d2e240a74d2bc0074dffbc57cf7d62b8146cb82/
                                   googleapiclient/http.py#L111
     At the moment this is the best way we know of to extract the HTTP failure reason.
     Additionally, see https://github.com/googleapis/google-api-python-client/issues/662.
@@ -35,21 +26,19 @@
     try:
         data = json.loads(http_error.content.decode('utf-8'))
         if isinstance(data, dict):
             reason = data['error']['errors'][0]['reason']
         else:
             reason = data[0]['error']['errors']['reason']
     except (UnicodeDecodeError, ValueError, KeyError):
-        logger.warning(f"HttpError: {data}")
         return ''
     return reason
 
 
-@timeit
-def get_zones_in_project(project_id: str, compute: Resource, max_results: Optional[int] = None) -> Optional[List[Dict]]:
+def get_zones_in_project(project_id, compute, max_results=None):
     """
     Return the zones where the Compute Engine API is enabled for the given project_id.
     See https://cloud.google.com/compute/docs/reference/rest/v1/zones and
     https://cloud.google.com/compute/docs/reference/rest/v1/zones/list.
     If the API is not enabled or if the project returns a 404-not-found, return None.
     :param project_id: The project ID number to sync.  See  the `projectId` field in
     https://cloud.google.com/resource-manager/reference/rest/v1/projects
@@ -60,131 +49,91 @@
     try:
         req = compute.zones().list(project=project_id, maxResults=max_results)
         res = req.execute()
         return res['items']
     except HttpError as e:
         reason = _get_error_reason(e)
         if reason == 'accessNotConfigured':
-            logger.info(
+            logger.debug(
                 (
-                    "Google Compute Engine API access is not configured for project %s; skipping. "
+                    "Google Compute Engine API access is not configured for project %s. "
                     "Full details: %s"
                 ),
                 project_id,
                 e,
             )
             return None
         elif reason == 'notFound':
-            logger.info(
+            logger.debug(
                 (
                     "Project %s returned a 404 not found error. "
                     "Full details: %s"
                 ),
                 project_id,
                 e,
             )
             return None
-        elif reason == 'forbidden':
-            logger.info(
-                (
-                    "Your GCP identity does not have the compute.zones.list permission for project %s; skipping "
-                    "compute sync for this project. Full details: %s"
-                ),
-                project_id,
-                e,
-            )
-            return None
         else:
             raise
 
 
-@timeit
-def get_gcp_instance_responses(project_id: str, zones: Optional[List[Dict]], compute: Resource) -> List[Resource]:
+def get_gcp_instance_responses(project_id, zones, compute):
     """
     Return list of GCP instance response objects for a given project and list of zones
     :param project_id: The project ID
     :param zones: The list of zones to query for instances
     :param compute: The compute resource object
     :return: A list of response objects of the form {id: str, items: []} where each item in `items` is a GCP instance
     """
     if not zones:
         # If the Compute Engine API is not enabled for a project, there are no zones and therefore no instances.
         return []
-    response_objects: List[Resource] = []
+    response_objects = []
     for zone in zones:
         req = compute.instances().list(project=project_id, zone=zone['name'])
         res = req.execute()
         response_objects.append(res)
     return response_objects
 
 
-@timeit
-def get_gcp_subnets(projectid: str, region: str, compute: Resource) -> Resource:
+def get_gcp_subnets(projectid, region, compute):
     """
     Return list of all subnets in the given projectid and region
     :param projectid: THe projectid
     :param region: The region to pull subnets from
     :param compute: The compute resource object created by googleapiclient.discovery.build()
     :return: Response object containing data on all GCP subnets for a given project
     """
     req = compute.subnetworks().list(project=projectid, region=region)
     return req.execute()
 
 
-@timeit
-def get_gcp_vpcs(projectid: str, compute: Resource) -> Resource:
+def get_gcp_vpcs(projectid, compute):
     """
     Get VPC data for given project
     :param projectid: The project ID
     :param compute: The compute resource object created by googleapiclient.discovery.build()
     :return: VPC response object
     """
     req = compute.networks().list(project=projectid)
     return req.execute()
 
 
-@timeit
-def get_gcp_regional_forwarding_rules(project_id: str, region: str, compute: Resource) -> Resource:
-    """
-    Return list of all regional forwarding rules in the given project_id and region
-    :param project_id: The project ID
-    :param region: The region to pull forwarding rules from
-    :param compute: The compute resource object created by googleapiclient.discovery.build()
-    :return: Response object containing data on all GCP forwarding rules for a given project
-    """
-    req = compute.forwardingRules().list(project=project_id, region=region)
-    return req.execute()
-
-
-@timeit
-def get_gcp_global_forwarding_rules(project_id: str, compute: Resource) -> Resource:
-    """
-    Return list of all global forwarding rules in the given project_id and region
-    :param project_id: The project ID
-    :param compute: The compute resource object created by googleapiclient.discovery.build()
-    :return: Response object containing data on all GCP forwarding rules for a given project
-    """
-    req = compute.globalForwardingRules().list(project=project_id)
-    return req.execute()
-
-
-@timeit
-def get_gcp_firewall_ingress_rules(project_id: str, compute: Resource) -> Resource:
+def get_gcp_firewall_ingress_rules(project_id, compute):
     """
     Get ingress Firewall data for a given project
     :param project_id: The project ID to get firewalls for
     :param compute: The compute resource object created by googleapiclient.discovery.build()
     :return: Firewall response object
     """
     req = compute.firewalls().list(project=project_id, filter='(direction="INGRESS")')
     return req.execute()
 
 
-@timeit
-def transform_gcp_instances(response_objects: List[Dict]) -> List[Dict]:
+def transform_gcp_instances(response_objects):
     """
     Process the GCP instance response objects and return a flattened list of GCP instances with all the necessary fields
     we need to load it into Neo4j
     :param response_objects: The return data from get_gcp_instance_responses()
     :return: A list of GCP instances
     """
     instance_list = []
@@ -201,52 +150,51 @@
                 nic['subnet_partial_uri'] = _parse_compute_full_uri_to_partial_uri(nic['subnetwork'])
                 nic['vpc_partial_uri'] = _parse_compute_full_uri_to_partial_uri(nic['network'])
 
             instance_list.append(instance)
     return instance_list
 
 
-def _parse_instance_uri_prefix(prefix: str) -> InstanceUriPrefix:
+def _parse_instance_uri_prefix(prefix):
     """
     Helper function to parse a GCP prefix string of the form `projects/{project}/zones/{zone}/instances`
     :param prefix: String of the form `projects/{project}/zones/{zone}/instances`
     :return: namedtuple with fields project_id and zone_name
     """
     split_list = prefix.split('/')
 
     return InstanceUriPrefix(
         project_id=split_list[1],
         zone_name=split_list[3],
     )
 
 
-def _parse_compute_full_uri_to_partial_uri(full_uri: str, version: str = 'v1') -> str:
+def _parse_compute_full_uri_to_partial_uri(full_uri, version='v1'):
     """
     Take a GCP Compute object's self_link of the form
     `https://www.googleapis.com/compute/{version}/projects/{project}/{location specifier}/{subtype}/{resource name}`
     and converts it to its partial URI `{project}/{location specifier}/{subtype}/{resource name}`.
     This is designed for GCP compute_objects that have compute/{version specifier}/ in their `self_link`s.
     :param network_full_uri: The full URI
     :param version: The version number; default to v1 since at the time of this writing v1 is the only Compute API.
     :return: Partial URI `{project}/{location specifier}/{subtype}/{resource name}`
     """
     return full_uri.split(f'compute/{version}/')[1]
 
 
-def _create_gcp_network_tag_id(vpc_partial_uri: str, tag: str) -> str:
+def _create_gcp_network_tag_id(vpc_partial_uri, tag):
     """
     Generate an ID for a GCP network tag
     :param vpc_partial_uri: The VPC that this tag applies to
     :return: An ID for the GCP network tag
     """
     return f"{vpc_partial_uri}/tags/{tag}"
 
 
-@timeit
-def transform_gcp_vpcs(vpc_res: Dict) -> List[Dict]:
+def transform_gcp_vpcs(vpc_res):
     """
     Transform the VPC response object for Neo4j ingestion
     :param vpc_res: The return data
     :return: List of VPCs ready for ingestion to Neo4j
     """
     vpc_list = []
 
@@ -265,26 +213,25 @@
         vpc['description'] = v.get('description', None)
         vpc['routing_config_routing_mode'] = v.get('routingConfig', {}).get('routingMode', None)
 
         vpc_list.append(vpc)
     return vpc_list
 
 
-@timeit
-def transform_gcp_subnets(subnet_res: Dict) -> List[Dict]:
+def transform_gcp_subnets(subnet_res):
     """
     Add additional fields to the subnet object to make it easier to process in `load_gcp_subnets()`.
     :param subnet_res: The response object returned from compute.subnetworks.list()
     :return: A transformed subnet_res
     """
     # The `id` in the response object has the form `projects/{project}/regions/{region}/subnetworks`.
     # We can include this in each subnet object in the list to form the partial_uri later on.
     prefix = subnet_res['id']
     projectid = prefix.split('/')[1]
-    subnet_list: List[Dict] = []
+    subnet_list = []
     for s in subnet_res.get('items', []):
         subnet = {}
 
         # Has the form `projects/{project}/regions/{region}/subnetworks/{subnet_name}`
         partial_uri = f"{prefix}/{s['name']}"
         subnet['id'] = partial_uri
         subnet['partial_uri'] = partial_uri
@@ -302,73 +249,22 @@
         subnet['self_link'] = s['selfLink']
         subnet['private_ip_google_access'] = s.get('privateIpGoogleAccess', None)
 
         subnet_list.append(subnet)
     return subnet_list
 
 
-@timeit
-def transform_gcp_forwarding_rules(fwd_response: Resource) -> List[Dict]:
-    """
-    Add additional fields to the forwarding rule object to make it easier to process in `load_gcp_forwarding_rules()`.
-    :param fwd_response: The response object returned from compute.forwardRules.list()
-    :return: A transformed fwd_response
-    """
-    fwd_list: List[Dict] = []
-    prefix = fwd_response['id']
-    project_id = prefix.split('/')[1]
-    for fwd in fwd_response.get('items', []):
-        forwarding_rule: Dict[str, Any] = {}
-
-        fwd_partial_uri = f"{prefix}/{fwd['name']}"
-        forwarding_rule['id'] = fwd_partial_uri
-        forwarding_rule['partial_uri'] = fwd_partial_uri
-
-        forwarding_rule['project_id'] = project_id
-        # Region looks like "https://www.googleapis.com/compute/v1/projects/{project}/regions/{region name}"
-        region = fwd.get('region', None)
-        forwarding_rule['region'] = region.split('/')[-1] if region else None
-        forwarding_rule['ip_address'] = fwd.get('IPAddress', None)
-        forwarding_rule['ip_protocol'] = fwd.get('IPProtocol', None)
-        forwarding_rule['allow_global_access'] = fwd.get('allowGlobalAccess', None)
-
-        forwarding_rule['load_balancing_scheme'] = fwd.get('loadBalancingScheme', None)
-        forwarding_rule['name'] = fwd.get('name', None)
-        forwarding_rule['port_range'] = fwd.get('portRange', None)
-        forwarding_rule['ports'] = fwd.get('ports', None)
-        forwarding_rule['self_link'] = fwd.get('selfLink', None)
-        target = fwd.get('target', None)
-        if target:
-            forwarding_rule['target'] = _parse_compute_full_uri_to_partial_uri(target)
-        else:
-            forwarding_rule['target'] = None
-
-        network = fwd.get('network', None)
-        if network:
-            forwarding_rule['network'] = network
-            forwarding_rule['network_partial_uri'] = _parse_compute_full_uri_to_partial_uri(network)
-
-        subnetwork = fwd.get('subnetwork', None)
-        if subnetwork:
-            forwarding_rule['subnetwork'] = subnetwork
-            forwarding_rule['subnetwork_partial_uri'] = _parse_compute_full_uri_to_partial_uri(subnetwork)
-
-        fwd_list.append(forwarding_rule)
-    return fwd_list
-
-
-@timeit
-def transform_gcp_firewall(fw_response: Resource) -> List[Dict]:
+def transform_gcp_firewall(fw_response):
     """
     Adjust the firewall response objects into a format that is easy to write to Neo4j.
     Also see _transform_fw_entry and _parse_port_string_to_rule().
     :param fw_response: Firewall response object from the GCP API
     :return: List of transformed firewall rule objects.
     """
-    fw_list: List[Dict] = []
+    fw_list = []
     prefix = fw_response['id']
     for fw in fw_response.get('items', []):
         fw_partial_uri = f"{prefix}/{fw['name']}"
         fw['id'] = fw_partial_uri
         fw['vpc_partial_uri'] = _parse_compute_full_uri_to_partial_uri(fw['network'])
 
         fw['transformed_allow_list'] = []
@@ -385,15 +281,15 @@
             transformed_deny_rules = _transform_fw_entry(deny_rule, fw_partial_uri, is_allow_rule=False)
             fw['transformed_deny_list'].extend(transformed_deny_rules)
 
         fw_list.append(fw)
     return fw_list
 
 
-def _transform_fw_entry(rule: Dict, fw_partial_uri: str, is_allow_rule: bool) -> List[Dict]:
+def _transform_fw_entry(rule, fw_partial_uri, is_allow_rule):
     """
     Takes a rule entry from a GCP firewall object's allow or deny list and converts it to a list of one or more
     dicts representing a firewall rule for each port and port range.  This format is easier to load into Neo4j.
 
     Example 1 - single port range:
     Input: `{'IPProtocol': 'tcp', 'ports': ['0-65535']}, fw_id, is_allow_rule=True`
     Output: `[ {fromport: 0, toport: 65535, protocol: tcp, ruleid: fw_id/allow/0to65535tcp} ]`
@@ -409,15 +305,15 @@
     Output: `[ {fromport: None, toport: None, protocol: icmp, ruleid: fw_id/allow/icmp} ]`
 
     :param rule: A rule entry object
     :param fw_partial_uri: The parent GCPFirewall's unique identifier
     :param is_allow_rule: Whether the rule is an `allow` rule.  If false it is a `deny` rule.
     :return: A list of one or more transformed rules
     """
-    result: List[Dict] = []
+    result = []
     # rule['ruleid'] = f"{fw_partial_uri}/"
     protocol = rule['IPProtocol']
 
     # If the protocol covered is TCP or UDP then we need to handle ports
     if protocol == 'tcp' or protocol == 'udp':
 
         # If ports are specified then create rules for each port and range
@@ -436,15 +332,15 @@
     # The protocol is  ICMP, ESP, AH, IPIP, SCTP, or proto numbers and ports don't apply
     else:
         rule = _parse_port_string_to_rule(None, protocol, fw_partial_uri, is_allow_rule)
         result.append(rule)
         return result
 
 
-def _parse_port_string_to_rule(port: Optional[str], protocol: str, fw_partial_uri: str, is_allow_rule: bool) -> Dict:
+def _parse_port_string_to_rule(port, protocol, fw_partial_uri, is_allow_rule):
     """
     Takes a string argument representing a GCP firewall rule port or port range and returns a dict that is easier to
     load into Neo4j.
 
     Example 1 - single port range:
     Input: `'0-65535', 'tcp', fw_id, is_allow_rule=True`
     Output: `{fromport: 0, toport: 65535, protocol: tcp, ruleid: fw_id/allow/0to65535tcp}`
@@ -492,90 +388,86 @@
         'ruleid': f"{fw_partial_uri}/{rule_type}/{port_range_str}{protocol}",
         'fromport': fromport,
         'toport': toport,
         'protocol': protocol,
     }
 
 
-@timeit
-def load_gcp_instances(neo4j_session: neo4j.Session, data: List[Dict], gcp_update_tag: int) -> None:
+def load_gcp_instances(neo4j_session, data, gcp_update_tag):
     """
     Ingest GCP instance objects to Neo4j
     :param neo4j_session: The Neo4j session object
     :param data: List of GCP instances to ingest. Basically the output of
     https://cloud.google.com/compute/docs/reference/rest/v1/instances/list
     :param gcp_update_tag: The timestamp value to set our new Neo4j nodes with
     :return: Nothing
     """
     query = """
-    MERGE (p:GCPProject{id:$ProjectId})
+    MERGE (p:GCPProject{id:{ProjectId}})
     ON CREATE SET p.firstseen = timestamp()
-    SET p.lastupdated = $gcp_update_tag
+    SET p.lastupdated = {gcp_update_tag}
 
-    MERGE (i:Instance:GCPInstance{id:$PartialUri})
+    MERGE (i:Instance:GCPInstance{id:{PartialUri}})
     ON CREATE SET i.firstseen = timestamp(),
-    i.partial_uri = $PartialUri
-    SET i.self_link = $SelfLink,
-    i.instancename = $InstanceName,
-    i.hostname = $Hostname,
-    i.zone_name = $ZoneName,
-    i.project_id = $ProjectId,
-    i.status = $Status,
-    i.lastupdated = $gcp_update_tag
+    i.partial_uri = {PartialUri}
+    SET i.self_link = {SelfLink},
+    i.instancename = {InstanceName},
+    i.hostname = {Hostname},
+    i.zone_name = {ZoneName},
+    i.project_id = {ProjectId},
+    i.lastupdated = {gcp_update_tag}
     WITH i, p
 
     MERGE (p)-[r:RESOURCE]->(i)
     ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $gcp_update_tag
+    SET r.lastupdated = {gcp_update_tag}
     """
     for instance in data:
         neo4j_session.run(
             query,
             ProjectId=instance['project_id'],
             PartialUri=instance['partial_uri'],
             SelfLink=instance['selfLink'],
             InstanceName=instance['name'],
             ZoneName=instance['zone_name'],
             Hostname=instance.get('hostname', None),
-            Status=instance['status'],
             gcp_update_tag=gcp_update_tag,
         )
         _attach_instance_tags(neo4j_session, instance, gcp_update_tag)
         _attach_gcp_nics(neo4j_session, instance, gcp_update_tag)
         _attach_gcp_vpc(neo4j_session, instance['partial_uri'], gcp_update_tag)
 
 
-@timeit
-def load_gcp_vpcs(neo4j_session: neo4j.Session, vpcs: List[Dict], gcp_update_tag: int) -> None:
+def load_gcp_vpcs(neo4j_session, vpcs, gcp_update_tag):
     """
     Ingest VPCs to Neo4j
     :param neo4j_session: The Neo4j session object
     :param vpcs: List of VPCs to ingest
     :param gcp_update_tag: The timestamp value to set our new Neo4j nodes with
     :return: Nothing
     """
     query = """
-    MERGE(p:GCPProject{id:$ProjectId})
+    MERGE(p:GCPProject{id:{ProjectId}})
     ON CREATE SET p.firstseen = timestamp()
-    SET p.lastupdated = $gcp_update_tag
+    SET p.lastupdated = {gcp_update_tag}
 
-    MERGE(vpc:GCPVpc{id:$PartialUri})
+    MERGE(vpc:GCPVpc{id:{PartialUri}})
     ON CREATE SET vpc.firstseen = timestamp(),
-    vpc.partial_uri = $PartialUri
-    SET vpc.self_link = $SelfLink,
-    vpc.name = $VpcName,
-    vpc.project_id = $ProjectId,
-    vpc.auto_create_subnetworks = $AutoCreateSubnetworks,
-    vpc.routing_config_routing_mode = $RoutingMode,
-    vpc.description = $Description,
-    vpc.lastupdated = $gcp_update_tag
+    vpc.partial_uri = {PartialUri}
+    SET vpc.self_link = {SelfLink},
+    vpc.name = {VpcName},
+    vpc.project_id = {ProjectId},
+    vpc.auto_create_subnetworks = {AutoCreateSubnetworks},
+    vpc.routing_config_routing_mode = {RoutingMode},
+    vpc.description = {Description},
+    vpc.lastupdated = {gcp_update_tag}
 
     MERGE (p)-[r:RESOURCE]->(vpc)
     ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $gcp_update_tag
+    SET r.lastupdated = {gcp_update_tag}
     """
     for vpc in vpcs:
         neo4j_session.run(
             query,
             ProjectId=vpc['project_id'],
             PartialUri=vpc['partial_uri'],
             SelfLink=vpc['self_link'],
@@ -583,44 +475,43 @@
             AutoCreateSubnetworks=vpc['auto_create_subnetworks'],
             RoutingMode=vpc['routing_config_routing_mode'],
             Description=vpc['description'],
             gcp_update_tag=gcp_update_tag,
         )
 
 
-@timeit
-def load_gcp_subnets(neo4j_session: neo4j.Session, subnets: List[Dict], gcp_update_tag: int) -> None:
+def load_gcp_subnets(neo4j_session, subnets, gcp_update_tag):
     """
     Ingest GCP subnet data to Neo4j
     :param neo4j_session: The Neo4j session
     :param subnets: List of the subnets
     :param gcp_update_tag: The timestamp to set these Neo4j nodes with
     :return: Nothing
     """
     query = """
-    MERGE(vpc:GCPVpc{id:$VpcPartialUri})
+    MERGE(vpc:GCPVpc{id:{VpcPartialUri}})
     ON CREATE SET vpc.firstseen = timestamp(),
-    vpc.partial_uri = $VpcPartialUri
+    vpc.partial_uri = {VpcPartialUri}
 
-    MERGE(subnet:GCPSubnet{id:$PartialUri})
+    MERGE(subnet:GCPSubnet{id:{PartialUri}})
     ON CREATE SET subnet.firstseen = timestamp(),
-    subnet.partial_uri = $PartialUri
-    SET subnet.self_link = $SubnetSelfLink,
-    subnet.project_id = $ProjectId,
-    subnet.name = $SubnetName,
-    subnet.region = $Region,
-    subnet.gateway_address = $GatewayAddress,
-    subnet.ip_cidr_range = $IpCidrRange,
-    subnet.private_ip_google_access = $PrivateIpGoogleAccess,
-    subnet.vpc_partial_uri = $VpcPartialUri,
-    subnet.lastupdated = $gcp_update_tag
+    subnet.partial_uri = {PartialUri}
+    SET subnet.self_link = {SubnetSelfLink},
+    subnet.project_id = {ProjectId},
+    subnet.name = {SubnetName},
+    subnet.region = {Region},
+    subnet.gateway_address = {GatewayAddress},
+    subnet.ip_cidr_range = {IpCidrRange},
+    subnet.private_ip_google_access = {PrivateIpGoogleAccess},
+    subnet.vpc_partial_uri = {VpcPartialUri},
+    subnet.lastupdated = {gcp_update_tag}
 
     MERGE (vpc)-[r:RESOURCE]->(subnet)
     ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $gcp_update_tag
+    SET r.lastupdated = {gcp_update_tag}
     """
     for s in subnets:
         neo4j_session.run(
             query,
             VpcPartialUri=s['vpc_partial_uri'],
             VpcSelfLink=s['vpc_self_link'],
             PartialUri=s['partial_uri'],
@@ -631,236 +522,125 @@
             GatewayAddress=s['gateway_address'],
             IpCidrRange=s['ip_cidr_range'],
             PrivateIpGoogleAccess=s['private_ip_google_access'],
             gcp_update_tag=gcp_update_tag,
         )
 
 
-@timeit
-def load_gcp_forwarding_rules(neo4j_session: neo4j.Session, fwd_rules: List[Dict], gcp_update_tag: int) -> None:
-    """
-    Ingest GCP forwarding rules data to Neo4j
-    :param neo4j_session: The Neo4j session
-    :param fwd_rules: List of forwarding rules
-    :param gcp_update_tag: The timestamp to set these Neo4j nodes with
-    :return: Nothing
-    """
-
-    query = """
-        MERGE(fwd:GCPForwardingRule{id:$PartialUri})
-        ON CREATE SET fwd.firstseen = timestamp(),
-        fwd.partial_uri = $PartialUri
-        SET fwd.ip_address = $IPAddress,
-        fwd.ip_protocol = $IPProtocol,
-        fwd.load_balancing_scheme = $LoadBalancingScheme,
-        fwd.name = $Name,
-        fwd.network = $NetworkPartialUri,
-        fwd.port_range = $PortRange,
-        fwd.ports = $Ports,
-        fwd.project_id = $ProjectId,
-        fwd.region = $Region,
-        fwd.self_link = $SelfLink,
-        fwd.subnetwork = $SubNetworkPartialUri,
-        fwd.target = $TargetPartialUri,
-        fwd.lastupdated = $gcp_update_tag
-    """
-
-    for fwd in fwd_rules:
-        network = fwd.get('network', None)
-        subnetwork = fwd.get('subnetwork', None)
-
-        neo4j_session.run(
-            query,
-            PartialUri=fwd['partial_uri'],
-            IPAddress=fwd['ip_address'],
-            IPProtocol=fwd['ip_protocol'],
-            LoadBalancingScheme=fwd['load_balancing_scheme'],
-            Name=fwd['name'],
-            Network=network,
-            NetworkPartialUri=fwd.get('network_partial_uri', None),
-            PortRange=fwd.get('port_range', None),
-            Ports=fwd.get('ports', None),
-            ProjectId=fwd['project_id'],
-            Region=fwd.get('region', None),
-            SelfLink=fwd['self_link'],
-            SubNetwork=subnetwork,
-            SubNetworkPartialUri=fwd.get('subnetwork_partial_uri', None),
-            TargetPartialUri=fwd['target'],
-            gcp_update_tag=gcp_update_tag,
-        )
-
-        if subnetwork:
-            _attach_fwd_rule_to_subnet(neo4j_session, fwd, gcp_update_tag)
-        elif network:
-            _attach_fwd_rule_to_vpc(neo4j_session, fwd, gcp_update_tag)
-
-
-@timeit
-def _attach_fwd_rule_to_subnet(neo4j_session: neo4j.Session, fwd: Dict, gcp_update_tag: int) -> None:
-    query = """
-        MERGE(subnet:GCPSubnet{id:$SubNetworkPartialUri})
-        ON CREATE SET subnet.firstseen = timestamp(),
-        subnet.partial_uri = $SubNetworkPartialUri
-        SET subnet.lastupdated = $gcp_update_tag
-
-        WITH subnet
-        MATCH(fwd:GCPForwardingRule{id:$PartialUri})
-
-        MERGE(subnet)-[p:RESOURCE]->(fwd)
-        ON CREATE SET p.firstseen = timestamp()
-        SET p.lastupdated = $gcp_update_tag
-    """
-
-    neo4j_session.run(
-        query,
-        PartialUri=fwd['partial_uri'],
-        SubNetworkPartialUri=fwd.get('subnetwork_partial_uri', None),
-        gcp_update_tag=gcp_update_tag,
-    )
-
-
-@timeit
-def _attach_fwd_rule_to_vpc(neo4j_session: neo4j.Session, fwd: Dict, gcp_update_tag: int) -> None:
-    query = """
-        MERGE (vpc:GCPVpc{id:$NetworkPartialUri})
-        ON CREATE SET vpc.firstseen = timestamp(),
-        vpc.partial_uri = $NetworkPartialUri
-
-        WITH vpc
-        MATCH (fwd:GCPForwardingRule{id:$PartialUri})
-
-        MERGE (vpc)-[r:RESOURCE]->(fwd)
-        ON CREATE SET r.firstseen = timestamp()
-        SET r.lastupdated = $gcp_update_tag
-    """
-
-    neo4j_session.run(
-        query,
-        PartialUri=fwd['partial_uri'],
-        NetworkPartialUri=fwd.get('network_partial_uri', None),
-        gcp_update_tag=gcp_update_tag,
-    )
-
-
-@timeit
-def _attach_instance_tags(neo4j_session: neo4j.Session, instance: Resource, gcp_update_tag: int) -> None:
+def _attach_instance_tags(neo4j_session, instance, gcp_update_tag):
     """
     Attach tags to GCP instance and to the VPCs that they are defined in.
     :param neo4j_session: The session
     :param instance: The instance object
     :param gcp_update_tag: The timestamp
     :return: Nothing
     """
     query = """
-    MATCH (i:GCPInstance{id:$InstanceId})
+    MATCH (i:GCPInstance{id:{InstanceId}})
 
-    MERGE (t:GCPNetworkTag{id:$TagId})
-    ON CREATE SET t.tag_id = $TagId,
-    t.value = $TagValue,
+    MERGE (t:GCPNetworkTag{id:{TagId}})
+    ON CREATE SET t.tag_id = {TagId},
+    t.value = {TagValue},
     t.firstseen = timestamp()
-    SET t.lastupdated = $gcp_update_tag
+    SET t.lastupdated = {gcp_update_tag}
 
     MERGE (i)-[h:TAGGED]->(t)
     ON CREATE SET h.firstseen = timestamp()
-    SET h.lastupdated = $gcp_update_tag
+    SET h.lastupdated = {gcp_update_tag}
 
     WITH t
-    MATCH (vpc:GCPVpc{id:$VpcPartialUri})
+    MATCH (vpc:GCPVpc{id:{VpcPartialUri}})
 
     MERGE (vpc)<-[d:DEFINED_IN]-(t)
     ON CREATE SET d.firstseen = timestamp()
-    SET d.lastupdated = $gcp_update_tag
+    SET d.lastupdated = {gcp_update_tag}
     """
     for tag in instance.get('tags', {}).get('items', []):
         for nic in instance.get('networkInterfaces', []):
             tag_id = _create_gcp_network_tag_id(nic['vpc_partial_uri'], tag)
             neo4j_session.run(
                 query,
                 InstanceId=instance['partial_uri'],
                 TagId=tag_id,
                 TagValue=tag,
                 VpcPartialUri=nic['vpc_partial_uri'],
                 gcp_update_tag=gcp_update_tag,
             )
 
 
-@timeit
-def _attach_gcp_nics(neo4j_session: neo4j.Session, instance: Resource, gcp_update_tag: int) -> None:
+def _attach_gcp_nics(neo4j_session, instance, gcp_update_tag):
     """
     Attach GCP Network Interfaces to GCP Instances and GCP Subnets.
     Then, attach GCP Instances directly to VPCs.
     :param neo4j_session: The Neo4j session
     :param instance: The GCP instance
     :param gcp_update_tag: Timestamp to set the nodes
     :return: Nothing
     """
     query = """
-    MATCH (i:GCPInstance{id:$InstanceId})
-    MERGE (nic:GCPNetworkInterface:NetworkInterface{id:$NicId})
+    MATCH (i:GCPInstance{id:{InstanceId}})
+    MERGE (nic:GCPNetworkInterface:NetworkInterface{id:{NicId}})
     ON CREATE SET nic.firstseen = timestamp(),
-    nic.nic_id = $NicId
-    SET nic.private_ip = $NetworkIP,
-    nic.name = $NicName,
-    nic.lastupdated = $gcp_update_tag
+    nic.nic_id = {NicId}
+    SET nic.private_ip = {NetworkIP},
+    nic.name = {NicName},
+    nic.lastupdated = {gcp_update_tag}
 
     MERGE (i)-[r:NETWORK_INTERFACE]->(nic)
     ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $gcp_update_tag
+    SET r.lastupdated = {gcp_update_tag}
 
-    MERGE (subnet:GCPSubnet{id:$SubnetPartialUri})
+    MERGE (subnet:GCPSubnet{id:{SubnetPartialUri}})
     ON CREATE SET subnet.firstseen = timestamp(),
-    subnet.partial_uri = $SubnetPartialUri
-    SET subnet.lastupdated = $gcp_update_tag
+    subnet.partial_uri = {SubnetPartialUri}
+    SET subnet.lastupdated = {gcp_update_tag}
 
     MERGE (nic)-[p:PART_OF_SUBNET]->(subnet)
     ON CREATE SET p.firstseen = timestamp()
-    SET p.lastupdated = $gcp_update_tag
+    SET p.lastupdated = {gcp_update_tag}
     """
     for nic in instance.get('networkInterfaces', []):
         # Make an ID for GCPNetworkInterface nodes because GCP doesn't define one but we need to uniquely identify them
         nic_id = f"{instance['partial_uri']}/networkinterfaces/{nic['name']}"
         neo4j_session.run(
             query,
             InstanceId=instance['partial_uri'],
             NicId=nic_id,
-            NetworkIP=nic.get('networkIP'),
+            NetworkIP=nic['networkIP'],
             NicName=nic['name'],
             gcp_update_tag=gcp_update_tag,
             SubnetPartialUri=nic['subnet_partial_uri'],
         )
         _attach_gcp_nic_access_configs(neo4j_session, nic_id, nic, gcp_update_tag)
 
 
-@timeit
-def _attach_gcp_nic_access_configs(
-    neo4j_session: neo4j.Session, nic_id: str, nic: Resource, gcp_update_tag: int,
-) -> None:
+def _attach_gcp_nic_access_configs(neo4j_session, nic_id, nic, gcp_update_tag):
     """
     Attach an access configuration to the GCP NIC.
     :param neo4j_session: The Neo4j session
     :param instance: The GCP instance
     :param gcp_update_tag: The timestamp to set updated nodes to
     :return: Nothing
     """
     query = """
-    MATCH (nic{id:$NicId})
-    MERGE (ac:GCPNicAccessConfig{id:$AccessConfigId})
+    MATCH (nic{id:{NicId}})
+    MERGE (ac:GCPNicAccessConfig{id:{AccessConfigId}})
     ON CREATE SET ac.firstseen = timestamp(),
-    ac.access_config_id = $AccessConfigId
-    SET ac.type=$Type,
-    ac.name = $Name,
-    ac.public_ip = $NatIP,
-    ac.set_public_ptr = $SetPublicPtr,
-    ac.public_ptr_domain_name = $PublicPtrDomainName,
-    ac.network_tier = $NetworkTier,
-    ac.lastupdated = $gcp_update_tag
+    ac.access_config_id = {AccessConfigId}
+    SET ac.type={Type},
+    ac.name = {Name},
+    ac.public_ip = {NatIP},
+    ac.set_public_ptr = {SetPublicPtr},
+    ac.public_ptr_domain_name = {PublicPtrDomainName},
+    ac.network_tier = {NetworkTier},
+    ac.lastupdated = {gcp_update_tag}
 
     MERGE (nic)-[r:RESOURCE]->(ac)
     ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $gcp_update_tag
+    SET r.lastupdated = {gcp_update_tag}
     """
     for ac in nic.get('accessConfigs', []):
         # Make an ID for GCPNicAccessConfig nodes because GCP doesn't define one but we need to uniquely identify them
         access_config_id = f"{nic_id}/accessconfigs/{ac['type']}"
         neo4j_session.run(
             query,
             NicId=nic_id,
@@ -871,64 +651,62 @@
             SetPublicPtr=ac.get('setPublicPtr', None),
             PublicPtrDomainName=ac.get('publicPtrDomainName', None),
             NetworkTier=ac.get('networkTier', None),
             gcp_update_tag=gcp_update_tag,
         )
 
 
-@timeit
-def _attach_gcp_vpc(neo4j_session: neo4j.Session, instance_id: str, gcp_update_tag: int) -> None:
+def _attach_gcp_vpc(neo4j_session, instance_id, gcp_update_tag):
     """
     Attach a GCP instance directly to a VPC
     :param neo4j_session: neo4j_session
     :param instance: The GCP instance object
     :param gcp_update_tag:
     :return: Nothing
     """
     query = """
-    MATCH (i:GCPInstance{id:$InstanceId})-[:NETWORK_INTERFACE]->(nic:GCPNetworkInterface)
+    MATCH (i:GCPInstance{id:{InstanceId}})-[:NETWORK_INTERFACE]->(nic:GCPNetworkInterface)
           -[p:PART_OF_SUBNET]->(sn:GCPSubnet)<-[r:RESOURCE]-(vpc:GCPVpc)
     MERGE (i)-[m:MEMBER_OF_GCP_VPC]->(vpc)
     ON CREATE SET m.firstseen = timestamp()
-    SET m.lastupdated = $gcp_update_tag
+    SET m.lastupdated = {gcp_update_tag}
     """
     neo4j_session.run(
         query,
         InstanceId=instance_id,
         gcp_update_tag=gcp_update_tag,
     )
 
 
-@timeit
-def load_gcp_ingress_firewalls(neo4j_session: neo4j.Session, fw_list: List[Resource], gcp_update_tag: int) -> None:
+def load_gcp_ingress_firewalls(neo4j_session, fw_list, gcp_update_tag):
     """
     Load the firewall list to Neo4j
     :param fw_list: The transformed list of firewalls
     :return: Nothing
     """
     query = """
-    MERGE (fw:GCPFirewall{id:$FwPartialUri})
+    MERGE (fw:GCPFirewall{id:{FwPartialUri}})
     ON CREATE SET fw.firstseen = timestamp(),
-    fw.partial_uri = $FwPartialUri
-    SET fw.direction = $Direction,
-    fw.disabled = $Disabled,
-    fw.name = $Name,
-    fw.priority = $Priority,
-    fw.self_link = $SelfLink,
-    fw.has_target_service_accounts = $HasTargetServiceAccounts,
-    fw.lastupdated = $gcp_update_tag
+    fw.partial_uri = {FwPartialUri}
+    SET fw.direction = {Direction},
+    fw.disabled = {Disabled},
+    fw.name = {Name},
+    fw.priority = {Priority},
+    fw.self_link = {SelfLink},
+    fw.has_target_service_accounts = {HasTargetServiceAccounts},
+    fw.lastupdated = {gcp_update_tag}
 
-    MERGE (vpc:GCPVpc{id:$VpcPartialUri})
+    MERGE (vpc:GCPVpc{id:{VpcPartialUri}})
     ON CREATE SET vpc.firstseen = timestamp(),
-    vpc.partial_uri = $VpcPartialUri
-    SET vpc.lastupdated = $gcp_update_tag
+    vpc.partial_uri = {VpcPartialUri}
+    SET vpc.lastupdated = {gcp_update_tag}
 
     MERGE (vpc)-[r:RESOURCE]->(fw)
     ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $gcp_update_tag
+    SET r.lastupdated = {gcp_update_tag}
     """
     for fw in fw_list:
         neo4j_session.run(
             query,
             FwPartialUri=fw['id'],
             Direction=fw['direction'],
             Disabled=fw['disabled'],
@@ -939,286 +717,220 @@
             HasTargetServiceAccounts=fw['has_target_service_accounts'],
             gcp_update_tag=gcp_update_tag,
         )
         _attach_firewall_rules(neo4j_session, fw, gcp_update_tag)
         _attach_target_tags(neo4j_session, fw, gcp_update_tag)
 
 
-@timeit
-def _attach_firewall_rules(neo4j_session: neo4j.Session, fw: Resource, gcp_update_tag: int) -> None:
+def _attach_firewall_rules(neo4j_session, fw, gcp_update_tag):
     """
     Attach the allow_rules to the Firewall object
     :param neo4j_session: The Neo4j session
     :param fw: The Firewall object
     :param gcp_update_tag: The timestamp
     :return: Nothing
     """
-    template = Template("""
-    MATCH (fw:GCPFirewall{id:$FwPartialUri})
+    query = """
+    MATCH (fw:GCPFirewall{id:{FwPartialUri}})
 
-    MERGE (rule:IpRule:IpPermissionInbound:GCPIpRule{id:$RuleId})
+    MERGE (rule:IpRule:IpPermissionInbound:GCPIpRule{id:{RuleId}})
     ON CREATE SET rule.firstseen = timestamp(),
-    rule.ruleid = $RuleId
-    SET rule.protocol = $Protocol,
-    rule.fromport = $FromPort,
-    rule.toport = $ToPort,
-    rule.lastupdated = $gcp_update_tag
+    rule.ruleid = {RuleId}
+    SET rule.protocol = {Protocol},
+    rule.fromport = {FromPort},
+    rule.toport = {ToPort},
+    rule.lastupdated = {gcp_update_tag}
 
-    MERGE (rng:IpRange{id:$Range})
+    MERGE (rng:IpRange{id:{Range}})
     ON CREATE SET rng.firstseen = timestamp(),
-    rng.range = $Range
-    SET rng.lastupdated = $gcp_update_tag
+    rng.range = {Range}
+    SET rng.lastupdated = {gcp_update_tag}
 
     MERGE (rng)-[m:MEMBER_OF_IP_RULE]->(rule)
     ON CREATE SET m.firstseen = timestamp()
-    SET m.lastupdated = $gcp_update_tag
-
-    MERGE (fw)<-[r:$fw_rule_relationship_label]-(rule)
-    ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $gcp_update_tag
-    """)
+    SET m.lastupdated = {gcp_update_tag}
+    """
     for list_type in 'transformed_allow_list', 'transformed_deny_list':
         if list_type == 'transformed_allow_list':
-            label = "ALLOWED_BY"
+            query += """
+            MERGE (fw)<-[r:ALLOWED_BY]-(rule)
+            ON CREATE SET r.firstseen = timestamp()
+            SET r.lastupdated = {gcp_update_tag}
+            """
         else:
-            label = "DENIED_BY"
+            query += """
+            MERGE (fw)<-[r:DENIED_BY]-(rule)
+            ON CREATE SET r.firstseen = timestamp()
+            SET r.lastupdated = {gcp_update_tag}
+            """
         for rule in fw[list_type]:
             # It is possible for sourceRanges to not be specified for this rule
             # If sourceRanges is not specified then the rule must specify sourceTags.
             # Since an IP range cannot have a tag applied to it, it is ok if we don't ingest this rule.
             for ip_range in fw.get('sourceRanges', []):
                 neo4j_session.run(
-                    template.safe_substitute(fw_rule_relationship_label=label),
+                    query,
                     FwPartialUri=fw['id'],
                     RuleId=rule['ruleid'],
                     Protocol=rule['protocol'],
                     FromPort=rule.get('fromport'),
                     ToPort=rule.get('toport'),
                     Range=ip_range,
                     gcp_update_tag=gcp_update_tag,
                 )
 
 
-@timeit
-def _attach_target_tags(neo4j_session: neo4j.Session, fw: Resource, gcp_update_tag: int) -> None:
+def _attach_target_tags(neo4j_session, fw, gcp_update_tag):
     """
     Attach target tags to the firewall object
     :param neo4j_session: The neo4j session
     :param fw: The firewall object
     :param gcp_update_tag: The timestamp
     :return: Nothing
     """
     query = """
-    MATCH (fw:GCPFirewall{id:$FwPartialUri})
+    MATCH (fw:GCPFirewall{id:{FwPartialUri}})
 
-    MERGE (t:GCPNetworkTag{id:$TagId})
+    MERGE (t:GCPNetworkTag{id:{TagId}})
     ON CREATE SET t.firstseen = timestamp(),
-    t.tag_id = $TagId,
-    t.value = $TagValue
-    SET t.lastupdated = $gcp_update_tag
+    t.tag_id = {TagId},
+    t.value = {TagValue}
+    SET t.lastupdated = {gcp_update_tag}
 
     MERGE (fw)-[h:TARGET_TAG]->(t)
     ON CREATE SET h.firstseen = timestamp()
-    SET h.lastupdated = $gcp_update_tag
+    SET h.lastupdated = {gcp_update_tag}
     """
     for tag in fw.get('targetTags', []):
         tag_id = _create_gcp_network_tag_id(fw['vpc_partial_uri'], tag)
         neo4j_session.run(
             query,
             FwPartialUri=fw['id'],
             TagId=tag_id,
             TagValue=tag,
             gcp_update_tag=gcp_update_tag,
         )
 
 
-@timeit
-def cleanup_gcp_instances(neo4j_session: neo4j.Session, common_job_parameters: Dict) -> None:
+def cleanup_gcp_instances(session, common_job_parameters):
     """
     Delete out-of-date GCP instance nodes and relationships
-    :param neo4j_session: The Neo4j session
+    :param session: The Neo4j session
     :param common_job_parameters: dict of other job parameters to pass to Neo4j
     :return: Nothing
     """
-    run_cleanup_job('gcp_compute_instance_cleanup.json', neo4j_session, common_job_parameters)
+    run_cleanup_job('gcp_compute_instance_cleanup.json', session, common_job_parameters)
 
 
-@timeit
-def cleanup_gcp_vpcs(neo4j_session: neo4j.Session, common_job_parameters: Dict) -> None:
+def cleanup_gcp_vpcs(session, common_job_parameters):
     """
     Delete out-of-date GCP VPC nodes and relationships
-    :param neo4j_session: The Neo4j session
+    :param session: The Neo4j session
     :param common_job_parameters: dict of other job parameters to pass to Neo4j
     :return: Nothing
     """
-    run_cleanup_job('gcp_compute_vpc_cleanup.json', neo4j_session, common_job_parameters)
+    run_cleanup_job('gcp_compute_vpc_cleanup.json', session, common_job_parameters)
 
 
-@timeit
-def cleanup_gcp_subnets(neo4j_session: neo4j.Session, common_job_parameters: Dict) -> None:
+def cleanup_gcp_subnets(session, common_job_parameters):
     """
     Delete out-of-date GCP VPC subnet nodes and relationships
-    :param neo4j_session: The Neo4j session
+    :param session: The Neo4j session
     :param common_job_parameters: dict of other job parameters to pass to Neo4j
     :return: Nothing
     """
-    run_cleanup_job('gcp_compute_vpc_subnet_cleanup.json', neo4j_session, common_job_parameters)
+    run_cleanup_job('gcp_compute_vpc_subnet_cleanup.json', session, common_job_parameters)
 
 
-@timeit
-def cleanup_gcp_forwarding_rules(neo4j_session: neo4j.Session, common_job_parameters: Dict) -> None:
-    """
-    Delete out-of-date GCP forwarding rules and relationships
-    :param neo4j_session: The Neo4j session
-    :param common_job_parameters: dict of other job parameters to pass to Neo4j
-    :return: Nothing
-    """
-    run_cleanup_job('gcp_compute_forwarding_rules_cleanup.json', neo4j_session, common_job_parameters)
-
-
-@timeit
-def cleanup_gcp_firewall_rules(neo4j_session: neo4j.Session, common_job_parameters: Dict) -> None:
+def cleanup_gcp_firewall_rules(session, common_job_parameters):
     """
     Delete out of date GCP firewalls and their relationships
-    :param neo4j_session: The Neo4j session
+    :param session: The Neo4j session
     :param common_job_parameters: dict of other job parameters to pass to Neo4j
     :return: Nothing
     """
-    run_cleanup_job('gcp_compute_firewall_cleanup.json', neo4j_session, common_job_parameters)
+    run_cleanup_job('gcp_compute_firewall_cleanup.json', session, common_job_parameters)
 
 
-@timeit
-def sync_gcp_instances(
-    neo4j_session: neo4j.Session, compute: Resource, project_id: str, zones: Optional[List[Dict]],
-    gcp_update_tag: int, common_job_parameters: Dict,
-) -> None:
+def sync_gcp_instances(session, compute, project_id, zones, gcp_update_tag, common_job_parameters):
     """
     Get GCP instances using the Compute resource object, ingest to Neo4j, and clean up old data.
-    :param neo4j_session: The Neo4j session object
+    :param session: The Neo4j session object
     :param compute: The GCP Compute resource object
     :param project_id: The project ID number to sync.  See  the `projectId` field in
     https://cloud.google.com/resource-manager/reference/rest/v1/projects
     :param zones: The list of all zone names that are enabled for this project; this is the output of
     `get_zones_in_project()`
     :param gcp_update_tag: The timestamp value to set our new Neo4j nodes with
     :param common_job_parameters: dict of other job parameters to pass to Neo4j
     :return: Nothing
     """
     instance_responses = get_gcp_instance_responses(project_id, zones, compute)
     instance_list = transform_gcp_instances(instance_responses)
-    load_gcp_instances(neo4j_session, instance_list, gcp_update_tag)
-    # TODO scope the cleanup to the current project - https://github.com/lyft/cartography/issues/381
-    cleanup_gcp_instances(neo4j_session, common_job_parameters)
+    load_gcp_instances(session, instance_list, gcp_update_tag)
+    cleanup_gcp_instances(session, common_job_parameters)
 
 
-@timeit
-def sync_gcp_vpcs(
-    neo4j_session: neo4j.Session, compute: Resource, project_id: str, gcp_update_tag: int,
-    common_job_parameters: Dict,
-) -> None:
+def sync_gcp_vpcs(session, compute, project_id, gcp_update_tag, common_job_parameters):
     """
     Get GCP VPCs, ingest to Neo4j, and clean up old data.
-    :param neo4j_session: The Neo4j session
+    :param session: The Neo4j session
     :param compute: The GCP Compute resource object
     :param project_id: The project ID to sync
     :param gcp_update_tag: The timestamp value to set our new Neo4j nodes with
     :param common_job_parameters: dict of other job parameters to pass to Neo4j
     :return: Nothing
     """
     vpc_res = get_gcp_vpcs(project_id, compute)
     vpcs = transform_gcp_vpcs(vpc_res)
-    load_gcp_vpcs(neo4j_session, vpcs, gcp_update_tag)
-    # TODO scope the cleanup to the current project - https://github.com/lyft/cartography/issues/381
-    cleanup_gcp_vpcs(neo4j_session, common_job_parameters)
+    load_gcp_vpcs(session, vpcs, gcp_update_tag)
+    cleanup_gcp_vpcs(session, common_job_parameters)
 
 
-@timeit
-def sync_gcp_subnets(
-    neo4j_session: neo4j.Session, compute: Resource, project_id: str, regions: List[str], gcp_update_tag: int,
-    common_job_parameters: Dict,
-) -> None:
+def sync_gcp_subnets(session, compute, project_id, regions, gcp_update_tag, common_job_parameters):
     for r in regions:
         subnet_res = get_gcp_subnets(project_id, r, compute)
         subnets = transform_gcp_subnets(subnet_res)
-        load_gcp_subnets(neo4j_session, subnets, gcp_update_tag)
-        # TODO scope the cleanup to the current project - https://github.com/lyft/cartography/issues/381
-        cleanup_gcp_subnets(neo4j_session, common_job_parameters)
-
+        load_gcp_subnets(session, subnets, gcp_update_tag)
+        cleanup_gcp_subnets(session, common_job_parameters)
 
-@timeit
-def sync_gcp_forwarding_rules(
-    neo4j_session: neo4j.Session, compute: Resource, project_id: str, regions: List[str], gcp_update_tag: int,
 
-    common_job_parameters: Dict,
-) -> None:
-    """
-    Sync GCP Both Global and Regional Forwarding Rules, ingest to Neo4j, and clean up old data.
-    :param neo4j_session: The Neo4j session
-    :param compute: The GCP Compute resource object
-    :param project_id: The project ID to sync
-    :param regions: List of regions.
-    :param gcp_update_tag: The timestamp value to set our new Neo4j nodes with
-    :param common_job_parameters: dict of other job parameters to pass to Neo4j
-    :return: Nothing
-    """
-    global_fwd_response = get_gcp_global_forwarding_rules(project_id, compute)
-    forwarding_rules = transform_gcp_forwarding_rules(global_fwd_response)
-    load_gcp_forwarding_rules(neo4j_session, forwarding_rules, gcp_update_tag)
-    # TODO scope the cleanup to the current project - https://github.com/lyft/cartography/issues/381
-    cleanup_gcp_forwarding_rules(neo4j_session, common_job_parameters)
-
-    for r in regions:
-        fwd_response = get_gcp_regional_forwarding_rules(project_id, r, compute)
-        forwarding_rules = transform_gcp_forwarding_rules(fwd_response)
-        load_gcp_forwarding_rules(neo4j_session, forwarding_rules, gcp_update_tag)
-        # TODO scope the cleanup to the current project - https://github.com/lyft/cartography/issues/381
-        cleanup_gcp_forwarding_rules(neo4j_session, common_job_parameters)
-
-
-@timeit
-def sync_gcp_firewall_rules(
-    neo4j_session: neo4j.Session, compute: Resource, project_id: str, gcp_update_tag: int,
-    common_job_parameters: Dict,
-) -> None:
+def sync_gcp_firewall_rules(session, compute, project_id, gcp_update_tag, common_job_parameters):
     """
     Sync GCP firewalls
-    :param neo4j_session: The Neo4j session
+    :param session: The Neo4j session
     :param compute: The Compute resource object
     :param project_id: The project ID that the firewalls are in
     :param common_job_parameters: dict of other job params to pass to Neo4j
     :return: Nothing
     """
     fw_response = get_gcp_firewall_ingress_rules(project_id, compute)
     fw_list = transform_gcp_firewall(fw_response)
-    load_gcp_ingress_firewalls(neo4j_session, fw_list, gcp_update_tag)
-    # TODO scope the cleanup to the current project - https://github.com/lyft/cartography/issues/381
-    cleanup_gcp_firewall_rules(neo4j_session, common_job_parameters)
+    load_gcp_ingress_firewalls(session, fw_list, gcp_update_tag)
+    cleanup_gcp_firewall_rules(session, common_job_parameters)
 
 
-def _zones_to_regions(zones: List[str]) -> List[Set]:
+def _zones_to_regions(zones):
     """
     Return list of regions from the input list of zones
     :param zones: List of zones. This is the output from `get_zones_in_project()`.
     :return: List of regions available to the project
     """
     regions = set()
-    for zone in zones:
+    for z in zones:
         # Chop off the last 2 chars to turn the zone to a region
-        region = zone['name'][:-2]     # type: ignore
-        regions.add(region)
-    return list(regions)     # type: ignore
+        r = z['name'][:-2]
+        regions.add(r)
+    return list(regions)
 
 
-def sync(
-    neo4j_session: neo4j.Session, compute: Resource, project_id: str, gcp_update_tag: int,
-    common_job_parameters: dict,
-) -> None:
+def sync(session, compute, project_id, gcp_update_tag, common_job_parameters):
     """
     Sync all objects that we need the GCP Compute resource object for.
-    :param neo4j_session: The Neo4j session object
+    :param session: The Neo4j session object
     :param compute: The GCP Compute resource object
     :param project_id: The project ID number to sync.
     :param project_id: The project ID number to sync.  See  the `projectId` field in
     https://cloud.google.com/resource-manager/reference/rest/v1/projects
     :param gcp_update_tag: The timestamp value to set our new Neo4j nodes with
     :param common_job_parameters: dict of other job parameters to pass to Neo4j
     :return: Nothing
@@ -1226,12 +938,11 @@
     logger.info("Syncing Compute objects for project %s.", project_id)
     zones = get_zones_in_project(project_id, compute)
     # Only pull additional assets for this project if the Compute API is enabled
     if zones is None:
         return
     else:
         regions = _zones_to_regions(zones)
-        sync_gcp_vpcs(neo4j_session, compute, project_id, gcp_update_tag, common_job_parameters)
-        sync_gcp_firewall_rules(neo4j_session, compute, project_id, gcp_update_tag, common_job_parameters)
-        sync_gcp_subnets(neo4j_session, compute, project_id, regions, gcp_update_tag, common_job_parameters)
-        sync_gcp_instances(neo4j_session, compute, project_id, zones, gcp_update_tag, common_job_parameters)
-        sync_gcp_forwarding_rules(neo4j_session, compute, project_id, regions, gcp_update_tag, common_job_parameters)
+        sync_gcp_vpcs(session, compute, project_id, gcp_update_tag, common_job_parameters)
+        sync_gcp_firewall_rules(session, compute, project_id, gcp_update_tag, common_job_parameters)
+        sync_gcp_subnets(session, compute, project_id, regions, gcp_update_tag, common_job_parameters)
+        sync_gcp_instances(session, compute, project_id, zones, gcp_update_tag, common_job_parameters)
```

### Comparing `cartography-0.81.0/cartography/intel/oci/iam.py` & `cartography-0.9.0/cartography/intel/aws/iam.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,461 +1,448 @@
-# Copyright (c) 2020, Oracle and/or its affiliates.
-# OCI Identity API-centric functions
-# https://docs.cloud.oracle.com/iaas/Content/Identity/Concepts/overview.htm
 import logging
-import re
-from typing import Any
-from typing import Dict
-from typing import List
 
-import neo4j
-import oci
+import policyuniverse.statement
 
-from . import utils
 from cartography.util import run_cleanup_job
 
 logger = logging.getLogger(__name__)
 
 
-def sync_compartments(
-    neo4j_session: neo4j.Session,
-    iam: oci.identity.identity_client.IdentityClient,
-    current_tenancy_id: str,
-    oci_update_tag: int,
-    common_job_parameters: Dict[str, Any],
-) -> None:
-    logger.debug("Syncing IAM compartments for account '%s'.", current_tenancy_id)
-    data = get_compartment_list_data(iam, current_tenancy_id)
-    load_compartments(neo4j_session, data['Compartments'], current_tenancy_id, oci_update_tag)
-    run_cleanup_job('oci_import_compartments_cleanup.json', neo4j_session, common_job_parameters)
-
-
-def get_compartment_list_data_recurse(
-    iam: oci.identity.identity_client.IdentityClient,
-    compartment_list: Dict[str, Any],
-    compartment_id: str,
-) -> None:
-
-    response = oci.pagination.list_call_get_all_results(iam.list_compartments, compartment_id)
-    if not response.data:
-        return
-    compartment_list.update(
-        {"Compartments": list(compartment_list["Compartments"]) + utils.oci_object_to_json(response.data)},
-    )
-    for compartment in response.data:
-        get_compartment_list_data_recurse(iam, compartment_list, compartment.id)
+def get_group_policies(session, group_name):
+    client = session.client('iam')
+    paginator = client.get_paginator('list_group_policies')
+    policy_names = []
+    for page in paginator.paginate(GroupName=group_name):
+        policy_names.extend(page['PolicyNames'])
+    return {'PolicyNames': policy_names}
 
 
-def get_compartment_list_data(
-    iam: oci.identity.identity_client.IdentityClient,
-    current_tenancy_id: str,
-) -> Dict[str, Any]:
-    compartment_list = {"Compartments": ""}
-    get_compartment_list_data_recurse(iam, compartment_list, current_tenancy_id)
-    return compartment_list
-
-
-def load_compartments(
-    neo4j_session: neo4j.Session,
-    compartments: List[Dict[str, Any]],
-    current_oci_tenancy_id: str,
-    oci_update_tag: int,
-) -> None:
-    ingest_compartment = """
-    MERGE (cnode:OCICompartment{ocid: $OCID})
-    ON CREATE SET cnode:OCICompartment, cnode.firstseen = timestamp(),
-    cnode.createdate = $CREATE_DATE
-    SET cnode.name = $NAME, cnode.compartmentid = $COMPARTMENT_ID
-    WITH cnode
-    MATCH (aa) WHERE (aa:OCITenancy OR aa:OCICompartment) AND aa.ocid=$COMPARTMENT_ID
-    MERGE (aa)-[r:OCI_COMPARTMENT]->(cnode)
-    ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $oci_update_tag
-    """
+def get_group_policy_info(session, group_name, policy_name):
+    client = session.client('iam')
+    return client.get_group_policy(GroupName=group_name, PolicyName=policy_name)
 
-    for compartment in compartments:
-        neo4j_session.run(
-            ingest_compartment,
-            OCID=compartment["id"],
-            COMPARTMENT_ID=compartment["compartment-id"],
-            DESCRIPTION=compartment["description"],
-            NAME=compartment["name"],
-            CREATE_DATE=compartment["time-created"],
-            OCI_TENANCY_ID=current_oci_tenancy_id,
-            oci_update_tag=oci_update_tag,
-        )
+
+def get_group_membership_data(session, group_name):
+    client = session.client('iam')
+    return client.get_group(GroupName=group_name)
+
+
+def get_user_list_data(session):
+    client = session.client('iam')
+    paginator = client.get_paginator('list_users')
+    users = []
+    for page in paginator.paginate():
+        users.extend(page['Users'])
+    return {'Users': users}
+
+
+def get_group_list_data(session):
+    client = session.client('iam')
+    paginator = client.get_paginator('list_groups')
+    groups = []
+    for page in paginator.paginate():
+        groups.extend(page['Groups'])
+    return {'Groups': groups}
+
+
+def get_policy_list_data(session):
+    client = session.client('iam')
+    paginator = client.get_paginator('list_policies')
+    policies = []
+    for page in paginator.paginate():
+        policies.extend(page['Policies'])
+    return {'Policies': policies}
+
+
+def get_role_list_data(session):
+    client = session.client('iam')
+    paginator = client.get_paginator('list_roles')
+    roles = []
+    for page in paginator.paginate():
+        roles.extend(page['Roles'])
+    return {'Roles': roles}
+
+
+def get_role_policies(session, role_name):
+    client = session.client('iam')
+    paginator = client.get_paginator('list_role_policies')
+    policy_names = []
+    for page in paginator.paginate(RoleName=role_name):
+        policy_names.extend(page['PolicyNames'])
+    return {'PolicyNames': policy_names}
+
+
+def get_role_policy_info(session, role_name, policy_name):
+    client = session.client('iam')
+    return client.get_role_policy(RoleName=role_name, PolicyName=policy_name)
+
+
+def get_account_access_key_data(session, username):
+    client = session.client('iam')
+    # NOTE we can get away without using a paginator here because users are limited to two access keys
+    return client.list_access_keys(UserName=username)
 
 
-def load_users(
-    neo4j_session: neo4j.Session,
-    users: List[Dict[str, Any]],
-    current_oci_tenancy_id: str,
-    oci_update_tag: int,
-) -> None:
+def load_users(session, users, current_aws_account_id, aws_update_tag):
     ingest_user = """
-    MERGE (unode:OCIUser{ocid: $OCID})
-    ON CREATE SET unode:OCIUser, unode.firstseen = timestamp(),
-    unode.createdate = $CREATE_DATE
-    SET unode.name = $USERNAME, unode.compartmentid = $COMPARTMENT_ID, unode.description = $DESCRIPTION,
-    unode.email = $EMAIL, unode.lifecycle_state = $LIFECYCLE_STATE, unode.is_mfa_activated = $IS_MFA_ACTIVATED,
-    unode.can_use_api_keys = $CAN_USE_API_KEYS, unode.can_use_auth_tokens = $CAN_USE_AUTH_TOKENS,
-    unode.can_use_console_password = $CAN_USE_CONSOLE_PASSWORD,
-    unode.can_use_customer_secret_keys = $CAN_USE_CUSTOMER_SECRET_KEYS,
-    unode.can_use_smtp_credentials = $CAN_USE_SMTP_CREDENTIALS,
-    unode.lastupdated = $oci_update_tag
+    MERGE (unode:AWSUser{arn: {ARN}})
+    ON CREATE SET unode:AWSPrincipal, unode.userid = {USERID}, unode.firstseen = timestamp(),
+    unode.createdate = {CREATE_DATE}
+    SET unode.name = {USERNAME}, unode.path = {PATH}, unode.passwordlastused = {PASSWORD_LASTUSED},
+    unode.lastupdated = {aws_update_tag}
     WITH unode
-    MATCH (aa:OCITenancy{ocid: $OCI_TENANCY_ID})
+    MATCH (aa:AWSAccount{id: {AWS_ACCOUNT_ID}})
     MERGE (aa)-[r:RESOURCE]->(unode)
     ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $oci_update_tag
+    SET r.lastupdated = {aws_update_tag}
     """
 
     for user in users:
-        neo4j_session.run(
+        session.run(
             ingest_user,
-            OCID=user["id"],
-            CREATE_DATE=str(user["time-created"]),
-            USERNAME=user["name"],
-            DESCRIPTION=user["description"],
-            EMAIL=user["email"],
-            LIFECYCLE_STATE=user["lifecycle-state"],
-            IS_MFA_ACTIVATED=user["is-mfa-activated"],
-            CAN_USE_API_KEYS=user["capabilities"]["can-use-api-keys"],
-            CAN_USE_AUTH_TOKENS=user["capabilities"]["can-use-auth-tokens"],
-            CAN_USE_CONSOLE_PASSWORD=user["capabilities"]["can-use-console-password"],
-            CAN_USE_CUSTOMER_SECRET_KEYS=user["capabilities"]["can-use-customer-secret-keys"],
-            CAN_USE_SMTP_CREDENTIALS=user["capabilities"]["can-use-smtp-credentials"],
-            COMPARTMENT_ID=user["compartment-id"],
-            OCI_TENANCY_ID=current_oci_tenancy_id,
-            oci_update_tag=oci_update_tag,
+            ARN=user["Arn"],
+            USERID=user["UserId"],
+            CREATE_DATE=str(user["CreateDate"]),
+            USERNAME=user["UserName"],
+            PATH=user["Path"],
+            PASSWORD_LASTUSED=str(user.get("PasswordLastUsed", "")),
+            AWS_ACCOUNT_ID=current_aws_account_id,
+            aws_update_tag=aws_update_tag,
         )
 
 
-def get_user_list_data(
-    iam: oci.identity.identity_client.IdentityClient,
-    current_tenancy_id: str,
-) -> Dict[str, List[Dict[str, Any]]]:
-    response = oci.pagination.list_call_get_all_results(iam.list_users, current_tenancy_id)
-    return {'Users': utils.oci_object_to_json(response.data)}
-
-
-def sync_users(
-    neo4j_session: neo4j.Session,
-    iam: oci.identity.identity_client.IdentityClient,
-    current_tenancy_id: str,
-    oci_update_tag: int,
-    common_job_parameters: Dict[str, Any],
-) -> None:
-    logger.debug("Syncing IAM users for account '%s'.", current_tenancy_id)
-    data = get_user_list_data(iam, current_tenancy_id)
-    load_users(neo4j_session, data['Users'], current_tenancy_id, oci_update_tag)
-    run_cleanup_job('oci_import_users_cleanup.json', neo4j_session, common_job_parameters)
-
-
-def get_group_list_data(
-    iam: oci.identity.identity_client.IdentityClient,
-    current_tenancy_id: str,
-) -> Dict[str, List[Dict[str, Any]]]:
-    response = oci.pagination.list_call_get_all_results(iam.list_groups, current_tenancy_id)
-    return {'Groups': utils.oci_object_to_json(response.data)}
-
-
-def load_groups(
-    neo4j_session: neo4j.Session,
-    groups: List[Dict[str, Any]],
-    current_tenancy_id: str,
-    oci_update_tag: int,
-) -> None:
+def load_groups(session, groups, current_aws_account_id, aws_update_tag):
     ingest_group = """
-    MERGE (gnode:OCIGroup{ocid: $OCID})
-    ON CREATE SET gnode.firstseen = timestamp(), gnode.createdate = $CREATE_DATE
-    SET gnode.name = $GROUP_NAME, gnode.compartmentid = $COMPARTMENT_ID, gnode.lastupdated = $oci_update_tag,
-    gnode.description = $DESCRIPTION
+    MERGE (gnode:AWSGroup{arn: {ARN}})
+    ON CREATE SET gnode.groupid = {GROUP_ID}, gnode.firstseen = timestamp(), gnode.createdate = {CREATE_DATE}
+    SET gnode.name = {GROUP_NAME}, gnode.path = {PATH},gnode.lastupdated = {aws_update_tag}
     WITH gnode
-    MATCH (aa:OCITenancy{ocid: $OCI_TENANCY_ID})
+    MATCH (aa:AWSAccount{id: {AWS_ACCOUNT_ID}})
     MERGE (aa)-[r:RESOURCE]->(gnode)
     ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $oci_update_tag
+    SET r.lastupdated = {aws_update_tag}
     """
 
     for group in groups:
-        neo4j_session.run(
+        session.run(
             ingest_group,
-            OCID=group["id"],
-            CREATE_DATE=str(group["time-created"]),
-            GROUP_NAME=group["name"],
-            COMPARTMENT_ID=group["compartment-id"],
-            DESCRIPTION=group["description"],
-            OCI_TENANCY_ID=current_tenancy_id,
-            oci_update_tag=oci_update_tag,
+            ARN=group["Arn"],
+            GROUP_ID=group["GroupId"],
+            CREATE_DATE=str(group["CreateDate"]),
+            GROUP_NAME=group["GroupName"],
+            PATH=group["Path"],
+            AWS_ACCOUNT_ID=current_aws_account_id,
+            aws_update_tag=aws_update_tag,
         )
 
 
-def sync_groups(
-    neo4j_session: neo4j.Session,
-    iam: oci.identity.identity_client.IdentityClient,
-    current_tenancy_id: str,
-    oci_update_tag: int,
-    common_job_parameters: Dict[str, Any],
-) -> None:
-    logger.debug("Syncing IAM groups for account '%s'.", current_tenancy_id)
-    data = get_group_list_data(iam, current_tenancy_id)
-    load_groups(neo4j_session, data["Groups"], current_tenancy_id, oci_update_tag)
-    run_cleanup_job('oci_import_groups_cleanup.json', neo4j_session, common_job_parameters)
-
-
-def get_group_membership_data(
-    iam: oci.identity.identity_client.IdentityClient,
-    group_id: str,
-    current_tenancy_id: str,
-) -> Dict[str, List[Dict[str, Any]]]:
-    response = oci.pagination.list_call_get_all_results(
-        iam.list_user_group_memberships, compartment_id=current_tenancy_id, group_id=group_id,
-    )
-    return {'GroupMemberships': utils.oci_object_to_json(response.data)}
+def load_policies(session, policies, current_aws_account_id, aws_update_tag):
+    ingest_policy = """
+    MERGE (pnode:AWSPolicy{arn: {ARN}})
+    ON CREATE SET pnode.policyid = {POLICY_ID}, pnode.firstseen = timestamp(), pnode.createdate = {CREATE_DATE}
+    SET pnode.name = {POLICY_NAME}, pnode.path = {PATH}, pnode.defaultversionid = {DEFAULT_VERSION_ID},
+    pnode.updatedate = {POLICY_UPDATE}, pnode.isattachable = {IS_ATTACHABLE},
+    pnode.attachmentcount = {ATTACHMENT_COUNT},
+    pnode.lastupdated = {aws_update_tag}
+    WITH pnode
+    MATCH (aa:AWSAccount{id: {AWS_ACCOUNT_ID}})
+    MERGE (aa)-[r:AWS_POLICY]->(pnode)
+    ON CREATE SET r.firstseen = timestamp()
+    SET r.lastupdated = {aws_update_tag}
+    """
 
+    for policy in policies:
+        session.run(
+            ingest_policy,
+            ARN=policy["Arn"],
+            POLICY_ID=policy["PolicyId"],
+            POLICY_NAME=policy["PolicyName"],
+            PATH=policy["Path"],
+            DEFAULT_VERSION_ID=policy["DefaultVersionId"],
+            CREATE_DATE=str(policy["CreateDate"]),
+            POLICY_UPDATE=str(policy["UpdateDate"]),
+            IS_ATTACHABLE=policy["IsAttachable"],
+            ATTACHMENT_COUNT=policy["AttachmentCount"],
+            AWS_ACCOUNT_ID=current_aws_account_id,
+            aws_update_tag=aws_update_tag,
+        )
 
-def sync_group_memberships(
-    neo4j_session: neo4j.Session,
-    iam: oci.identity.identity_client.IdentityClient,
-    current_tenancy_id: str,
-    oci_update_tag: int,
-    common_job_parameters: Dict[str, Any],
-) -> None:
-    logger.debug("Syncing IAM group membership for account '%s'.", current_tenancy_id)
-    query = "MATCH (group:OCIGroup)<-[:RESOURCE]-(OCITenancy{ocid: $OCI_TENANCY_ID}) " \
-            "return group.name as name, group.ocid as ocid;"
-    groups = neo4j_session.run(query, OCI_TENANCY_ID=current_tenancy_id)
-    groups_membership = {
-        group["ocid"]: get_group_membership_data(iam, group['ocid'], current_tenancy_id) for group in groups
-    }
-    load_group_memberships(neo4j_session, groups_membership, oci_update_tag)
-    run_cleanup_job(
-        'oci_import_groups_membership_cleanup.json',
-        neo4j_session,
-        common_job_parameters,
-    )
+
+def load_roles(session, roles, current_aws_account_id, aws_update_tag):
+    ingest_role = """
+    MERGE (rnode:AWSRole{arn: {Arn}})
+    ON CREATE SET rnode:AWSPrincipal, rnode.roleid = {RoleId}, rnode.firstseen = timestamp(),
+    rnode.createdate = {CreateDate}
+    ON MATCH SET rnode.name = {RoleName}, rnode.path = {Path}
+    SET rnode.lastupdated = {aws_update_tag}
+    WITH rnode
+    MATCH (aa:AWSAccount{id: {AWS_ACCOUNT_ID}})
+    MERGE (aa)-[r:AWS_ROLE]->(rnode)
+    ON CREATE SET r.firstseen = timestamp()
+    SET r.lastupdated = {aws_update_tag}
+    """
+
+    ingest_policy_statement = """
+    MERGE (spnnode:AWSPrincipal{arn: {SpnArn}})
+    ON CREATE SET spnnode.firstseen = timestamp()
+    SET spnnode.lastupdated = {aws_update_tag}, spnnode.type = {SpnType}
+    WITH spnnode
+    MATCH (role:AWSRole{arn: {RoleArn}})
+    MERGE (role)-[r:TRUSTS_AWS_PRINCIPAL]->(spnnode)
+    ON CREATE SET r.firstseen = timestamp()
+    SET r.lastupdated = {aws_update_tag}
+    """
+
+    # TODO support conditions
+
+    for role in roles:
+        session.run(
+            ingest_role,
+            Arn=role["Arn"],
+            RoleId=role["RoleId"],
+            CreateDate=str(role["CreateDate"]),
+            RoleName=role["RoleName"],
+            Path=role["Path"],
+            AWS_ACCOUNT_ID=current_aws_account_id,
+            aws_update_tag=aws_update_tag,
+        )
+
+        for statement in role["AssumeRolePolicyDocument"]["Statement"]:
+            principal = statement["Principal"]
+            principal_values = []
+            if 'AWS' in principal:
+                principal_type, principal_values = 'AWS', principal['AWS']
+            elif 'Service' in principal:
+                principal_type, principal_values = 'Service', principal['Service']
+            elif 'Federated' in principal:
+                principal_type, principal_values = 'Federated', principal['Federated']
+            if not isinstance(principal_values, list):
+                principal_values = [principal_values]
+            for principal_value in principal_values:
+                session.run(
+                    ingest_policy_statement,
+                    SpnArn=principal_value,
+                    SpnType=principal_type,
+                    RoleArn=role['Arn'],
+                    aws_update_tag=aws_update_tag,
+                )
 
 
-def load_group_memberships(
-    neo4j_session: neo4j.Session,
-    group_memberships: Dict[str, Any],
-    oci_update_tag: int,
-) -> None:
+def load_group_memberships(session, group_memberships, aws_update_tag):
     ingest_membership = """
-    MATCH (group:OCIGroup{ocid: $GROUP_OCID})
+    MATCH (group:AWSGroup{name: {GroupName}})
     WITH group
-    MATCH (user:OCIUser{ocid: $USER_OCID})
-    MERGE (user)-[r:MEMBER_OCID_GROUP]->(group)
+    MATCH (user:AWSUser{arn: {PrincipalArn}})
+    MERGE (user)-[r:MEMBER_AWS_GROUP]->(group)
     ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $oci_update_tag
+    SET r.lastupdated = {aws_update_tag}
     """
-    for group_ocid, membership_data in group_memberships.items():
-        for info in membership_data["GroupMemberships"]:
-            neo4j_session.run(
+
+    for group_name, membership_data in group_memberships.items():
+        for info in membership_data["Users"]:
+            principal_arn = info["Arn"]
+            session.run(
                 ingest_membership,
-                COMPARTMENT_ID=info["compartment-id"],
-                GROUP_OCID=info["group-id"],
-                USER_OCID=info["user-id"],
-                oci_update_tag=oci_update_tag,
+                GroupName=group_name,
+                PrincipalArn=principal_arn,
+                aws_update_tag=aws_update_tag,
             )
 
 
-def load_policies(
-    neo4j_session: neo4j.Session,
-    policies: List[Dict[str, Any]],
-    current_tenancy_id: str,
-    oci_update_tag: int,
-) -> None:
-    ingest_policy = """
-    MERGE (pnode:OCIPolicy{ocid: $OCID})
-    ON CREATE SET pnode.firstseen = timestamp(), pnode.createdate = $CREATE_DATE
-    SET pnode.name = $POLICY_NAME, pnode.compartmentid = $COMPARTMENT_ID, pnode.description = $DESCRIPTION,
-    pnode.statements = $STATEMENTS,
-    pnode.updatedate = $POLICY_UPDATE, pnode.lastupdated = $oci_update_tag
-    WITH pnode
-    MATCH (aa) WHERE (aa:OCITenancy OR aa:OCICompartment) AND aa.ocid=$COMPARTMENT_ID
-    MERGE (aa)-[r:OCI_POLICY]->(pnode)
+def _find_roles_assumable_in_policy(policy_data):
+    ret = []
+    statements = policy_data["PolicyDocument"]["Statement"]
+    if isinstance(statements, dict):
+        statements = [statements]
+    for statement in statements:
+        parsed_statement = policyuniverse.statement.Statement(statement)
+        if parsed_statement.effect == 'Allow' and 'sts:assumerole' in parsed_statement.actions_expanded:
+            ret.extend(list(parsed_statement.resources))
+    return ret
+
+
+def load_group_policies(session, group_policies, aws_update_tag):
+    ingest_policies_assume_role = """
+    MATCH (group:AWSGroup{name: {GroupName}})
+    WITH group
+    MERGE (role:AWSRole{arn: {RoleArn}})
+    ON CREATE SET role.firstseen = timestamp()
+    SET role.lastupdated = {aws_update_tag}
+    WITH role, group
+    MERGE (group)-[r:STS_ASSUMEROLE_ALLOW]->(role)
     ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $oci_update_tag
+    SET r.lastupdated = {aws_update_tag}
     """
 
-    for policy in policies:
-        neo4j_session.run(
-            ingest_policy,
-            OCID=policy["id"],
-            POLICY_NAME=policy["name"],
-            COMPARTMENT_ID=policy["compartment-id"],
-            DESCRIPTION=policy["description"],
-            STATEMENTS=policy["statements"],
-            CREATE_DATE=str(policy["time-created"]),
-            POLICY_UPDATE=str(policy["version-date"]),
-            OCI_TENANCY_ID=current_tenancy_id,
-            oci_update_tag=oci_update_tag,
-        )
-
+    for group_name, policies in group_policies.items():
+        for policy_name, policy_data in policies.items():
+            for role_arn in _find_roles_assumable_in_policy(policy_data):
+                # TODO resource ARNs may contain wildcards, e.g. arn:aws:iam::*:role/admin --
+                # TODO policyuniverse can't expand resource wildcards so further thought is needed here
+                session.run(
+                    ingest_policies_assume_role,
+                    GroupName=group_name,
+                    RoleArn=role_arn,
+                    aws_update_tag=aws_update_tag,
+                )
+
+
+def load_role_policies(session, role_policies, aws_update_tag):
+    ingest_policies_assume_role = """
+    MATCH (assumer:AWSRole{name: {RoleName}})
+    WITH assumer
+    MERGE (role:AWSRole{arn: {RoleArn}})
+    ON CREATE SET role.firstseen = timestamp()
+    SET role.lastupdated = {aws_update_tag}
+    WITH role, assumer
+    MERGE (assumer)-[r:STS_ASSUMEROLE_ALLOW]->(role)
+    ON CREATE SET r.firstseen = timestamp()
+    SET r.lastupdated = {aws_update_tag}
+    """
 
-def get_policy_list_data(
-    iam: oci.identity.identity_client.IdentityClient,
-    current_tenancy_id: str,
-) -> Dict[str, List[Dict[str, Any]]]:
-    response = oci.pagination.list_call_get_all_results(iam.list_policies, compartment_id=current_tenancy_id)
-    return {'Policies': utils.oci_object_to_json(response.data)}
-
-
-def sync_policies(
-    neo4j_session: neo4j.Session,
-    iam: oci.identity.identity_client.IdentityClient,
-    current_tenancy_id: str,
-    oci_update_tag: int,
-    common_job_parameters: Dict[str, Any],
-) -> None:
-    logger.debug("Syncing IAM policies for account '%s'.", current_tenancy_id)
-    compartments = utils.get_compartments_in_tenancy(neo4j_session, current_tenancy_id)
-    for compartment in compartments:
-        logger.debug(
-            "Syncing OCI policies for compartment '%s' in account '%s'.", compartment['ocid'], current_tenancy_id,
-        )
-        data = get_policy_list_data(iam, compartment["ocid"])
-        if (data["Policies"]):
-            load_policies(neo4j_session, data["Policies"], current_tenancy_id, oci_update_tag)
-    run_cleanup_job('oci_import_policies_cleanup.json', neo4j_session, common_job_parameters)
-
-
-def load_oci_policy_group_reference(
-    neo4j_session: neo4j.Session,
-    policy_id: str,
-    group_id: str,
-    tenancy_id: str,
-    oci_update_tag: int,
-) -> None:
-    ingest_policy_group_reference = """
-    MATCH (aa:OCIPolicy{ocid: $POLICY_ID})
-    MATCH (bb:OCIGroup{ocid: $GROUP_ID})
-    MERGE (aa)-[r:OCI_POLICY_REFERENCE]->(bb)
+    for role_name, policies in role_policies.items():
+        for policy_name, policy_data in policies.items():
+            for role_arn in _find_roles_assumable_in_policy(policy_data):
+                # TODO resource ARNs may contain wildcards, e.g. arn:aws:iam::*:role/admin --
+                # TODO policyuniverse can't expand resource wildcards so further thought is needed here
+                session.run(
+                    ingest_policies_assume_role,
+                    RoleName=role_name,
+                    RoleArn=role_arn,
+                    aws_update_tag=aws_update_tag,
+                )
+
+
+def load_user_access_keys(session, user_access_keys, aws_update_tag):
+    # TODO change the node label to reflect that this is a user access key, not an account access key
+    ingest_account_key = """
+    MATCH (user:AWSUser{name: {UserName}})
+    WITH user
+    MERGE (key:AccountAccessKey{accesskeyid: {AccessKeyId}})
+    ON CREATE SET key.firstseen = timestamp(), key.createdate = {CreateDate}
+    SET key.status = {Status}, key.lastupdated = {aws_update_tag}
+    WITH user,key
+    MERGE (user)-[r:AWS_ACCESS_KEY]->(key)
     ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $oci_update_tag
+    SET r.lastupdated = {aws_update_tag}
     """
-    neo4j_session.run(
-        ingest_policy_group_reference,
-        POLICY_ID=policy_id,
-        GROUP_ID=group_id,
-        oci_update_tag=oci_update_tag,
+
+    for username, access_keys in user_access_keys.items():
+        for key in access_keys["AccessKeyMetadata"]:
+            if key.get('AccessKeyId'):
+                session.run(
+                    ingest_account_key,
+                    UserName=username,
+                    AccessKeyId=key['AccessKeyId'],
+                    CreateDate=str(key['CreateDate']),
+                    Status=key['Status'],
+                    aws_update_tag=aws_update_tag,
+                )
+
+
+def sync_users(neo4j_session, boto3_session, current_aws_account_id, aws_update_tag, common_job_parameters):
+    logger.debug("Syncing IAM users for account '%s'.", current_aws_account_id)
+    data = get_user_list_data(boto3_session)
+    load_users(neo4j_session, data['Users'], current_aws_account_id, aws_update_tag)
+    run_cleanup_job('aws_import_users_cleanup.json', neo4j_session, common_job_parameters)
+
+
+def sync_groups(neo4j_session, boto3_session, current_aws_account_id, aws_update_tag, common_job_parameters):
+    logger.debug("Syncing IAM groups for account '%s'.", current_aws_account_id)
+    data = get_group_list_data(boto3_session)
+    load_groups(neo4j_session, data['Groups'], current_aws_account_id, aws_update_tag)
+    run_cleanup_job('aws_import_groups_cleanup.json', neo4j_session, common_job_parameters)
+
+
+def sync_policies(neo4j_session, boto3_session, current_aws_account_id, aws_update_tag, common_job_parameters):
+    logger.debug("Syncing IAM policies for account '%s'.", current_aws_account_id)
+    data = get_policy_list_data(boto3_session)
+    load_policies(neo4j_session, data['Policies'], current_aws_account_id, aws_update_tag)
+    run_cleanup_job('aws_import_policies_cleanup.json', neo4j_session, common_job_parameters)
+
+
+def sync_roles(neo4j_session, boto3_session, current_aws_account_id, aws_update_tag, common_job_parameters):
+    logger.debug("Syncing IAM roles for account '%s'.", current_aws_account_id)
+    data = get_role_list_data(boto3_session)
+    load_roles(neo4j_session, data['Roles'], current_aws_account_id, aws_update_tag)
+    run_cleanup_job('aws_import_roles_cleanup.json', neo4j_session, common_job_parameters)
+
+
+def sync_group_memberships(neo4j_session, boto3_session, current_aws_account_id, aws_update_tag, common_job_parameters):
+    logger.debug("Syncing IAM group membership for account '%s'.", current_aws_account_id)
+    query = "MATCH (group:AWSGroup)<-[:RESOURCE]-(AWSAccount{id: {AWS_ACCOUNT_ID}}) return group.name as name;"
+    result = neo4j_session.run(query, AWS_ACCOUNT_ID=current_aws_account_id)
+    groups = [r['name'] for r in result]
+    groups_membership = {name: get_group_membership_data(boto3_session, name) for name in groups}
+    load_group_memberships(neo4j_session, groups_membership, aws_update_tag)
+    run_cleanup_job(
+        'aws_import_groups_membership_cleanup.json',
+        neo4j_session,
+        common_job_parameters,
     )
 
 
-def load_oci_policy_compartment_reference(
-    neo4j_session: neo4j.Session,
-    policy_id: str,
-    compartment_id: str,
-    tenancy_id: str,
-    oci_update_tag: int,
-) -> None:
-    ingest_policy_compartment_reference = """
-    MATCH (aa:OCIPolicy{ocid: $POLICY_ID})
-    MATCH (bb:OCICompartment{ocid: $COMPARTMENT_ID})
-    MERGE (aa)-[r:OCI_POLICY_REFERENCE]->(bb)
-    ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $oci_update_tag
-    """
-    neo4j_session.run(
-        ingest_policy_compartment_reference,
-        POLICY_ID=policy_id,
-        COMPARTMENT_ID=compartment_id,
-        oci_update_tag=oci_update_tag,
+def sync_group_policies(neo4j_session, boto3_session, current_aws_account_id, aws_update_tag, common_job_parameters):
+    logger.debug("Syncing IAM group policies for account '%s'.", current_aws_account_id)
+    query = "MATCH (group:AWSGroup)<-[:RESOURCE]-(AWSAccount{id: {AWS_ACCOUNT_ID}}) return group.name as name;"
+    result = neo4j_session.run(query, AWS_ACCOUNT_ID=current_aws_account_id)
+    groups = [r['name'] for r in result]
+    groups_policies = {}
+    for group_name in groups:
+        groups_policies[group_name] = {}
+        for policy_name in get_group_policies(boto3_session, group_name)['PolicyNames']:
+            groups_policies[group_name][policy_name] = get_group_policy_info(boto3_session, group_name, policy_name)
+    load_group_policies(neo4j_session, groups_policies, aws_update_tag)
+    run_cleanup_job(
+        'aws_import_groups_policy_cleanup.json',
+        neo4j_session,
+        common_job_parameters,
     )
 
 
-# Parse the statements inside OCI Policies and load the corresponding relationships they reference.
-def sync_oci_policy_references(
-    neo4j_session: neo4j.Session,
-    tenancy_id: str,
-    oci_update_tag: int,
-    common_job_parameters: Dict[str, Any],
-) -> None:
-    groups = list(utils.get_groups_in_tenancy(neo4j_session, tenancy_id))
-    compartments = list(utils.get_compartments_in_tenancy(neo4j_session, tenancy_id))
-    policies = list(utils.get_policies_in_tenancy(neo4j_session, tenancy_id))
-    for policy in policies:
-        check_compart = policy["compartmentid"]
-        for statement in policy["statements"]:
-            m = re.search('(?<=group\\s)[^ ]*(?=\\s)', statement)
-            if m:
-                for group in groups:
-                    if group["name"].lower() == m.group(0).lower():
-                        load_oci_policy_group_reference(
-                            neo4j_session, policy["ocid"], group["ocid"], tenancy_id, oci_update_tag,
-                        )
-            m = re.search('(?<=compartment\\s)[^ ]*(?=$)', statement)
-            if m:
-                for compartment in compartments:
-                    # Only look at the compartment or subcompartment name referenced in the policy statement
-                    # in which the policy is a member of.
-                    if compartment["ocid"] == check_compart or compartment["compartmentid"] == check_compart:
-                        if compartment["name"].lower() == m.group(0).lower():
-                            load_oci_policy_compartment_reference(
-                                neo4j_session, policy["ocid"], compartment['ocid'], tenancy_id, oci_update_tag,
-                            )
-
-
-def get_region_subscriptions_list_data(
-    iam: oci.identity.identity_client.IdentityClient,
-    current_tenancy_id: str,
-) -> Dict[str, List[Dict[str, Any]]]:
-    response = oci.pagination.list_call_get_all_results(iam.list_region_subscriptions, current_tenancy_id)
-    return {'RegionSubscriptions': utils.oci_object_to_json(response.data)}
-
-
-def load_region_subscriptions(
-    neo4j_session: neo4j.Session,
-    regions: List[Dict[str, Any]],
-    tenancy_id: str,
-    oci_update_tag: int,
-) -> None:
+def sync_role_policies(neo4j_session, boto3_session, current_aws_account_id, aws_update_tag, common_job_parameters):
+    logger.debug("Syncing IAM role policies for account '%s'.", current_aws_account_id)
     query = """
-    MERGE (aa:OCIRegion{key: $REGION_KEY})
-    ON CREATE SET aa.firstseen = timestamp()
-    SET aa.lastupdated = $oci_update_tag, aa.name = $REGION_NAME
-    WITH aa
-    MATCH (bb:OCITenancy{ocid: $OCI_TENANCY_ID})
-    MERGE (bb)-[r:OCI_REGION_SUBSCRIPTION]->(aa)
-    ON CREATE SET r.firstseen = timestamp()
-    SET r.lastupdated = $oci_update_tag
+    MATCH (role:AWSRole)<-[:AWS_ROLE]-(AWSAccount{id: {AWS_ACCOUNT_ID}})
+    WHERE exists(role.name)
+    RETURN role.name AS name;
     """
-    for region in regions:
-        neo4j_session.run(
-            query,
-            REGION_KEY=region["region-key"],
-            REGION_NAME=region["region-name"],
-            oci_update_tag=oci_update_tag,
-            OCI_TENANCY_ID=tenancy_id,
-        )
+    result = neo4j_session.run(query, AWS_ACCOUNT_ID=current_aws_account_id)
+    roles = [r['name'] for r in result]
+    roles_policies = {}
+    for role_name in roles:
+        roles_policies[role_name] = {}
+        for policy_name in get_role_policies(boto3_session, role_name)['PolicyNames']:
+            roles_policies[role_name][policy_name] = get_role_policy_info(boto3_session, role_name, policy_name)
+    load_role_policies(neo4j_session, roles_policies, aws_update_tag)
+    run_cleanup_job(
+        'aws_import_roles_policy_cleanup.json',
+        neo4j_session,
+        common_job_parameters,
+    )
+
+
+def sync_user_access_keys(neo4j_session, boto3_session, current_aws_account_id, aws_update_tag, common_job_parameters):
+    logger.debug("Syncing IAM user access keys for account '%s'.", current_aws_account_id)
+    query = "MATCH (user:AWSUser)<-[:RESOURCE]-(AWSAccount{id: {AWS_ACCOUNT_ID}}) return user.name as name"
+    result = neo4j_session.run(query, AWS_ACCOUNT_ID=current_aws_account_id)
+    usernames = [r['name'] for r in result]
+    account_access_key = {name: get_account_access_key_data(boto3_session, name) for name in usernames}
+    load_user_access_keys(neo4j_session, account_access_key, aws_update_tag)
+    run_cleanup_job(
+        'aws_import_account_access_key_cleanup.json',
+        neo4j_session,
+        common_job_parameters,
+    )
 
 
-def sync_region_subscriptions(
-    neo4j_session: neo4j.Session,
-    iam: oci.identity.identity_client.IdentityClient,
-    current_tenancy_id: str,
-    oci_update_tag: int,
-    common_job_parameters: Dict[str, Any],
-) -> None:
-    logger.debug("Syncing IAM region subscriptions for account '%s'.", current_tenancy_id)
-    data = get_region_subscriptions_list_data(iam, current_tenancy_id)
-    load_region_subscriptions(neo4j_session, data["RegionSubscriptions"], current_tenancy_id, oci_update_tag)
-    # run_cleanup_job('oci_import_region_subscriptions_cleanup.json', neo4j_session, common_job_parameters)
-
-
-def sync(
-    neo4j_session: neo4j.Session,
-    iam: oci.identity.identity_client.IdentityClient,
-    tenancy_id: str,
-    oci_update_tag: int,
-    common_job_parameters: Dict[str, Any],
-) -> None:
-    logger.info("Syncing IAM for account '%s'.", tenancy_id)
-    sync_users(neo4j_session, iam, tenancy_id, oci_update_tag, common_job_parameters)
-    sync_groups(neo4j_session, iam, tenancy_id, oci_update_tag, common_job_parameters)
-    sync_group_memberships(neo4j_session, iam, tenancy_id, oci_update_tag, common_job_parameters)
-    sync_compartments(neo4j_session, iam, tenancy_id, oci_update_tag, common_job_parameters)
-    sync_policies(neo4j_session, iam, tenancy_id, oci_update_tag, common_job_parameters)
-    sync_oci_policy_references(neo4j_session, tenancy_id, oci_update_tag, common_job_parameters)
-    sync_region_subscriptions(neo4j_session, iam, tenancy_id, oci_update_tag, common_job_parameters)
+def sync(neo4j_session, boto3_session, account_id, update_tag, common_job_parameters):
+    logger.info("Syncing IAM for account '%s'.", account_id)
+    sync_users(neo4j_session, boto3_session, account_id, update_tag, common_job_parameters)
+    sync_groups(neo4j_session, boto3_session, account_id, update_tag, common_job_parameters)
+    sync_policies(neo4j_session, boto3_session, account_id, update_tag, common_job_parameters)
+    sync_roles(neo4j_session, boto3_session, account_id, update_tag, common_job_parameters)
+    sync_group_memberships(neo4j_session, boto3_session, account_id, update_tag, common_job_parameters)
+    sync_group_policies(neo4j_session, boto3_session, account_id, update_tag, common_job_parameters)
+    sync_role_policies(neo4j_session, boto3_session, account_id, update_tag, common_job_parameters)
+    sync_user_access_keys(neo4j_session, boto3_session, account_id, update_tag, common_job_parameters)
+    run_cleanup_job('aws_import_principals_cleanup.json', neo4j_session, common_job_parameters)
```

### Comparing `cartography-0.81.0/cartography/sync.py` & `cartography-0.9.0/cartography/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,237 +1,181 @@
 import argparse
+import getpass
 import logging
-import time
-from collections import OrderedDict
-from typing import Callable
-from typing import List
-from typing import Tuple
-from typing import Union
-
-import neo4j.exceptions
-from neo4j import GraphDatabase
-from statsd import StatsClient
-
-import cartography.intel.analysis
-import cartography.intel.aws
-import cartography.intel.azure
-import cartography.intel.bigfix
-import cartography.intel.create_indexes
-import cartography.intel.crowdstrike
-import cartography.intel.crxcavator.crxcavator
-import cartography.intel.cve
-import cartography.intel.digitalocean
-import cartography.intel.duo
-import cartography.intel.gcp
-import cartography.intel.github
-import cartography.intel.gsuite
-import cartography.intel.kubernetes
-import cartography.intel.lastpass
-import cartography.intel.oci
-import cartography.intel.okta
-from cartography.config import Config
-from cartography.stats import set_stats_client
-from cartography.util import STATUS_FAILURE
-from cartography.util import STATUS_SUCCESS
-
-logger = logging.getLogger(__name__)
-
-
-TOP_LEVEL_MODULES = OrderedDict({  # preserve order so that the default sync always runs `analysis` at the very end
-    'create-indexes': cartography.intel.create_indexes.run,
-    'aws': cartography.intel.aws.start_aws_ingestion,
-    'azure': cartography.intel.azure.start_azure_ingestion,
-    'crowdstrike': cartography.intel.crowdstrike.start_crowdstrike_ingestion,
-    'gcp': cartography.intel.gcp.start_gcp_ingestion,
-    'gsuite': cartography.intel.gsuite.start_gsuite_ingestion,
-    'crxcavator': cartography.intel.crxcavator.start_extension_ingestion,
-    'cve': cartography.intel.cve.start_cve_ingestion,
-    'oci': cartography.intel.oci.start_oci_ingestion,
-    'okta': cartography.intel.okta.start_okta_ingestion,
-    'github': cartography.intel.github.start_github_ingestion,
-    'digitalocean': cartography.intel.digitalocean.start_digitalocean_ingestion,
-    'kubernetes': cartography.intel.kubernetes.start_k8s_ingestion,
-    'lastpass': cartography.intel.lastpass.start_lastpass_ingestion,
-    'bigfix': cartography.intel.bigfix.start_bigfix_ingestion,
-    'duo': cartography.intel.duo.start_duo_ingestion,
-    'analysis': cartography.intel.analysis.run,
-})
+import os
+import sys
 
+import cartography.sync
 
-class Sync:
-    """
-    A cartography sync task.
-
-    The role of the sync task is to ensure the data in the graph database represents reality. It does this by executing
-    a sequence of sync "stages" which are responsible for retrieving data from various sources (APIs, files, etc.),
-    pushing that data to Neo4j, and removing now-invalid nodes and relationships from the graph. An instance of this
-    class can be configured to run any number of stages in a specific order.
-    """
 
-    def __init__(self):
-        # NOTE we may need meta-stages at some point to allow hooking into pre-sync, sync, and post-sync
-        self._stages = OrderedDict()
-
-    def add_stage(self, name: str, func: Callable) -> None:
-        """
-        Add one stage to the sync task.
-
-        :type name: string
-        :param name: The name of the stage.
-        :type func: Callable
-        :param func: The object to call when the stage is executed.
-        """
-        self._stages[name] = func
-
-    def add_stages(self, stages: List[Tuple[str, Callable]]) -> None:
-        """
-        Add multiple stages to the sync task.
-
-        :type stages: List[Tuple[string, Callable]]
-        :param stages: A list of stage names and stage callable pairs.
-        """
-        for name, func in stages:
-            self.add_stage(name, func)
-
-    def run(self, neo4j_driver: neo4j.Driver, config: Union[Config, argparse.Namespace]) -> int:
-        """
-        Execute all stages in the sync task in sequence.
-
-        :type neo4j_driver: neo4j.Driver
-        :param neo4j_driver: Neo4j driver object.
-        :type config: cartography.config.Config
-        :param config: Configuration for the sync run.
-        """
-        logger.info("Starting sync with update tag '%d'", config.update_tag)
-        with neo4j_driver.session(database=config.neo4j_database) as neo4j_session:
-            for stage_name, stage_func in self._stages.items():
-                logger.info("Starting sync stage '%s'", stage_name)
-                try:
-                    stage_func(neo4j_session, config)
-                except (KeyboardInterrupt, SystemExit):
-                    logger.warning("Sync interrupted during stage '%s'.", stage_name)
-                    raise
-                except Exception:
-                    logger.exception("Unhandled exception during sync stage '%s'", stage_name)
-                    raise  # TODO this should be configurable
-                logger.info("Finishing sync stage '%s'", stage_name)
-        logger.info("Finishing sync with update tag '%d'", config.update_tag)
-        return STATUS_SUCCESS
+logger = logging.getLogger(__name__)
 
 
-def run_with_config(sync: Sync, config: Union[Config, argparse.Namespace]) -> int:
+class CLI:
     """
-    Execute the cartography.sync.Sync.run method with parameters built from the given configuration object.
-
-    This function will create a Neo4j driver object from the given Neo4j configuration options (URI, auth, etc.) and
-    will choose a sensible update tag if one is not specified in the given configuration.
-
     :type sync: cartography.sync.Sync
-    :param sync: A sync task to run.
-    :type config: cartography.config.Config
-    :param config: The configuration to use to run the sync task.
-    """
-    # Initialize statsd client if enabled
-    if config.statsd_enabled:
-        set_stats_client(
-            StatsClient(
-                host=config.statsd_host,
-                port=config.statsd_port,
-                prefix=config.statsd_prefix,
+    :param sync: A sync task for the command line program to execute.
+    :type prog: string
+    :param prog: The name of the command line program. This will be displayed in usage and help output.
+    """
+
+    def __init__(self, sync, prog=None):
+        self.prog = prog
+        self.sync = sync
+        self.parser = self._build_parser()
+
+    def _build_parser(self):
+        """
+        :rtype: argparse.ArgumentParser
+        :return: A cartography argument parser. Calling parse_args on the argument parser will return an object which
+            implements the cartography.config.Config interface.
+        """
+        parser = argparse.ArgumentParser(
+            prog=self.prog,
+            description=(
+                "cartography consolidates infrastructure assets and the relationships between them in an intuitive "
+                "graph view. This application can be used to pull configuration data from multiple sources, load it "
+                "in to Neo4j, and run arbitrary enrichment and analysis on that data. Please make sure you have Neo4j "
+                "running and have configured AWS credentials with the SecurityAudit IAM policy before getting started. "
+                "Running cartography with no parameters will execute a simple sync against a Neo4j instance running "
+                "locally. It will use your default AWS credentials and will not execute and post-sync analysis jobs. "
+                "Please see the per-parameter documentation below for information on how to connect to different Neo4j "
+                "instances, use auth when communicating with Neo4j, sync data from multiple AWS accounts, and execute "
+                "arbitrary analysis jobs after the conclusion of the sync."
             ),
+            epilog='For more documentation please visit: https://github.com/lyft/cartography',
         )
+        parser.add_argument(
+            '-v',
+            '--verbose',
+            action='store_true',
+            help='Enable verbose logging for cartography.',
+        )
+        parser.add_argument(
+            '-q',
+            '--quiet',
+            action='store_true',
+            help='Restrict cartography logging to warnings and errors only.',
+        )
+        parser.add_argument(
+            '--neo4j-uri',
+            type=str,
+            default='bolt://localhost:7687',
+            help=(
+                'A valid Neo4j URI to sync against. See '
+                'https://neo4j.com/docs/api/python-driver/current/driver.html#uri for complete documentation on the '
+                'structure of a Neo4j URI.'
+            ),
+        )
+        parser.add_argument(
+            '--neo4j-user',
+            type=str,
+            default=None,
+            help='A username with which to authenticate to Neo4j.',
+        )
+        parser.add_argument(
+            '--neo4j-password-env-var',
+            type=str,
+            default=None,
+            help='The name of an environment variable containing a password with which to authenticate to Neo4j.',
+        )
+        parser.add_argument(
+            '--neo4j-password-prompt',
+            action='store_true',
+            help=(
+                'Present an interactive prompt for a password with which to authenticate to Neo4j. This parameter '
+                'supersedes other methods of supplying a Neo4j password.'
+            ),
+        )
+        # TODO add the below parameters to a 'sync' subparser
+        parser.add_argument(
+            '--update-tag',
+            type=int,
+            default=None,
+            help=(
+                'A unique tag to apply to all Neo4j nodes and relationships created or updated during the sync run. '
+                'This tag is used by cleanup jobs to identify nodes and relationships that are stale and need to be '
+                'removed from the graph. By default, cartography will use a UNIX timestamp as the update tag.'
+            ),
+        )
+        parser.add_argument(
+            '--aws-sync-all-profiles',
+            action='store_true',
+            help=(
+                'Enable AWS sync for all discovered named profiles. When this parameter is supplied cartography will '
+                'discover all configured AWS named profiles (see '
+                'https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-profiles.html) and run the AWS sync '
+                'job for each profile not named "default". If this parameter is not supplied, cartography will use the '
+                'default AWS credentials available in your environment to run the AWS sync once. When using this '
+                'parameter it is suggested that you create an AWS config file containing a named profile for each AWS '
+                'account you want to sync and use the AWS_CONFIG_FILE environment variable to point to that config '
+                'file (see https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-envvars.html). cartography '
+                'respects the AWS CLI/SDK environment variables and does not override them.'
+            ),
+        )
+        parser.add_argument(
+            '--analysis-job-directory',
+            type=str,
+            default=None,
+            help=(
+                'A path to a directory containing analysis jobs to run at the conclusion of the sync. cartography will '
+                'discover all JSON files in the given directory (and its subdirectories) and pass them to the GraphJob '
+                'API to execute against the graph. This allows you to apply data transformation and augmentation at '
+                'the end of a sync run without writing code. cartography does not guarantee the order in which the '
+                'jobs are executed.'
+            ),
+        )
+        return parser
 
-    neo4j_auth = None
-    if config.neo4j_user or config.neo4j_password:
-        neo4j_auth = (config.neo4j_user, config.neo4j_password)
-    try:
-        neo4j_driver = GraphDatabase.driver(
-            config.neo4j_uri,
-            auth=neo4j_auth,
-            max_connection_lifetime=config.neo4j_max_connection_lifetime,
-        )
-    except neo4j.exceptions.ServiceUnavailable as e:
-        logger.debug("Error occurred during Neo4j connect.", exc_info=True)
-        logger.error(
-            (
-                "Unable to connect to Neo4j using the provided URI '%s', an error occurred: '%s'. Make sure the Neo4j "
-                "server is running and accessible from your network."
-            ),
-            config.neo4j_uri,
-            e,
-        )
-        return STATUS_FAILURE
-    except neo4j.exceptions.AuthError as e:
-        logger.debug("Error occurred during Neo4j auth.", exc_info=True)
-        if not neo4j_auth:
-            logger.error(
-                (
-                    "Unable to auth to Neo4j, an error occurred: '%s'. cartography attempted to connect to Neo4j "
-                    "without any auth. Check your Neo4j server settings to see if auth is required and, if it is, "
-                    "provide cartography with a valid username and password."
-                ),
-                e,
-            )
-        else:
-            logger.error(
-                (
-                    "Unable to auth to Neo4j, an error occurred: '%s'. cartography attempted to connect to Neo4j with "
-                    "a username and password. Check your Neo4j server settings to see if the username and password "
-                    "provided to cartography are valid credentials."
-                ),
-                e,
-            )
-        return STATUS_FAILURE
-    default_update_tag = int(time.time())
-    if not config.update_tag:
-        config.update_tag = default_update_tag
-    return sync.run(neo4j_driver, config)
-
-
-def build_default_sync() -> Sync:
-    """
-    Build the default cartography sync, which runs all intelligence modules shipped with the cartography package.
+    def main(self, argv):
+        """
+        Entrypoint for the command line interface.
 
-    :rtype: cartography.sync.Sync
-    :return: The default cartography sync object.
-    """
-    sync = Sync()
-    sync.add_stages([
-        (stage_name, stage_func) for stage_name, stage_func in TOP_LEVEL_MODULES.items()
-    ])
-    return sync
+        :type argv: string
+        :param argv: The parameters supplied to the command line program.
+        """
+        # TODO support parameter lookup in environment variables if not present on command line
+        config = self.parser.parse_args(argv)
+        if config.verbose:
+            logging.getLogger('cartography').setLevel(logging.DEBUG)
+        elif config.quiet:
+            logging.getLogger('cartography').setLevel(logging.WARNING)
+        else:
+            logging.getLogger('cartography').setLevel(logging.INFO)
+        logger.debug("Launching cartography with CLI configuration: %r", vars(config))
+        if config.neo4j_user:
+            config.neo4j_password = None
+            if config.neo4j_password_prompt:
+                logger.info("Reading password for Neo4j user '%s' interactively.", config.neo4j_user)
+                config.neo4j_password = getpass.getpass()
+            elif config.neo4j_password_env_var:
+                logger.debug(
+                    "Reading password for Neo4j user '%s' from environment variable '%s'.",
+                    config.neo4j_user,
+                    config.neo4j_password_env_var,
+                )
+                config.neo4j_password = os.environ.get(config.neo4j_password_env_var)
+            if not config.neo4j_password:
+                logger.warning("Neo4j username was provided but a password could not be found.")
+        else:
+            config.neo4j_password = None
+        try:
+            return cartography.sync.run_with_config(self.sync, config)
+        except KeyboardInterrupt:
+            return 130
 
 
-def parse_and_validate_selected_modules(selected_modules: str) -> List[str]:
-    """
-    Ensures that user-selected modules passed through the CLI are valid and parses them to a list of str.
-    :param selected_modules: comma separated string of module names provided by user
-    :return: A validated list of module names that we will run
+def main(argv=None):
     """
-    validated_modules: List[str] = []
-    for module in selected_modules.split(','):
-        module = module.strip()
-
-        if module in TOP_LEVEL_MODULES.keys():
-            validated_modules.append(module)
-        else:
-            valid_modules = ', '.join(TOP_LEVEL_MODULES.keys())
-            raise ValueError(
-                f'Error parsing `selected_modules`. You specified "{selected_modules}". '
-                f'Please check that your string is formatted properly. '
-                f'Example valid input looks like "aws,gcp,analysis" or "azure, oci, crowdstrike". '
-                f'Our full list of valid values is: {valid_modules}.',
-            )
-    return validated_modules
+    Entrypoint for the default cartography command line interface.
 
+    This entrypoint build and executed the default cartography sync. See cartography.sync.build_default_sync.
 
-def build_sync(selected_modules_as_str: str) -> Sync:
-    """
-    Returns a cartography sync object where all the sync stages are from the user-specified comma separated list of
-    modules to run.
+    :rtype: int
+    :return: The return code.
     """
-    selected_modules = parse_and_validate_selected_modules(selected_modules_as_str)
-    sync = Sync()
-    sync.add_stages(
-        [(sync_name, TOP_LEVEL_MODULES[sync_name]) for sync_name in selected_modules],
-    )
-    return sync
+    logging.basicConfig(level=logging.INFO)
+    logging.getLogger('neo4j.bolt').setLevel(logging.WARNING)
+    logging.getLogger('botocore').setLevel(logging.WARNING)
+    argv = argv if argv is not None else sys.argv[1:]
+    default_sync = cartography.sync.build_default_sync()
+    return CLI(default_sync, prog='cartography').main(argv)
```

### Comparing `cartography-0.81.0/cartography.egg-info/PKG-INFO` & `cartography-0.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: cartography
-Version: 0.81.0
+Version: 0.9.0
 Summary: Explore assets and their relationships across your technical infrastructure.
 Home-page: https://www.github.com/lyft/cartography
 Maintainer: Lyft
 Maintainer-email: security@lyft.com
 License: apache2
+Description: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE
-
-file: README.md
```

### Comparing `cartography-0.81.0/setup.py` & `cartography-0.9.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,46 @@
 from setuptools import find_packages
 from setuptools import setup
 
-__version__ = '0.81.0'
+__version__ = '0.9.0'
 
 
 setup(
     name='cartography',
     version=__version__,
     description='Explore assets and their relationships across your technical infrastructure.',
-    long_description='file: README.md',
-    long_description_content_type='text/markdown',
     url='https://www.github.com/lyft/cartography',
     maintainer='Lyft',
     maintainer_email='security@lyft.com',
     license='apache2',
     packages=find_packages(exclude=['tests*']),
     package_data={
-        'cartography': ['py.typed'],
         'cartography.data': [
             '*.cypher',
-            '*.yaml',
         ],
         'cartography.data.jobs.analysis': [
             '*.json',
         ],
         'cartography.data.jobs.cleanup': [
             '*.json',
         ],
     },
     dependency_links=[],
     install_requires=[
-        "backoff>=2.1.2",
-        "boto3>=1.15.1",
-        "botocore>=1.18.1",
+        "boto3>=1.7.0",
+        "botocore>=1.12.0",
         "dnspython>=1.15.0",
-        "neo4j>=4.4.4,<5.0.0",
+        "neo4j-driver>=1.7.0",
+        "neobolt>=1.7.0",
         "policyuniverse>=1.1.0.0",
+        "python-dateutil>=2.7.0",
         "google-api-python-client>=1.7.8",
         "oauth2client>=4.1.3",
         "marshmallow>=3.0.0rc7",
-        "oci>=2.71.0",
-        "okta<1.0.0",
-        "pyyaml>=5.3.1",
         "requests>=2.22.0",
-        "statsd",
-        "packaging",
-        "python-digitalocean>=1.16.0",
-        "adal>=1.2.4",
-        "azure-cli-core>=2.26.0",
-        "azure-mgmt-compute>=5.0.0",
-        "azure-mgmt-resource>=10.2.0",
-        "azure-mgmt-cosmosdb>=6.0.0",
-        "msrestazure >= 0.6.4",
-        "azure-mgmt-storage>=16.0.0",
-        "azure-mgmt-sql<=1.0.0",
-        "azure-identity>=1.5.0",
-        "kubernetes>=22.6.0",
-        "pdpyras>=4.3.0",
-        "crowdstrike-falconpy>=0.5.1",
-        "python-dateutil",
-        "xmltodict",
-        "duo-client",
     ],
     extras_require={
         ':python_version<"3.7"': [
             "importlib-resources",
         ],
     },
     entry_points={
@@ -76,13 +52,13 @@
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.6',
         'Topic :: Security',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
 )
```

