# Comparing `tmp/ir_measures-0.3.1.tar.gz` & `tmp/ir_measures-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ir_measures-0.3.1.tar", last modified: Sat Aug 20 17:46:15 2022, max compression
+gzip compressed data, was "ir_measures-0.3.3.tar", last modified: Fri Jun 23 11:49:16 2023, max compression
```

## Comparing `ir_measures-0.3.1.tar` & `ir_measures-0.3.3.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-20 17:46:15.000000 ir_measures-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (116)    11358 2022-08-20 17:46:13.000000 ir_measures-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)      101 2022-08-20 17:46:13.000000 ir_measures-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     6447 2022-08-20 17:46:15.000000 ir_measures-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4635 2022-08-20 17:46:13.000000 ir_measures-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-20 17:46:15.000000 ir_measures-0.3.1/ir_measures/
--rw-r--r--   0 runner    (1001) docker     (116)     2043 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4322 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-20 17:46:15.000000 ir_measures-0.3.1/ir_measures/bin/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     4686 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/bin/gdeval.pl
--rw-r--r--   0 runner    (1001) docker     (116)     8042 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/bin/msmarco_eval.py
--rw-r--r--   0 runner    (1001) docker     (116)     2418 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/generate_docs.py
--rw-r--r--   0 runner    (1001) docker     (116)      296 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/lazylibs.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-20 17:46:15.000000 ir_measures-0.3.1/ir_measures/measures/
--rw-r--r--   0 runner    (1001) docker     (116)     1644 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      872 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (116)     1245 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/ap.py
--rw-r--r--   0 runner    (1001) docker     (116)     5055 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     1167 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/bpm.py
--rw-r--r--   0 runner    (1001) docker     (116)      890 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/bpref.py
--rw-r--r--   0 runner    (1001) docker     (116)      988 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/compat.py
--rw-r--r--   0 runner    (1001) docker     (116)     8613 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/diversity.py
--rw-r--r--   0 runner    (1001) docker     (116)      735 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/err.py
--rw-r--r--   0 runner    (1001) docker     (116)      889 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/infap.py
--rw-r--r--   0 runner    (1001) docker     (116)     2182 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/inst.py
--rw-r--r--   0 runner    (1001) docker     (116)      806 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/iprec.py
--rw-r--r--   0 runner    (1001) docker     (116)      614 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/judged.py
--rw-r--r--   0 runner    (1001) docker     (116)     1414 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/ndcg.py
--rw-r--r--   0 runner    (1001) docker     (116)     4493 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/nerr.py
--rw-r--r--   0 runner    (1001) docker     (116)      420 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/numq.py
--rw-r--r--   0 runner    (1001) docker     (116)      633 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/numrel.py
--rw-r--r--   0 runner    (1001) docker     (116)      807 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/numret.py
--rw-r--r--   0 runner    (1001) docker     (116)      971 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/p.py
--rw-r--r--   0 runner    (1001) docker     (116)      878 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/r.py
--rw-r--r--   0 runner    (1001) docker     (116)     1106 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/rbp.py
--rw-r--r--   0 runner    (1001) docker     (116)      942 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/rprec.py
--rw-r--r--   0 runner    (1001) docker     (116)     1140 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/rr.py
--rw-r--r--   0 runner    (1001) docker     (116)      905 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/sdcg.py
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/set_measures.py
--rw-r--r--   0 runner    (1001) docker     (116)      894 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/measures/success.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-20 17:46:15.000000 ir_measures-0.3.1/ir_measures/providers/
--rw-r--r--   0 runner    (1001) docker     (116)      714 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2439 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/providers/accuracy_provider.py
--rw-r--r--   0 runner    (1001) docker     (116)     4514 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     2963 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/providers/compat_provider.py
--rw-r--r--   0 runner    (1001) docker     (116)     9562 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/providers/cwl_eval.py
--rw-r--r--   0 runner    (1001) docker     (116)     2024 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/providers/fallback_provider.py
--rw-r--r--   0 runner    (1001) docker     (116)     2934 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/providers/gdeval_provider.py
--rw-r--r--   0 runner    (1001) docker     (116)     1739 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/providers/judged_provider.py
--rw-r--r--   0 runner    (1001) docker     (116)     2121 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/providers/msmarco_provider.py
--rw-r--r--   0 runner    (1001) docker     (116)     6010 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/providers/pyndeval_provider.py
--rw-r--r--   0 runner    (1001) docker     (116)     9408 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/providers/pytrec_eval_provider.py
--rw-r--r--   0 runner    (1001) docker     (116)     5949 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/providers/ranx_provider.py
--rw-r--r--   0 runner    (1001) docker     (116)     2554 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/providers/runtime_provider.py
--rw-r--r--   0 runner    (1001) docker     (116)     6210 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/providers/trectools_provider.py
--rw-r--r--   0 runner    (1001) docker     (116)    17879 2022-08-20 17:46:13.000000 ir_measures-0.3.1/ir_measures/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-20 17:46:15.000000 ir_measures-0.3.1/ir_measures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6447 2022-08-20 17:46:15.000000 ir_measures-0.3.1/ir_measures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2096 2022-08-20 17:46:15.000000 ir_measures-0.3.1/ir_measures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-20 17:46:15.000000 ir_measures-0.3.1/ir_measures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       63 2022-08-20 17:46:15.000000 ir_measures-0.3.1/ir_measures.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       96 2022-08-20 17:46:15.000000 ir_measures-0.3.1/ir_measures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2022-08-20 17:46:15.000000 ir_measures-0.3.1/ir_measures.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       47 2022-08-20 17:46:13.000000 ir_measures-0.3.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (116)       44 2022-08-20 17:46:13.000000 ir_measures-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-08-20 17:46:15.000000 ir_measures-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1640 2022-08-20 17:46:13.000000 ir_measures-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-20 17:46:15.000000 ir_measures-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (116)     1690 2022-08-20 17:46:13.000000 ir_measures-0.3.1/test/test_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (116)      645 2022-08-20 17:46:13.000000 ir_measures-0.3.1/test/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1446 2022-08-20 17:46:13.000000 ir_measures-0.3.1/test/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (116)     2469 2022-08-20 17:46:13.000000 ir_measures-0.3.1/test/test_cwl_eval.py
--rw-r--r--   0 runner    (1001) docker     (116)     3030 2022-08-20 17:46:13.000000 ir_measures-0.3.1/test/test_gdeval.py
--rw-r--r--   0 runner    (1001) docker     (116)     4984 2022-08-20 17:46:13.000000 ir_measures-0.3.1/test/test_measures.py
--rw-r--r--   0 runner    (1001) docker     (116)    11544 2022-08-20 17:46:13.000000 ir_measures-0.3.1/test/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (116)     1901 2022-08-20 17:46:13.000000 ir_measures-0.3.1/test/test_pyndeval.py
--rw-r--r--   0 runner    (1001) docker     (116)    20416 2022-08-20 17:46:13.000000 ir_measures-0.3.1/test/test_pytrec_eval.py
--rw-r--r--   0 runner    (1001) docker     (116)     6950 2022-08-20 17:46:13.000000 ir_measures-0.3.1/test/test_ranx.py
--rw-r--r--   0 runner    (1001) docker     (116)     4351 2022-08-20 17:46:13.000000 ir_measures-0.3.1/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (116)     7354 2022-08-20 17:46:13.000000 ir_measures-0.3.1/test/test_util.py
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2023-06-23 11:49:16.953198 ir_measures-0.3.3/
+-rw-rw-r--   0 sean      (1000) sean      (1000)    11358 2023-06-23 11:48:47.000000 ir_measures-0.3.3/LICENSE.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)      101 2023-06-23 11:48:47.000000 ir_measures-0.3.3/MANIFEST.in
+-rw-rw-r--   0 sean      (1000) sean      (1000)     5082 2023-06-23 11:49:16.953198 ir_measures-0.3.3/PKG-INFO
+-rw-rw-r--   0 sean      (1000) sean      (1000)     4671 2023-06-23 11:48:47.000000 ir_measures-0.3.3/README.md
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2023-06-23 11:49:16.949198 ir_measures-0.3.3/ir_measures/
+-rw-rw-r--   0 sean      (1000) sean      (1000)     2043 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/__init__.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     4322 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/__main__.py
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2023-06-23 11:49:16.949198 ir_measures-0.3.3/ir_measures/bin/
+-rw-rw-r--   0 sean      (1000) sean      (1000)        0 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/bin/__init__.py
+-rwxrwxr-x   0 sean      (1000) sean      (1000)     4686 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/bin/gdeval.pl
+-rw-rw-r--   0 sean      (1000) sean      (1000)     8042 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/bin/msmarco_eval.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     2787 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/generate_docs.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)      296 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/lazylibs.py
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2023-06-23 11:49:16.953198 ir_measures-0.3.3/ir_measures/measures/
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1644 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/__init__.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)      872 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/accuracy.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1362 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/ap.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     5055 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/base.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1143 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/bpm.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)      877 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/bpref.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)      955 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/compat.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     8535 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/diversity.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)      735 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/err.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)      889 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/infap.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     2124 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/inst.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)      948 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/iprec.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)      615 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/judged.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1522 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/ndcg.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     4397 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/nerr.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)      420 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/numq.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)      633 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/numrel.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)      807 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/numret.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1100 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/p.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1020 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/r.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1082 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/rbp.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1067 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/rprec.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1257 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/rr.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)      905 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/sdcg.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     2726 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/set_measures.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1036 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/measures/success.py
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2023-06-23 11:49:16.953198 ir_measures-0.3.3/ir_measures/providers/
+-rw-rw-r--   0 sean      (1000) sean      (1000)      714 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/providers/__init__.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     2439 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/providers/accuracy_provider.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     4514 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/providers/base.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     2892 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/providers/compat_provider.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     9685 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/providers/cwl_eval.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     2024 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/providers/fallback_provider.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     2962 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/providers/gdeval_provider.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     2367 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/providers/judged_provider.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     2149 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/providers/msmarco_provider.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     6010 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/providers/pyndeval_provider.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)    10245 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/providers/pytrec_eval_provider.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     6155 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/providers/ranx_provider.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     2554 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/providers/runtime_provider.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     6328 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/providers/trectools_provider.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)    17879 2023-06-23 11:48:47.000000 ir_measures-0.3.3/ir_measures/util.py
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2023-06-23 11:49:16.949198 ir_measures-0.3.3/ir_measures.egg-info/
+-rw-rw-r--   0 sean      (1000) sean      (1000)     5082 2023-06-23 11:49:16.000000 ir_measures-0.3.3/ir_measures.egg-info/PKG-INFO
+-rw-rw-r--   0 sean      (1000) sean      (1000)     2116 2023-06-23 11:49:16.000000 ir_measures-0.3.3/ir_measures.egg-info/SOURCES.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)        1 2023-06-23 11:49:16.000000 ir_measures-0.3.3/ir_measures.egg-info/dependency_links.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)       62 2023-06-23 11:49:16.000000 ir_measures-0.3.3/ir_measures.egg-info/entry_points.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)       96 2023-06-23 11:49:16.000000 ir_measures-0.3.3/ir_measures.egg-info/requires.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)       12 2023-06-23 11:49:16.000000 ir_measures-0.3.3/ir_measures.egg-info/top_level.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)       47 2023-06-23 11:48:47.000000 ir_measures-0.3.3/requirements-test.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)       44 2023-06-23 11:48:47.000000 ir_measures-0.3.3/requirements.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)       38 2023-06-23 11:49:16.953198 ir_measures-0.3.3/setup.cfg
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1640 2023-06-23 11:48:47.000000 ir_measures-0.3.3/setup.py
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2023-06-23 11:49:16.953198 ir_measures-0.3.3/test/
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1690 2023-06-23 11:48:47.000000 ir_measures-0.3.3/test/test_accuracy.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)      645 2023-06-23 11:48:47.000000 ir_measures-0.3.3/test/test_aggregate.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1446 2023-06-23 11:48:47.000000 ir_measures-0.3.3/test/test_compat.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     2469 2023-06-23 11:48:47.000000 ir_measures-0.3.3/test/test_cwl_eval.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     3030 2023-06-23 11:48:47.000000 ir_measures-0.3.3/test/test_gdeval.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1386 2023-06-23 11:48:47.000000 ir_measures-0.3.3/test/test_judged.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     4984 2023-06-23 11:48:47.000000 ir_measures-0.3.3/test/test_measures.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)    11544 2023-06-23 11:48:47.000000 ir_measures-0.3.3/test/test_providers.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     1901 2023-06-23 11:48:47.000000 ir_measures-0.3.3/test/test_pyndeval.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)    22804 2023-06-23 11:48:47.000000 ir_measures-0.3.3/test/test_pytrec_eval.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     6950 2023-06-23 11:48:47.000000 ir_measures-0.3.3/test/test_ranx.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     4351 2023-06-23 11:48:47.000000 ir_measures-0.3.3/test/test_runtime.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)     7354 2023-06-23 11:48:47.000000 ir_measures-0.3.3/test/test_util.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ir_measures-0.3.1/LICENSE.txt` & `ir_measures-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/README.md` & `ir_measures-0.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -171,7 +171,8 @@
 
 ## Credits
 
  - Sean MacAvaney, University of Glasgow
  - Craig Macdonald, University of Glasgow
  - Charlie Clarke, University of Waterloo
  - Benjamin Piwowarski, CNRS
