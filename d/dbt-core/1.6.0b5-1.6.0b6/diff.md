# Comparing `tmp/dbt-core-1.6.0b5.tar.gz` & `tmp/dbt-core-1.6.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-core-1.6.0b5.tar", last modified: Thu Jun 22 20:11:20 2023, max compression
+gzip compressed data, was "dbt-core-1.6.0b6.tar", last modified: Fri Jun 23 21:14:41 2023, max compression
```

## Comparing `dbt-core-1.6.0b5.tar` & `dbt-core-1.6.0b6.tar`

### file list

```diff
@@ -1,334 +1,334 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.507325 dbt-core-1.6.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-22 20:11:20.507325 dbt-core-1.6.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.467325 dbt-core-1.6.0b5/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.467325 dbt-core-1.6.0b5/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.471325 dbt-core-1.6.0b5/dbt/adapters/base/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    56679 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/reference_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.471325 dbt-core-1.6.0b5/dbt/adapters/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/relation_configs/config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/relation_configs/config_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/relation_configs/config_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.471325 dbt-core-1.6.0b5/dbt/adapters/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/sql/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/sql/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.471325 dbt-core-1.6.0b5/dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    17531 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/option_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.475325 dbt-core-1.6.0b5/dbt/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/_jinja_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/agate_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/jinja_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/yaml_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22301 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/compilation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.475325 dbt-core-1.6.0b5/dbt/config/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/config/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/config/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16504 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.475325 dbt-core-1.6.0b5/dbt/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22966 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/configured.py
--rw-r--r--   0 runner    (1001) docker     (123)    12760 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/context_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/exceptions_jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/macro_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    59340 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.479325 dbt-core-1.6.0b5/dbt/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.479325 dbt-core-1.6.0b5/dbt/contracts/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51708 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/manifest_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/node_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    52874 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/semantic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    22403 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/unparsed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/publication.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/dataclass_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deprecations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.479325 dbt-core-1.6.0b5/dbt/deps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deps/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deps/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deps/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deps/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deps/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deps/tarball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.459325 dbt-core-1.6.0b5/dbt/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.483325 dbt-core-1.6.0b5/dbt/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.483325 dbt-core-1.6.0b5/dbt/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/docs/source/_ext/dbt_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.483325 dbt-core-1.6.0b5/dbt/events/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/adapter_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/eventmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    62836 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)   115702 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    80024 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.483325 dbt-core-1.6.0b5/dbt/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/graph/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/graph/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/graph/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    29783 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/graph/selector_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/graph/selector_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/helper_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.483325 dbt-core-1.6.0b5/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.487325 dbt-core-1.6.0b5/dbt/include/global_project/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.487325 dbt-core-1.6.0b5/dbt/include/global_project/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/docs/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.463325 dbt-core-1.6.0b5/dbt/include/global_project/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.487325 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/drop_relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/freshness.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/schema.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.487325 dbt-core-1.6.0b5/dbt/include/global_project/macros/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/etc/datetime.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/etc/statement.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.487325 dbt-core-1.6.0b5/dbt/include/global_project/macros/generic_test_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/generic_test_sql/not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/generic_test_sql/relationships.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/generic_test_sql/unique.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.491325 dbt-core-1.6.0b5/dbt/include/global_project/macros/get_custom_name/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.491325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/configs.sql
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/hooks.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.463325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.491325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.491325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/create_materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/refresh_materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.491325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.491325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.491325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/seeds/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.495325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.495325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/tests/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.495325 dbt-core-1.6.0b5/dbt/include/global_project/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/data_types.sql
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/literal.sql
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/replace.sql
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/split_part.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.463325 dbt-core-1.6.0b5/dbt/include/global_project/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/global_project/tests/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/tests/generic/builtin.sql
--rw-r--r--   0 runner    (1001) docker     (123)  1497953 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/starter_project/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/starter_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/starter_project/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.463325 dbt-core-1.6.0b5/dbt/include/starter_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/starter_project/models/example/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/starter_project/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/seeds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/starter_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/starter_project/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/internal_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/node_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.503325 dbt-core-1.6.0b5/dbt/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    17933 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/generic_test_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)    70786 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    51456 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/partial.py
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/schema_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/schema_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/schema_yaml_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/selected_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/semver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.507325 dbt-core-1.6.0b5/dbt/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16559 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/freshness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/list.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/run_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.507325 dbt-core-1.6.0b5/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.507325 dbt-core-1.6.0b5/dbt/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18918 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/tests/fixtures/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    18815 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.507325 dbt-core-1.6.0b5/dbt_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-22 20:11:20.000000 dbt-core-1.6.0b5/dbt_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-06-22 20:11:20.000000 dbt-core-1.6.0b5/dbt_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:11:20.000000 dbt-core-1.6.0b5/dbt_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-22 20:11:20.000000 dbt-core-1.6.0b5/dbt_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:11:20.000000 dbt-core-1.6.0b5/dbt_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-22 20:11:20.000000 dbt-core-1.6.0b5/dbt_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-22 20:11:20.000000 dbt-core-1.6.0b5/dbt_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 20:11:20.507325 dbt-core-1.6.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.095272 dbt-core-1.6.0b6/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-23 21:14:41.095272 dbt-core-1.6.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.059273 dbt-core-1.6.0b6/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.059273 dbt-core-1.6.0b6/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.063273 dbt-core-1.6.0b6/dbt/adapters/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/base/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/base/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56679 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/base/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/base/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/base/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/base/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/base/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/reference_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.063273 dbt-core-1.6.0b6/dbt/adapters/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/relation_configs/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/relation_configs/config_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/relation_configs/config_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.063273 dbt-core-1.6.0b6/dbt/adapters/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/sql/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/adapters/sql/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.063273 dbt-core-1.6.0b6/dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17531 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/cli/option_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/cli/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/cli/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.067273 dbt-core-1.6.0b6/dbt/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/clients/_jinja_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/clients/agate_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/clients/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/clients/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/clients/jinja_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/clients/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/clients/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/clients/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/compilation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.067273 dbt-core-1.6.0b6/dbt/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/config/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16504 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.067273 dbt-core-1.6.0b6/dbt/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22966 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/context/configured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12760 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/context/context_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/context/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/context/exceptions_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/context/macro_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/context/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/context/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59340 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/context/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/context/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/context/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.071272 dbt-core-1.6.0b6/dbt/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.071272 dbt-core-1.6.0b6/dbt/contracts/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51725 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/graph/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/graph/manifest_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/graph/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/graph/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/graph/node_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52874 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/graph/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/graph/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/graph/semantic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22434 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/graph/unparsed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/graph/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/publication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/contracts/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/dataclass_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/deprecations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.071272 dbt-core-1.6.0b6/dbt/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/deps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/deps/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/deps/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/deps/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/deps/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/deps/tarball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.055273 dbt-core-1.6.0b6/dbt/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.071272 dbt-core-1.6.0b6/dbt/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.071272 dbt-core-1.6.0b6/dbt/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/docs/source/_ext/dbt_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.071272 dbt-core-1.6.0b6/dbt/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/events/adapter_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/events/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/events/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/events/eventmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/events/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/events/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/events/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62836 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115702 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/events/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80024 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.075272 dbt-core-1.6.0b6/dbt/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/graph/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/graph/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/graph/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29783 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/graph/selector_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/graph/selector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/helper_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.075272 dbt-core-1.6.0b6/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.075272 dbt-core-1.6.0b6/dbt/include/global_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.075272 dbt-core-1.6.0b6/dbt/include/global_project/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/docs/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.055273 dbt-core-1.6.0b6/dbt/include/global_project/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.075272 dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/drop_relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.079272 dbt-core-1.6.0b6/dbt/include/global_project/macros/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/etc/datetime.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/etc/statement.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.079272 dbt-core-1.6.0b6/dbt/include/global_project/macros/generic_test_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/generic_test_sql/not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/generic_test_sql/relationships.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/generic_test_sql/unique.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.079272 dbt-core-1.6.0b6/dbt/include/global_project/macros/get_custom_name/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.079272 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/configs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/hooks.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.055273 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.079272 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.079272 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/materialized_view/create_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/materialized_view/refresh_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.079272 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.079272 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/view/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.079272 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/seeds/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.083272 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.083272 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.083272 dbt-core-1.6.0b6/dbt/include/global_project/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.083272 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/data_types.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/literal.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/split_part.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.055273 dbt-core-1.6.0b6/dbt/include/global_project/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.083272 dbt-core-1.6.0b6/dbt/include/global_project/tests/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-23 21:14:28.000000 dbt-core-1.6.0b6/dbt/include/global_project/tests/generic/builtin.sql
+-rw-r--r--   0 runner    (1001) docker     (123)  1497953 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/include/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.087272 dbt-core-1.6.0b6/dbt/include/starter_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/include/starter_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/include/starter_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/include/starter_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.087272 dbt-core-1.6.0b6/dbt/include/starter_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/include/starter_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.087272 dbt-core-1.6.0b6/dbt/include/starter_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/include/starter_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.055273 dbt-core-1.6.0b6/dbt/include/starter_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.087272 dbt-core-1.6.0b6/dbt/include/starter_project/models/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.087272 dbt-core-1.6.0b6/dbt/include/starter_project/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/include/starter_project/seeds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.087272 dbt-core-1.6.0b6/dbt/include/starter_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/include/starter_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.087272 dbt-core-1.6.0b6/dbt/include/starter_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/include/starter_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/internal_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/node_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.091272 dbt-core-1.6.0b6/dbt/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17933 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/generic_test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70787 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51456 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/schema_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/schema_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20531 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/schema_yaml_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/parser/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/selected_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/semver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.091272 dbt-core-1.6.0b6/dbt/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16559 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/freshness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/run_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/task/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.091272 dbt-core-1.6.0b6/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.091272 dbt-core-1.6.0b6/dbt/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18918 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/tests/fixtures/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18815 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/dbt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:41.095272 dbt-core-1.6.0b6/dbt_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-23 21:14:40.000000 dbt-core-1.6.0b6/dbt_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-06-23 21:14:41.000000 dbt-core-1.6.0b6/dbt_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:14:40.000000 dbt-core-1.6.0b6/dbt_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 21:14:40.000000 dbt-core-1.6.0b6/dbt_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:14:40.000000 dbt-core-1.6.0b6/dbt_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-23 21:14:40.000000 dbt-core-1.6.0b6/dbt_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-23 21:14:40.000000 dbt-core-1.6.0b6/dbt_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 21:14:41.095272 dbt-core-1.6.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-23 21:14:29.000000 dbt-core-1.6.0b6/setup.py
```

### Comparing `dbt-core-1.6.0b5/PKG-INFO` & `dbt-core-1.6.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.6.0b5
+Version: 1.6.0b6
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b5 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b6 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `dbt-core-1.6.0b5/README.md` & `dbt-core-1.6.0b6/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/base/__init__.py` & `dbt-core-1.6.0b6/dbt/adapters/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/base/column.py` & `dbt-core-1.6.0b6/dbt/adapters/base/column.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/base/connections.py` & `dbt-core-1.6.0b6/dbt/adapters/base/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/base/impl.py` & `dbt-core-1.6.0b6/dbt/adapters/base/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/base/meta.py` & `dbt-core-1.6.0b6/dbt/adapters/base/meta.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/base/plugin.py` & `dbt-core-1.6.0b6/dbt/adapters/base/plugin.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/base/query_headers.py` & `dbt-core-1.6.0b6/dbt/adapters/base/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/base/relation.py` & `dbt-core-1.6.0b6/dbt/adapters/base/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/cache.py` & `dbt-core-1.6.0b6/dbt/adapters/cache.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/factory.py` & `dbt-core-1.6.0b6/dbt/adapters/factory.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/protocol.py` & `dbt-core-1.6.0b6/dbt/adapters/protocol.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/reference_keys.py` & `dbt-core-1.6.0b6/dbt/adapters/reference_keys.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/relation_configs/config_base.py` & `dbt-core-1.6.0b6/dbt/adapters/relation_configs/config_base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/relation_configs/config_change.py` & `dbt-core-1.6.0b6/dbt/adapters/relation_configs/config_change.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/relation_configs/config_validation.py` & `dbt-core-1.6.0b6/dbt/adapters/relation_configs/config_validation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/sql/connections.py` & `dbt-core-1.6.0b6/dbt/adapters/sql/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/adapters/sql/impl.py` & `dbt-core-1.6.0b6/dbt/adapters/sql/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/cli/exceptions.py` & `dbt-core-1.6.0b6/dbt/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/cli/flags.py` & `dbt-core-1.6.0b6/dbt/cli/flags.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/cli/main.py` & `dbt-core-1.6.0b6/dbt/cli/main.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/cli/option_types.py` & `dbt-core-1.6.0b6/dbt/cli/option_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/cli/options.py` & `dbt-core-1.6.0b6/dbt/cli/options.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/cli/params.py` & `dbt-core-1.6.0b6/dbt/cli/params.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/cli/requires.py` & `dbt-core-1.6.0b6/dbt/cli/requires.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/cli/resolvers.py` & `dbt-core-1.6.0b6/dbt/cli/resolvers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/cli/types.py` & `dbt-core-1.6.0b6/dbt/cli/types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/clients/_jinja_blocks.py` & `dbt-core-1.6.0b6/dbt/clients/_jinja_blocks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/clients/agate_helper.py` & `dbt-core-1.6.0b6/dbt/clients/agate_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/clients/git.py` & `dbt-core-1.6.0b6/dbt/clients/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/clients/jinja.py` & `dbt-core-1.6.0b6/dbt/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/clients/jinja_static.py` & `dbt-core-1.6.0b6/dbt/clients/jinja_static.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/clients/registry.py` & `dbt-core-1.6.0b6/dbt/clients/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/clients/system.py` & `dbt-core-1.6.0b6/dbt/clients/system.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/clients/yaml_helper.py` & `dbt-core-1.6.0b6/dbt/clients/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/compilation.py` & `dbt-core-1.6.0b6/dbt/compilation.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,16 +175,16 @@
                 self.dependency(node.unique_id, (manifest.metrics[dependency].unique_id))
             else:
                 raise GraphDependencyNotFoundError(node, dependency)
 
     def link_graph(self, manifest: Manifest):
         for source in manifest.sources.values():
             self.add_node(source.unique_id)
-        for semantic_node in manifest.semantic_nodes.values():
-            self.add_node(semantic_node.unique_id)
+        for semantic_model in manifest.semantic_models.values():
+            self.add_node(semantic_model.unique_id)
 
         for node in manifest.nodes.values():
             self.link_node(node, manifest)
         for exposure in manifest.exposures.values():
             self.link_node(exposure, manifest)
         for metric in manifest.metrics.values():
             self.link_node(metric, manifest)
```

