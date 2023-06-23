# Comparing `tmp/domain-admin-1.4.6.tar.gz` & `tmp/domain-admin-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domain-admin-1.4.6.tar", last modified: Thu Jun 22 10:52:32 2023, max compression
+gzip compressed data, was "domain-admin-1.4.7.tar", last modified: Fri Jun 23 08:18:08 2023, max compression
```

## Comparing `domain-admin-1.4.6.tar` & `domain-admin-1.4.7.tar`

### file list

```diff
@@ -1,274 +1,272 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.851818 domain-admin-1.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-22 10:51:57.000000 domain-admin-1.4.6/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-06-22 10:51:57.000000 domain-admin-1.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-06-22 10:52:32.851818 domain-admin-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-06-22 10:51:57.000000 domain-admin-1.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.823816 domain-admin-1.4.6/domain_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.827817 domain-admin-1.4.6/domain_admin/api/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/api/address_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/api/cert_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14936 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/api/domain_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/api/domain_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/api/group_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/api/ip_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/api/log_scheduler_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/api/notify_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/api/whois_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.827817 domain-admin-1.4.6/domain_admin/config/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/config/default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/config/env_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.827817 domain-admin-1.4.6/domain_admin/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/enums/config_key_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/enums/event_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/enums/notify_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/enums/status_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/enums/version_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.827817 domain-admin-1.4.6/domain_admin/migrate/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/migrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/migrate/migrate_102_to_103.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/migrate/migrate_106_to_110.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/migrate/migrate_110_to_1212.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/migrate/migrate_1212_to_1213.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/migrate/migrate_1213_to_131.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/migrate/migrate_136_to_140_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/migrate/migrate_140_alpha_to_140.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/migrate/migrate_143_to_144.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/migrate/migrate_145_to_146.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/migrate/migrate_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.831817 domain-admin-1.4.6/domain_admin/model/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/model/address_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/model/cache_domain_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/model/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/model/domain_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/model/domain_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/model/group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/model/log_scheduler_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/model/notify_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/model/system_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/model/user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/model/version_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.831817 domain-admin-1.4.6/domain_admin/public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.831817 domain-admin-1.4.6/domain_admin/public/.git/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.831817 domain-admin-1.4.6/domain_admin/public/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/hooks/sendemail-validate.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.831817 domain-admin-1.4.6/domain_admin/public/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-06-22 10:52:24.000000 domain-admin-1.4.6/domain_admin/public/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.831817 domain-admin-1.4.6/domain_admin/public/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.819816 domain-admin-1.4.6/domain_admin/public/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.831817 domain-admin-1.4.6/domain_admin/public/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/logs/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.819816 domain-admin-1.4.6/domain_admin/public/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.831817 domain-admin-1.4.6/domain_admin/public/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/logs/refs/remotes/origin/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.823816 domain-admin-1.4.6/domain_admin/public/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/09/
--r--r--r--   0 runner    (1001) docker     (123)      462 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/09/278e753ec894398fba1f020046becf09fc87ac
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/0e/
--r--r--r--   0 runner    (1001) docker     (123)    77506 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/0e/f475a319963dd1aacf0fc47b71470eaedf059f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/1d/
--r--r--r--   0 runner    (1001) docker     (123)    10075 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/1d/5380125d8b56c0426f9651cb8fb148b47a4c27
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/1e/
--r--r--r--   0 runner    (1001) docker     (123)     8053 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/1e/7aa10bfedf8d97dde9cb7aba03c27a21b38b5d
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/21/
--r--r--r--   0 runner    (1001) docker     (123)       61 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/39/
--r--r--r--   0 runner    (1001) docker     (123)     8278 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/39/720bcc4033027c81269e1e306eaa1a0a258f5e
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/3c/
--r--r--r--   0 runner    (1001) docker     (123)     3081 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/43/
--r--r--r--   0 runner    (1001) docker     (123)      118 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/43/821b00bc50e6d85ddb7c8b8764b0190b655bcd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/46/
--r--r--r--   0 runner    (1001) docker     (123)   157226 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/46/ad27d72c0155033bf1b726e7ea6c21e7a2c236
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/58/
--r--r--r--   0 runner    (1001) docker     (123)     3129 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/58/21b3dc5966d68feea58616b9eb14a01cf8bebf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/5b/
--r--r--r--   0 runner    (1001) docker     (123)    62564 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/5b/1c488a74d8c3493cec2a99903972521902b410
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/5c/
--r--r--r--   0 runner    (1001) docker     (123)     1737 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/5c/a27d4acbd01639d7aa9db00e30292216ae9abc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/5f/
--r--r--r--   0 runner    (1001) docker     (123)      530 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/60/
--r--r--r--   0 runner    (1001) docker     (123)      639 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/60/cfeb3ecc9f05c7e229dd6dbfdf59866837dadc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/62/
--r--r--r--   0 runner    (1001) docker     (123)     4034 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/62/3131e94f94d1e618a711ab624a9399fe97000c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/6d/
--r--r--r--   0 runner    (1001) docker     (123)      612 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/7a/
--r--r--r--   0 runner    (1001) docker     (123)   279768 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/7a/b699b6eea6b7e3d3c0130b97bdca0def787fef
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/7f/
--r--r--r--   0 runner    (1001) docker     (123)      368 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/7f/64d8af0501887e805dc9ccf8228f4fb5e73fdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/84/
--r--r--r--   0 runner    (1001) docker     (123)     6513 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/84/dd9b1c439b10196ee913724e7e397b1ca64611
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/86/
--r--r--r--   0 runner    (1001) docker     (123)      222 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/86/cdc14d00229d56aacb47f2847c0648fa55ac9f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/8b/
--r--r--r--   0 runner    (1001) docker     (123)    41901 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/8b/19737c31c38191351e2550ceba02f876fb253a
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/8c/
--r--r--r--   0 runner    (1001) docker     (123)       69 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/8c/f880f5a9481ef71cd22e08d59e7d366775b360
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/ac/
--r--r--r--   0 runner    (1001) docker     (123)     1426 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/ac/f72e52b26a93100d038e14a1bd41c24b600d0d
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/b6/
--r--r--r--   0 runner    (1001) docker     (123)      665 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/b6/62426b8ad9d0316365b50394ec678f47cd4e77
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/b9/
--r--r--r--   0 runner    (1001) docker     (123)     1023 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/b9/13334fbada159730c9e541676075660c1fddf0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/d4/
--r--r--r--   0 runner    (1001) docker     (123)    63351 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/d4/e6befa9509ad978e37ee1775a65dc42a315655
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.835817 domain-admin-1.4.6/domain_admin/public/.git/objects/f2/
--r--r--r--   0 runner    (1001) docker     (123)      473 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/f2/fc652c091392e96c19ef83a927c91a8cc22064
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.839817 domain-admin-1.4.6/domain_admin/public/.git/objects/fa/
--r--r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/fa/8a73e08c548681ec26512cf098b66eb0f1751e
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.839817 domain-admin-1.4.6/domain_admin/public/.git/objects/fd/
--r--r--r--   0 runner    (1001) docker     (123)     5204 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.823816 domain-admin-1.4.6/domain_admin/public/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.839817 domain-admin-1.4.6/domain_admin/public/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.823816 domain-admin-1.4.6/domain_admin/public/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.839817 domain-admin-1.4.6/domain_admin/public/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/refs/remotes/origin/dist
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/.git/shallow
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.839817 domain-admin-1.4.6/domain_admin/public/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/css/ConditionFilterGroup.a91875e6.css
--rw-r--r--   0 runner    (1001) docker     (123)   328914 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/css/index.38f500bb.css
--rwxr-xr-x   0 runner    (1001) docker     (123)    15406 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.839817 domain-admin-1.4.6/domain_admin/public/gif/
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/gif/user-avatar.ea67286d.gif
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.843818 domain-admin-1.4.6/domain_admin/public/js/
--rw-r--r--   0 runner    (1001) docker     (123)    22343 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/ConditionFilterGroup.041de17b.js
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/ConnectStatus.06a43ab1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/SelectGroup.8b48ceb9.js
--rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/element-icon.ade3aa7e.js
--rw-r--r--   0 runner    (1001) docker     (123)   749550 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/element-plus.dcbfaaa8.js
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/event-enums.6c6f25e7.js
--rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/index.04a154f7.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/index.3031492f.js
--rw-r--r--   0 runner    (1001) docker     (123)    27072 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/index.622f67d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/index.99aab946.js
--rw-r--r--   0 runner    (1001) docker     (123)   421881 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/index.a21f1476.js
--rw-r--r--   0 runner    (1001) docker     (123)    26676 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/index.a5094d31.js
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/index.b61a18d3.js
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/index.e2c97624.js
--rw-r--r--   0 runner    (1001) docker     (123)   238631 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/index.faa1c0be.js
--rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/vendor-lib.4c56f242.js
--rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/js/vendor-vue.edbe275b.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.843818 domain-admin-1.4.6/domain_admin/public/svg/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-22 10:52:25.000000 domain-admin-1.4.6/domain_admin/public/svg/logo.184a2d7d.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.843818 domain-admin-1.4.6/domain_admin/router/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/router/api_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/router/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.843818 domain-admin-1.4.6/domain_admin/service/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/async_task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/cache_domain_info_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/domain_info_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    16236 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/domain_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/email_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/file_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/global_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/group_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/notify_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/render_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/scheduler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/system_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/token_service.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/version_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/service/work_weixin_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.847818 domain-admin-1.4.6/domain_admin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/templates/cert-email.html
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/templates/cert-export.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/templates/domain-email.html
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/templates/domain-export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.847818 domain-admin-1.4.6/domain_admin/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/bcrypt_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.847818 domain-admin-1.4.6/domain_admin/utils/cert_util/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/cert_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/cert_util/cert_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/cert_util/cert_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/cert_util/cert_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/cert_util/cert_openssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/cert_util/cert_openssl_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/cert_util/cert_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/cert_util/cert_socket_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/datetime_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/domain_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/file_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.847818 domain-admin-1.4.6/domain_admin/utils/flask_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/flask_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/flask_ext/api_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/flask_ext/app_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/flask_ext/flask_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/flask_ext/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/flask_ext/http_code_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.847818 domain-admin-1.4.6/domain_admin/utils/flask_ext/json/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/flask_ext/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/flask_ext/json/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/flask_ext/json/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/flask_ext/json/json_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/flask_ext/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/flask_ext/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/ip_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/json_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.847818 domain-admin-1.4.6/domain_admin/utils/open_api/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/open_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/open_api/ding_talk_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/open_api/feishu_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/open_api/work_weixin_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.847818 domain-admin-1.4.6/domain_admin/utils/peewee_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/peewee_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/peewee_ext/model_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/secret_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/text_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/time_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.851818 domain-admin-1.4.6/domain_admin/utils/whois_util/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/whois_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/whois_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/whois_util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25896 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/whois_util/whois-servers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/utils/whois_util/whois_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-06-22 10:51:57.000000 domain-admin-1.4.6/domain_admin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.827817 domain-admin-1.4.6/domain_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-06-22 10:52:32.000000 domain-admin-1.4.6/domain_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-06-22 10:52:32.000000 domain-admin-1.4.6/domain_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 10:52:32.000000 domain-admin-1.4.6/domain_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-22 10:52:32.000000 domain-admin-1.4.6/domain_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-22 10:52:32.000000 domain-admin-1.4.6/domain_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 10:52:32.000000 domain-admin-1.4.6/domain_admin.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:52:32.851818 domain-admin-1.4.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-22 10:51:57.000000 domain-admin-1.4.6/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 10:52:32.851818 domain-admin-1.4.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1928 2023-06-22 10:51:57.000000 domain-admin-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.586971 domain-admin-1.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-23 08:17:52.000000 domain-admin-1.4.7/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-06-23 08:17:52.000000 domain-admin-1.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12514 2023-06-23 08:18:08.586971 domain-admin-1.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-06-23 08:17:52.000000 domain-admin-1.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.566971 domain-admin-1.4.7/domain_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.566971 domain-admin-1.4.7/domain_admin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/api/address_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/api/cert_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/api/domain_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/api/domain_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/api/group_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/api/ip_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/api/log_scheduler_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/api/notify_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/api/whois_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.566971 domain-admin-1.4.7/domain_admin/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/config/default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/config/env_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.566971 domain-admin-1.4.7/domain_admin/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/enums/config_key_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/enums/event_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/enums/notify_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/enums/status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/enums/version_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.570971 domain-admin-1.4.7/domain_admin/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/migrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/migrate/migrate_102_to_103.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/migrate/migrate_106_to_110.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/migrate/migrate_110_to_1212.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/migrate/migrate_1212_to_1213.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/migrate/migrate_1213_to_131.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/migrate/migrate_136_to_140_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/migrate/migrate_140_alpha_to_140.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/migrate/migrate_143_to_144.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/migrate/migrate_145_to_146.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/migrate/migrate_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.570971 domain-admin-1.4.7/domain_admin/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/model/address_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/model/domain_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/model/domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/model/group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/model/log_scheduler_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/model/notify_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/model/system_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/model/user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/model/version_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.570971 domain-admin-1.4.7/domain_admin/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.570971 domain-admin-1.4.7/domain_admin/public/.git/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.570971 domain-admin-1.4.7/domain_admin/public/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/hooks/sendemail-validate.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.570971 domain-admin-1.4.7/domain_admin/public/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.570971 domain-admin-1.4.7/domain_admin/public/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.558971 domain-admin-1.4.7/domain_admin/public/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.570971 domain-admin-1.4.7/domain_admin/public/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/logs/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.558971 domain-admin-1.4.7/domain_admin/public/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.570971 domain-admin-1.4.7/domain_admin/public/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/logs/refs/remotes/origin/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.562971 domain-admin-1.4.7/domain_admin/public/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/09/
+-r--r--r--   0 runner    (1001) docker     (123)      462 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/09/278e753ec894398fba1f020046becf09fc87ac
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/0e/
+-r--r--r--   0 runner    (1001) docker     (123)    77506 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/0e/f475a319963dd1aacf0fc47b71470eaedf059f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/1d/
+-r--r--r--   0 runner    (1001) docker     (123)    10075 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/1d/5380125d8b56c0426f9651cb8fb148b47a4c27
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/1e/
+-r--r--r--   0 runner    (1001) docker     (123)     8053 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/1e/7aa10bfedf8d97dde9cb7aba03c27a21b38b5d
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/21/
+-r--r--r--   0 runner    (1001) docker     (123)       61 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/39/
+-r--r--r--   0 runner    (1001) docker     (123)     8278 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/39/720bcc4033027c81269e1e306eaa1a0a258f5e
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/3c/
+-r--r--r--   0 runner    (1001) docker     (123)     3081 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/43/
+-r--r--r--   0 runner    (1001) docker     (123)      118 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/43/821b00bc50e6d85ddb7c8b8764b0190b655bcd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/46/
+-r--r--r--   0 runner    (1001) docker     (123)   157226 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/46/ad27d72c0155033bf1b726e7ea6c21e7a2c236
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/58/
+-r--r--r--   0 runner    (1001) docker     (123)     3129 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/58/21b3dc5966d68feea58616b9eb14a01cf8bebf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/5b/
+-r--r--r--   0 runner    (1001) docker     (123)    62564 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/5b/1c488a74d8c3493cec2a99903972521902b410
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/5c/
+-r--r--r--   0 runner    (1001) docker     (123)     1737 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/5c/a27d4acbd01639d7aa9db00e30292216ae9abc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/5f/
+-r--r--r--   0 runner    (1001) docker     (123)      530 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/60/
+-r--r--r--   0 runner    (1001) docker     (123)      639 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/60/cfeb3ecc9f05c7e229dd6dbfdf59866837dadc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/62/
+-r--r--r--   0 runner    (1001) docker     (123)     4034 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/62/3131e94f94d1e618a711ab624a9399fe97000c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/6d/
+-r--r--r--   0 runner    (1001) docker     (123)      612 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/7a/
+-r--r--r--   0 runner    (1001) docker     (123)   279768 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/7a/b699b6eea6b7e3d3c0130b97bdca0def787fef
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/7f/
+-r--r--r--   0 runner    (1001) docker     (123)      368 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/7f/64d8af0501887e805dc9ccf8228f4fb5e73fdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/84/
+-r--r--r--   0 runner    (1001) docker     (123)     6513 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/84/dd9b1c439b10196ee913724e7e397b1ca64611
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/86/
+-r--r--r--   0 runner    (1001) docker     (123)      222 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/86/cdc14d00229d56aacb47f2847c0648fa55ac9f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/8b/
+-r--r--r--   0 runner    (1001) docker     (123)    41901 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/8b/19737c31c38191351e2550ceba02f876fb253a
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/8c/
+-r--r--r--   0 runner    (1001) docker     (123)       69 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/8c/f880f5a9481ef71cd22e08d59e7d366775b360
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/ac/
+-r--r--r--   0 runner    (1001) docker     (123)     1426 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/ac/f72e52b26a93100d038e14a1bd41c24b600d0d
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/b6/
+-r--r--r--   0 runner    (1001) docker     (123)      665 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/b6/62426b8ad9d0316365b50394ec678f47cd4e77
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/b9/
+-r--r--r--   0 runner    (1001) docker     (123)     1023 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/b9/13334fbada159730c9e541676075660c1fddf0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/d4/
+-r--r--r--   0 runner    (1001) docker     (123)    63351 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/d4/e6befa9509ad978e37ee1775a65dc42a315655
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/f2/
+-r--r--r--   0 runner    (1001) docker     (123)      473 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/f2/fc652c091392e96c19ef83a927c91a8cc22064
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/fa/
+-r--r--r--   0 runner    (1001) docker     (123)      202 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/fa/8a73e08c548681ec26512cf098b66eb0f1751e
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/objects/fd/
+-r--r--r--   0 runner    (1001) docker     (123)     5204 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.562971 domain-admin-1.4.7/domain_admin/public/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.574971 domain-admin-1.4.7/domain_admin/public/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.562971 domain-admin-1.4.7/domain_admin/public/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.578971 domain-admin-1.4.7/domain_admin/public/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/refs/remotes/origin/dist
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/.git/shallow
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.578971 domain-admin-1.4.7/domain_admin/public/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/css/ConditionFilterGroup.a91875e6.css
+-rw-r--r--   0 runner    (1001) docker     (123)   328914 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/css/index.38f500bb.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15406 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.578971 domain-admin-1.4.7/domain_admin/public/gif/
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/gif/user-avatar.ea67286d.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.582971 domain-admin-1.4.7/domain_admin/public/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    22343 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/ConditionFilterGroup.041de17b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/ConnectStatus.06a43ab1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/SelectGroup.8b48ceb9.js
+-rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/element-icon.ade3aa7e.js
+-rw-r--r--   0 runner    (1001) docker     (123)   749550 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/element-plus.dcbfaaa8.js
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/event-enums.6c6f25e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/index.04a154f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/index.3031492f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27072 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/index.622f67d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/index.99aab946.js
+-rw-r--r--   0 runner    (1001) docker     (123)   421881 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/index.a21f1476.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26676 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/index.a5094d31.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/index.b61a18d3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/index.e2c97624.js
+-rw-r--r--   0 runner    (1001) docker     (123)   238631 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/index.faa1c0be.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/vendor-lib.4c56f242.js
+-rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/js/vendor-vue.edbe275b.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.582971 domain-admin-1.4.7/domain_admin/public/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-23 08:18:06.000000 domain-admin-1.4.7/domain_admin/public/svg/logo.184a2d7d.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.582971 domain-admin-1.4.7/domain_admin/router/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/router/api_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/router/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.582971 domain-admin-1.4.7/domain_admin/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/async_task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/domain_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14635 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/domain_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/email_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/file_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/global_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/group_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/notify_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/render_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/scheduler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/system_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/token_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/version_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/service/work_weixin_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.582971 domain-admin-1.4.7/domain_admin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/templates/cert-email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/templates/cert-export.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/templates/domain-email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/templates/domain-export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.582971 domain-admin-1.4.7/domain_admin/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/bcrypt_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.586971 domain-admin-1.4.7/domain_admin/utils/cert_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/cert_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/cert_util/cert_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/cert_util/cert_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/cert_util/cert_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/cert_util/cert_openssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/cert_util/cert_openssl_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/cert_util/cert_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/cert_util/cert_socket_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/datetime_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/domain_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/file_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.586971 domain-admin-1.4.7/domain_admin/utils/flask_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/flask_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/flask_ext/api_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/flask_ext/app_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/flask_ext/flask_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/flask_ext/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/flask_ext/http_code_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.586971 domain-admin-1.4.7/domain_admin/utils/flask_ext/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/flask_ext/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/flask_ext/json/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/flask_ext/json/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/flask_ext/json/json_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/flask_ext/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/flask_ext/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/ip_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/json_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.586971 domain-admin-1.4.7/domain_admin/utils/open_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/open_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/open_api/ding_talk_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/open_api/feishu_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/open_api/work_weixin_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.586971 domain-admin-1.4.7/domain_admin/utils/peewee_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/peewee_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/peewee_ext/model_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/secret_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/text_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/time_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.586971 domain-admin-1.4.7/domain_admin/utils/whois_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/whois_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/whois_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/whois_util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25896 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/whois_util/whois-servers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/utils/whois_util/whois_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-06-23 08:17:52.000000 domain-admin-1.4.7/domain_admin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.566971 domain-admin-1.4.7/domain_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12514 2023-06-23 08:18:08.000000 domain-admin-1.4.7/domain_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-23 08:18:08.000000 domain-admin-1.4.7/domain_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 08:18:08.000000 domain-admin-1.4.7/domain_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-23 08:18:08.000000 domain-admin-1.4.7/domain_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 08:18:08.000000 domain-admin-1.4.7/domain_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 08:18:08.000000 domain-admin-1.4.7/domain_admin.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:18:08.586971 domain-admin-1.4.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-23 08:17:52.000000 domain-admin-1.4.7/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 08:18:08.586971 domain-admin-1.4.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1928 2023-06-23 08:17:52.000000 domain-admin-1.4.7/setup.py
```

### Comparing `domain-admin-1.4.6/LICENSE` & `domain-admin-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/PKG-INFO` & `domain-admin-1.4.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,25 @@
-Metadata-Version: 2.1
-Name: domain-admin
-Version: 1.4.6
-Summary: a domain ssl cert admin
-Home-page: https://github.com/mouday/domain-admin
-Author: Peng Shiyu
-Author-email: pengshiyuyx@gmail.com
-License: MIT
-Keywords: domain ssl cert
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Domain Admin
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/domain-admin)](https://pypi.org/project/domain-admin)
 [![PyPI](https://img.shields.io/pypi/v/domain-admin.svg)](https://pypi.org/project/domain-admin)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/domain-admin?label=pypi%20downloads)](https://pypi.org/project/domain-admin)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/mouday/domain-admin?label=docker%20version&sort=semver)](https://hub.docker.com/r/mouday/domain-admin)
 [![Docker Pulls](https://img.shields.io/docker/pulls/mouday/domain-admin)](https://hub.docker.com/r/mouday/domain-admin)
 [![Build Status](https://app.travis-ci.com/mouday/domain-admin.svg?branch=master)](https://app.travis-ci.com/mouday/domain-admin)
 [![PyPI - License](https://img.shields.io/pypi/l/domain-admin)](https://github.com/mouday/domain-admin/blob/master/LICENSE)
 
 ![](https://raw.githubusercontent.com/mouday/domain-admin/master/image/domain.svg)
 
-基于Python + Vue3.js 技术栈实现的域名和SSL证书监测平台
-
-核心功能：到期自动邮件提醒
+基于Python3 + Vue3.js 技术栈实现的域名和SSL证书监测平台
 
 用于解决，不同业务域名SSL证书，申请自不同的平台，到期后不能及时收到通知，导致线上访问异常，被老板责骂的问题
 
+核心功能：`域名` 和`SSL证书` 的过期监控，到期提醒，支持邮件、webhook、企业微信、钉钉、飞书等通知方式
+
 支持平台：macOS、Linux、Windows
 
 - 项目地址：https://github.com/mouday/domain-admin
 - 国内镜像：https://gitee.com/mouday/domain-admin
 - pypi：https://pypi.org/project/domain-admin
 - docker：https://hub.docker.com/r/mouday/domain-admin
 
@@ -320,14 +307,59 @@
 
 ### 5、邮件发送失败
 
 可尝试更换端口25或465
 
 ### 6、webhook模板
 
+采用`jinja2` 模板引擎
+
+传入模板的参数示例：
+
+```json
+{
+    "list":[
+        {
+            "domain": "www.demo.com",
+            "start_date": "2023-06-01",
+            "expire_date": "2023-06-21",
+            "expire_days": 20
+        }
+    ]
+}
+```
+
+参数说明
+
+| 参数  | 类型  | 说明 |
+| -| - | - |
+| domain | string | 域名/证书域名
+| start_date | string | 生效时间
+| expire_date | string | 过期时间
+| expire_days | int | 剩余天数
+
+
+示例
+
+```json
+{
+  "title": "域名到期提醒",
+  "content": "{% for row in list %}{{row.domain}} {{row.start_date or '-' }} - {{row.expire_date or '-' }} ({{row.expire_days}}){% endfor %}"
+}
+```
+
+渲染结果
+
+```json
+{
+  "title": "域名到期提醒",
+  "content": "www.demo.com 2023-06-01 - 2023-06-21 (20)"
+}
+```
+
 可以参考接口文档：[更新用户通知配置](docs/notify/updateNotifyOfUser.md)
 
 ### 7、监控域名非443的端口
 
 域名格式
 
 ```
```

### Comparing `domain-admin-1.4.6/README.md` & `domain-admin-1.4.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,38 @@
+Metadata-Version: 2.1
+Name: domain-admin
+Version: 1.4.7
+Summary: a domain ssl cert admin
+Home-page: https://github.com/mouday/domain-admin
+Author: Peng Shiyu
+Author-email: pengshiyuyx@gmail.com
+License: MIT
+Keywords: domain ssl cert
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Domain Admin
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/domain-admin)](https://pypi.org/project/domain-admin)
 [![PyPI](https://img.shields.io/pypi/v/domain-admin.svg)](https://pypi.org/project/domain-admin)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/domain-admin?label=pypi%20downloads)](https://pypi.org/project/domain-admin)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/mouday/domain-admin?label=docker%20version&sort=semver)](https://hub.docker.com/r/mouday/domain-admin)
 [![Docker Pulls](https://img.shields.io/docker/pulls/mouday/domain-admin)](https://hub.docker.com/r/mouday/domain-admin)
 [![Build Status](https://app.travis-ci.com/mouday/domain-admin.svg?branch=master)](https://app.travis-ci.com/mouday/domain-admin)
 [![PyPI - License](https://img.shields.io/pypi/l/domain-admin)](https://github.com/mouday/domain-admin/blob/master/LICENSE)
 
 ![](https://raw.githubusercontent.com/mouday/domain-admin/master/image/domain.svg)
 
-基于Python + Vue3.js 技术栈实现的域名和SSL证书监测平台
-
-核心功能：到期自动邮件提醒
+基于Python3 + Vue3.js 技术栈实现的域名和SSL证书监测平台
 
 用于解决，不同业务域名SSL证书，申请自不同的平台，到期后不能及时收到通知，导致线上访问异常，被老板责骂的问题
 
+核心功能：`域名` 和`SSL证书` 的过期监控，到期提醒，支持邮件、webhook、企业微信、钉钉、飞书等通知方式
+
 支持平台：macOS、Linux、Windows
 
 - 项目地址：https://github.com/mouday/domain-admin
 - 国内镜像：https://gitee.com/mouday/domain-admin
 - pypi：https://pypi.org/project/domain-admin
 - docker：https://hub.docker.com/r/mouday/domain-admin
 
@@ -307,14 +320,59 @@
 
 ### 5、邮件发送失败
 
 可尝试更换端口25或465
 
 ### 6、webhook模板
 
+采用`jinja2` 模板引擎
+
+传入模板的参数示例：
+
+```json
+{
+    "list":[
+        {
+            "domain": "www.demo.com",
+            "start_date": "2023-06-01",
+            "expire_date": "2023-06-21",
+            "expire_days": 20
+        }
+    ]
+}
+```
+
+参数说明
+
+| 参数  | 类型  | 说明 |
+| -| - | - |
+| domain | string | 域名/证书域名
+| start_date | string | 生效时间
+| expire_date | string | 过期时间
+| expire_days | int | 剩余天数
+
+
+示例
+
+```json
+{
+  "title": "域名到期提醒",
+  "content": "{% for row in list %}{{row.domain}} {{row.start_date or '-' }} - {{row.expire_date or '-' }} ({{row.expire_days}}){% endfor %}"
+}
+```
+
+渲染结果
+
+```json
+{
+  "title": "域名到期提醒",
+  "content": "www.demo.com 2023-06-01 - 2023-06-21 (20)"
+}
+```
+
 可以参考接口文档：[更新用户通知配置](docs/notify/updateNotifyOfUser.md)
 
 ### 7、监控域名非443的端口
 
 域名格式
 
 ```
```

### Comparing `domain-admin-1.4.6/domain_admin/api/address_api.py` & `domain-admin-1.4.7/domain_admin/api/address_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/api/auth_api.py` & `domain-admin-1.4.7/domain_admin/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/api/domain_api.py` & `domain-admin-1.4.7/domain_admin/api/domain_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,28 +46,30 @@
     }
 
     row = DomainModel.create(**data)
 
     domain_service.update_domain_row(row)
 
     # 顺带添加到域名监测列表
-    first_domain_info_row = DomainInfoModel.select(
-        DomainInfoModel.id
-    ).where(
-        DomainInfoModel.domain == data['root_domain'],
-        DomainInfoModel.user_id == current_user_id
-    ).first()
-
-    if not first_domain_info_row:
-        domain_info_service.add_domain_info(
-            domain=domain_util.get_root_domain(domain),
-            comment=alias,
-            group_id=group_id,
-            user_id=current_user_id,
-        )
+    if not domain_util.is_ipv4(domain):
+
+        first_domain_info_row = DomainInfoModel.select(
+            DomainInfoModel.id
+        ).where(
+            DomainInfoModel.domain == data['root_domain'],
+            DomainInfoModel.user_id == current_user_id
+        ).first()
+
+        if not first_domain_info_row:
+            domain_info_service.add_domain_info(
+                domain=domain_util.get_root_domain(domain),
+                comment=alias,
+                group_id=group_id,
+                user_id=current_user_id,
+            )
 
     return {'id': row.id}
 
 
 def update_domain_setting():
     """
     更新域名配置信息
```

### Comparing `domain-admin-1.4.6/domain_admin/api/domain_info_api.py` & `domain-admin-1.4.7/domain_admin/api/domain_info_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/api/group_api.py` & `domain-admin-1.4.7/domain_admin/api/group_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/api/log_scheduler_api.py` & `domain-admin-1.4.7/domain_admin/api/log_scheduler_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/api/notify_api.py` & `domain-admin-1.4.7/domain_admin/api/notify_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/api/system_api.py` & `domain-admin-1.4.7/domain_admin/api/system_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/api/user_api.py` & `domain-admin-1.4.7/domain_admin/api/user_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/config/default_config.py` & `domain-admin-1.4.7/domain_admin/config/default_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/enums/config_key_enum.py` & `domain-admin-1.4.7/domain_admin/enums/config_key_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/enums/version_enum.py` & `domain-admin-1.4.7/domain_admin/enums/version_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/main.py` & `domain-admin-1.4.7/domain_admin/main.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/migrate/migrate_102_to_103.py` & `domain-admin-1.4.7/domain_admin/migrate/migrate_102_to_103.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/migrate/migrate_106_to_110.py` & `domain-admin-1.4.7/domain_admin/migrate/migrate_106_to_110.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/migrate/migrate_110_to_1212.py` & `domain-admin-1.4.7/domain_admin/migrate/migrate_110_to_1212.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/migrate/migrate_1212_to_1213.py` & `domain-admin-1.4.7/domain_admin/migrate/migrate_1212_to_1213.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/migrate/migrate_1213_to_131.py` & `domain-admin-1.4.7/domain_admin/migrate/migrate_1213_to_131.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/migrate/migrate_136_to_140_alpha.py` & `domain-admin-1.4.7/domain_admin/migrate/migrate_136_to_140_alpha.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/migrate/migrate_140_alpha_to_140.py` & `domain-admin-1.4.7/domain_admin/migrate/migrate_140_alpha_to_140.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/migrate/migrate_143_to_144.py` & `domain-admin-1.4.7/domain_admin/migrate/migrate_143_to_144.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/migrate/migrate_145_to_146.py` & `domain-admin-1.4.7/domain_admin/migrate/migrate_145_to_146.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/migrate/migrate_common.py` & `domain-admin-1.4.7/domain_admin/migrate/migrate_common.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/model/address_model.py` & `domain-admin-1.4.7/domain_admin/model/address_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/model/base_model.py` & `domain-admin-1.4.7/domain_admin/model/base_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/model/cache_domain_info_model.py` & `domain-admin-1.4.7/domain_admin/model/log_scheduler_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,38 @@
 # -*- coding: utf-8 -*-
+import math
 from datetime import datetime
 
-from peewee import CharField, IntegerField, DateTimeField, AutoField
+from peewee import IntegerField, DateTimeField, BooleanField, TextField, AutoField
 
 from domain_admin.model.base_model import BaseModel
-from domain_admin.utils import time_util
+from domain_admin.utils import datetime_util
 
 
-class CacheDomainInfoModel(BaseModel):
-    """
-    域名信息缓存表
-    @since 1.2.12
-    @Deprecated @since 1.4.0
-    """
+class LogSchedulerModel(BaseModel):
+    """日志"""
     id = AutoField(primary_key=True)
 
-    # 域名
-    domain = CharField(unique=True)
+    # 状态
+    status = BooleanField(default=False)
 
-    # 域名注册时间
-    domain_start_time = DateTimeField(default=None, null=True)
-
-    # 域名过期时间
-    domain_expire_time = DateTimeField(default=None, null=True)
-
-    # 缓存过期时间
-    expire_time = DateTimeField(default=None, null=True)
+    # 错误信息
+    error_message = TextField(default='')
 
     # 创建时间
     create_time = DateTimeField(default=datetime.now)
 
     # 更新时间
-    update_time = DateTimeField(default=datetime.now)
+    update_time = DateTimeField(default=None, null=True)
 
     class Meta:
-        table_name = 'cache_domain_info'
+        table_name = 'log_scheduler'
 
     @property
-    def is_expired(self) -> [bool, None]:
-        """
-        过期时间
-        :return:
-        """
-        if self.expire_time:
-            return (self.expire_time - datetime.now()).seconds <= 0
-        else:
-            return None
+    def total_time(self):
+        if isinstance(self.update_time, datetime) and isinstance(self.create_time, datetime):
+            return math.ceil(self.update_time.timestamp() - self.create_time.timestamp())
 
     @property
-    def domain_expire_days(self) -> int:
-        """域名过期天数"""
-        return time_util.get_diff_days(datetime.now(), self.domain_expire_time)
+    def total_time_label(self):
+        if self.total_time:
+            return datetime_util.seconds_for_human(self.total_time)
```

### Comparing `domain-admin-1.4.6/domain_admin/model/database.py` & `domain-admin-1.4.7/domain_admin/model/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,36 +11,34 @@
 from domain_admin.model import domain_info_model
 from domain_admin.model import group_model
 from domain_admin.model import system_model
 from domain_admin.model import user_model
 from domain_admin.model import log_scheduler_model
 from domain_admin.model import notify_model
 from domain_admin.model import version_model
-from domain_admin.model import cache_domain_info_model
 
 # 需要查询初始数据操作的表放前面
 tables = [
     (system_model.SystemModel, system_model.init_table_data),
     (version_model.VersionModel, None),
     (user_model.UserModel, user_model.init_table_data),
     (log_scheduler_model.LogSchedulerModel, None),
     (group_model.GroupModel, None),
     (domain_model.DomainModel, None),
     (notify_model.NotifyModel, None),
-    (cache_domain_info_model.CacheDomainInfoModel, None),
     (address_model.AddressModel, None),
     (domain_info_model.DomainInfoModel, None),
 ]
 
 
 def init_database():
     db.connect()
 
     for model, init_func in tables:
         if not model.table_exists():
-            logger.debug('create table: %s', model._meta.table_name)
+            logger.info('create table: %s', model._meta.table_name)
             model.create_table()
 
             if init_func:
                 init_func()
 
     db.close()
```

### Comparing `domain-admin-1.4.6/domain_admin/model/domain_info_model.py` & `domain-admin-1.4.7/domain_admin/model/domain_info_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/model/domain_model.py` & `domain-admin-1.4.7/domain_admin/model/domain_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/model/group_model.py` & `domain-admin-1.4.7/domain_admin/model/group_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/model/notify_model.py` & `domain-admin-1.4.7/domain_admin/model/notify_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/model/system_model.py` & `domain-admin-1.4.7/domain_admin/model/system_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/model/user_model.py` & `domain-admin-1.4.7/domain_admin/model/user_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/model/version_model.py` & `domain-admin-1.4.7/domain_admin/model/version_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/hooks/commit-msg.sample` & `domain-admin-1.4.7/domain_admin/public/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/hooks/fsmonitor-watchman.sample` & `domain-admin-1.4.7/domain_admin/public/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/hooks/pre-commit.sample` & `domain-admin-1.4.7/domain_admin/public/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/hooks/pre-push.sample` & `domain-admin-1.4.7/domain_admin/public/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/hooks/pre-rebase.sample` & `domain-admin-1.4.7/domain_admin/public/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/hooks/pre-receive.sample` & `domain-admin-1.4.7/domain_admin/public/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/hooks/prepare-commit-msg.sample` & `domain-admin-1.4.7/domain_admin/public/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/hooks/push-to-checkout.sample` & `domain-admin-1.4.7/domain_admin/public/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/hooks/sendemail-validate.sample` & `domain-admin-1.4.7/domain_admin/public/.git/hooks/sendemail-validate.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/hooks/update.sample` & `domain-admin-1.4.7/domain_admin/public/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/0e/f475a319963dd1aacf0fc47b71470eaedf059f` & `domain-admin-1.4.7/domain_admin/public/.git/objects/0e/f475a319963dd1aacf0fc47b71470eaedf059f`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/1d/5380125d8b56c0426f9651cb8fb148b47a4c27` & `domain-admin-1.4.7/domain_admin/public/.git/objects/1d/5380125d8b56c0426f9651cb8fb148b47a4c27`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/1e/7aa10bfedf8d97dde9cb7aba03c27a21b38b5d` & `domain-admin-1.4.7/domain_admin/public/.git/objects/1e/7aa10bfedf8d97dde9cb7aba03c27a21b38b5d`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/39/720bcc4033027c81269e1e306eaa1a0a258f5e` & `domain-admin-1.4.7/domain_admin/public/.git/objects/39/720bcc4033027c81269e1e306eaa1a0a258f5e`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949` & `domain-admin-1.4.7/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/46/ad27d72c0155033bf1b726e7ea6c21e7a2c236` & `domain-admin-1.4.7/domain_admin/public/.git/objects/46/ad27d72c0155033bf1b726e7ea6c21e7a2c236`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/58/21b3dc5966d68feea58616b9eb14a01cf8bebf` & `domain-admin-1.4.7/domain_admin/public/.git/objects/58/21b3dc5966d68feea58616b9eb14a01cf8bebf`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/5b/1c488a74d8c3493cec2a99903972521902b410` & `domain-admin-1.4.7/domain_admin/public/.git/objects/5b/1c488a74d8c3493cec2a99903972521902b410`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/5c/a27d4acbd01639d7aa9db00e30292216ae9abc` & `domain-admin-1.4.7/domain_admin/public/.git/objects/5c/a27d4acbd01639d7aa9db00e30292216ae9abc`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34` & `domain-admin-1.4.7/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/60/cfeb3ecc9f05c7e229dd6dbfdf59866837dadc` & `domain-admin-1.4.7/domain_admin/public/.git/objects/60/cfeb3ecc9f05c7e229dd6dbfdf59866837dadc`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/62/3131e94f94d1e618a711ab624a9399fe97000c` & `domain-admin-1.4.7/domain_admin/public/.git/objects/62/3131e94f94d1e618a711ab624a9399fe97000c`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc` & `domain-admin-1.4.7/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/7a/b699b6eea6b7e3d3c0130b97bdca0def787fef` & `domain-admin-1.4.7/domain_admin/public/.git/objects/7a/b699b6eea6b7e3d3c0130b97bdca0def787fef`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/84/dd9b1c439b10196ee913724e7e397b1ca64611` & `domain-admin-1.4.7/domain_admin/public/.git/objects/84/dd9b1c439b10196ee913724e7e397b1ca64611`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/8b/19737c31c38191351e2550ceba02f876fb253a` & `domain-admin-1.4.7/domain_admin/public/.git/objects/8b/19737c31c38191351e2550ceba02f876fb253a`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/ac/f72e52b26a93100d038e14a1bd41c24b600d0d` & `domain-admin-1.4.7/domain_admin/public/.git/objects/ac/f72e52b26a93100d038e14a1bd41c24b600d0d`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/b6/62426b8ad9d0316365b50394ec678f47cd4e77` & `domain-admin-1.4.7/domain_admin/public/.git/objects/b6/62426b8ad9d0316365b50394ec678f47cd4e77`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/b9/13334fbada159730c9e541676075660c1fddf0` & `domain-admin-1.4.7/domain_admin/public/.git/objects/b9/13334fbada159730c9e541676075660c1fddf0`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/d4/e6befa9509ad978e37ee1775a65dc42a315655` & `domain-admin-1.4.7/domain_admin/public/.git/objects/d4/e6befa9509ad978e37ee1775a65dc42a315655`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3` & `domain-admin-1.4.7/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/css/ConditionFilterGroup.a91875e6.css` & `domain-admin-1.4.7/domain_admin/public/css/ConditionFilterGroup.a91875e6.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/css/index.38f500bb.css` & `domain-admin-1.4.7/domain_admin/public/css/index.38f500bb.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/favicon.ico` & `domain-admin-1.4.7/domain_admin/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/gif/user-avatar.ea67286d.gif` & `domain-admin-1.4.7/domain_admin/public/gif/user-avatar.ea67286d.gif`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/index.html` & `domain-admin-1.4.7/domain_admin/public/index.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/ConditionFilterGroup.041de17b.js` & `domain-admin-1.4.7/domain_admin/public/js/ConditionFilterGroup.041de17b.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/ConnectStatus.06a43ab1.js` & `domain-admin-1.4.7/domain_admin/public/js/ConnectStatus.06a43ab1.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/SelectGroup.8b48ceb9.js` & `domain-admin-1.4.7/domain_admin/public/js/SelectGroup.8b48ceb9.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/element-icon.ade3aa7e.js` & `domain-admin-1.4.7/domain_admin/public/js/element-icon.ade3aa7e.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/element-plus.dcbfaaa8.js` & `domain-admin-1.4.7/domain_admin/public/js/element-plus.dcbfaaa8.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/event-enums.6c6f25e7.js` & `domain-admin-1.4.7/domain_admin/public/js/event-enums.6c6f25e7.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/index.04a154f7.js` & `domain-admin-1.4.7/domain_admin/public/js/index.04a154f7.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/index.3031492f.js` & `domain-admin-1.4.7/domain_admin/public/js/index.3031492f.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/index.622f67d4.js` & `domain-admin-1.4.7/domain_admin/public/js/index.622f67d4.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/index.99aab946.js` & `domain-admin-1.4.7/domain_admin/public/js/index.99aab946.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/index.a21f1476.js` & `domain-admin-1.4.7/domain_admin/public/js/index.a21f1476.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/index.a5094d31.js` & `domain-admin-1.4.7/domain_admin/public/js/index.a5094d31.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/index.b61a18d3.js` & `domain-admin-1.4.7/domain_admin/public/js/index.b61a18d3.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/index.e2c97624.js` & `domain-admin-1.4.7/domain_admin/public/js/index.e2c97624.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/index.faa1c0be.js` & `domain-admin-1.4.7/domain_admin/public/js/index.faa1c0be.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/vendor-lib.4c56f242.js` & `domain-admin-1.4.7/domain_admin/public/js/vendor-lib.4c56f242.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/js/vendor-vue.edbe275b.js` & `domain-admin-1.4.7/domain_admin/public/js/vendor-vue.edbe275b.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/public/svg/logo.184a2d7d.svg` & `domain-admin-1.4.7/domain_admin/public/svg/logo.184a2d7d.svg`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/router/api_map.py` & `domain-admin-1.4.7/domain_admin/router/api_map.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/router/permission.py` & `domain-admin-1.4.7/domain_admin/router/permission.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/service/auth_service.py` & `domain-admin-1.4.7/domain_admin/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/service/domain_info_service.py` & `domain-admin-1.4.7/domain_admin/service/domain_info_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 domain_info_service.py
 """
+import random
+import time
 import traceback
 from datetime import datetime
 from typing import List
 
 from peewee import chunked
 from playhouse.shortcuts import model_to_dict
 
@@ -58,15 +60,20 @@
     :return:
     """
     domain_whois = None
 
     try:
         domain_whois = whois_util.get_domain_info(row.domain)
     except Exception as e:
-        pass
+        # 增加容错
+        try:
+            time.sleep(3)
+            domain_whois = whois_util.get_domain_info(row.domain)
+        except Exception as e:
+            pass
 
     update_row = DomainInfoModel()
 
     if domain_whois:
         update_row.domain_start_time = domain_whois['start_time']
         update_row.domain_expire_time = domain_whois['expire_time']
```

### Comparing `domain-admin-1.4.6/domain_admin/service/domain_service.py` & `domain-admin-1.4.7/domain_admin/service/domain_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,102 +1,34 @@
 # -*- coding: utf-8 -*-
 """
 domain_service.py
 """
-import time
 import traceback
 import warnings
 from datetime import datetime
 from typing import List
 
 from peewee import chunked
 from playhouse.shortcuts import model_to_dict
 
 from domain_admin.log import logger
 from domain_admin.model.address_model import AddressModel
 from domain_admin.model.domain_model import DomainModel
 from domain_admin.model.group_model import GroupModel
-from domain_admin.model.log_scheduler_model import LogSchedulerModel
 from domain_admin.model.user_model import UserModel
-from domain_admin.service import email_service, render_service, global_data_service, cache_domain_info_service
+from domain_admin.service import email_service, render_service
 from domain_admin.service import file_service
 from domain_admin.service import notify_service
 from domain_admin.service import system_service
-from domain_admin.utils import datetime_util, cert_util, whois_util, file_util, time_util
+from domain_admin.utils import datetime_util, cert_util, whois_util
 from domain_admin.utils import domain_util
-from domain_admin.utils.cert_util import cert_common, cert_socket_v2
+from domain_admin.utils.cert_util import cert_common, cert_socket_v2, cert_openssl_v2
 from domain_admin.utils.flask_ext.app_exception import AppException, ForbiddenAppException
 
 
-def update_domain_info(domain_row: DomainModel):
-    """
-    更新域名信息
-    :param row:
-    :return:
-    """
-    # logger.info("%s", model_to_dict(domain_row))
-
-    # 获取域名信息
-    domain_info = None
-
-    err = ''
-
-    try:
-        domain_info = cache_domain_info_service.get_domain_info(domain_row.domain)
-    except Exception as e:
-        err = e.__str__()
-        pass
-
-    update_data = {
-        'domain_start_time': None,
-        "domain_expire_time": None,
-        'domain_expire_days': 0,
-    }
-
-    if domain_info:
-        update_data = {
-            'domain_start_time': domain_info.domain_start_time,
-            "domain_expire_time": domain_info.domain_expire_time,
-            'domain_expire_days': domain_info.domain_expire_days,
-        }
-
-    DomainModel.update(
-        **update_data,
-        domain_check_time=datetime_util.get_datetime(),
-        update_time=datetime_util.get_datetime(),
-    ).where(
-        DomainModel.id == domain_row.id
-    ).execute()
-
-    return err
-
-
-def update_ip_info(row: DomainModel):
-    """
-    更新ip信息
-    :param row:
-    :return:
-    """
-    # 获取ip地址
-    domain_ip = ''
-
-    try:
-        domain_ip = cert_common.get_domain_ip(row.domain)
-    except Exception as e:
-        pass
-
-    DomainModel.update(
-        ip=domain_ip,
-        ip_check_time=datetime_util.get_datetime(),
-        update_time=datetime_util.get_datetime(),
-    ).where(
-        DomainModel.id == row.id
-    ).execute()
-
-
 def update_domain_host_list(domain_row: DomainModel):
     """
     更新ip信息
     :param row:
     :return:
     @since v1.2.24
     """
@@ -149,15 +81,15 @@
     """
 
     # 获取证书信息
     cert_info = {}
 
     err = ''
     try:
-        cert_info = cert_socket_v2.get_ssl_cert_info(
+        cert_info = cert_openssl_v2.get_ssl_cert_by_openssl(
             domain=domain_row.domain,
             host=address_row.host,
             port=domain_row.port
         )
     except Exception as e:
         err = e.__str__()
         logger.error(traceback.format_exc())
@@ -539,14 +471,16 @@
 
     email_service.send_email(
         subject='[Domain Admin]证书过期提醒',
         content=content,
         to_addresses=email_list,
         content_type='html'
     )
+
+
 def check_permission_and_get_row(domain_id, user_id):
     """
     权限检查
     :param domain_id:
     :param user_id:
     :return:
     """
```

### Comparing `domain-admin-1.4.6/domain_admin/service/email_service.py` & `domain-admin-1.4.7/domain_admin/service/email_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/service/file_service.py` & `domain-admin-1.4.7/domain_admin/service/file_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/service/notify_service.py` & `domain-admin-1.4.7/domain_admin/service/notify_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,14 +286,16 @@
         logger.warn("webhook url未设置")
         return
 
     # 支持模板变量
     template = Template(notify_row.webhook_body)
     body_render = template.render(data)
 
+    logger.info(body_render)
+
     res = requests.request(
         method=notify_row.webhook_method,
         url=notify_row.webhook_url,
         headers=notify_row.webhook_headers,
         data=body_render.encode('utf-8'))
 
     res.encoding = res.apparent_encoding
```

### Comparing `domain-admin-1.4.6/domain_admin/service/scheduler_service.py` & `domain-admin-1.4.7/domain_admin/service/scheduler_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/service/system_service.py` & `domain-admin-1.4.7/domain_admin/service/system_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/service/token_service.py` & `domain-admin-1.4.7/domain_admin/service/token_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/service/version_service.py` & `domain-admin-1.4.7/domain_admin/service/version_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/service/work_weixin_service.py` & `domain-admin-1.4.7/domain_admin/service/work_weixin_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/templates/cert-email.html` & `domain-admin-1.4.7/domain_admin/templates/cert-email.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/templates/domain-email.html` & `domain-admin-1.4.7/domain_admin/templates/domain-email.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/bcrypt_util.py` & `domain-admin-1.4.7/domain_admin/utils/bcrypt_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/cert_util/__init__.py` & `domain-admin-1.4.7/domain_admin/utils/cert_util/__init__.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/cert_util/cert_common.py` & `domain-admin-1.4.7/domain_admin/utils/cert_util/cert_common.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/cert_util/cert_openssl.py` & `domain-admin-1.4.7/domain_admin/utils/cert_util/cert_openssl.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/cert_util/cert_socket.py` & `domain-admin-1.4.7/domain_admin/utils/cert_util/cert_socket.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/cert_util/cert_socket_v2.py` & `domain-admin-1.4.7/domain_admin/utils/cert_util/cert_socket_v2.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 import socket
 import ssl
 import typing
 
 from domain_admin.log import logger
 from domain_admin.utils import time_util
-from domain_admin.utils.cert_util import cert_common
 
 
 def get_domain_host_list(domain: str, port: int = 80) -> typing.List[str]:
     """
     获取域名映射主机地址列表，一对多关系
     :param domain: 域名
     :param port: 端口
@@ -67,15 +66,18 @@
     返回解析好的证书信息数据
     :param domain:
     :param host:
     :param port:
     :param timeout:
     :return:
     """
-    return resolve_cert(get_ssl_cert(domain, host, port, timeout))
+    cert = get_ssl_cert(domain, host, port, timeout)
+    print(cert)
+
+    return resolve_cert(cert)
 
 
 def resolve_cert(cert: typing.Dict):
     """
     解析证书信息，仅解析重要信息
     :param cert:
     :return:
@@ -85,8 +87,11 @@
         "expire_date": time_util.parse_time(cert['notAfter']),
     }
 
     return data
 
 
 if __name__ == '__main__':
-    print(get_ssl_cert_info('dev.csdn.net', '120.46.209.149'))
+    # print(get_ssl_cert_info('www.taobao.com', '111.62.93.139'))
+    print(get_ssl_cert_info('38.60.47.102', '38.60.47.102'))
+    # print('www.baidu.com'.encode('idna')) # b'www.baidu.com'
+    # print('www.baidu.com'.encode('punycode')) # b'www.baidu.com-'
```

### Comparing `domain-admin-1.4.6/domain_admin/utils/datetime_util.py` & `domain-admin-1.4.7/domain_admin/utils/datetime_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/domain_util.py` & `domain-admin-1.4.7/domain_admin/utils/domain_util.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 """
 
 import re
 
 from typing import NamedTuple
 
 import tldextract
+from tldextract.remote import looks_like_ip
 from tldextract.tldextract import ExtractResult
 
+from domain_admin.log import logger
 from domain_admin.utils import file_util
 from domain_admin.utils.cert_util import cert_consts
 
 
 class ParsedDomain(NamedTuple):
     """
     解析后的domain数据
@@ -128,8 +130,55 @@
 def get_root_domain(domain: str) -> str:
     """
     解析出域名和顶级后缀
     :param domain:
     :return:
     """
     extract_result = extract_domain(domain)
-    return '.'.join([extract_result.domain, extract_result.suffix])
+    return extract_result.registered_domain
+    # return '.'.join([extract_result.domain, extract_result.suffix])
+
+
+def is_ipv4(ip) -> bool:
+    """
+    检测一个字符串是否是ipv4地址
+    :param ip:
+    :return:
+    """
+    return looks_like_ip(ip)
+
+    # if re.match("(\d+\.){3}\d+", ip):
+    #     return True
+    # else:
+    #     return False
+
+
+def encode_hostname(hostname: str) -> str:
+    """
+    编码中文域名，英文域名原样返回
+    :param hostname: 中文域名
+    :return:
+    """
+    return hostname.encode('idna').decode('ascii')
+
+
+def verify_cert_common_name(common_name, domain):
+    """
+    验证证书
+    :param common_name:
+    :param domain:
+    :return:
+    """
+    logger.info("%s <=> %s", common_name, domain)
+
+    if '*' in common_name:
+        # 通配符 SSL 证书
+        common_name_root_domain = get_root_domain(common_name)
+        root_domain = get_root_domain(domain)
+        return common_name_root_domain == root_domain
+    else:
+        # 普通证书
+        return common_name == domain
+
+
+if __name__ == '__main__':
+    print(get_root_domain("*.juejin.cn"))
```

### Comparing `domain-admin-1.4.6/domain_admin/utils/email_util.py` & `domain-admin-1.4.7/domain_admin/utils/email_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/flask_ext/api_result.py` & `domain-admin-1.4.7/domain_admin/utils/flask_ext/api_result.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/flask_ext/app_exception.py` & `domain-admin-1.4.7/domain_admin/utils/flask_ext/app_exception.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/flask_ext/flask_app.py` & `domain-admin-1.4.7/domain_admin/utils/flask_ext/flask_app.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/flask_ext/handler.py` & `domain-admin-1.4.7/domain_admin/utils/flask_ext/handler.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/ip_util.py` & `domain-admin-1.4.7/domain_admin/utils/ip_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/json_util.py` & `domain-admin-1.4.7/domain_admin/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/open_api/ding_talk_api.py` & `domain-admin-1.4.7/domain_admin/utils/open_api/ding_talk_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/open_api/feishu_api.py` & `domain-admin-1.4.7/domain_admin/utils/open_api/feishu_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/open_api/work_weixin_api.py` & `domain-admin-1.4.7/domain_admin/utils/open_api/work_weixin_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/peewee_ext/model_util.py` & `domain-admin-1.4.7/domain_admin/utils/peewee_ext/model_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/text_util.py` & `domain-admin-1.4.7/domain_admin/utils/text_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/time_util.py` & `domain-admin-1.4.7/domain_admin/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/whois_util/config.py` & `domain-admin-1.4.7/domain_admin/utils/whois_util/config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/whois_util/util.py` & `domain-admin-1.4.7/domain_admin/utils/whois_util/util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/whois_util/whois-servers.txt` & `domain-admin-1.4.7/domain_admin/utils/whois_util/whois-servers.txt`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.6/domain_admin/utils/whois_util/whois_util.py` & `domain-admin-1.4.7/domain_admin/utils/whois_util/whois_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,31 +26,37 @@
 def resolve_domain(domain: str) -> str:
     """
     域名转换
     :param domain:
     :return:
     """
     # 解析出域名和顶级后缀
-    extract_result = domain_util.extract_domain(domain)
-
-    root_domain = extract_result.domain
-    suffix = extract_result.suffix
-
-    # 处理包含中文的域名
-    if text_util.has_chinese(suffix):
-        pass
-
-    elif text_util.has_chinese(root_domain):
-        chinese = text_util.extract_chinese(root_domain)
-        punycode = chinese.encode('punycode').decode()
-        root_domain = f"xn--{punycode}"
-
-    domain_and_suffix = '.'.join([root_domain, suffix])
+    if domain_util.is_ipv4(domain):
+        return domain
+    else:
+        root_domain = domain_util.get_root_domain(domain)
+        return domain_util.encode_hostname(root_domain)
 
-    return domain_and_suffix
+    # extract_result = domain_util.extract_domain(domain)
+    #
+    # root_domain = extract_result.domain
+    # suffix = extract_result.suffix
+    #
+    # # 处理包含中文的域名
+    # if text_util.has_chinese(suffix):
+    #     pass
+    #
+    # elif text_util.has_chinese(root_domain):
+    #     chinese = text_util.extract_chinese(root_domain)
+    #     punycode = chinese.encode('punycode').decode()
+    #     root_domain = f"xn--{punycode}"
+    #
+    # domain_and_suffix = '.'.join([root_domain, suffix])
+    #
+    # return domain_and_suffix
 
 
 def parse_time(time_str, time_format=None):
     """
     解析时间字符串为时间对象
     :param time_str:
     :param time_format:
@@ -69,22 +75,26 @@
     加载whois_servers配置
     :return:
     """
     whois_servers = load_whois_servers()
 
     config = {}
 
+    # 通用配置
     for root, server in whois_servers.items():
-        # 通用配置
         server_config = deepcopy(DEFAULT_WHOIS_CONFIG)
         server_config['whois_server'] = server
-        config[root] = server_config
+        config[domain_util.encode_hostname(root)] = server_config
+
+    # 自定义配置优先
+    for key, value in CUSTOM_WHOIS_CONFIGS.items():
+        config[domain_util.encode_hostname(key)] = value
 
-    # 合并配置自定义配置优先
-    return {**config, **CUSTOM_WHOIS_CONFIGS}
+    # 合并配置
+    return config
 
 
 def get_whois_config(domain: str) -> [str, None]:
     """
     获取域名信息所在服务器
     :param domain:
     :return:
```

### Comparing `domain-admin-1.4.6/domain_admin.egg-info/PKG-INFO` & `domain-admin-1.4.7/domain_admin.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domain-admin
-Version: 1.4.6
+Version: 1.4.7
 Summary: a domain ssl cert admin
 Home-page: https://github.com/mouday/domain-admin
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: domain ssl cert
 Classifier: Programming Language :: Python :: 3.7
@@ -19,20 +19,20 @@
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/mouday/domain-admin?label=docker%20version&sort=semver)](https://hub.docker.com/r/mouday/domain-admin)
 [![Docker Pulls](https://img.shields.io/docker/pulls/mouday/domain-admin)](https://hub.docker.com/r/mouday/domain-admin)
 [![Build Status](https://app.travis-ci.com/mouday/domain-admin.svg?branch=master)](https://app.travis-ci.com/mouday/domain-admin)
 [![PyPI - License](https://img.shields.io/pypi/l/domain-admin)](https://github.com/mouday/domain-admin/blob/master/LICENSE)
 
 ![](https://raw.githubusercontent.com/mouday/domain-admin/master/image/domain.svg)
 
-基于Python + Vue3.js 技术栈实现的域名和SSL证书监测平台
-
-核心功能：到期自动邮件提醒
+基于Python3 + Vue3.js 技术栈实现的域名和SSL证书监测平台
 
 用于解决，不同业务域名SSL证书，申请自不同的平台，到期后不能及时收到通知，导致线上访问异常，被老板责骂的问题
 
+核心功能：`域名` 和`SSL证书` 的过期监控，到期提醒，支持邮件、webhook、企业微信、钉钉、飞书等通知方式
+
 支持平台：macOS、Linux、Windows
 
 - 项目地址：https://github.com/mouday/domain-admin
 - 国内镜像：https://gitee.com/mouday/domain-admin
 - pypi：https://pypi.org/project/domain-admin
 - docker：https://hub.docker.com/r/mouday/domain-admin
 
@@ -320,14 +320,59 @@
 
 ### 5、邮件发送失败
 
 可尝试更换端口25或465
 
 ### 6、webhook模板
 
+采用`jinja2` 模板引擎
+
+传入模板的参数示例：
+
+```json
+{
+    "list":[
+        {
+            "domain": "www.demo.com",
+            "start_date": "2023-06-01",
+            "expire_date": "2023-06-21",
+            "expire_days": 20
+        }
+    ]
+}
+```
+
+参数说明
+
+| 参数  | 类型  | 说明 |
+| -| - | - |
+| domain | string | 域名/证书域名
+| start_date | string | 生效时间
+| expire_date | string | 过期时间
+| expire_days | int | 剩余天数
+
+
+示例
+
+```json
+{
+  "title": "域名到期提醒",
+  "content": "{% for row in list %}{{row.domain}} {{row.start_date or '-' }} - {{row.expire_date or '-' }} ({{row.expire_days}}){% endfor %}"
+}
+```
+
+渲染结果
+
+```json
+{
+  "title": "域名到期提醒",
+  "content": "www.demo.com 2023-06-01 - 2023-06-21 (20)"
+}
+```
+
 可以参考接口文档：[更新用户通知配置](docs/notify/updateNotifyOfUser.md)
 
 ### 7、监控域名非443的端口
 
 域名格式
 
 ```
```

### Comparing `domain-admin-1.4.6/domain_admin.egg-info/SOURCES.txt` & `domain-admin-1.4.7/domain_admin.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 domain_admin/migrate/migrate_140_alpha_to_140.py
 domain_admin/migrate/migrate_143_to_144.py
 domain_admin/migrate/migrate_145_to_146.py
 domain_admin/migrate/migrate_common.py
 domain_admin/model/__init__.py
 domain_admin/model/address_model.py
 domain_admin/model/base_model.py
-domain_admin/model/cache_domain_info_model.py
 domain_admin/model/database.py
 domain_admin/model/domain_info_model.py
 domain_admin/model/domain_model.py
 domain_admin/model/group_model.py
 domain_admin/model/log_scheduler_model.py
 domain_admin/model/notify_model.py
 domain_admin/model/system_model.py
@@ -138,15 +137,14 @@
 domain_admin/public/svg/logo.184a2d7d.svg
 domain_admin/router/__init__.py
 domain_admin/router/api_map.py
 domain_admin/router/permission.py
 domain_admin/service/__init__.py
 domain_admin/service/async_task_service.py
 domain_admin/service/auth_service.py
-domain_admin/service/cache_domain_info_service.py
 domain_admin/service/domain_info_service.py
 domain_admin/service/domain_service.py
 domain_admin/service/email_service.py
 domain_admin/service/file_service.py
 domain_admin/service/global_data_service.py
 domain_admin/service/group_service.py
 domain_admin/service/notify_service.py
```

### Comparing `domain-admin-1.4.6/setup.py` & `domain-admin-1.4.7/setup.py`

 * *Files identical despite different names*