+ - Harry Scells, Leipzig University
```

### Comparing `ir_measures-0.3.1/ir_measures/__init__.py` & `ir_measures-0.3.3/ir_measures/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.1"
+__version__ = "0.3.3"
 import sys
 import logging
 from . import util
 from . import lazylibs
 from .util import (parse_measure, parse_trec_measure,
                    read_trec_qrels, read_trec_run,
                    Qrel, ScoredDoc, Metric,
@@ -38,25 +38,25 @@
 
 define = providers.define
 define_byquery = providers.define_byquery
 
 CwlMetric = providers.CwlMetric
 
 DefaultPipeline = providers.FallbackProvider([
+    runtime,
     pytrec_eval,
     cwl_eval,
     compat,
     pyndeval,
     # trectools,  # buggy; will add back later
     judged,
     msmarco,
     gdeval,  # doesn't work when installed from package #9
     accuracy,
     ranx,
-    runtime,
 ])
 evaluator = DefaultPipeline.evaluator
 calc_ctxt = DefaultPipeline.calc_ctxt # deprecated; replaced with evaluator
 iter_calc = DefaultPipeline.iter_calc
 calc_aggregate = DefaultPipeline.calc_aggregate
 
 __all__ = measures.__all__
```

### Comparing `ir_measures-0.3.1/ir_measures/__main__.py` & `ir_measures-0.3.3/ir_measures/__main__.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/bin/gdeval.pl` & `ir_measures-0.3.3/ir_measures/bin/gdeval.pl`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/bin/msmarco_eval.py` & `ir_measures-0.3.3/ir_measures/bin/msmarco_eval.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/generate_docs.py` & `ir_measures-0.3.3/ir_measures/generate_docs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,25 @@
+import re
 import ir_measures
 
+def docstring2rst(docstring):
+    citation = re.search(r'<cite>(.*)</cite>', docstring, flags=re.M | re.S)
+    docstring = re.sub(r'<cite>(.*)</cite>', '', docstring, flags=re.M | re.S).replace('    ', '')
+    if citation:
+        citation = citation.group(1).replace('\n', '\n  ')
+        return f'''
+{docstring}
+
+::
+
+{citation}
+'''
+    else:
+        return docstring
+
 def main():
     with open('docs/measures.rst', 'wt') as f:
         measures, aliases = [], []
         for name, val in ir_measures.measures.registry.items():
             if name == val.NAME:
                 measures.append((name, val))
             else:
@@ -15,15 +31,15 @@
 =========================
 ''')
         for name, val in measures:
             f.write(f'''
 ``{name}``
 -------------------------
 
-{val.__doc__.replace('    ', '')}
+{docstring2rst(val.__doc__)}
 ''')
             if val.SUPPORTED_PARAMS:
                 f.write('''**Parameters:**\n\n''')
                 for p, param in val.SUPPORTED_PARAMS.items():
                     f.write(f'- ``{p}`` ({param.dtype.__name__}) - {param.desc}\n')
                 f.write('\n\n')
             measure_providers = [(n, [m for m in p.SUPPORTED_MEASURES if m.__name__ == val.__name__]) for n, p in ir_measures.providers.registry.items()]
@@ -55,15 +71,15 @@
 =========================
 ''')
         for name, val in sorted(ir_measures.providers.registry.items()):
             f.write(f'''
 ``{name}``
 -------------------------
 
-{val.__doc__.replace('    ', ' ')}
+{docstring2rst(val.__doc__)}
 ''')
             f.write('''**Supported Measures:**\n\n''')
             for measure in val.SUPPORTED_MEASURES:
                 f.write(f' - ``{measure}``\n')
             f.write('\n\n')
 
 if __name__ == '__main__':
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/__init__.py` & `ir_measures-0.3.3/ir_measures/measures/__init__.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/measures/accuracy.py` & `ir_measures-0.3.3/ir_measures/measures/accuracy.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/measures/ap.py` & `ir_measures-0.3.3/ir_measures/measures/ap.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,32 +6,33 @@
     """
     The [Mean] Average Precision ([M]AP). The average precision of a single query is the mean
     of the precision scores at each relevant item returned in a search results list.
     
     AP is typically used for adhoc ranking tasks where getting as many relevant items as possible is. It is commonly referred to as MAP,
     by taking the mean of AP over the query set.
 
-::
-
-    @article{Harman:1992:ESIR,
-      author = {Donna Harman},
-      title = {Evaluation Issues in Information Retrieval},
-      journal = {Information Processing and Management},
-      volume = {28},
-      number = {4},
-      pages = {439 - -440},
-      year = {1992},
-    }
+<cite>
+@article{Harman:1992:ESIR,
+  author = {Donna Harman},
+  title = {Evaluation Issues in Information Retrieval},
+  journal = {Information Processing and Management},
+  volume = {28},
+  number = {4},
+  pages = {439 - -440},
+  year = {1992},
+}
+</cite>
     """
     __name__ = 'AP'
     NAME = __name__
     PRETTY_NAME = '(Mean) Average Precision'
     SHORT_DESC = 'The mean of the precision scores at each relevant item retrieved.'
     SUPPORTED_PARAMS = {
         'cutoff': measures.ParamInfo(dtype=int, required=False, desc='ranking cutoff threshold'),
-        'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)')
+        'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)'),
+        'judged_only': measures.ParamInfo(dtype=bool, default=False, desc='ignore returned documents that do not have relevance judgments'),
     }
 
 
 AP = _AP()
 MAP = AP
 measures.register(AP, ['MAP'])
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/base.py` & `ir_measures-0.3.3/ir_measures/measures/base.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/measures/bpm.py` & `ir_measures-0.3.3/ir_measures/measures/bpm.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from .base import Measure, ParamInfo
 
 
 class _BPM(measures.Measure):
     """
     The Bejeweled Player Model (BPM).
 
-::
-
-     @inproceedings{Zhang:2017:EWS:3077136.3080841,
-       author = {Zhang, Fan and Liu, Yiqun and Li, Xin and Zhang, Min and Xu, Yinghui and Ma, Shaoping},
-       title = {Evaluating Web Search with a Bejeweled Player Model},
-       booktitle = {SIGIR},
-       year = {2017},
-       url = {http://doi.acm.org/10.1145/3077136.3080841}
-     }
+<cite>
+@inproceedings{Zhang:2017:EWS:3077136.3080841,
+  author = {Zhang, Fan and Liu, Yiqun and Li, Xin and Zhang, Min and Xu, Yinghui and Ma, Shaoping},
+  title = {Evaluating Web Search with a Bejeweled Player Model},
+  booktitle = {SIGIR},
+  year = {2017},
+  url = {http://doi.acm.org/10.1145/3077136.3080841}
+}
+</cite>
     """
     __name__ = 'BPM'
     NAME = __name__
     PRETTY_NAME = 'Bejeweled Player Model'
     SHORT_DESC = 'A measure that balances both gain and user patience to determine when they stop traversing search results.'
     SUPPORTED_PARAMS = {
         'cutoff': measures.ParamInfo(dtype=int, required=True, desc='ranking cutoff threshold'),
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/bpref.py` & `ir_measures-0.3.3/ir_measures/measures/bpref.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 
 class _Bpref(measures.Measure):
     """
     Binary Preference (Bpref).
     This measure examines the relative ranks of judged relevant and non-relevant documents. Non-judged documents are not considered. 
 
-::
-
-    @inproceedings{Buckley2004RetrievalEW,
-      title={Retrieval evaluation with incomplete information},
-      author={Chris Buckley and Ellen M. Voorhees},
-      booktitle={SIGIR},
-      year={2004}
-    }
+<cite>
+@inproceedings{Buckley2004RetrievalEW,
+  title={Retrieval evaluation with incomplete information},
+  author={Chris Buckley and Ellen M. Voorhees},
+  booktitle={SIGIR},
+  year={2004}
+}
+</cite>
     """
     __name__ = 'Bpref'
     NAME = __name__
     PRETTY_NAME = 'Binary Preference'
     SHORT_DESC = 'The relative ranks of judged relevant and non-relevant documents.'
     SUPPORTED_PARAMS = {
         'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)')
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/compat.py` & `ir_measures-0.3.3/ir_measures/measures/compat.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 from .base import Measure, ParamInfo
 
 
 class _Compat(measures.Measure):
     """
     Compatibility measure desribed in:
 
-::
-
-    @article{10.1145/3451161,
-      author = {Clarke, Charles L. A. and Vtyurina, Alexandra and Smucker, Mark D.},
-      title = {Assessing Top-k Preferences},
-      journal = {ACM Transactions on Information Systems},
-      volume = {39},
-      number = {3},
-      articleno = {33},
-      numpages = {21},
-      year = {2021},
-      url = {https://doi.org/10.1145/3451161},
-    }
+<cite>
+@article{10.1145/3451161,
+  author = {Clarke, Charles L. A. and Vtyurina, Alexandra and Smucker, Mark D.},
+  title = {Assessing Top-k Preferences},
+  journal = {ACM Transactions on Information Systems},
+  volume = {39},
+  number = {3},
+  articleno = {33},
+  numpages = {21},
+  year = {2021},
+  url = {https://doi.org/10.1145/3451161},
+}
+</cite>
     """
     __name__ = 'Compat'
     NAME = __name__
     PRETTY_NAME = 'Compatibility'
     SHORT_DESC = 'The Rank Biased Overlap between the results and an ideal ranking.'
     SUPPORTED_PARAMS = {
         'p': measures.ParamInfo(dtype=float, default=0.95, desc='persistence'),
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/diversity.py` & `ir_measures-0.3.3/ir_measures/measures/diversity.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from .base import BaseMeasure, ParamInfo
 
 
 class _ERR_IA(measures.BaseMeasure):
     """
     Intent-Aware Expected Reciprocal Rank with collection-independent normalisation.
 
-::
-
-    @inproceedings{10.1145/1645953.1646033,
-      author = {Chapelle, Olivier and Metlzer, Donald and Zhang, Ya and Grinspan, Pierre},
-      title = {Expected Reciprocal Rank for Graded Relevance},
-      booktitle = {CIKM},
-      year = {2009}
-    }
+<cite>
+@inproceedings{10.1145/1645953.1646033,
+  author = {Chapelle, Olivier and Metlzer, Donald and Zhang, Ya and Grinspan, Pierre},
+  title = {Expected Reciprocal Rank for Graded Relevance},
+  booktitle = {CIKM},
+  year = {2009}
+}
+</cite>
     """
     __name__ = 'ERR_IA'
     NAME = __name__
     PRETTY_NAME = 'Intent-Aware Expected Reciprocal Rank'
     SHORT_DESC = 'A version of ERR that accounts for multiple possible query intents.'
     SUPPORTED_PARAMS = {
         'cutoff': measures.ParamInfo(dtype=int, required=False, desc='ranking cutoff threshold'),
@@ -25,22 +25,22 @@
         'judged_only': measures.ParamInfo(dtype=bool, default=False, desc='calculate measure using only judged documents (i.e., discard unjudged documents)'),
     }
 
 class _nERR_IA(measures.BaseMeasure):
     """
     Intent-Aware Expected Reciprocal Rank with collection-dependent normalisation.
 
-::
-
-    @inproceedings{10.1145/1645953.1646033,
-      author = {Chapelle, Olivier and Metlzer, Donald and Zhang, Ya and Grinspan, Pierre},
-      title = {Expected Reciprocal Rank for Graded Relevance},
-      booktitle = {CIKM},
-      year = {2009}
-    }
+<cite>
+@inproceedings{10.1145/1645953.1646033,
+  author = {Chapelle, Olivier and Metlzer, Donald and Zhang, Ya and Grinspan, Pierre},
+  title = {Expected Reciprocal Rank for Graded Relevance},
+  booktitle = {CIKM},
+  year = {2009}
+}
+</cite>
     """
     __name__ = 'nERR_IA'
     NAME = __name__
     PRETTY_NAME = 'Intent-Aware Normalised Expected Reciprocal Rank'
     SHORT_DESC = 'A normalised version of ERR that accounts for multiple possible query intents.'
     SUPPORTED_PARAMS = {
         'cutoff': measures.ParamInfo(dtype=int, required=False, desc='ranking cutoff threshold'),
@@ -48,22 +48,22 @@
         'judged_only': measures.ParamInfo(dtype=bool, default=False, desc='calculate measure using only judged documents (i.e., discard unjudged documents)'),
     }
 
 class _alpha_DCG(measures.BaseMeasure):
     """
     A version of DCG that accounts for multiple possible query intents.
 
-::
-
-    @inproceedings{Clarke2008NoveltyAD,
-      title={Novelty and diversity in information retrieval evaluation},
-      author={Charles L. A. Clarke and Maheedhar Kolla and Gordon V. Cormack and Olga Vechtomova and Azin Ashkan and Stefan B{\"u}ttcher and Ian MacKinnon},
-      booktitle={SIGIR},
-      year={2008}
-    }
+<cite>
+@inproceedings{Clarke2008NoveltyAD,
+  title={Novelty and diversity in information retrieval evaluation},
+  author={Charles L. A. Clarke and Maheedhar Kolla and Gordon V. Cormack and Olga Vechtomova and Azin Ashkan and Stefan B{\"u}ttcher and Ian MacKinnon},
+  booktitle={SIGIR},
+  year={2008}
+}
+</cite>
     """
     __name__ = 'alpha_DCG'
     NAME = __name__
     PRETTY_NAME = 'Alpha Discounted Cumulative Gain'
     SHORT_DESC = 'A version of DCG that accounts for multiple possible query intents.'
     SUPPORTED_PARAMS = {
         'cutoff': measures.ParamInfo(dtype=int, required=False, desc='ranking cutoff threshold'),
@@ -72,22 +72,22 @@
         'judged_only': measures.ParamInfo(dtype=bool, default=False, desc='calculate measure using only judged documents (i.e., discard unjudged documents)'),
     }
 
 class _alpha_nDCG(measures.BaseMeasure):
     """
     A version of nDCG that accounts for multiple possible query intents.
 
-::
-
-    @inproceedings{Clarke2008NoveltyAD,
-      title={Novelty and diversity in information retrieval evaluation},
-      author={Charles L. A. Clarke and Maheedhar Kolla and Gordon V. Cormack and Olga Vechtomova and Azin Ashkan and Stefan B{\"u}ttcher and Ian MacKinnon},
-      booktitle={SIGIR},
-      year={2008}
-    }
+<cite>
+@inproceedings{Clarke2008NoveltyAD,
+  title={Novelty and diversity in information retrieval evaluation},
+  author={Charles L. A. Clarke and Maheedhar Kolla and Gordon V. Cormack and Olga Vechtomova and Azin Ashkan and Stefan B{\"u}ttcher and Ian MacKinnon},
+  booktitle={SIGIR},
+  year={2008}
+}
+</cite>
     """
     __name__ = 'alpha_nDCG'
     NAME = __name__
     PRETTY_NAME = 'Alpha Normalised Discounted Cumulative Gain'
     SHORT_DESC = 'A version of nDCG that accounts for multiple possible query intents.'
     SUPPORTED_PARAMS = {
         'cutoff': measures.ParamInfo(dtype=int, required=False, desc='ranking cutoff threshold'),
@@ -96,22 +96,22 @@
         'judged_only': measures.ParamInfo(dtype=bool, default=False, desc='calculate measure using only judged documents (i.e., discard unjudged documents)'),
     }
 
 class _NRBP(measures.BaseMeasure):
     """
     Novelty- and Rank-Biased Precision with collection-independent normalisation.
 
-::
-
-    @InProceedings{10.1007/978-3-642-04417-5_17,
-      author="Clarke, Charles L. A. and Kolla, Maheedhar and Vechtomova, Olga",
-      title="An Effectiveness Measure for Ambiguous and Underspecified Queries ",
-      booktitle="ICTIR",
-      year="2009"
-    }
+<cite>
+@InProceedings{10.1007/978-3-642-04417-5_17,
+  author="Clarke, Charles L. A. and Kolla, Maheedhar and Vechtomova, Olga",
+  title="An Effectiveness Measure for Ambiguous and Underspecified Queries ",
+  booktitle="ICTIR",
+  year="2009"
+}
+</cite>
     """
     __name__ = 'NRBP'
     NAME = __name__
     PRETTY_NAME = 'Novelty- and Rank-Biased Precision'
     SHORT_DESC = 'A version of RBP that accounts for multiple possible query intents.'
     SUPPORTED_PARAMS = {
         'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)'),
@@ -119,22 +119,22 @@
         'beta': measures.ParamInfo(dtype=float, default=0.5, desc='Patience'),
     }
 
 class _nNRBP(measures.BaseMeasure):
     """
     Novelty- and Rank-Biased Precision with collection-dependent normalisation.
 
-::
-
-    @InProceedings{10.1007/978-3-642-04417-5_17,
-      author="Clarke, Charles L. A. and Kolla, Maheedhar and Vechtomova, Olga",
-      title="An Effectiveness Measure for Ambiguous and Underspecified Queries ",
-      booktitle="ICTIR",
-      year="2009"
-    }
+<cite>
+@InProceedings{10.1007/978-3-642-04417-5_17,
+  author="Clarke, Charles L. A. and Kolla, Maheedhar and Vechtomova, Olga",
+  title="An Effectiveness Measure for Ambiguous and Underspecified Queries ",
+  booktitle="ICTIR",
+  year="2009"
+}
+</cite>
     """
     __name__ = 'nNRBP'
     NAME = __name__
     PRETTY_NAME = 'Normalised Novelty- and Rank-Biased Precision'
     SHORT_DESC = 'A normalised version of RBP that accounts for multiple possible query intents.'
     SUPPORTED_PARAMS = {
         'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)'),
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/err.py` & `ir_measures-0.3.3/ir_measures/measures/err.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/measures/infap.py` & `ir_measures-0.3.3/ir_measures/measures/infap.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/measures/inst.py` & `ir_measures-0.3.3/ir_measures/measures/inst.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from .base import Measure, ParamInfo, SumAgg
 
 
 class _INST(measures.Measure):
     """
     INST, a variant of INSQ
 
-::
-
-     @inproceedings{10.1145/2766462.2767728,
-       author = {Bailey, Peter and Moffat, Alistair and Scholer, Falk and Thomas, Paul},
-       title = {User Variability and IR System Evaluation},
-       year = {2015},
-       booktitle = {Proceedings of the 38th International ACM SIGIR Conference on Research and Development in Information Retrieval},
-       pages = {625–634},
-       series = {SIGIR '15},
-       url = {https://doi.org/10.1145/2766462.2767728}
-     }
+<cite>
+@inproceedings{10.1145/2766462.2767728,
+  author = {Bailey, Peter and Moffat, Alistair and Scholer, Falk and Thomas, Paul},
+  title = {User Variability and IR System Evaluation},
+  year = {2015},
+  booktitle = {Proceedings of the 38th International ACM SIGIR Conference on Research and Development in Information Retrieval},
+  pages = {625–634},
+  series = {SIGIR '15},
+  url = {https://doi.org/10.1145/2766462.2767728}
+}
+</cite>
     """
     __name__ = 'INST'
     NAME = __name__
     PRETTY_NAME = 'INST'
     SHORT_DESC = 'An improved version of INSQ that better handles when either no documents or all retrieved documents are relevant.'
     SUPPORTED_PARAMS = {
         'T': measures.ParamInfo(dtype=float, default=1.0, desc='total desired gain (normalized)'),
@@ -29,23 +29,23 @@
     }
 
 
 class _INSQ(measures.Measure):
     """
     INSQ
 
-::
-
-     @inproceedings{Moffat:2012:MMI:2407085.2407092,
-       author = {Moffat, Alistair and Scholer, Falk and Thomas, Paul},
-       title = {Models and Metrics: IR Evaluation As a User Process},
-       booktitle = {Proceedings of the Seventeenth Australasian Document Computing Symposium},
-       year = {2012},
-       url = {http://doi.acm.org/10.1145/2407085.2407092}
-     }
+<cite>
+@inproceedings{Moffat:2012:MMI:2407085.2407092,
+  author = {Moffat, Alistair and Scholer, Falk and Thomas, Paul},
+  title = {Models and Metrics: IR Evaluation As a User Process},
+  booktitle = {Proceedings of the Seventeenth Australasian Document Computing Symposium},
+  year = {2012},
+  url = {http://doi.acm.org/10.1145/2407085.2407092}
+}
+</cite>
     """
     __name__ = 'INSQ'
     NAME = __name__
     PRETTY_NAME = 'INSQ'
     SHORT_DESC = 'A weighted precision measure based on the conditional probability of the user continuing to the next item.'
     SUPPORTED_PARAMS = {
         'T': measures.ParamInfo(dtype=float, default=1.0, desc='total desired gain (normalized)'),
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/iprec.py` & `ir_measures-0.3.3/ir_measures/measures/iprec.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,13 +11,14 @@
     __name__ = 'IPrec'
     NAME = __name__
     PRETTY_NAME = 'Interpolated Precision@recall'
     SHORT_DESC = 'The interpolated precision at a given recall cutoff.'
     AT_PARAM = 'recall'
     SUPPORTED_PARAMS = {
         'recall': measures.ParamInfo(dtype=float, required=True, desc='recall threshold'),
-        'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)')
+        'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)'),
+        'judged_only': measures.ParamInfo(dtype=bool, default=False, desc='ignore returned documents that do not have relevance judgments'),
     }
 
 
 IPrec = _IPrec()
 measures.register(IPrec)
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/judged.py` & `ir_measures-0.3.3/ir_measures/measures/judged.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
     a rel lower than any judgment.
     """
     __name__ = 'Judged'
     NAME = __name__
     PRETTY_NAME = 'Judgment Rate at k'
     SHORT_DESC = 'The percentage of results in the top k that have a relevance judgment.'
     SUPPORTED_PARAMS = {
-        'cutoff': measures.ParamInfo(dtype=int, required=True, desc='ranking cutoff threshold'),
+        'cutoff': measures.ParamInfo(dtype=int, required=False, desc='ranking cutoff threshold'),
     }
 
 
 Judged = _Judged()
 measures.register(Judged)
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/ndcg.py` & `ir_measures-0.3.3/ir_measures/measures/ndcg.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,35 +4,36 @@
 
 class _nDCG(measures.Measure):
     """
     The normalized Discounted Cumulative Gain (nDCG).
     Uses graded labels - systems that put the highest graded documents at the top of the ranking.
     It is normalized wrt. the Ideal NDCG, i.e. documents ranked in descending order of graded label.
 
-::
-
-    @article{Jarvelin:2002:CGE:582415.582418,
-      author = {J\"{a}rvelin, Kalervo and Kek\"{a}l\"{a}inen, Jaana},
-      title = {Cumulated Gain-based Evaluation of IR Techniques},
-      journal = {ACM Trans. Inf. Syst.},
-      volume = {20},
-      number = {4},
-      year = {2002},
-      pages = {422--446},
-      numpages = {25},
-      url = {http://doi.acm.org/10.1145/582415.582418},
-    }
+<cite>
+@article{Jarvelin:2002:CGE:582415.582418,
+  author = {J\"{a}rvelin, Kalervo and Kek\"{a}l\"{a}inen, Jaana},
+  title = {Cumulated Gain-based Evaluation of IR Techniques},
+  journal = {ACM Trans. Inf. Syst.},
+  volume = {20},
+  number = {4},
+  year = {2002},
+  pages = {422--446},
+  numpages = {25},
+  url = {http://doi.acm.org/10.1145/582415.582418},
+}
+</cite>
     """
     __name__ = 'nDCG'
     NAME = __name__
     PRETTY_NAME = 'Normalised Discounted Cumulative Gain'
     SHORT_DESC = 'A measure of the total gain a user encounters in a result list, discounted by rank and normalised against an ideal ranking.'
     SUPPORTED_PARAMS = {
         'cutoff': measures.ParamInfo(dtype=int, required=False, desc='ranking cutoff threshold'),
         'dcg': measures.ParamInfo(dtype=str, choices=['log2', 'exp-log2'], default='log2', desc='DCG formulation'),
         'gains': measures.ParamInfo(dtype=dict, desc='custom gain mapping (int-to-int)'),
+        'judged_only': measures.ParamInfo(dtype=bool, default=False, desc='ignore returned documents that do not have relevance judgments'),
     }
 
 
 nDCG = _nDCG()
 NDCG = nDCG
 measures.register(nDCG, ['NDCG'])
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/nerr.py` & `ir_measures-0.3.3/ir_measures/measures/nerr.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from .base import Measure, ParamInfo
 
 
 class _NERR8(measures.Measure):
     """
     Version of the Not (but Nearly) Expected Reciprocal Rank (NERR) measure, version from Equation (8) of the the following paper.
 
-::
-
-     @inproceedings{Azzopardi:2021:ECE:3471158.3472239,
-       author = {Azzopardi, Leif and Mackenzie, Joel and Moffat, Alistair},
-       title = {{ERR} is not {C/W/L}: Exploring the Relationship Between Expected Reciprocal Rank and Other Metrics},
-       booktitle = {ICTIR},
-       year = {2021},
-       url = {https://doi.org/10.1145/3471158.3472239}
-     }
+<cite>
+@inproceedings{Azzopardi:2021:ECE:3471158.3472239,
+  author = {Azzopardi, Leif and Mackenzie, Joel and Moffat, Alistair},
+  title = {{ERR} is not {C/W/L}: Exploring the Relationship Between Expected Reciprocal Rank and Other Metrics},
+  booktitle = {ICTIR},
+  year = {2021},
+  url = {https://doi.org/10.1145/3471158.3472239}
+}
+</cite>
     """
     __name__ = 'NERR8'
     NAME = __name__
     PRETTY_NAME = 'Nearly Expected Reciprocal Rank Eq 8'
     SHORT_DESC = 'A C/W/L approximation of ERR using gain-based stopping with truncation at k.'
     SUPPORTED_PARAMS = {
         'cutoff': measures.ParamInfo(dtype=int, required=True, desc='ranking cutoff threshold'),
@@ -26,23 +26,23 @@
         'max_rel': measures.ParamInfo(dtype=int, required=True, desc='maximum relevance score'),
     }
 
 class _NERR9(measures.Measure):
     """
     Version of the Not (but Nearly) Expected Reciprocal Rank (NERR) measure, version from Equation (9) of the the following paper.
 
-::
-
-     @inproceedings{Azzopardi:2021:ECE:3471158.3472239,
-       author = {Azzopardi, Leif and Mackenzie, Joel and Moffat, Alistair},
-       title = {{ERR} is not {C/W/L}: Exploring the Relationship Between Expected Reciprocal Rank and Other Metrics},
-       booktitle = {ICTIR},
-       year = {2021},
-       url = {https://doi.org/10.1145/3471158.3472239}
-     }
+<cite>
+@inproceedings{Azzopardi:2021:ECE:3471158.3472239,
+  author = {Azzopardi, Leif and Mackenzie, Joel and Moffat, Alistair},
+  title = {{ERR} is not {C/W/L}: Exploring the Relationship Between Expected Reciprocal Rank and Other Metrics},
+  booktitle = {ICTIR},
+  year = {2021},
+  url = {https://doi.org/10.1145/3471158.3472239}
+}
+</cite>
     """
     __name__ = 'NERR9'
     NAME = __name__
     PRETTY_NAME = 'Nearly Expected Reciprocal Rank Eq 9'
     SHORT_DESC = 'A C/W/L approximation of ERR using gain-based stopping and discount with truncation at k.'
     SUPPORTED_PARAMS = {
         'cutoff': measures.ParamInfo(dtype=int, required=True, desc='ranking cutoff threshold'),
@@ -50,23 +50,23 @@
         'max_rel': measures.ParamInfo(dtype=int, required=True, desc='maximum relevance score'),
     }
 
 class _NERR10(measures.Measure):
     """
     Version of the Not (but Nearly) Expected Reciprocal Rank (NERR) measure, version from Equation (10) of the the following paper.
 
-::
-
-     @inproceedings{Azzopardi:2021:ECE:3471158.3472239,
-       author = {Azzopardi, Leif and Mackenzie, Joel and Moffat, Alistair},
-       title = {{ERR} is not {C/W/L}: Exploring the Relationship Between Expected Reciprocal Rank and Other Metrics},
-       booktitle = {ICTIR},
-       year = {2021},
-       url = {https://doi.org/10.1145/3471158.3472239}
-     }
+<cite>
+@inproceedings{Azzopardi:2021:ECE:3471158.3472239,
+  author = {Azzopardi, Leif and Mackenzie, Joel and Moffat, Alistair},
+  title = {{ERR} is not {C/W/L}: Exploring the Relationship Between Expected Reciprocal Rank and Other Metrics},
+  booktitle = {ICTIR},
+  year = {2021},
+  url = {https://doi.org/10.1145/3471158.3472239}
+}
+</cite>
     """
     __name__ = 'NERR10'
     NAME = __name__
     PRETTY_NAME = 'Nearly Expected Reciprocal Rank Eq 10'
     SHORT_DESC = 'A C/W/L approximation of ERR using gain-based stopping and RBP patience (p).'
     SUPPORTED_PARAMS = {
         'p': measures.ParamInfo(dtype=float, default=0.9, desc='persistence'),
@@ -74,23 +74,23 @@
         'max_rel': measures.ParamInfo(dtype=int, required=True, desc='maximum relevance score'),
     }
 
 class _NERR11(measures.Measure):
     """
     Version of the Not (but Nearly) Expected Reciprocal Rank (NERR) measure, version from Equation (12) of the the following paper.
 
-::
-
-     @inproceedings{Azzopardi:2021:ECE:3471158.3472239,
-       author = {Azzopardi, Leif and Mackenzie, Joel and Moffat, Alistair},
-       title = {{ERR} is not {C/W/L}: Exploring the Relationship Between Expected Reciprocal Rank and Other Metrics},
-       booktitle = {ICTIR},
-       year = {2021},
-       url = {https://doi.org/10.1145/3471158.3472239}
-     }
+<cite>
+@inproceedings{Azzopardi:2021:ECE:3471158.3472239,
+  author = {Azzopardi, Leif and Mackenzie, Joel and Moffat, Alistair},
+  title = {{ERR} is not {C/W/L}: Exploring the Relationship Between Expected Reciprocal Rank and Other Metrics},
+  booktitle = {ICTIR},
+  year = {2021},
+  url = {https://doi.org/10.1145/3471158.3472239}
+}
+</cite>
     """
     __name__ = 'NERR11'
     NAME = __name__
     PRETTY_NAME = 'Nearly Expected Reciprocal Rank Eq 11'
     SHORT_DESC = 'A C/W/L approximation of ERR using gain based stopping and INST Goal (T).'
     SUPPORTED_PARAMS = {
         'T': measures.ParamInfo(dtype=float, default=1.0, desc='total desired gain (normalized)'),
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/numrel.py` & `ir_measures-0.3.3/ir_measures/measures/numrel.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/measures/numret.py` & `ir_measures-0.3.3/ir_measures/measures/numret.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/measures/p.py` & `ir_measures-0.3.3/ir_measures/measures/r.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 from ir_measures import measures
 from .base import Measure, ParamInfo
 
 
-class _P(measures.Measure):
+class _R(measures.Measure):
     """
-    Basic measure for that computes the percentage of documents in the top cutoff results
-    that are labeled as relevant. cutoff is a required parameter, and can be provided as
-    P@cutoff.
+    Recall@k (R@k). The fraction of relevant documents for a query that have been retrieved by rank k.
 
-::
-
-    @misc{rijsbergen:1979:ir,
-      title={Information Retrieval.},
-      author={Van Rijsbergen, Cornelis J},
-      year={1979},
-      publisher={USA: Butterworth-Heinemann}
-    }
+    NOTE: Some tasks define Recall@k as whether any relevant documents are found in the top k results.
+    This software follows the TREC convention and refers to that measure as Success@k.
     """
-    __name__ = 'P'
+    __name__ = 'R'
     NAME = __name__
-    PRETTY_NAME = 'Precision at k'
-    SHORT_DESC = 'The percentage of documents in the top k results that are relevant.'
+    PRETTY_NAME = 'Recall at k'
+    SHORT_DESC = 'The percentage of relevant documents retrieved in the top k results.'
     SUPPORTED_PARAMS = {
         'cutoff': measures.ParamInfo(dtype=int, required=True, desc='ranking cutoff threshold'),
-        'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)')
+        'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)'),
+        'judged_only': measures.ParamInfo(dtype=bool, default=False, desc='ignore returned documents that do not have relevance judgments'),
     }
 
 
-P = _P()
-Precision = P
-measures.register(P, ['Precision'])
+R = _R()
+Recall = R
+measures.register(R, ['Recall'])
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/r.py` & `ir_measures-0.3.3/ir_measures/measures/sdcg.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from ir_measures import measures
 from .base import Measure, ParamInfo
 
 
-class _R(measures.Measure):
+class _SDCG(measures.Measure):
     """
-    Recall@k (R@k). The fraction of relevant documents for a query that have been retrieved by rank k.
-
-    NOTE: Some tasks define Recall@k as whether any relevant documents are found in the top k results.
-    This software follows the TREC convention and refers to that measure as Success@k.
+    The Scaled Discounted Cumulative Gain (SDCG), a variant of nDCG that assumes more
+    fully-relevant documents exist but are not labeled.
     """
-    __name__ = 'R'
+    __name__ = 'SDCG'
     NAME = __name__
-    PRETTY_NAME = 'Recall at k'
-    SHORT_DESC = 'The percentage of relevant documents retrieved in the top k results.'
+    PRETTY_NAME = 'Scaled Discounted Cumulative Gain'
+    SHORT_DESC = 'nDCG, but assuming there are at least "cutoff" relevant documents'
     SUPPORTED_PARAMS = {
         'cutoff': measures.ParamInfo(dtype=int, required=True, desc='ranking cutoff threshold'),
-        'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)')
+        'dcg': measures.ParamInfo(dtype=str, choices=['log2'], default='log2', desc='DCG formulation'),
+        'min_rel': measures.ParamInfo(dtype=int, default=0, desc='minimum relevance score'),
+        'max_rel': measures.ParamInfo(dtype=int, required=True, desc='maximum relevance score'),
     }
 
 
-R = _R()
-Recall = R
-measures.register(R, ['Recall'])
+SDCG = _SDCG()
+measures.register(SDCG)
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/rbp.py` & `ir_measures-0.3.3/ir_measures/measures/rbp.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from .base import Measure, ParamInfo
 
 
 class _RBP(measures.Measure):
     """
     The Rank-Biased Precision (RBP).
 
-::
-
-     @article{Moffat:2008:RPM:1416950.1416952,
-       author = {Moffat, Alistair and Zobel, Justin},
-       title = {Rank-biased Precision for Measurement of Retrieval Effectiveness},
-       journal = {ACM Trans. Inf. Syst.},
-       year = {2008},
-       url = {http://doi.acm.org/10.1145/1416950.1416952}
-     }
+<cite>
+@article{Moffat:2008:RPM:1416950.1416952,
+  author = {Moffat, Alistair and Zobel, Justin},
+  title = {Rank-biased Precision for Measurement of Retrieval Effectiveness},
+  journal = {ACM Trans. Inf. Syst.},
+  year = {2008},
+  url = {http://doi.acm.org/10.1145/1416950.1416952}
+}
+</cite>
     """
     __name__ = 'RBP'
     NAME = __name__
     PRETTY_NAME = 'Rank-Biased Precision'
     SHORT_DESC = 'A measure of the rate at which utility is gained as a user traverses a result list with a degree of persistence.'
     SUPPORTED_PARAMS = {
         'cutoff': measures.ParamInfo(dtype=int, required=False, desc='ranking cutoff threshold'),
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/rprec.py` & `ir_measures-0.3.3/ir_measures/measures/rprec.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 
 
 class _Rprec(measures.Measure):
     """
     The precision at R, where R is the number of relevant documents for a given query. Has the cute property that
     it is also the recall at R.
 
-::
-
-    @misc{Buckley2005RetrievalSE,
-      title={Retrieval System Evaluation},
-      author={Chris Buckley and Ellen M. Voorhees},
-      annote={Chapter 3 in TREC: Experiment and Evaluation in Information Retrieval},
-      howpublished={MIT Press},
-      year={2005}
-    }
+<cite>
+@misc{Buckley2005RetrievalSE,
+  title={Retrieval System Evaluation},
+  author={Chris Buckley and Ellen M. Voorhees},
+  annote={Chapter 3 in TREC: Experiment and Evaluation in Information Retrieval},
+  howpublished={MIT Press},
+  year={2005}
+}
+</cite>
     """
     __name__ = 'Rprec'
     NAME = __name__
     PRETTY_NAME = 'Precsion at R'
     SHORT_DESC = 'Precsion at R, where R is the number of relevant documents for a given query.'
     SUPPORTED_PARAMS = {
-        'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)')
+        'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)'),
+        'judged_only': measures.ParamInfo(dtype=bool, default=False, desc='ignore returned documents that do not have relevance judgments'),
     }
 
 
 Rprec = _Rprec()
 RPrec = Rprec
 measures.register(Rprec, ['RPrec'])
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/rr.py` & `ir_measures-0.3.3/ir_measures/measures/rr.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 
 class _RR(measures.Measure):
     """
     The [Mean] Reciprocal Rank ([M]RR) is a precision-focused measure that scores based on the reciprocal of the rank of the
     highest-scoring relevance document. An optional cutoff can be provided to limit the
     depth explored. rel (default 1) controls which relevance level is considered relevant.
 
-::
-
-    @article{kantor2000trec,
-      title={The TREC-5 Confusion Track},
-      author={Kantor, Paul and Voorhees, Ellen},
-      journal={Information Retrieval},
-      volume={2},
-      number={2-3},
-      pages={165--176},
-      year={2000}
-    }
+<cite>
+@article{kantor2000trec,
+  title={The TREC-5 Confusion Track},
+  author={Kantor, Paul and Voorhees, Ellen},
+  journal={Information Retrieval},
+  volume={2},
+  number={2-3},
+  pages={165--176},
+  year={2000}
+}
+</cite>
     """
     __name__ = 'RR'
     NAME = __name__
     PRETTY_NAME = '(Mean) Reciprocal Rank'
     SHORT_DESC = 'The reciprocal of the rank of the first relevant document.'
     SUPPORTED_PARAMS = {
         'cutoff': measures.ParamInfo(dtype=int, required=False, desc='ranking cutoff threshold'),
-        'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)')
+        'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)'),
+        'judged_only': measures.ParamInfo(dtype=bool, default=False, desc='ignore returned documents that do not have relevance judgments'),
     }
 
 
 RR = _RR()
 MRR = RR
 measures.register(RR, ['MRR'])
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/set_measures.py` & `ir_measures-0.3.3/ir_measures/measures/set_measures.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     __name__ = 'SetP'
     NAME = __name__
     PRETTY_NAME = 'Set Precision'
     SHORT_DESC = 'The precision among all returned documents.'
     SUPPORTED_PARAMS = {
         'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)'),
         'relative': measures.ParamInfo(dtype=bool, default=False, desc='calculate the measure using the maximum possible SetP for the provided result size'),
+        'judged_only': measures.ParamInfo(dtype=bool, default=False, desc='ignore returned documents that do not have relevance judgments'),
     }
 
 SetP = _SetP()
 SetRelP = _SetP(relative=True)
 measures.register(SetP)
 measures.register(SetRelP, name='SetRelP')
 
@@ -43,14 +44,15 @@
     __name__ = 'SetF'
     PRETTY_NAME = 'Set F1'
     SHORT_DESC = 'The F1 score among all returned documents'
     NAME = __name__
     SUPPORTED_PARAMS = {
         'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)'),
         'beta': measures.ParamInfo(dtype=float, default=1., desc='relative importance of R to P in the harmonic mean'),
+        'judged_only': measures.ParamInfo(dtype=bool, default=False, desc='ignore returned documents that do not have relevance judgments'),
     }
 
 SetF = _SetF()
 measures.register(SetF)
 
 class _SetAP(measures.Measure):
     """
@@ -58,11 +60,12 @@
     """
     __name__ = 'SetAP'
     PRETTY_NAME = 'Set Average Precision'
     SHORT_DESC = 'The Average Precision among all returned documents'
     NAME = __name__
     SUPPORTED_PARAMS = {
         'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)'),
+        'judged_only': measures.ParamInfo(dtype=bool, default=False, desc='ignore returned documents that do not have relevance judgments'),
     }
 
 SetAP = _SetAP()
 measures.register(SetAP)
```

### Comparing `ir_measures-0.3.1/ir_measures/measures/success.py` & `ir_measures-0.3.3/ir_measures/measures/success.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,13 +11,14 @@
     """
     __name__ = 'Success'
     NAME = __name__
     PRETTY_NAME = 'Success at k'
     SHORT_DESC = 'An indicator if any relevant document is retrieved in the top k results.'
     SUPPORTED_PARAMS = {
         'cutoff': measures.ParamInfo(dtype=int, required=True, desc='ranking cutoff threshold'),
-        'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)')
+        'rel': measures.ParamInfo(dtype=int, default=1, desc='minimum relevance score to be considered relevant (inclusive)'),
+        'judged_only': measures.ParamInfo(dtype=bool, default=False, desc='ignore returned documents that do not have relevance judgments'),
     }
 
 
 Success = _Success()
 measures.register(Success)
```

### Comparing `ir_measures-0.3.1/ir_measures/providers/__init__.py` & `ir_measures-0.3.3/ir_measures/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/providers/accuracy_provider.py` & `ir_measures-0.3.3/ir_measures/providers/accuracy_provider.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/providers/base.py` & `ir_measures-0.3.3/ir_measures/providers/base.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/providers/compat_provider.py` & `ir_measures-0.3.3/ir_measures/providers/compat_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,26 +2,29 @@
 import ir_measures
 from ir_measures import providers, measures, Metric
 from ir_measures.providers.base import Any, Choices, NOT_PROVIDED
 
 
 class CompatProvider(providers.Provider):
     """
-    Version of the compatibility measure desribed in
-        @article{10.1145/3451161,
-          author = {Clarke, Charles L. A. and Vtyurina, Alexandra and Smucker, Mark D.},
-          title = {Assessing Top-k Preferences},
-          journal = {ACM Transactions on Information Systems},
-          volume = {39},
-          number = {3},
-          articleno = {33},
-          numpages = {21},
-          year = {2021},
-          url = {https://doi.org/10.1145/3451161},
-        }
+    Version of the compatibility measure desribed in:
+
+<cite>
+@article{10.1145/3451161,
+  author = {Clarke, Charles L. A. and Vtyurina, Alexandra and Smucker, Mark D.},
+  title = {Assessing Top-k Preferences},
+  journal = {ACM Transactions on Information Systems},
+  volume = {39},
+  number = {3},
+  articleno = {33},
+  numpages = {21},
+  year = {2021},
+  url = {https://doi.org/10.1145/3451161},
+}
+</cite>
     """
     NAME = 'compat'
     SUPPORTED_MEASURES = [
         measures._Compat(p=Any(), normalize=Any())
     ]
 
     def _evaluator(self, measures, qrels):
```

### Comparing `ir_measures-0.3.1/ir_measures/providers/cwl_eval.py` & `ir_measures-0.3.3/ir_measures/providers/cwl_eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,28 +24,28 @@
 
 class CwlEvalProvider(providers.Provider):
     """
     cwl_eval, providing C/W/L ("cool") framework measures.
 
     https://github.com/ireval/cwl
 
-::
-
-    @inproceedings{azzopardi2019cwl,
-      author = {Azzopardi, Leif and Thomas, Paul and Moffat, Alistair},
-      title = {cwl\\_eval: An Evaluation Tool for Information Retrieval},
-      booktitle = {SIGIR},
-      year = {2019}
-    }
+<cite>
+@inproceedings{azzopardi2019cwl,
+  author = {Azzopardi, Leif and Thomas, Paul and Moffat, Alistair},
+  title = {cwl\\_eval: An Evaluation Tool for Information Retrieval},
+  booktitle = {SIGIR},
+  year = {2019}
+}
+</cite>
     """
     NAME = 'cwl_eval'
     SUPPORTED_MEASURES = [
-        measures._P(cutoff=Any(), rel=Any()),
-        measures._RR(cutoff=Choices(NOT_PROVIDED), rel=Any()),
-        measures._AP(cutoff=Choices(NOT_PROVIDED), rel=Any()),
+        measures._P(cutoff=Any(), rel=Any(), judged_only=Choices(False)),
+        measures._RR(cutoff=Choices(NOT_PROVIDED), rel=Any(), judged_only=Choices(False)),
+        measures._AP(cutoff=Choices(NOT_PROVIDED), rel=Any(), judged_only=Choices(False)),
         measures._RBP(cutoff=Choices(NOT_PROVIDED), rel=Any(required=True), p=Any()),
         measures._BPM(cutoff=Any(), T=Any(), min_rel=Any(), max_rel=Any(required=True)),
         measures._SDCG(cutoff=Any(required=True), dcg=Choices('log2'), min_rel=Any(), max_rel=Any(required=True)),
         measures._NERR8(cutoff=Any(required=True), min_rel=Any(), max_rel=Any(required=True)),
         measures._NERR9(cutoff=Any(required=True), min_rel=Any(), max_rel=Any(required=True)),
         measures._NERR10(p=Any(), min_rel=Any(), max_rel=Any(required=True)),
         measures._NERR11(T=Any(), min_rel=Any(), max_rel=Any(required=True)),
@@ -112,26 +112,27 @@
             if self._max_observed_rel > self.max_rel:
                 logger.warning(f'max_rel={self.max_rel} but at least one relevance score of {self._max_observed_rel} was observed. Scores greater than {self.max_rel} were treated as {self.max_rel}.')
             if self._max_observed_rel < self.max_rel:
                 logger.warning(f'max_rel={self.max_rel} but at the highest relevance score observed was {self._max_observed_rel}. This is sometimes expected, e.g., if annotated on a scale up to {self._max_observed_rel} but no such documents were found.')
 
 
 class CwlEvaluator(providers.Evaluator):
-    def __init__(self, measures, qrels, invocations):
+    def __init__(self, measures, qrels, invocations, verify_gains=True):
         self.qrhs = {}
         for inv_key in invocations.keys():
             self.qrhs[inv_key] = IrmQrelHandler(*inv_key)
         qids = set()
         for qrel in ir_measures.util.QrelsConverter(qrels).as_namedtuple_iter():
             qids.add(qrel.query_id)
             rel = max(qrel.relevance, 0) # clip all negative scores to 0, following trec_eval convention
             for qrh in self.qrhs.values():
                 qrh.put_value(qrel.query_id, qrel.doc_id, rel)
-        for qrh in self.qrhs.values():
-            qrh.verify_gains()
+        if verify_gains:
+            for qrh in self.qrhs.values():
+                qrh.verify_gains()
         self.invocations = invocations
         super().__init__(measures, qids)
 
     def _iter_calc(self, run):
         # adapted from cwl_eval's main() method
         ranking_makers = None
         curr_qid = None
```

### Comparing `ir_measures-0.3.1/ir_measures/providers/fallback_provider.py` & `ir_measures-0.3.3/ir_measures/providers/fallback_provider.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/providers/gdeval_provider.py` & `ir_measures-0.3.3/ir_measures/providers/gdeval_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class GdevalProvider(providers.Provider):
     """
     gdeval
     """
     NAME = 'gdeval'
     SUPPORTED_MEASURES = [
-        measures._nDCG(cutoff=Any(required=True), dcg=Choices('exp-log2'), gains=Choices(NOT_PROVIDED)),
+        measures._nDCG(cutoff=Any(required=True), dcg=Choices('exp-log2'), gains=Choices(NOT_PROVIDED), judged_only=Choices(False)),
         measures._ERR(cutoff=Any(required=True)),
     ]
 
     def _evaluator(self, measures, qrels):
         MEASURES = ('nDCG', 'ERR')
         cutoffs = {}
         for measure in ir_measures.util.flatten_measures(measures):
```

### Comparing `ir_measures-0.3.1/ir_measures/providers/judged_provider.py` & `ir_measures-0.3.3/ir_measures/providers/judged_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,13 +35,29 @@
     def _iter_calc(self, run):
         run = ir_measures.util.RunConverter(run).as_dict_of_dict()
         sorted_run = {q: list(sorted(run[q].items(), key=lambda x: (-x[1], x[0]))) for q in run}
         for qid in run:
             qid_qrels = self.qrels.get(qid)
             if qid_qrels:
                 for cutoff, measure in self.cutoffs:
-                    judged_c = sum((did in qid_qrels) for did, _ in sorted_run.get(qid, [])[:cutoff])
+                    current_run = sorted_run.get(qid, [])
+                    # When there is no cutoff, default to the
+                    # size of the run.
+                    if cutoff == NOT_PROVIDED:
+                        cutoff = len(current_run)
+
+                    cutoff_run = current_run[:cutoff]
+                    judged_c = sum((did in qid_qrels) for did, _ in cutoff_run)
+
+                    # The cutoff should be recalculated if it is
+                    # less than the size of then run.
+                    if len(cutoff_run) < cutoff:
+                        cutoff = len(cutoff_run)
+
+                    # A cutoff larger than the run size causes
+                    # this calculation to be incorrect.
                     value = judged_c / cutoff
+
                     yield Metric(query_id=qid, measure=measure, value=value)
 
 
 providers.register(JudgedProvider())
```

### Comparing `ir_measures-0.3.1/ir_measures/providers/msmarco_provider.py` & `ir_measures-0.3.3/ir_measures/providers/msmarco_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class MsMarcoProvider(providers.Provider):
     """
     MS MARCO's implementation of RR
     """
     NAME = 'msmarco'
     SUPPORTED_MEASURES = [
-        measures._RR(cutoff=Any(), rel=Any()),
+        measures._RR(cutoff=Any(), rel=Any(), judged_only=Choices(False)),
     ]
 
     def _evaluator(self, measures, qrels):
         measures = ir_measures.util.flatten_measures(measures)
 
         invocations = []
         for measure in measures:
```

### Comparing `ir_measures-0.3.1/ir_measures/providers/pyndeval_provider.py` & `ir_measures-0.3.3/ir_measures/providers/pyndeval_provider.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/providers/pytrec_eval_provider.py` & `ir_measures-0.3.3/ir_measures/providers/pytrec_eval_provider.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,43 +16,42 @@
 
 class PytrecEvalProvider(providers.Provider):
     """
     pytrec_eval
 
     https://github.com/cvangysel/pytrec_eval
 
-::
-
-    @inproceedings{VanGysel2018pytreceval,
-        title={Pytrec\\_eval: An Extremely Fast Python Interface to trec\\_eval},
-        author={Van Gysel, Christophe and de Rijke, Maarten},
-        publisher={ACM},
-        booktitle={SIGIR},
-        year={2018},
-    }
-
+<cite>
+@inproceedings{VanGysel2018pytreceval,
+    title={Pytrec\\_eval: An Extremely Fast Python Interface to trec\\_eval},
+    author={Van Gysel, Christophe and de Rijke, Maarten},
+    publisher={ACM},
+    booktitle={SIGIR},
+    year={2018},
+}
+</cite>
     """
     NAME = 'pytrec_eval'
     SUPPORTED_MEASURES = [
-        measures._P(cutoff=Any(), rel=Any()),
-        measures._RR(cutoff=Choices(NOT_PROVIDED), rel=Any()),
-        measures._Rprec(rel=Any()),
-        measures._AP(cutoff=Any(), rel=Any()),
-        measures._nDCG(cutoff=Any(), dcg=Choices('log2'), gains=Any()),
-        measures._R(cutoff=Any()),
+        measures._P(cutoff=Any(), rel=Any(), judged_only=Any()),
+        measures._RR(cutoff=Choices(NOT_PROVIDED), rel=Any(), judged_only=Any()),
+        measures._Rprec(rel=Any(), judged_only=Any()),
+        measures._AP(cutoff=Any(), rel=Any(), judged_only=Any()),
+        measures._nDCG(cutoff=Any(), dcg=Choices('log2'), gains=Any(), judged_only=Any()),
+        measures._R(cutoff=Any(), judged_only=Any()),
         measures._Bpref(rel=Any()),
         measures._NumRet(rel=Any()),
         measures._NumQ(),
         measures._NumRel(rel=Choices(1)), # for some reason, relevance_level doesn't flow through to num_rel, so can only support rel=1
-        measures._SetAP(rel=Any()),
-        measures._SetF(rel=Any(), beta=Any()),
-        measures._SetP(rel=Any(), relative=Any()),
+        measures._SetAP(rel=Any(), judged_only=Any()),
+        measures._SetF(rel=Any(), beta=Any(), judged_only=Any()),
+        measures._SetP(rel=Any(), relative=Any(), judged_only=Any()),
         measures._SetR(rel=Any()),
-        measures._Success(rel=Any(), cutoff=Any()),
-        measures._IPrec(recall=Any()),
+        measures._Success(rel=Any(), cutoff=Any(), judged_only=Any()),
+        measures._IPrec(recall=Any(), judged_only=Any()),
         measures._infAP(rel=Any()),
         # Cannot support Judged because software doesn't support negative relevance levels: <https://github.com/cvangysel/pytrec_eval/blob/2362660e02c324df281932cc23ad7efd31cd3957/src/pytrec_eval.cpp#L354>
     ]
 
     def __init__(self):
         super().__init__()
         self.pytrec_eval = None
@@ -69,120 +68,122 @@
 
     def _build_invokers(self, measures, qrels):
         invocations = {}
         setf_count = 0
         for measure in measures:
             match_str = None
             if measure.NAME == 'P':
-                invocation_key = (measure['rel'], 0, None)
+                invocation_key = (measure['rel'], 0, None, measure['judged_only'])
                 measure_str = f'P_{measure["cutoff"]}'
             elif measure.NAME == 'RR':
-                invocation_key = (measure['rel'], 0, None)
+                invocation_key = (measure['rel'], 0, None, measure['judged_only'])
                 measure_str = f'recip_rank'
             elif measure.NAME == 'Rprec':
-                invocation_key = (measure['rel'], 0, None)
+                invocation_key = (measure['rel'], 0, None, measure['judged_only'])
                 measure_str = f'Rprec'
             elif measure.NAME == 'AP':
-                invocation_key = (measure['rel'], 0, None)
+                invocation_key = (measure['rel'], 0, None, measure['judged_only'])
                 if measure['cutoff'] is NOT_PROVIDED:
                     measure_str = f'map'
                 else:
                     measure_str = f'map_cut_{measure["cutoff"]}'
             elif measure.NAME == 'infAP':
-                invocation_key = (measure['rel'], 0, None)
+                invocation_key = (measure['rel'], 0, None, False)
                 measure_str = f'infAP'
             elif measure.NAME == 'nDCG':
                 if measure['gains'] is NOT_PROVIDED:
                     # Doesn't matter where this goes... Put it in an existing invocation, or just (1,) if none yet exist
                     if invocations:
                         invocation_key = next(iter(invocations))
+                        if invocation_key[3] != measure['judged_only']:
+                            invocation_key = (invocation_key[0], invocation_key[1], invocation_key[2], measure['judged_only'])
                     else:
-                        invocation_key = (1, 0, None)
+                        invocation_key = (1, 0, None, measure['judged_only'])
                 else:
-                    invocation_key = (1, 0, hashabledict(measure['gains']))
+                    invocation_key = (1, 0, hashabledict(measure['gains']), measure['judged_only'])
                 if measure['cutoff'] is NOT_PROVIDED:
                     measure_str = f'ndcg'
                 else:
                     measure_str = f'ndcg_cut_{measure["cutoff"]}'
             elif measure.NAME == 'R':
-                invocation_key = (measure['rel'], 0, None)
+                invocation_key = (measure['rel'], 0, None, measure['judged_only'])
                 measure_str = f'recall_{measure["cutoff"]}'
             elif measure.NAME == 'Bpref':
-                invocation_key = (measure['rel'], 0, None)
+                invocation_key = (measure['rel'], 0, None, False)
                 measure_str = f'bpref'
             elif measure.NAME == 'NumRet':
                 if measure['rel'] is NOT_PROVIDED:
                     # Doesn't matter where this goes... Put it in an existing invocation, or just (1,) if none yet exist
                     if invocations:
                         invocation_key = next(iter(invocations))
                     else:
-                        invocation_key = (1, 0, None)
+                        invocation_key = (1, 0, None, False)
                     measure_str = 'num_ret'
                 else:
-                    invocation_key = (measure['rel'], 0, None)
+                    invocation_key = (measure['rel'], 0, None, False)
                     measure_str = 'num_rel_ret'
             elif measure.NAME == 'NumQ':
                 # Doesn't matter where this goes... Put it in an existing invocation, or just (1,) if none yet exist
                 if invocations:
                     invocation_key = next(iter(invocations))
                 else:
-                    invocation_key = (1, 0, None)
+                    invocation_key = (1, 0, None, False)
                 measure_str = 'num_q'
             elif measure.NAME == 'NumRel':
-                invocation_key = (measure['rel'], 0, None)
+                invocation_key = (measure['rel'], 0, None, False)
                 measure_str = 'num_rel'
             elif measure.NAME == 'SetAP':
-                invocation_key = (measure['rel'], 0, None)
+                invocation_key = (measure['rel'], 0, None, measure['judged_only'])
                 measure_str = f'set_map'
             elif measure.NAME == 'SetF':
                 # set_F is strange (or buggy?) in both trec_eval and pytrec_eval. It only accepts
                 # the first beta argument it's given, which is why we use the setf_count approach
                 # to handle multiple invocations. It also is always reported as the name set_F by
                 # pytrec_eval, so we need different measure_str and match_str here.
-                invocation_key = (measure['rel'], setf_count, None)
+                invocation_key = (measure['rel'], setf_count, None, measure['judged_only'])
                 setf_count += 1
                 measure_str = f'set_F_{measure["beta"]}'
                 match_str = 'set_F'
                 if measure['beta'] == 1.:
                     measure_str = f'set_F'
                 else:
                     measure_str = f'set_F_{measure["beta"]}'
             elif measure.NAME == 'SetP':
                 if measure['relative']:
-                    invocation_key = (measure['rel'], 0, None)
+                    invocation_key = (measure['rel'], 0, None, measure['judged_only'])
                     measure_str = f'set_relative_P'
                 else:
-                    invocation_key = (measure['rel'], 0, None)
+                    invocation_key = (measure['rel'], 0, None, measure['judged_only'])
                     measure_str = f'set_P'
             elif measure.NAME == 'SetR':
-                invocation_key = (measure['rel'], 0, None)
+                invocation_key = (measure['rel'], 0, None, False)
                 measure_str = f'set_recall'
             elif measure.NAME == 'Success':
-                invocation_key = (measure['rel'], 0, None)
+                invocation_key = (measure['rel'], 0, None, measure['judged_only'])
                 measure_str = f'success_{measure["cutoff"]}'
             elif measure.NAME == 'IPrec':
-                invocation_key = (measure['rel'], 0, None)
+                invocation_key = (measure['rel'], 0, None, measure['judged_only'])
                 measure_str = f'iprec_at_recall_{measure["recall"]:.2f}'
             else:
                 raise ValueError(f'unsupported measure {measure}')
 
             if match_str is None:
                 match_str = measure_str
 
             if invocation_key not in invocations:
                 invocations[invocation_key] = {}
             invocations[invocation_key][match_str] = (measure, measure_str)
 
         invokers = []
-        for (rel_level, it, gains), measure_map in invocations.items():
+        for (rel_level, it, gains, judged_only), measure_map in invocations.items():
             these_qrels = qrels
             if gains is not None:
                 # Map the gains
                 these_qrels = {qid: {did: gains.get(score, score) for did, score in vals.items()} for qid, vals in these_qrels.items()}
-            invokers.append(PytrecEvalInvoker(self.pytrec_eval, these_qrels, measure_map, rel_level))
+            invokers.append(PytrecEvalInvoker(self.pytrec_eval, these_qrels, measure_map, rel_level, judged_only))
 
         return invokers
 
     def initialize(self):
         try:
             import pytrec_eval
             self.pytrec_eval = pytrec_eval
@@ -199,16 +200,16 @@
         # Convert qrels to dict_of_dict (input format used by pytrec_eval)
         run = ir_measures.util.RunConverter(run).as_dict_of_dict()
         for invoker in self.invokers:
             yield from invoker.iter_calc(run)
 
 
 class PytrecEvalInvoker:
-    def __init__(self, pte, qrels, measure_map, rel_level):
-        self.evaluator = pte.RelevanceEvaluator(qrels, [m for _, m in measure_map.values()], relevance_level=rel_level)
+    def __init__(self, pte, qrels, measure_map, rel_level, judged_only):
+        self.evaluator = pte.RelevanceEvaluator(qrels, [m for _, m in measure_map.values()], relevance_level=rel_level, judged_docs_only_flag=1 if judged_only else 0)
         self.measure_map = measure_map
 
     def iter_calc(self, run):
         result = self.evaluator.evaluate(run)
         for query_id, measures in result.items():
             for measure_str, value in measures.items():
                 yield Metric(query_id=query_id, measure=self.measure_map[measure_str][0], value=value)
```

### Comparing `ir_measures-0.3.1/ir_measures/providers/ranx_provider.py` & `ir_measures-0.3.3/ir_measures/providers/ranx_provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,37 +6,36 @@
 
 class RanxProvider(providers.Provider):
     """
     ranx
 
     https://amenra.github.io/ranx/
 
-::
-
-    @misc{ranx2021,
-      title = {ranx: A Blazing-Fast Python Library for Ranking Evaluation and Comparison},
-      author = {Bassani, Elias},
-      year = {2021},
-      publisher = {GitHub},
-      howpublished = {\\url{https://github.com/AmenRa/ranx}},
-    }
-
+<cite>
+@misc{ranx2021,
+  title = {ranx: A Blazing-Fast Python Library for Ranking Evaluation and Comparison},
+  author = {Bassani, Elias},
+  year = {2021},
+  publisher = {GitHub},
+  howpublished = {\\url{https://github.com/AmenRa/ranx}},
+}
+</cite>
     """
     NAME = 'ranx'
     SUPPORTED_MEASURES = [
-        measures._P(cutoff=Any(), rel=Any()),
-        measures._SetP(rel=Any()),
-        measures._RR(cutoff=Choices(NOT_PROVIDED), rel=Any()),
-        measures._Rprec(rel=Any()),
-        measures._AP(cutoff=Any(), rel=Any()),
-        measures._nDCG(cutoff=Any(), dcg=Choices('log2', 'exp-log2'), gains=Choices(NOT_PROVIDED)),
-        measures._R(cutoff=Any()),
+        measures._P(cutoff=Any(), rel=Any(), judged_only=Choices(False)),
+        measures._SetP(rel=Any(), judged_only=Choices(False)),
+        measures._RR(cutoff=Choices(NOT_PROVIDED), rel=Any(), judged_only=Choices(False)),
+        measures._Rprec(rel=Any(), judged_only=Choices(False)),
+        measures._AP(cutoff=Any(), rel=Any(), judged_only=Choices(False)),
+        measures._nDCG(cutoff=Any(), dcg=Choices('log2', 'exp-log2'), gains=Choices(NOT_PROVIDED), judged_only=Choices(False)),
+        measures._R(cutoff=Any(), judged_only=Choices(False)),
         measures._SetR(rel=Any()),
         measures._NumRet(rel=Any(required=True)),
-        measures._Success(cutoff=Any(required=True), rel=Any()),
+        measures._Success(cutoff=Any(required=True), rel=Any(), judged_only=Choices(False)),
     ]
 
     def __init__(self):
         super().__init__()
         self.ranx = None
 
     def _evaluator(self, measures, qrels):
```

### Comparing `ir_measures-0.3.1/ir_measures/providers/runtime_provider.py` & `ir_measures-0.3.3/ir_measures/providers/runtime_provider.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures/providers/trectools_provider.py` & `ir_measures-0.3.3/ir_measures/providers/trectools_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,33 +8,32 @@
 
 class TrectoolsProvider(providers.Provider):
     """
     trectools
 
     https://github.com/joaopalotti/trectools
 
-::
-
-    @inproceedings{palotti2019,
-       author = {Palotti, Joao and Scells, Harrisen and Zuccon, Guido},
-       title = {TrecTools: an open-source Python library for Information Retrieval practitioners involved in TREC-like campaigns},
-       series = {SIGIR'19},
-       year = {2019},
-       location = {Paris, France},
-       publisher = {ACM}
-    }
-
+<cite>
+@inproceedings{palotti2019,
+   author = {Palotti, Joao and Scells, Harrisen and Zuccon, Guido},
+   title = {TrecTools: an open-source Python library for Information Retrieval practitioners involved in TREC-like campaigns},
+   series = {SIGIR'19},
+   year = {2019},
+   location = {Paris, France},
+   publisher = {ACM}
+}
+</cite>
     """
     NAME = 'trectools'
     SUPPORTED_MEASURES = [
-        measures._P(cutoff=Any(), rel=Choices(1)),
-        measures._RR(cutoff=Choices(NOT_PROVIDED), rel=Choices(1)),
-        measures._Rprec(rel=Choices(1)),
-        measures._AP(cutoff=Any(), rel=Choices(1)),
-        measures._nDCG(cutoff=Any(), dcg=Any(), gains=Choices(NOT_PROVIDED)),
+        measures._P(cutoff=Any(), rel=Choices(1), judged_only=Choices(False)),
+        measures._RR(cutoff=Choices(NOT_PROVIDED), rel=Choices(1), judged_only=Choices(False)),
+        measures._Rprec(rel=Choices(1), judged_only=Choices(False)),
+        measures._AP(cutoff=Any(), rel=Choices(1), judged_only=Choices(False)),
+        measures._nDCG(cutoff=Any(), dcg=Any(), gains=Choices(NOT_PROVIDED), judged_only=Choices(False)),
         measures._Bpref(rel=Choices(1)),
         measures._RBP(cutoff=Any(), p=Any(), rel=Any()),
         # Other supported metrics: urbp, ubpref, alpha_urbp, geometric_map, unjudged
     ]
 
     def __init__(self):
         super().__init__()
```

### Comparing `ir_measures-0.3.1/ir_measures/util.py` & `ir_measures-0.3.3/ir_measures/util.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/ir_measures.egg-info/SOURCES.txt` & `ir_measures-0.3.3/ir_measures.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 ir_measures/providers/runtime_provider.py
 ir_measures/providers/trectools_provider.py
 test/test_accuracy.py
 test/test_aggregate.py
 test/test_compat.py
 test/test_cwl_eval.py
 test/test_gdeval.py
+test/test_judged.py
 test/test_measures.py
 test/test_providers.py
 test/test_pyndeval.py
 test/test_pytrec_eval.py
 test/test_ranx.py
 test/test_runtime.py
 test/test_util.py
```

### Comparing `ir_measures-0.3.1/setup.py` & `ir_measures-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/test/test_accuracy.py` & `ir_measures-0.3.3/test/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/test/test_aggregate.py` & `ir_measures-0.3.3/test/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/test/test_compat.py` & `ir_measures-0.3.3/test/test_compat.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/test/test_cwl_eval.py` & `ir_measures-0.3.3/test/test_cwl_eval.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/test/test_gdeval.py` & `ir_measures-0.3.3/test/test_gdeval.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/test/test_measures.py` & `ir_measures-0.3.3/test/test_measures.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/test/test_providers.py` & `ir_measures-0.3.3/test/test_providers.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/test/test_pyndeval.py` & `ir_measures-0.3.3/test/test_pyndeval.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/test/test_pytrec_eval.py` & `ir_measures-0.3.3/test/test_pytrec_eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -567,10 +567,73 @@
 
         measure = ir_measures.nDCG(gains={0:1,1:4})
         self.assertMetrics(
                 provider.iter_calc([measure], qrels, run),
                 [Metric(query_id='0', measure=measure, value=0.97177),
                 Metric(query_id='1', measure=measure, value=0.14949)])
 
+    def test_P(self):
+        qrels = list(ir_measures.read_trec_qrels('''
+0 0 D0 -1
+0 0 D1 1
+0 0 D3 2
+0 0 D4 1
+1 0 D0 1
+1 0 D3 0
+1 0 D4 -1
+'''))
+        run = list(ir_measures.read_trec_run('''
+0 0 D0 1 0.8 run
+0 0 D2 2 0.7 run
+0 0 D1 3 0.3 run
+0 0 D3 4 0.4 run
+0 0 D4 5 0.1 run
+1 0 D1 1 0.8 run
+1 0 D0 2 0.7 run
+1 0 D3 3 0.3 run
+1 0 D2 4 0.4 run
+'''))
+        provider = ir_measures.pytrec_eval
+        measure = ir_measures.P@4
+        self.assertMetrics(
+                provider.iter_calc([measure], qrels, run),
+                [Metric(query_id='0', measure=measure, value=0.5),
+                Metric(query_id='1', measure=measure, value=0.25)])
+
+        measure = ir_measures.P(judged_only=True)@4
+        self.assertMetrics(
+                provider.iter_calc([measure], qrels, run),
+                [Metric(query_id='0', measure=measure, value=0.75),
+                Metric(query_id='1', measure=measure, value=0.25)])
+
+    def test_judged_only(self):
+        qrels = list(ir_measures.read_trec_qrels('''
+0 0 D0 -1
+0 0 D1 1
+0 0 D3 2
+0 0 D4 1
+'''))
+        run = list(ir_measures.read_trec_run('''
+0 0 D0 1 0.8 run
+0 0 D2 2 0.7 run
+0 0 D1 3 0.3 run
+0 0 D3 4 0.4 run
+0 0 D4 5 0.1 run
+'''))
+        run_unudged_removed = list(ir_measures.read_trec_run('''
+0 0 D1 3 0.3 run
+0 0 D3 4 0.4 run
+0 0 D4 5 0.1 run
+''')) # D0 is removed because trec_eval considers negative labels as unjudged (??). See <https://github.com/usnistgov/trec_eval/blob/d95ca64e14a47d763ae349fb65e6d8cde4141dbd/form_res_rels.c#L219>
+        provider = ir_measures.pytrec_eval
+        for measure in [ir_measures.P@4, ir_measures.RR, ir_measures.Rprec, ir_measures.AP, ir_measures.AP@4, ir_measures.nDCG, ir_measures.nDCG@4, ir_measures.R@2, ir_measures.SetP, ir_measures.SetAP, ir_measures.SetF, ir_measures.Success@2, ir_measures.IPrec@0.5]:
+            with self.subTest(measure):
+                self.assertMetrics(
+                        [Metric(m.query_id, measure, m.value) for m in provider.iter_calc([measure(judged_only=True)], qrels, run)],
+                        provider.iter_calc([measure], qrels, run_unudged_removed))
+                self.assertMetrics(
+                        [Metric(m.query_id, measure, m.value) for m in provider.iter_calc([measure(judged_only=True)], qrels, run)],
+                        provider.iter_calc([measure], qrels, run),
+                        not_equal=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ir_measures-0.3.1/test/test_ranx.py` & `ir_measures-0.3.3/test/test_ranx.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/test/test_runtime.py` & `ir_measures-0.3.3/test/test_runtime.py`

 * *Files identical despite different names*

### Comparing `ir_measures-0.3.1/test/test_util.py` & `ir_measures-0.3.3/test/test_util.py`

 * *Files identical despite different names*

