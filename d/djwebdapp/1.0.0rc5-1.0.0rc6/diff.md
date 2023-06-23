# Comparing `tmp/djwebdapp-1.0.0rc5.tar.gz` & `tmp/djwebdapp-1.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djwebdapp-1.0.0rc5.tar", last modified: Fri Feb 17 13:15:37 2023, max compression
+gzip compressed data, was "djwebdapp-1.0.0rc6.tar", last modified: Thu Feb 23 14:59:50 2023, max compression
```

## Comparing `djwebdapp-1.0.0rc5.tar` & `djwebdapp-1.0.0rc6.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.416944 djwebdapp-1.0.0rc5/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5103 2023-02-17 13:15:37.416944 djwebdapp-1.0.0rc5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3715 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-17 13:15:37.416944 djwebdapp-1.0.0rc5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1199 2023-02-17 13:15:36.000000 djwebdapp-1.0.0rc5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.400277 djwebdapp-1.0.0rc5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.400277 djwebdapp-1.0.0rc5/src/djwebdapp/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1940 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.403611 djwebdapp-1.0.0rc5/src/djwebdapp/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.403611 djwebdapp-1.0.0rc5/src/djwebdapp/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/management/commands/history_download.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/management/commands/index.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/management/commands/normalize.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/management/commands/refresh_balances.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/management/commands/spool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.406944 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     7904 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0002_alter_transaction_receiver_alter_transaction_sender.py
--rw-rw-rw-   0 root         (0) root         (0)      741 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0003_transaction_txgroup_alter_transaction_hash_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0004_alter_transaction_options.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0005_alter_transaction_unique_together_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0006_blockchain_min_confirmations_alter_transaction_state.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0007_alter_transaction_amount.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0008_transaction_index.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0009_account_index.py
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0010_alter_transaction_nonce.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0011_rename_max_level_blockchain_index_level.py
--rw-rw-rw-   0 root         (0) root         (0)      437 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0012_transaction_number.py
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0013_transaction_normalized_dependency.py
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0014_alter_account_unique_together.py
--rw-rw-rw-   0 root         (0) root         (0)      974 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0015_alter_transaction_state.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19402 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/models.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/normalizers.py
--rw-rw-rw-   0 root         (0) root         (0)     9416 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/provider.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.403611 djwebdapp-1.0.0rc5/src/djwebdapp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5103 2023-02-17 13:15:37.000000 djwebdapp-1.0.0rc5/src/djwebdapp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4886 2023-02-17 13:15:37.000000 djwebdapp-1.0.0rc5/src/djwebdapp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-17 13:15:37.000000 djwebdapp-1.0.0rc5/src/djwebdapp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      514 2023-02-17 13:15:37.000000 djwebdapp-1.0.0rc5/src/djwebdapp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-02-17 13:15:37.000000 djwebdapp-1.0.0rc5/src/djwebdapp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.406944 djwebdapp-1.0.0rc5/src/djwebdapp_ethereum/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_ethereum/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_ethereum/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_ethereum/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.406944 djwebdapp-1.0.0rc5/src/djwebdapp_ethereum/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1274 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_ethereum/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_ethereum/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      918 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_ethereum/models.py
--rw-rw-rw-   0 root         (0) root         (0)     7102 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_ethereum/provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.406944 djwebdapp-1.0.0rc5/src/djwebdapp_example/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/balance.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/balance_update.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/deploy_fa12.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.410277 djwebdapp-1.0.0rc5/src/djwebdapp_example/ethereum/
--rw-rw-rw-   0 root         (0) root         (0)      486 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/ethereum/blockchain.py
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/ethereum/client.py
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/ethereum/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/ethereum/deploy_contract.py
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/ethereum/index.py
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/ethereum/load.py
--rw-rw-rw-   0 root         (0) root         (0)     1651 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/ethereum/mint_normalize.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/ethereum/normalize.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/ethereum/transfer.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/ethereum/wallet_import.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.410277 djwebdapp-1.0.0rc5/src/djwebdapp_example/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2586 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2969 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/models.py
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/spool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.413611 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/
--rw-rw-rw-   0 root         (0) root         (0)     6019 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/FA12.json
--rw-rw-rw-   0 root         (0) root         (0)      940 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/FA12.py
--rw-rw-rw-   0 root         (0) root         (0)      725 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/Proxy.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/blockchain.py
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/call_parallel.py
--rw-rw-rw-   0 root         (0) root         (0)    23855 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/callee.json
--rw-rw-rw-   0 root         (0) root         (0)      670 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/callee.py
--rw-rw-rw-   0 root         (0) root         (0)    31361 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/caller.json
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/caller.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/client.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)     1055 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/deploy_contract.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/index.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/load.py
--rw-rw-rw-   0 root         (0) root         (0)     1615 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/mint_normalize.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/normalize.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/transfer.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/wallet_import.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/wait.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_example/wallet_create.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.413611 djwebdapp-1.0.0rc5/src/djwebdapp_fa2/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_fa2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_fa2/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_fa2/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.413611 djwebdapp-1.0.0rc5/src/djwebdapp_fa2/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     5901 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_fa2/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_fa2/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2778 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_fa2/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2068 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_fa2/normalizers.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_fa2/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_fa2/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_fa2/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.413611 djwebdapp-1.0.0rc5/src/djwebdapp_multisig/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_multisig/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_multisig/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_multisig/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.413611 djwebdapp-1.0.0rc5/src/djwebdapp_multisig/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2711 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_multisig/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_multisig/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1091 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_multisig/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.416944 djwebdapp-1.0.0rc5/src/djwebdapp_rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_rest_framework/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_rest_framework/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.416944 djwebdapp-1.0.0rc5/src/djwebdapp_rest_framework/migrations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_rest_framework/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_rest_framework/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3845 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_rest_framework/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.416944 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.416944 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.416944 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/management/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 13:15:37.416944 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      616 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/migrations/0002_tezostransaction_caller.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/migrations/0003_tezoscall_tezoscontract.py
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/migrations/0004_delete_tezoscall_delete_tezoscontract.py
--rw-rw-rw-   0 root         (0) root         (0)      830 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/migrations/0005_tezoscall_tezoscontract.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-17 13:15:33.000000 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5032 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/models.py
--rw-rw-rw-   0 root         (0) root         (0)    16038 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc5/src/djwebdapp_tezos/provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.017473 djwebdapp-1.0.0rc6/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5103 2023-02-23 14:59:50.017473 djwebdapp-1.0.0rc6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3715 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-23 14:59:50.017473 djwebdapp-1.0.0rc6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2023-02-23 14:59:49.000000 djwebdapp-1.0.0rc6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:49.997473 djwebdapp-1.0.0rc6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.000806 djwebdapp-1.0.0rc6/src/djwebdapp/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1940 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.000806 djwebdapp-1.0.0rc6/src/djwebdapp/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.000806 djwebdapp-1.0.0rc6/src/djwebdapp/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/management/commands/history_download.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/management/commands/index.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/management/commands/normalize.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/management/commands/refresh_balances.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/management/commands/spool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.004139 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     7904 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0002_alter_transaction_receiver_alter_transaction_sender.py
+-rw-rw-rw-   0 root         (0) root         (0)      741 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0003_transaction_txgroup_alter_transaction_hash_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0004_alter_transaction_options.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0005_alter_transaction_unique_together_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0006_blockchain_min_confirmations_alter_transaction_state.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0007_alter_transaction_amount.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0008_transaction_index.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0009_account_index.py
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0010_alter_transaction_nonce.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0011_rename_max_level_blockchain_index_level.py
+-rw-rw-rw-   0 root         (0) root         (0)      437 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0012_transaction_number.py
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0013_transaction_normalized_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0014_alter_account_unique_together.py
+-rw-rw-rw-   0 root         (0) root         (0)      974 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0015_alter_transaction_state.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19402 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/normalizers.py
+-rw-rw-rw-   0 root         (0) root         (0)     9416 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.000806 djwebdapp-1.0.0rc6/src/djwebdapp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5103 2023-02-23 14:59:49.000000 djwebdapp-1.0.0rc6/src/djwebdapp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4886 2023-02-23 14:59:49.000000 djwebdapp-1.0.0rc6/src/djwebdapp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 14:59:49.000000 djwebdapp-1.0.0rc6/src/djwebdapp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      514 2023-02-23 14:59:49.000000 djwebdapp-1.0.0rc6/src/djwebdapp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-02-23 14:59:49.000000 djwebdapp-1.0.0rc6/src/djwebdapp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.004139 djwebdapp-1.0.0rc6/src/djwebdapp_ethereum/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_ethereum/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_ethereum/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_ethereum/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.004139 djwebdapp-1.0.0rc6/src/djwebdapp_ethereum/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_ethereum/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_ethereum/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      918 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_ethereum/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     7102 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_ethereum/provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.007473 djwebdapp-1.0.0rc6/src/djwebdapp_example/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/balance.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/balance_update.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/deploy_fa12.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.007473 djwebdapp-1.0.0rc6/src/djwebdapp_example/ethereum/
+-rw-rw-rw-   0 root         (0) root         (0)      486 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/ethereum/blockchain.py
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/ethereum/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/ethereum/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/ethereum/deploy_contract.py
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/ethereum/index.py
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/ethereum/load.py
+-rw-rw-rw-   0 root         (0) root         (0)     1651 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/ethereum/mint_normalize.py
+-rw-rw-rw-   0 root         (0) root         (0)      404 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/ethereum/normalize.py
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/ethereum/transfer.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/ethereum/wallet_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.007473 djwebdapp-1.0.0rc6/src/djwebdapp_example/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2586 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/spool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.010806 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/
+-rw-rw-rw-   0 root         (0) root         (0)     6019 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/FA12.json
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/FA12.py
+-rw-rw-rw-   0 root         (0) root         (0)      725 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/Proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/blockchain.py
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/call_parallel.py
+-rw-rw-rw-   0 root         (0) root         (0)    23855 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/callee.json
+-rw-rw-rw-   0 root         (0) root         (0)      670 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/callee.py
+-rw-rw-rw-   0 root         (0) root         (0)    31361 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/caller.json
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/caller.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1055 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/deploy_contract.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/index.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/load.py
+-rw-rw-rw-   0 root         (0) root         (0)     1615 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/mint_normalize.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/normalize.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/transfer.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/wallet_import.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/wait.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_example/wallet_create.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.014139 djwebdapp-1.0.0rc6/src/djwebdapp_fa2/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_fa2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_fa2/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_fa2/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.014139 djwebdapp-1.0.0rc6/src/djwebdapp_fa2/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     5901 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_fa2/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_fa2/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2778 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_fa2/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_fa2/normalizers.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_fa2/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_fa2/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_fa2/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.014139 djwebdapp-1.0.0rc6/src/djwebdapp_multisig/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_multisig/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_multisig/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_multisig/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.014139 djwebdapp-1.0.0rc6/src/djwebdapp_multisig/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2711 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_multisig/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_multisig/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_multisig/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.014139 djwebdapp-1.0.0rc6/src/djwebdapp_rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_rest_framework/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_rest_framework/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.014139 djwebdapp-1.0.0rc6/src/djwebdapp_rest_framework/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_rest_framework/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_rest_framework/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_rest_framework/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.014139 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.014139 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.014139 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/management/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 14:59:50.017473 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      616 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/migrations/0002_tezostransaction_caller.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/migrations/0003_tezoscall_tezoscontract.py
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/migrations/0004_delete_tezoscall_delete_tezoscontract.py
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/migrations/0005_tezoscall_tezoscontract.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 14:59:46.000000 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6419 2023-02-23 14:48:57.000000 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    16038 2023-02-17 13:05:18.000000 djwebdapp-1.0.0rc6/src/djwebdapp_tezos/provider.py
```

### Comparing `djwebdapp-1.0.0rc5/PKG-INFO` & `djwebdapp-1.0.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djwebdapp
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: UNKNOWN
 Home-page: https://yourlabs.io/oss/djwebdapp
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: MIT
 Description: djWebdApp
         ~~~~~~~~~
