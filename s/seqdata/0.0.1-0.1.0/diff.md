# Comparing `tmp/seqdata-0.0.1.tar.gz` & `tmp/seqdata-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqdata-0.0.1.tar", max compression
+gzip compressed data, was "seqdata-0.1.0.tar", max compression
```

## Comparing `seqdata-0.0.1.tar` & `seqdata-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,19 @@
--rw-r--r--   0        0        0       10 2023-01-11 21:01:38.000000 seqdata-0.0.1/README.md
--rw-r--r--   0        0        0      664 2023-01-26 05:29:41.000000 seqdata-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    14625 2023-01-11 20:56:15.000000 seqdata-0.0.1/seqdata/.ipynb_checkpoints/_SeqData-checkpoint.py
--rw-r--r--   0        0        0     3813 2023-01-11 21:09:03.000000 seqdata-0.0.1/seqdata/.ipynb_checkpoints/_SeqDataset-checkpoint.py
--rw-r--r--   0        0        0        0 2023-01-11 20:56:14.000000 seqdata-0.0.1/seqdata/.ipynb_checkpoints/_utlis-checkpoint.py
--rw-r--r--   0        0        0      191 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/__init__.py
--rw-r--r--   0        0        0        0 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/_analyze/motif_enrichment.py
--rw-r--r--   0        0        0      398 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/_analyze/properties.py
--rw-r--r--   0        0        0        0 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/_core/__init__.py
--rw-r--r--   0        0        0     2332 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/_core/merge.py
--rw-r--r--   0        0        0    10345 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/_core/seqdata.py
--rw-r--r--   0        0        0     1691 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/_core/utils.py
--rw-r--r--   0        0        0        0 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/_encode/onehot.py
--rw-r--r--   0        0        0        0 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/_io/__init__.py
--rw-r--r--   0        0        0     8785 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/_io/read.py
--rw-r--r--   0        0        0     1653 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/_io/utils.py
--rw-r--r--   0        0        0     6932 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/_io/write.py
--rw-r--r--   0        0        0     1983 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/_preprocess/basic.py
--rw-r--r--   0        0        0     3233 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/_preprocess/encode.py
--rw-r--r--   0        0        0     8265 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/_preprocess/perturb.py
--rw-r--r--   0        0        0     9319 2023-01-26 05:18:07.000000 seqdata-0.0.1/seqdata/_preprocess/utils.py
--rw-r--r--   0        0        0        0 2023-01-11 20:56:15.000000 seqdata-0.0.1/seqdata/_utlis.py
--rw-r--r--   0        0        0     1073 2023-01-26 05:30:37.564838 seqdata-0.0.1/setup.py
--rw-r--r--   0        0        0      853 2023-01-26 05:30:37.565111 seqdata-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      844 2023-06-23 19:00:15.000000 seqdata-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1355 2023-06-23 18:57:24.000000 seqdata-0.1.0/seqdata/__init__.py
+-rw-r--r--   0        0        0     2412 2023-06-21 21:41:12.000000 seqdata-0.1.0/seqdata/_dataload/_SequenceDataset.py
+-rw-r--r--   0        0        0      981 2023-06-21 21:41:12.000000 seqdata-0.1.0/seqdata/_deprecated.py
+-rw-r--r--   0        0        0        0 2023-01-26 05:18:07.000000 seqdata-0.1.0/seqdata/_io/__init__.py
+-rw-r--r--   0        0        0    10816 2023-06-21 17:40:21.000000 seqdata-0.1.0/seqdata/_io/bed_ops.py
+-rw-r--r--   0        0        0     4943 2023-06-21 17:40:21.000000 seqdata-0.1.0/seqdata/_io/read.py
+-rw-r--r--   0        0        0      206 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/_io/readers/__init__.py
+-rw-r--r--   0        0        0    11173 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/_io/readers/bam.py
+-rw-r--r--   0        0        0    10022 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/_io/readers/fasta.py
+-rw-r--r--   0        0        0     6152 2023-06-21 17:40:21.000000 seqdata-0.1.0/seqdata/_io/readers/table.py
+-rw-r--r--   0        0        0    13505 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/_io/readers/vcf.py
+-rw-r--r--   0        0        0     9706 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/_io/readers/wig.py
+-rw-r--r--   0        0        0     2705 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/_io/utils.py
+-rw-r--r--   0        0        0     9375 2023-06-21 22:49:16.000000 seqdata-0.1.0/seqdata/torch.py
+-rw-r--r--   0        0        0     2281 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/types.py
+-rw-r--r--   0        0        0    12620 2023-06-21 21:41:12.000000 seqdata-0.1.0/seqdata/xarray/seqdata.py
+-rw-r--r--   0        0        0      901 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/xarray/utils.py
+-rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 seqdata-0.1.0/PKG-INFO
```