### Comparing `dbt-core-1.6.0b5/dbt/config/profile.py` & `dbt-core-1.6.0b6/dbt/config/profile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/config/project.py` & `dbt-core-1.6.0b6/dbt/config/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/config/renderer.py` & `dbt-core-1.6.0b6/dbt/config/renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/config/runtime.py` & `dbt-core-1.6.0b6/dbt/config/runtime.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/config/selectors.py` & `dbt-core-1.6.0b6/dbt/config/selectors.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/config/utils.py` & `dbt-core-1.6.0b6/dbt/config/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/constants.py` & `dbt-core-1.6.0b6/dbt/constants.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/context/base.py` & `dbt-core-1.6.0b6/dbt/context/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/context/configured.py` & `dbt-core-1.6.0b6/dbt/context/configured.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/context/context_config.py` & `dbt-core-1.6.0b6/dbt/context/context_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/context/docs.py` & `dbt-core-1.6.0b6/dbt/context/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/context/exceptions_jinja.py` & `dbt-core-1.6.0b6/dbt/context/exceptions_jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/context/macro_resolver.py` & `dbt-core-1.6.0b6/dbt/context/macro_resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/context/macros.py` & `dbt-core-1.6.0b6/dbt/context/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/context/manifest.py` & `dbt-core-1.6.0b6/dbt/context/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/context/providers.py` & `dbt-core-1.6.0b6/dbt/context/providers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/context/secret.py` & `dbt-core-1.6.0b6/dbt/context/secret.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/context/target.py` & `dbt-core-1.6.0b6/dbt/context/target.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/contracts/connection.py` & `dbt-core-1.6.0b6/dbt/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/contracts/files.py` & `dbt-core-1.6.0b6/dbt/contracts/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
     tests: Dict[str, Any] = field(default_factory=dict)
     sources: List[str] = field(default_factory=list)
     exposures: List[str] = field(default_factory=list)
     metrics: List[str] = field(default_factory=list)
     groups: List[str] = field(default_factory=list)
     # node patches contain models, seeds, snapshots, analyses
     ndp: List[str] = field(default_factory=list)