```

### Comparing `djwebdapp-1.0.0rc5/README.rst` & `djwebdapp-1.0.0rc6/README.rst`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/setup.py` & `djwebdapp-1.0.0rc6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     if name == 'binary':
         continue
     extras_require['all'] += deps
 
 
 setup(
     name='djwebdapp',
-    version='1.0.0rc5',
+    version='1.0.0rc6',
     setup_requires='setupmeta',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     install_requires=[
         'django-model-utils',
         'djfernet>=0.8.1',
         'django-picklefield>=3.0.1',
```

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp/admin.py` & `djwebdapp-1.0.0rc6/src/djwebdapp/admin.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp/management/commands/history_download.py` & `djwebdapp-1.0.0rc6/src/djwebdapp/management/commands/history_download.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp/management/commands/index.py` & `djwebdapp-1.0.0rc6/src/djwebdapp/management/commands/index.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp/management/commands/normalize.py` & `djwebdapp-1.0.0rc6/src/djwebdapp/management/commands/normalize.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0001_initial.py` & `djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0002_alter_transaction_receiver_alter_transaction_sender.py` & `djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0002_alter_transaction_receiver_alter_transaction_sender.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0003_transaction_txgroup_alter_transaction_hash_and_more.py` & `djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0003_transaction_txgroup_alter_transaction_hash_and_more.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0005_alter_transaction_unique_together_and_more.py` & `djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0005_alter_transaction_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0006_blockchain_min_confirmations_alter_transaction_state.py` & `djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0006_blockchain_min_confirmations_alter_transaction_state.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0008_transaction_index.py` & `djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0008_transaction_index.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0013_transaction_normalized_dependency.py` & `djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0013_transaction_normalized_dependency.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp/migrations/0015_alter_transaction_state.py` & `djwebdapp-1.0.0rc6/src/djwebdapp/migrations/0015_alter_transaction_state.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp/models.py` & `djwebdapp-1.0.0rc6/src/djwebdapp/models.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp/normalizers.py` & `djwebdapp-1.0.0rc6/src/djwebdapp/normalizers.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp/provider.py` & `djwebdapp-1.0.0rc6/src/djwebdapp/provider.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp.egg-info/PKG-INFO` & `djwebdapp-1.0.0rc6/src/djwebdapp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djwebdapp
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: UNKNOWN
 Home-page: https://yourlabs.io/oss/djwebdapp
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: MIT
 Description: djWebdApp
         ~~~~~~~~~
```

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp.egg-info/SOURCES.txt` & `djwebdapp-1.0.0rc6/src/djwebdapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp.egg-info/requires.txt` & `djwebdapp-1.0.0rc6/src/djwebdapp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_ethereum/migrations/0001_initial.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_ethereum/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_ethereum/models.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_ethereum/models.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_ethereum/provider.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_ethereum/provider.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/balance_update.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/balance_update.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/ethereum/deploy_contract.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/ethereum/deploy_contract.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/ethereum/index.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/ethereum/index.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/ethereum/mint_normalize.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/ethereum/mint_normalize.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/ethereum/wallet_import.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/ethereum/wallet_import.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/migrations/0001_initial.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/models.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/models.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/FA12.json` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/FA12.json`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/FA12.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/FA12.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/Proxy.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/Proxy.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/call_parallel.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/call_parallel.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/callee.json` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/callee.json`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/callee.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/callee.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/caller.json` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/caller.json`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/caller.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/caller.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/deploy_contract.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/deploy_contract.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/index.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/index.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/mint_normalize.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/mint_normalize.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_example/tezos/wallet_import.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_example/tezos/wallet_import.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_fa2/migrations/0001_initial.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_fa2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_fa2/models.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_fa2/models.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_fa2/normalizers.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_fa2/normalizers.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_fa2/views.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_fa2/views.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_multisig/migrations/0001_initial.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_multisig/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_multisig/models.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_multisig/models.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_rest_framework/views.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_rest_framework/views.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_tezos/migrations/0001_initial.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_tezos/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_tezos/migrations/0002_tezostransaction_caller.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_tezos/migrations/0002_tezostransaction_caller.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_tezos/migrations/0003_tezoscall_tezoscontract.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_tezos/migrations/0003_tezoscall_tezoscontract.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_tezos/migrations/0005_tezoscall_tezoscontract.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_tezos/migrations/0005_tezoscall_tezoscontract.py`

 * *Files identical despite different names*

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_tezos/models.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_tezos/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -104,15 +104,32 @@
                     **lookup_attributes,
                     **defaults,
                 )
                 instance.save_base(raw=True)
                 instance.refresh_from_db()
                 return instance, True
 