-    semantic_nodes: List[str] = field(default_factory=list)
+    semantic_models: List[str] = field(default_factory=list)
     # any macro patches in this file by macro unique_id.
     mcp: Dict[str, str] = field(default_factory=dict)
     # any source patches in this file. The entries are package, name pairs
     # Patches are only against external sources. Sources can be
     # created too, but those are in 'sources'
     sop: List[SourceKey] = field(default_factory=list)
     env_vars: Dict[str, Any] = field(default_factory=dict)
```

### Comparing `dbt-core-1.6.0b5/dbt/contracts/graph/manifest.py` & `dbt-core-1.6.0b6/dbt/contracts/graph/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -697,15 +697,15 @@
     metadata: ManifestMetadata = field(default_factory=ManifestMetadata)
     flat_graph: Dict[str, Any] = field(default_factory=dict)
     state_check: ManifestStateCheck = field(default_factory=ManifestStateCheck)
     source_patches: MutableMapping[SourceKey, SourcePatch] = field(default_factory=dict)
     disabled: MutableMapping[str, List[GraphMemberNode]] = field(default_factory=dict)
     env_vars: MutableMapping[str, str] = field(default_factory=dict)
     publications: MutableMapping[str, PublicationConfig] = field(default_factory=dict)
-    semantic_nodes: MutableMapping[str, SemanticModel] = field(default_factory=dict)
+    semantic_models: MutableMapping[str, SemanticModel] = field(default_factory=dict)
 
     _doc_lookup: Optional[DocLookup] = field(
         default=None, metadata={"serialize": lambda x: None, "deserialize": lambda x: None}
     )
     _source_lookup: Optional[SourceLookup] = field(
         default=None, metadata={"serialize": lambda x: None, "deserialize": lambda x: None}
     )