-            instance = self.filter(**lookup_attributes).update(**defaults)
+            self.filter(**lookup_attributes).update(**defaults)
+            instance = self.get(**lookup_attributes)
+            return instance, False
+
+    def get_or_create(self, *args, **kwargs):
+        if "tezostransaction_ptr" not in kwargs:
+            return super().get_or_create(*args, **kwargs)
+        else:
+            instance = self.filter(**kwargs).first()
+            if not instance:
+                instance = self.model(
+                    **kwargs,
+                )
+                instance.save_base(raw=True)
+                instance.refresh_from_db()
+                return instance, True
+
+            instance = self.filter(**kwargs).first()
             return instance, False
 
 
 class TezosContract(TezosTransaction):
     contract_file_name = None
     normalizer_class = Normalizer
     objects = TezosContractManager()
@@ -161,9 +178,31 @@
     def save(self, *args, **kwargs):
         if not self.function:
             self.function = self.entrypoint
         if not self.contract:
             self.contract = self.target_contract
         super().save(*args, **kwargs)
 
+    def update_or_create(self, *args, **kwargs):
+        if "tezostransaction_ptr" not in kwargs:
+            return super().update_or_create(*args, **kwargs)
+        else:
+            defaults = kwargs["defaults"]
+            del kwargs["defaults"]
+            lookup_attributes = kwargs
+
+            instance = self.filter(**lookup_attributes).first()
+            if not instance:
+                instance = self.model(
+                    **lookup_attributes,
+                    **defaults,
+                )
+                instance.save_base(raw=True)
+                instance.refresh_from_db()
+                return instance, True
+
+            self.filter(**lookup_attributes).update(**defaults)
+            instance = self.get(**lookup_attributes)
+            return instance, False
+
     class Meta:
         proxy = True
```

### Comparing `djwebdapp-1.0.0rc5/src/djwebdapp_tezos/provider.py` & `djwebdapp-1.0.0rc6/src/djwebdapp_tezos/provider.py`

 * *Files identical despite different names*