@@ -749,16 +749,16 @@
         """
         self.flat_graph = {
             "exposures": {k: v.to_dict(omit_none=False) for k, v in self.exposures.items()},
             "groups": {k: v.to_dict(omit_none=False) for k, v in self.groups.items()},
             "metrics": {k: v.to_dict(omit_none=False) for k, v in self.metrics.items()},
             "nodes": {k: v.to_dict(omit_none=False) for k, v in self.nodes.items()},
             "sources": {k: v.to_dict(omit_none=False) for k, v in self.sources.items()},
-            "semantic_nodes": {
-                k: v.to_dict(omit_none=False) for k, v in self.semantic_nodes.items()
+            "semantic_models": {
+                k: v.to_dict(omit_none=False) for k, v in self.semantic_models.items()
             },
         }
 
     def build_disabled_by_file_id(self):
         disabled_by_file_id = {}
         for node_list in self.disabled.values():
             for node in node_list:
@@ -812,15 +812,15 @@
     def get_resource_fqns(self) -> Mapping[str, PathSet]:
         resource_fqns: Dict[str, Set[Tuple[str, ...]]] = {}
         all_resources = chain(
             self.exposures.values(),
             self.nodes.values(),
             self.sources.values(),
             self.metrics.values(),
-            self.semantic_nodes.values(),
+            self.semantic_models.values(),
         )
         for resource in all_resources:
             resource_type_plural = resource.resource_type.pluralize()
             if resource_type_plural not in resource_fqns:
                 resource_fqns[resource_type_plural] = set()
             resource_fqns[resource_type_plural].add(tuple(resource.fqn))
         return resource_fqns
@@ -848,27 +848,27 @@
             groups={k: _deepcopy(v) for k, v in self.groups.items()},
             selectors={k: _deepcopy(v) for k, v in self.selectors.items()},
             metadata=self.metadata,
             disabled={k: _deepcopy(v) for k, v in self.disabled.items()},
             files={k: _deepcopy(v) for k, v in self.files.items()},
             state_check=_deepcopy(self.state_check),
             publications={k: _deepcopy(v) for k, v in self.publications.items()},
-            semantic_nodes={k: _deepcopy(v) for k, v in self.semantic_nodes.items()},
+            semantic_models={k: _deepcopy(v) for k, v in self.semantic_models.items()},
         )
         copy.build_flat_graph()
         return copy
 
     def build_parent_and_child_maps(self):
         edge_members = list(
             chain(
                 self.nodes.values(),
                 self.sources.values(),
                 self.exposures.values(),
                 self.metrics.values(),
-                self.semantic_nodes.values(),
+                self.semantic_models.values(),
             )
         )
         forward_edges, backward_edges = build_node_edges(edge_members)
         self.child_map = forward_edges
         self.parent_map = backward_edges
 
     def build_macro_child_map(self):
@@ -907,15 +907,15 @@
             groups=self.groups,
             selectors=self.selectors,
             metadata=self.metadata,
             disabled=self.disabled,
             child_map=self.child_map,
             parent_map=self.parent_map,
             group_map=self.group_map,
-            semantic_nodes=self.semantic_nodes,
+            semantic_models=self.semantic_models,
         )
 
     def write(self, path):
         self.writable_manifest().write(path)
 
     # Called in dbt.compilation.Linker.write_graph and
     # dbt.graph.queue.get and ._include_in_cost
@@ -924,16 +924,16 @@
             return self.nodes[unique_id]
         elif unique_id in self.sources:
             return self.sources[unique_id]
         elif unique_id in self.exposures:
             return self.exposures[unique_id]
         elif unique_id in self.metrics:
             return self.metrics[unique_id]
-        elif unique_id in self.semantic_nodes:
-            return self.semantic_nodes[unique_id]
+        elif unique_id in self.semantic_models:
+            return self.semantic_models[unique_id]
         else:
             # something terrible has happened
             raise dbt.exceptions.DbtInternalError(
                 "Expected node {} not found in manifest".format(unique_id)
             )
 
     @property
@@ -984,15 +984,15 @@
             self._analysis_lookup = AnalysisLookup(self)
         return self._analysis_lookup
 
     @property
     def pydantic_semantic_manifest(self) -> PydanticSemanticManifest:
         pydantic_semantic_manifest = PydanticSemanticManifest(metrics=[], semantic_models=[])
 
-        for semantic_model in self.semantic_nodes.values():
+        for semantic_model in self.semantic_models.values():
             pydantic_semantic_manifest.semantic_models.append(
                 PydanticSemanticModel.parse_obj(semantic_model.to_dict())
             )
 
         for metric in self.metrics.values():
             pydantic_semantic_manifest.metrics.append(PydanticMetric.parse_obj(metric.to_dict()))
 
@@ -1263,17 +1263,17 @@
 
     def add_doc(self, source_file: SourceFile, doc: Documentation):
         _check_duplicates(doc, self.docs)
         self.docs[doc.unique_id] = doc
         source_file.docs.append(doc.unique_id)
 
     def add_semantic_model(self, source_file: SchemaSourceFile, semantic_model: SemanticModel):
-        _check_duplicates(semantic_model, self.semantic_nodes)
-        self.semantic_nodes[semantic_model.unique_id] = semantic_model
-        source_file.semantic_nodes.append(semantic_model.unique_id)
+        _check_duplicates(semantic_model, self.semantic_models)
+        self.semantic_models[semantic_model.unique_id] = semantic_model
+        source_file.semantic_models.append(semantic_model.unique_id)
 
     # end of methods formerly in ParseResult
 
     # Provide support for copy.deepcopy() - we just need to avoid the lock!
     # pickle and deepcopy use this. It returns a callable object used to
     # create the initial version of the object and a tuple of arguments
     # for the object, i.e. the Manifest.
@@ -1294,15 +1294,15 @@
             self.metadata,
             self.flat_graph,
             self.state_check,
             self.source_patches,
             self.disabled,
             self.env_vars,
             self.publications,
-            self.semantic_nodes,
+            self.semantic_models,
             self._doc_lookup,
             self._source_lookup,
             self._ref_lookup,
             self._metric_lookup,
             self._disabled_lookup,
             self._analysis_lookup,
         )
@@ -1364,15 +1364,15 @@
         )
     )
     group_map: Optional[NodeEdgeMap] = field(
         metadata=dict(
             description="A mapping from group names to their nodes",
         )
     )
-    semantic_nodes: Mapping[UniqueID, SemanticModel] = field(
+    semantic_models: Mapping[UniqueID, SemanticModel] = field(
         metadata=dict(description=("The semantic models defined in the dbt project"))
     )
     metadata: ManifestMetadata = field(
         metadata=dict(
             description="Metadata about the manifest",
         )
     )
```

### Comparing `dbt-core-1.6.0b5/dbt/contracts/graph/manifest_upgrade.py` & `dbt-core-1.6.0b6/dbt/contracts/graph/manifest_upgrade.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,10 +98,10 @@
     for macro_content in manifest.get("macros", {}).values():
         if "root_path" in macro_content:
             del macro_content["root_path"]
     for doc_content in manifest.get("docs", {}).values():
         if "root_path" in doc_content:
             del doc_content["root_path"]
         doc_content["resource_type"] = "doc"
-    if "semantic_nodes" not in manifest:
-        manifest["semantic_nodes"] = {}
+    if "semantic_models" not in manifest:
+        manifest["semantic_models"] = {}
     return manifest
```

### Comparing `dbt-core-1.6.0b5/dbt/contracts/graph/metrics.py` & `dbt-core-1.6.0b6/dbt/contracts/graph/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/contracts/graph/model_config.py` & `dbt-core-1.6.0b6/dbt/contracts/graph/model_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/contracts/graph/node_args.py` & `dbt-core-1.6.0b6/dbt/contracts/graph/node_args.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/contracts/graph/nodes.py` & `dbt-core-1.6.0b6/dbt/contracts/graph/nodes.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/contracts/graph/semantic_models.py` & `dbt-core-1.6.0b6/dbt/contracts/graph/semantic_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,16 +116,16 @@
 # Measure objects
 # ====================================
 
 
 @dataclass
 class MeasureAggregationParameters(dbtClassMixin):
     percentile: Optional[float] = None
-    use_discrete_percentile: Optional[bool] = None
-    use_approximate_percentile: Optional[bool] = None
+    use_discrete_percentile: bool = False
+    use_approximate_percentile: bool = False
 
 
 @dataclass
 class NonAdditiveDimension(dbtClassMixin):
     name: str
     window_choice: AggregationType
     window_grouples: List[str]
```

### Comparing `dbt-core-1.6.0b5/dbt/contracts/graph/unparsed.py` & `dbt-core-1.6.0b6/dbt/contracts/graph/unparsed.py`

 * *Files 1% similar despite different names*

```diff
@@ -614,15 +614,15 @@
 
 
 @dataclass
 class UnparsedMetricTypeParams(dbtClassMixin):
     measure: Optional[Union[UnparsedMetricInputMeasure, str]] = None
     numerator: Optional[Union[UnparsedMetricInput, str]] = None
     denominator: Optional[Union[UnparsedMetricInput, str]] = None
-    expr: Optional[str] = None
+    expr: Optional[Union[str, bool]] = None
     window: Optional[str] = None
     grain_to_date: Optional[str] = None  # str is really a TimeGranularity Enum
     metrics: Optional[List[Union[UnparsedMetricInput, str]]] = None
 
 
 @dataclass
 class UnparsedMetric(dbtClassMixin):
@@ -694,15 +694,15 @@
 
 @dataclass
 class UnparsedMeasure(dbtClassMixin):
     name: str
     agg: str  # actually an enum
     description: Optional[str] = None
     create_metric: bool = False
-    expr: Optional[str] = None
+    expr: Optional[Union[str, bool, int]] = None
     agg_params: Optional[MeasureAggregationParameters] = None
     non_additive_dimension: Optional[UnparsedNonAdditiveDimension] = None
     agg_time_dimension: Optional[str] = None
 
 
 @dataclass
 class UnparsedDimensionTypeParams(dbtClassMixin):
```

### Comparing `dbt-core-1.6.0b5/dbt/contracts/graph/utils.py` & `dbt-core-1.6.0b6/dbt/contracts/graph/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/contracts/project.py` & `dbt-core-1.6.0b6/dbt/contracts/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/contracts/publication.py` & `dbt-core-1.6.0b6/dbt/contracts/publication.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/contracts/relation.py` & `dbt-core-1.6.0b6/dbt/contracts/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/contracts/results.py` & `dbt-core-1.6.0b6/dbt/contracts/results.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/contracts/selection.py` & `dbt-core-1.6.0b6/dbt/contracts/selection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/contracts/sql.py` & `dbt-core-1.6.0b6/dbt/contracts/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/contracts/state.py` & `dbt-core-1.6.0b6/dbt/contracts/state.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/contracts/util.py` & `dbt-core-1.6.0b6/dbt/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/dataclass_schema.py` & `dbt-core-1.6.0b6/dbt/dataclass_schema.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/deprecations.py` & `dbt-core-1.6.0b6/dbt/deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/deps/base.py` & `dbt-core-1.6.0b6/dbt/deps/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/deps/git.py` & `dbt-core-1.6.0b6/dbt/deps/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/deps/local.py` & `dbt-core-1.6.0b6/dbt/deps/local.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/deps/registry.py` & `dbt-core-1.6.0b6/dbt/deps/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/deps/resolver.py` & `dbt-core-1.6.0b6/dbt/deps/resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/deps/tarball.py` & `dbt-core-1.6.0b6/dbt/deps/tarball.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/docs/source/_ext/dbt_click.py` & `dbt-core-1.6.0b6/dbt/docs/source/_ext/dbt_click.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/docs/source/conf.py` & `dbt-core-1.6.0b6/dbt/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/events/adapter_endpoint.py` & `dbt-core-1.6.0b6/dbt/events/adapter_endpoint.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/events/base_types.py` & `dbt-core-1.6.0b6/dbt/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/events/contextvars.py` & `dbt-core-1.6.0b6/dbt/events/contextvars.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/events/eventmgr.py` & `dbt-core-1.6.0b6/dbt/events/eventmgr.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/events/format.py` & `dbt-core-1.6.0b6/dbt/events/format.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/events/functions.py` & `dbt-core-1.6.0b6/dbt/events/functions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/events/helpers.py` & `dbt-core-1.6.0b6/dbt/events/helpers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/events/types.py` & `dbt-core-1.6.0b6/dbt/events/types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/events/types_pb2.py` & `dbt-core-1.6.0b6/dbt/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/exceptions.py` & `dbt-core-1.6.0b6/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/flags.py` & `dbt-core-1.6.0b6/dbt/flags.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/graph/cli.py` & `dbt-core-1.6.0b6/dbt/graph/cli.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/graph/graph.py` & `dbt-core-1.6.0b6/dbt/graph/graph.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/graph/queue.py` & `dbt-core-1.6.0b6/dbt/graph/queue.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/graph/selector.py` & `dbt-core-1.6.0b6/dbt/graph/selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,16 @@
             source = self.manifest.sources[unique_id]
             return source.config.enabled
         elif unique_id in self.manifest.exposures:
             return True
         elif unique_id in self.manifest.metrics:
             metric = self.manifest.metrics[unique_id]
             return metric.config.enabled
+        elif unique_id in self.manifest.semantic_models:
+            return True
         node = self.manifest.nodes[unique_id]
 
         if self.include_empty_nodes:
             return node.config.enabled
         else:
             return not node.empty and node.config.enabled
 
@@ -187,14 +189,16 @@
             node = self.manifest.nodes[unique_id]
         elif unique_id in self.manifest.sources:
             node = self.manifest.sources[unique_id]
         elif unique_id in self.manifest.exposures:
             node = self.manifest.exposures[unique_id]
         elif unique_id in self.manifest.metrics:
             node = self.manifest.metrics[unique_id]
+        elif unique_id in self.manifest.semantic_models:
+            node = self.manifest.semantic_models[unique_id]
         else:
             raise DbtInternalError(f"Node {unique_id} not found in the manifest!")
         return self.node_is_match(node)
 
     def filter_selection(self, selected: Set[UniqueId]) -> Set[UniqueId]:
         """Return the subset of selected nodes that is a match for this
         selector.
```

### Comparing `dbt-core-1.6.0b5/dbt/graph/selector_methods.py` & `dbt-core-1.6.0b6/dbt/graph/selector_methods.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/graph/selector_spec.py` & `dbt-core-1.6.0b6/dbt/graph/selector_spec.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/helper_types.py` & `dbt-core-1.6.0b6/dbt/helper_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/README.md` & `dbt-core-1.6.0b6/dbt/include/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/docs/overview.md` & `dbt-core-1.6.0b6/dbt/include/global_project/docs/overview.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/apply_grants.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/columns.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/drop_relation.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/drop_relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/freshness.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/indexes.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/metadata.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/persist_docs.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/relation.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/schema.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/timestamps.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/adapters/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/etc/datetime.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/etc/datetime.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/etc/statement.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/configs.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/configs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/hooks.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/merge.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/table/table.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/view.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/seeds/helpers.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/seeds/seed.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/seeds/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/helpers.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/strategies.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/tests/helpers.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/tests/test.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/python_model/python.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/data_types.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/listagg.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/split_part.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/global_project/tests/generic/builtin.sql` & `dbt-core-1.6.0b6/dbt/include/global_project/tests/generic/builtin.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/index.html` & `dbt-core-1.6.0b6/dbt/include/index.html`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/starter_project/README.md` & `dbt-core-1.6.0b6/dbt/include/starter_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/include/starter_project/dbt_project.yml` & `dbt-core-1.6.0b6/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/internal_deprecations.py` & `dbt-core-1.6.0b6/dbt/internal_deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/logger.py` & `dbt-core-1.6.0b6/dbt/logger.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/node_types.py` & `dbt-core-1.6.0b6/dbt/node_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/__init__.py` & `dbt-core-1.6.0b6/dbt/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/analysis.py` & `dbt-core-1.6.0b6/dbt/parser/analysis.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/base.py` & `dbt-core-1.6.0b6/dbt/parser/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/common.py` & `dbt-core-1.6.0b6/dbt/parser/common.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/docs.py` & `dbt-core-1.6.0b6/dbt/parser/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/generic_test.py` & `dbt-core-1.6.0b6/dbt/parser/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/generic_test_builders.py` & `dbt-core-1.6.0b6/dbt/parser/generic_test_builders.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/hooks.py` & `dbt-core-1.6.0b6/dbt/parser/hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/macros.py` & `dbt-core-1.6.0b6/dbt/parser/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/manifest.py` & `dbt-core-1.6.0b6/dbt/parser/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1099,15 +1099,15 @@
             if exposure.created_at < self.started_at:
                 continue
             _process_refs(self.manifest, current_project, exposure)
         for metric in self.manifest.metrics.values():
             if metric.created_at < self.started_at:
                 continue
             _process_refs(self.manifest, current_project, metric)
-        for semantic_model in self.manifest.semantic_nodes.values():
+        for semantic_model in self.manifest.semantic_models.values():
             if semantic_model.created_at < self.started_at:
                 continue
             _process_refs(self.manifest, current_project, semantic_model)
             self.update_semantic_model(semantic_model)
 
     # Takes references in 'metrics' array of nodes and exposures, finds the target
     # node, and updates 'depends_on.nodes' with the unique id
```

### Comparing `dbt-core-1.6.0b5/dbt/parser/models.py` & `dbt-core-1.6.0b6/dbt/parser/models.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/partial.py` & `dbt-core-1.6.0b6/dbt/parser/partial.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/read_files.py` & `dbt-core-1.6.0b6/dbt/parser/read_files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/schema_generic_tests.py` & `dbt-core-1.6.0b6/dbt/parser/schema_generic_tests.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/schema_renderer.py` & `dbt-core-1.6.0b6/dbt/parser/schema_renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/schema_yaml_readers.py` & `dbt-core-1.6.0b6/dbt/parser/schema_yaml_readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,15 @@
         if type_params.grain_to_date is not None:
             grain_to_date = TimeGranularity(type_params.grain_to_date)
 
         return MetricTypeParams(
             measure=self._get_optional_input_measure(type_params.measure),
             numerator=self._get_optional_metric_input(type_params.numerator),
             denominator=self._get_optional_metric_input(type_params.denominator),
-            expr=type_params.expr,
+            expr=str(type_params.expr) if type_params.expr is not None else None,
             window=self._get_time_window(type_params.window),
             grain_to_date=grain_to_date,
             metrics=self._get_metric_inputs(type_params.metrics),
             # TODO This is a compiled list of measure/numerator/denominator as
             # well as the `input_measures` of included metrics. We're planning
             # on doing this as part of CT-2707
             # input_measures=?,
@@ -496,15 +496,15 @@
         for unparsed in unparsed_measures:
             measures.append(
                 Measure(
                     name=unparsed.name,
                     agg=AggregationType(unparsed.agg),
                     description=unparsed.description,
                     create_metric=unparsed.create_metric,
-                    expr=unparsed.expr,
+                    expr=str(unparsed.expr) if unparsed.expr is not None else None,
                     agg_params=unparsed.agg_params,
                     non_additive_dimension=self._get_non_additive_dimension(
                         unparsed.non_additive_dimension
                     ),
                     agg_time_dimension=unparsed.agg_time_dimension,
                 )
             )
```

### Comparing `dbt-core-1.6.0b5/dbt/parser/schemas.py` & `dbt-core-1.6.0b6/dbt/parser/schemas.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/search.py` & `dbt-core-1.6.0b6/dbt/parser/search.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/seeds.py` & `dbt-core-1.6.0b6/dbt/parser/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/singular_test.py` & `dbt-core-1.6.0b6/dbt/parser/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/snapshots.py` & `dbt-core-1.6.0b6/dbt/parser/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/sources.py` & `dbt-core-1.6.0b6/dbt/parser/sources.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/parser/sql.py` & `dbt-core-1.6.0b6/dbt/parser/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/semver.py` & `dbt-core-1.6.0b6/dbt/semver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/base.py` & `dbt-core-1.6.0b6/dbt/task/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/build.py` & `dbt-core-1.6.0b6/dbt/task/build.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/clean.py` & `dbt-core-1.6.0b6/dbt/task/clean.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/compile.py` & `dbt-core-1.6.0b6/dbt/task/compile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/debug.py` & `dbt-core-1.6.0b6/dbt/task/debug.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/deps.py` & `dbt-core-1.6.0b6/dbt/task/deps.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/freshness.py` & `dbt-core-1.6.0b6/dbt/task/freshness.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/generate.py` & `dbt-core-1.6.0b6/dbt/task/generate.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/init.py` & `dbt-core-1.6.0b6/dbt/task/init.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/list.py` & `dbt-core-1.6.0b6/dbt/task/list.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/printer.py` & `dbt-core-1.6.0b6/dbt/task/printer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/retry.py` & `dbt-core-1.6.0b6/dbt/task/retry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/run.py` & `dbt-core-1.6.0b6/dbt/task/run.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/run_operation.py` & `dbt-core-1.6.0b6/dbt/task/run_operation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/runnable.py` & `dbt-core-1.6.0b6/dbt/task/runnable.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/seed.py` & `dbt-core-1.6.0b6/dbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/serve.py` & `dbt-core-1.6.0b6/dbt/task/serve.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/show.py` & `dbt-core-1.6.0b6/dbt/task/show.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/snapshot.py` & `dbt-core-1.6.0b6/dbt/task/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/sql.py` & `dbt-core-1.6.0b6/dbt/task/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/task/test.py` & `dbt-core-1.6.0b6/dbt/task/test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/tests/fixtures/project.py` & `dbt-core-1.6.0b6/dbt/tests/fixtures/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/tests/util.py` & `dbt-core-1.6.0b6/dbt/tests/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/tracking.py` & `dbt-core-1.6.0b6/dbt/tracking.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/ui.py` & `dbt-core-1.6.0b6/dbt/ui.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/utils.py` & `dbt-core-1.6.0b6/dbt/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/dbt/version.py` & `dbt-core-1.6.0b6/dbt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,9 +228,9 @@
             # the path is like .../dbt/adapters/{plugin_name}/__version__.py
             # except it could be \\ on windows!
             plugin_root, _ = os.path.split(version_path)
             _, plugin_name = os.path.split(plugin_root)
             yield plugin_name
 
 
-__version__ = "1.6.0b5"
+__version__ = "1.6.0b6"
 installed = get_installed_version()
```

### Comparing `dbt-core-1.6.0b5/dbt_core.egg-info/PKG-INFO` & `dbt-core-1.6.0b6/dbt_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.6.0b5
+Version: 1.6.0b6
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b5 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b6 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `dbt-core-1.6.0b5/dbt_core.egg-info/SOURCES.txt` & `dbt-core-1.6.0b6/dbt_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b5/setup.py` & `dbt-core-1.6.0b6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
 package_name = "dbt-core"
-package_version = "1.6.0b5"
+package_version = "1.6.0b6"
 description = """With dbt, data analysts and engineers can build analytics \
 the way engineers build applications."""
 
 
 setup(
     name=package_name,
     version=package_version,
```

