# Comparing `tmp/geofetch-0.8.0.tar.gz` & `tmp/geofetch-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geofetch-0.8.0.tar", last modified: Mon May 23 19:29:12 2022, max compression
+gzip compressed data, was "geofetch-0.9.0.tar", last modified: Fri Jun 17 18:52:58 2022, max compression
```

## Comparing `geofetch-0.8.0.tar` & `geofetch-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 19:29:12.917898 geofetch-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-05-23 19:29:00.000000 geofetch-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-05-23 19:29:00.000000 geofetch-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-05-23 19:29:12.917898 geofetch-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-05-23 19:29:00.000000 geofetch-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 19:29:12.913898 geofetch-0.8.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 19:29:12.913898 geofetch-0.8.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (121)    17224 2022-05-23 19:29:00.000000 geofetch-0.8.0/docs/img/geofetch_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 19:29:12.913898 geofetch-0.8.0/geofetch/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-23 19:29:00.000000 geofetch-0.8.0/geofetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-23 19:29:00.000000 geofetch-0.8.0/geofetch/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-05-23 19:29:00.000000 geofetch-0.8.0/geofetch/config_processed_template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-05-23 19:29:00.000000 geofetch-0.8.0/geofetch/config_template.yaml
--rwxr-xr-x   0 runner    (1001) docker     (121)    72229 2022-05-23 19:29:00.000000 geofetch-0.8.0/geofetch/geofetch.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6629 2022-05-23 19:29:00.000000 geofetch-0.8.0/geofetch/sraconvert.py
--rw-r--r--   0 runner    (1001) docker     (121)    10851 2022-05-23 19:29:00.000000 geofetch-0.8.0/geofetch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 19:29:12.913898 geofetch-0.8.0/geofetch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-05-23 19:29:12.000000 geofetch-0.8.0/geofetch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-05-23 19:29:12.000000 geofetch-0.8.0/geofetch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-23 19:29:12.000000 geofetch-0.8.0/geofetch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-05-23 19:29:12.000000 geofetch-0.8.0/geofetch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-05-23 19:29:12.000000 geofetch-0.8.0/geofetch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-23 19:29:12.000000 geofetch-0.8.0/geofetch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 19:29:12.913898 geofetch-0.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-05-23 19:29:00.000000 geofetch-0.8.0/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-05-23 19:29:00.000000 geofetch-0.8.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-05-23 19:29:00.000000 geofetch-0.8.0/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-23 19:29:00.000000 geofetch-0.8.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-23 19:29:12.917898 geofetch-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1981 2022-05-23 19:29:00.000000 geofetch-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 18:52:58.567540 geofetch-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-06-17 18:52:48.000000 geofetch-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-06-17 18:52:48.000000 geofetch-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-06-17 18:52:58.563540 geofetch-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      827 2022-06-17 18:52:48.000000 geofetch-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 18:52:58.559540 geofetch-0.9.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 18:52:58.563540 geofetch-0.9.0/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (121)    17224 2022-06-17 18:52:48.000000 geofetch-0.9.0/docs/img/geofetch_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 18:52:58.563540 geofetch-0.9.0/geofetch/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-06-17 18:52:48.000000 geofetch-0.9.0/geofetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-17 18:52:48.000000 geofetch-0.9.0/geofetch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-06-17 18:52:48.000000 geofetch-0.9.0/geofetch/config_processed_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-06-17 18:52:48.000000 geofetch-0.9.0/geofetch/config_template.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (121)    85218 2022-06-17 18:52:48.000000 geofetch-0.9.0/geofetch/geofetch.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6629 2022-06-17 18:52:48.000000 geofetch-0.9.0/geofetch/sraconvert.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11703 2022-06-17 18:52:48.000000 geofetch-0.9.0/geofetch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 18:52:58.563540 geofetch-0.9.0/geofetch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-06-17 18:52:58.000000 geofetch-0.9.0/geofetch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2022-06-17 18:52:58.000000 geofetch-0.9.0/geofetch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 18:52:58.000000 geofetch-0.9.0/geofetch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-06-17 18:52:58.000000 geofetch-0.9.0/geofetch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-06-17 18:52:58.000000 geofetch-0.9.0/geofetch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-17 18:52:58.000000 geofetch-0.9.0/geofetch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 18:52:58.563540 geofetch-0.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-06-17 18:52:48.000000 geofetch-0.9.0/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-06-17 18:52:48.000000 geofetch-0.9.0/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-06-17 18:52:48.000000 geofetch-0.9.0/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-06-17 18:52:48.000000 geofetch-0.9.0/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-17 18:52:58.567540 geofetch-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-06-17 18:52:48.000000 geofetch-0.9.0/setup.py
```

### Comparing `geofetch-0.8.0/LICENSE.txt` & `geofetch-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geofetch-0.8.0/PKG-INFO` & `geofetch-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: geofetch
-Version: 0.8.0
+Version: 0.9.0
 Summary: Downloads data and metadata from GEO and SRA and creates standard PEPs.
 Home-page: https://github.com/pepkit/geofetch/
 Author: Nathan Sheffield, Vince Reuter, Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,bioinformatics,sequencing,ngs,workflow,GUI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # <img src="docs/img/geofetch_logo.svg" alt="geofetch logo" height="70">
 
+![Run pytests](https://github.com/pepkit/geofetch/workflows/Run%20pytests/badge.svg)
 [![PEP compatible](http://pepkit.github.io/img/PEP-compatible-green.svg)](http://pepkit.github.io)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-`geofetch` is a command-line tool that downloads sequencing data and metadata from GEO and SRA and creates [standard PEPs](http://pepkit.github.io). `geofetch` is hosted at [pypi](https://pypi.org/project/geofetch/) and documentation is hosted at [geofetch.databio.org](http://geofetch.databio.org) (source in the [/docs](/docs) folder).
+`geofetch` is a command-line tool that downloads sequencing data and metadata from GEO and SRA and creates [standard PEPs](http://pep.databio.org/). `geofetch` is hosted at [pypi](https://pypi.org/project/geofetch/) and documentation is hosted at [geofetch.databio.org](http://geofetch.databio.org) (source in the [/docs](/docs) folder).
 
 You can convert the result of geofetch into unmapped `bam` or `fastq` files with the included `sraconvert` command.
```

### Comparing `geofetch-0.8.0/README.md` & `geofetch-0.9.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # <img src="docs/img/geofetch_logo.svg" alt="geofetch logo" height="70">
 
+![Run pytests](https://github.com/pepkit/geofetch/workflows/Run%20pytests/badge.svg)
 [![PEP compatible](http://pepkit.github.io/img/PEP-compatible-green.svg)](http://pepkit.github.io)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-`geofetch` is a command-line tool that downloads sequencing data and metadata from GEO and SRA and creates [standard PEPs](http://pepkit.github.io). `geofetch` is hosted at [pypi](https://pypi.org/project/geofetch/) and documentation is hosted at [geofetch.databio.org](http://geofetch.databio.org) (source in the [/docs](/docs) folder).
+`geofetch` is a command-line tool that downloads sequencing data and metadata from GEO and SRA and creates [standard PEPs](http://pep.databio.org/). `geofetch` is hosted at [pypi](https://pypi.org/project/geofetch/) and documentation is hosted at [geofetch.databio.org](http://geofetch.databio.org) (source in the [/docs](/docs) folder).
 
 You can convert the result of geofetch into unmapped `bam` or `fastq` files with the included `sraconvert` command.
```

### Comparing `geofetch-0.8.0/docs/img/geofetch_logo.svg` & `geofetch-0.9.0/docs/img/geofetch_logo.svg`

 * *Files identical despite different names*

### Comparing `geofetch-0.8.0/geofetch/config_template.yaml` & `geofetch-0.9.0/geofetch/config_template.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 
 looper:
   output_dir: {project_name}
   pipeline_interfaces: {pipeline_interfaces}
 
 sample_modifiers:
   append:
+    {additional_columns}
     SRR_files: SRA
-    pipeline_interfaces: {pipeline_interfaces}
+    {pipeline_samples}
   derive:
     attributes: [read1, read2, SRR_files]
     sources:
       SRA: "${SRABAM}/{SRR}.bam"
       FQ: "${SRAFQ}/{SRR}.fastq.gz"
       FQ1: "${SRAFQ}/{SRR}_1.fastq.gz"
       FQ2: "${SRAFQ}/{SRR}_2.fastq.gz"      
@@ -51,7 +52,9 @@
         derive:
           attributes: [read1, read2, SRR_files]
           sources:
             SRA: "${SRARAW}/{SRR}.sra"
             FQ: "${SRAFQ}/{SRR}.fastq.gz"
             FQ1: "${SRAFQ}/{SRR}_1.fastq.gz"
             FQ2: "${SRAFQ}/{SRR}_2.fastq.gz"
+
+{pipeline_project}
```

### Comparing `geofetch-0.8.0/geofetch/geofetch.py` & `geofetch-0.9.0/geofetch/geofetch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 #!/usr/bin/env python3
 
-__author__ = ["Vince Reuter", "Nathan Sheffield", "Oleksandr Khoroshevskyi"]
+__author__ = ["Oleksandr Khoroshevskyi", "Vince Reuter", "Nathan Sheffield"]
 
-# Outline:
-# INPUT: A list of GSE ids, optionally including GSM ids to limit to.
-# example: GSE61150
-# 1. Grab SOFT file from
-# http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?targ=gsm&acc=GSE61150&form=text&view=full
-# 2. parse it, produce a table with all needed fields.
-# 3. Grab SRA values from field, use this link to grab SRA metadata:
-# http://trace.ncbi.nlm.nih.gov/Traces/sra/sra.cgi?save=efetch&db=sra&rettype=runinfo&term=SRX079566
-# http://trace.ncbi.nlm.nih.gov/Traces/sra/sra.cgi?save=efetch&db=sra&rettype=runinfo&term=SRP055171
-# http://trace.ncbi.nlm.nih.gov/Traces/sra/sra.cgi?save=efetch&db=sra&rettype=runinfo&term=SRX883589
-
-# 4. Parse the SRA RunInfo csv file and use the download_link field to grab the .sra file
 
 import argparse
 import copy
 import csv
 import os
 import re
 import subprocess
 import sys
+from string import punctuation
 
 # import tarfile
 import time
 
-from .utils import Accession, parse_accessions, parse_SOFT_line, convert_size
+from .utils import (
+    Accession,
+    parse_accessions,
+    parse_SOFT_line,
+    convert_size,
+    clean_soft_files,
+)
 from ._version import __version__
 
 from logmuse import add_logging_options, init_logger
 from ubiquerg import expandpath, is_command_callable
 
 _STRING_TYPES = str
 _LOGGER = None
@@ -75,45 +70,55 @@
         self,
         name="",
         metadata_root="",
         metadata_folder="",
         just_metadata=False,
         refresh_metadata=False,
         config_template=None,
-        pipeline_interfaces=None,
+        pipeline_samples=None,
+        pipeline_project=None,
         skip=0,
         acc_anno=False,
         use_key_subset=False,
         processed=True,
-        supp_by="samples",
+        data_source="samples",
         filter=None,
         filter_size=None,
         geo_folder=".",
         split_experiments=False,
         bam_folder="",
         fq_folder="",
         sra_folder="",
         bam_conversion=False,
         picard_path="",
         silent=False,
         verbosity=None,
         logdev=False,
         input=None,
+        const_limit_project=50,
+        const_limit_discard=250,
+        attr_limit_truncate=500,
+        discard_soft=False,
+        add_dotfile=False,
+        **kwargs,
     ):
 
         # self.args = args
         global _LOGGER
         #  _LOGGER = logger_via_cli(args, name="geofetch")
         _LOGGER = init_logger(name="geofetch", verbosity=verbosity, logfile=None)
         self._LOGGER = _LOGGER
 
         if name:
             self.project_name = name
         else:
-            self.project_name = os.path.splitext(os.path.basename(input))[0]
+            try:
+                self.project_name = os.path.splitext(os.path.basename(input))[0]
+            except TypeError:
+                self.project_name = "project_name"
 
         if metadata_folder:
             self.metadata_expanded = expandpath(metadata_folder)
             if os.path.isabs(self.metadata_expanded):
                 self.metadata_raw = metadata_folder
             else:
                 self.metadata_expanded = os.path.abspath(self.metadata_expanded)
@@ -127,61 +132,83 @@
                 self.metadata_expanded = os.path.abspath(self.metadata_expanded)
                 self.metadata_raw = os.path.abspath(metadata_root)
 
         self.just_metadata = just_metadata
         self.refresh_metadata = refresh_metadata
         self.config_template = config_template
 
+        # if user specified a pipeline interface path for samples, add it into the project config
+        if pipeline_samples and pipeline_samples != "null":
+            self.file_pipeline_samples = pipeline_samples
+            self.file_pipeline_samples = (
+                f"pipeline_interfaces: {self.file_pipeline_samples}"
+            )
+        else:
+            self.file_pipeline_samples = ""
+
         # if user specified a pipeline interface path, add it into the project config
-        self.pipeline_interfaces = pipeline_interfaces
-        if self.pipeline_interfaces:
-            self.file_pipeline_interfaces = self.pipeline_interfaces
+        if pipeline_project:
+            self.file_pipeline_project = (
+                f"looper:\n    pipeline_interfaces: {pipeline_project}"
+            )
         else:
-            self.file_pipeline_interfaces = "null"
+            self.file_pipeline_project = ""
 
         self.skip = skip
         self.acc_anno = acc_anno
         self.use_key_subset = use_key_subset
         self.processed = processed
-        self.supp_by = supp_by
+        self.supp_by = data_source
 
         if filter:
             self.filter_re = re.compile(filter.lower())
         else:
             self.filter_re = None
 
             # Postpend the project name as a subfolder (only for -m option)
             self.metadata_expanded = os.path.join(
                 self.metadata_expanded, self.project_name
             )
             self.metadata_raw = os.path.join(self.metadata_raw, self.project_name)
 
         if filter_size is not None:
-            self.filter_size = convert_size(filter_size.lower())
+            try:
+                self.filter_size = convert_size(filter_size.lower())
+            except ValueError as message:
+                self._LOGGER.error(message)
+                raise SystemExit()
         else:
             self.filter_size = filter_size
 
         self.geo_folder = geo_folder
         self.split_experiments = split_experiments
         self.bam_folder = bam_folder
         self.fq_folder = fq_folder
         self.sra_folder = sra_folder
         self.bam_conversion = bam_conversion
         self.picard_path = picard_path
         self.silent = silent
         self.verbosity = verbosity
         self.logdev = logdev
 
+        self.const_limit_project = const_limit_project
+        self.const_limit_discard = const_limit_discard
+        self.attr_limit_truncate = attr_limit_truncate
+
+        self.discard_soft = discard_soft
+        self.add_dotfile = add_dotfile
+
         self._LOGGER.info(f"Metadata folder: {self.metadata_expanded}")
 
         # check to make sure prefetch is callable
         if not just_metadata and not processed:
             if not is_command_callable("prefetch"):
                 raise SystemExit(
-                    "You must first install the sratoolkit, with prefetch in your PATH."
+                    "To download raw data You must first install the sratoolkit, with prefetch in your PATH."
+                    " Installation instruction: http://geofetch.databio.org/en/latest/install/"
                 )
 
         # Some sanity checks before proceeding
         if bam_conversion and not just_metadata and not self.which("samtools"):
             raise SystemExit("For SAM/BAM processing, samtools should be on PATH.")
 
     def fetch_all(self, input, name=None):
@@ -214,15 +241,15 @@
         for acc_GSE in acc_GSE_list.keys():
             ncount += 1
             if ncount <= self.skip:
                 continue
             elif ncount == self.skip + 1:
                 self._LOGGER.info(f"Skipped {self.skip} accessions. Starting now.")
             self._LOGGER.info(
-                f"\033[38;5;228mProcessing accession {ncount} of {nkeys}: '{acc_GSE}'\033[0m"
+                f"\033[38;5;200mProcessing accession {ncount} of {nkeys}: '{acc_GSE}'\033[0m"
             )
 
             if len(re.findall(GSE_PATTERN, acc_GSE)) != 1:
                 self._LOGGER.debug(len(re.findall(GSE_PATTERN, acc_GSE)))
                 self._LOGGER.warning(
                     "This does not appear to be a correctly formatted GSE accession! "
                     "Continue anyway..."
@@ -290,53 +317,62 @@
                     list_of_keys_series = self.get_list_of_keys(meta_processed_series)
                     self._LOGGER.info("Expanding metadata list...")
                     for key_in_list in list_of_keys_series:
                         meta_processed_series = self.expand_metadata_list(
                             meta_processed_series, key_in_list
                         )
 
-                    # adding metadata from current experiment to the project
-                    processed_metadata_samples.extend(meta_processed_samples)
-                    processed_metadata_exp.extend(meta_processed_series)
+                    # convert column names to lowercase and underscore
+                    meta_processed_samples = self.standardize_colnames(
+                        meta_processed_samples
+                    )
+                    meta_processed_series = self.standardize_colnames(
+                        meta_processed_series
+                    )
 
-                    # save PEP for each accession
+                    if not self.acc_anno:
+                        # adding metadata from current experiment to the project
+                        processed_metadata_samples.extend(meta_processed_samples)
+                        processed_metadata_exp.extend(meta_processed_series)
+
+                    # save PEP for each accession if acc-anno flag is true
                     if self.acc_anno and len(acc_GSE_list.keys()) > 1:
                         if self.supp_by == "all":
                             # samples
                             pep_acc_path_sample = os.path.join(
                                 self.metadata_raw,
-                                acc_GSE,
+                                f"{acc_GSE}_samples",
                                 acc_GSE + SAMPLE_SUPP_METADATA_FILE,
                             )
                             self.write_processed_annotation(
                                 meta_processed_samples, pep_acc_path_sample
                             )
 
                             # series
                             pep_acc_path_exp = os.path.join(
                                 self.metadata_raw,
-                                acc_GSE,
+                                f"{acc_GSE}_series",
                                 acc_GSE + EXP_SUPP_METADATA_FILE,
                             )
                             self.write_processed_annotation(
                                 meta_processed_series, pep_acc_path_exp
                             )
                         elif self.supp_by == "samples":
                             pep_acc_path_sample = os.path.join(
                                 self.metadata_raw,
-                                acc_GSE,
+                                f"{acc_GSE}_samples",
                                 acc_GSE + SAMPLE_SUPP_METADATA_FILE,
                             )
                             self.write_processed_annotation(
                                 meta_processed_samples, pep_acc_path_sample
                             )
                         elif self.supp_by == "series":
                             pep_acc_path_exp = os.path.join(
                                 self.metadata_raw,
-                                acc_GSE,
+                                f"{acc_GSE}_series",
                                 acc_GSE + EXP_SUPP_METADATA_FILE,
                             )
                             self.write_processed_annotation(
                                 meta_processed_series, pep_acc_path_exp
                             )
 
                     if not self.just_metadata:
@@ -381,14 +417,16 @@
                 # download gsm metadata
                 gsm_metadata = self.get_gsm_metadata(acc_GSE, acc_GSE_list, file_gsm)
                 metadata_dict[acc_GSE] = gsm_metadata
 
                 # download gsm metadata
                 result = self.get_SRA_meta(file_gse, file_sra, gsm_metadata)
                 if not result:
+                    # delete current acc if no raw data was found
+                    # del metadata_dict[acc_GSE]
                     continue
                 # Parse metadata from SRA
                 # Produce an annotated output from the GSM and SRARunInfo files.
                 # This will merge the GSM and SRA sample metadata into a dict of dicts,
                 # with one entry per sample.
                 # NB: There may be multiple SRA Runs (and thus lines in the RunInfo file)
                 # Corresponding to each sample.
@@ -418,15 +456,15 @@
                     # possibly set in the input tsv file
                     sample_name = None  # initialize to empty
                     try:
                         sample_name = acc_GSE_list[acc_GSE][
                             gsm_metadata[experiment]["gsm_id"]
                         ]
                     except KeyError:
-                        _LOGGER.warning(f"Error in sample_name ...")
+                        self._LOGGER.info(f"KeyError in sample_name, creating new...")
                     if not sample_name or sample_name == "":
                         temp = gsm_metadata[experiment]["Sample_title"]
                         # Now do a series of transformations to cleanse the sample name
                         temp = temp.replace(" ", "_")
                         # Do people put commas in their sample names? Yes.
                         temp = temp.replace(",", "_")
                         temp = temp.replace("__", "_")
@@ -493,15 +531,15 @@
                         # The first SRR for this SRX is added to GSM metadata
                         gsm_metadata[experiment]["SRR"] = run_name
 
                     # gsm_metadata[experiment].update(line)
 
                     # Write to filtered SRA Runinfo file
                     wwrite.writerow(line)
-                    self._LOGGER.info(f"Get SRR: {run_name} ({experiment})")
+                    self._LOGGER.info(f"Getting SRR: {run_name} ({experiment})")
                     bam_file = (
                         ""
                         if self.bam_folder == ""
                         else os.path.join(self.bam_folder, run_name + ".bam")
                     )
                     fq_file = (
                         ""
@@ -554,126 +592,71 @@
 
                 # accumulate subannotations
                 subannotation_dict[acc_GSE] = gsm_multi_table
 
         # Logging additional information about processing
         self._LOGGER.info(f"Finished processing {len(acc_GSE_list)} accession(s)")
 
+        # Logging cleaning process:
+        if self.discard_soft:
+            self._LOGGER.info(f"Cleaning soft files ...")
+            clean_soft_files(self.metadata_raw)
+
         if len(failed_runs) > 0:
             self._LOGGER.warn(
                 f"The following samples could not be downloaded: {failed_runs}"
             )
 
         #######################################################################################
 
         # saving PEPs for processed data
         if self.processed:
-            if self.supp_by == "all":
-                supp_sample_path_meta = os.path.join(
-                    self.metadata_raw, self.project_name + SAMPLE_SUPP_METADATA_FILE
-                )
-                self.write_processed_annotation(
-                    processed_metadata_samples, supp_sample_path_meta
-                )
-
-                supp_series_path_meta = os.path.join(
-                    self.metadata_raw, self.project_name + EXP_SUPP_METADATA_FILE
-                )
-                self.write_processed_annotation(
-                    processed_metadata_exp, supp_series_path_meta
-                )
-
-            elif self.supp_by == "samples":
-                supp_sample_path_meta = os.path.join(
-                    self.metadata_raw, self.project_name + SAMPLE_SUPP_METADATA_FILE
-                )
-                self.write_processed_annotation(
-                    processed_metadata_samples, supp_sample_path_meta
-                )
-
-            elif self.supp_by == "series":
-                supp_series_path_meta = os.path.join(
-                    self.metadata_raw, self.project_name + EXP_SUPP_METADATA_FILE
-                )
-                self.write_processed_annotation(
-                    processed_metadata_exp, supp_series_path_meta
-                )
-        else:
-            # Combine individual accessions into project-level annotations, and write
-            # individual accession files (if requested)
-            metadata_dict_combined = {}
-            for acc_GSE, gsm_metadata in metadata_dict.items():
-                file_annotation = os.path.join(
-                    self.metadata_expanded, acc_GSE + "_annotation.csv"
-                )
-                if self.acc_anno:
-                    self.write_gsm_annotation(
-                        gsm_metadata,
-                        file_annotation,
-                        use_key_subset=self.use_key_subset,
+            if not self.acc_anno:
+                if self.supp_by == "all":
+                    supp_sample_path_meta = os.path.join(
+                        self.metadata_raw,
+                        "PEP_samples",
+                        self.project_name + SAMPLE_SUPP_METADATA_FILE,
+                    )
+                    self.write_processed_annotation(
+                        processed_metadata_samples, supp_sample_path_meta
                     )
-                metadata_dict_combined.update(gsm_metadata)
 
-            subannotation_dict_combined = {}
-            for acc_GSE, gsm_multi_table in subannotation_dict.items():
-                file_subannotation = os.path.join(
-                    self.metadata_expanded, acc_GSE + "_subannotation.csv"
-                )
-                if self.acc_anno:
-                    self.write_subannotation(gsm_multi_table, file_subannotation)
-                subannotation_dict_combined.update(gsm_multi_table)
-            self._LOGGER.info(
-                "Creating complete project annotation sheets and config file..."
-            )
-            # If the project included more than one GSE, we can now output combined
-            # annotation tables for the entire project.
+                    supp_series_path_meta = os.path.join(
+                        self.metadata_raw,
+                        "PEP_series",
+                        self.project_name + EXP_SUPP_METADATA_FILE,
+                    )
+                    self.write_processed_annotation(
+                        processed_metadata_exp, supp_series_path_meta
+                    )
 
-            # Write combined annotation sheet
-            file_annotation = os.path.join(
-                self.metadata_raw, self.project_name + "_annotation.csv"
-            )
-            self.write_gsm_annotation(
-                metadata_dict_combined,
-                file_annotation,
-                use_key_subset=self.use_key_subset,
-            )
+                elif self.supp_by == "samples":
+                    supp_sample_path_meta = os.path.join(
+                        self.metadata_raw,
+                        "PEP_samples",
+                        self.project_name + SAMPLE_SUPP_METADATA_FILE,
+                    )
+                    self.write_processed_annotation(
+                        processed_metadata_samples, supp_sample_path_meta
+                    )
 
-            # Write combined subannotation table
-            if len(subannotation_dict_combined) > 0:
-                file_subannotation = os.path.join(
-                    self.metadata_raw, self.project_name + "_subannotation.csv"
-                )
-                self.write_subannotation(
-                    subannotation_dict_combined, file_subannotation
-                )
-            else:
-                file_subannotation = "null"
+                elif self.supp_by == "series":
+                    supp_series_path_meta = os.path.join(
+                        self.metadata_raw,
+                        "PEP_series",
+                        self.project_name + EXP_SUPP_METADATA_FILE,
+                    )
+                    self.write_processed_annotation(
+                        processed_metadata_exp, supp_series_path_meta
+                    )
 
-            # Write project config file
-            if not self.config_template:
-                geofetchdir = os.path.dirname(__file__)
-                self.config_template = os.path.join(geofetchdir, "config_template.yaml")
-
-            with open(self.config_template, "r") as template_file:
-                template = template_file.read()
-
-            template_values = {
-                "project_name": self.project_name,
-                "annotation": os.path.basename(file_annotation),
-                "subannotation": os.path.basename(file_subannotation),
-                "pipeline_interfaces": self.file_pipeline_interfaces,
-            }
-
-            for k, v in template_values.items():
-                placeholder = "{" + str(k) + "}"
-                template = template.replace(placeholder, str(v))
-
-            # save .yaml file
-            config = os.path.join(self.metadata_raw, self.project_name + "_config.yaml")
-            self._write(config, template, msg_pre="  Config file: ")
+        # saving PEPs for raw data
+        else:
+            self.write_raw_annotation(metadata_dict, subannotation_dict)
 
     def expand_metadata_list(self, metadata_list, dict_key):
         """
         Expanding list items in the list by creating new items or joining them
 
         :param list metadata_list: list of dicts that store metadata
         :param str dict_key: key in the dictionaries that have to be expanded
@@ -692,20 +675,36 @@
                         ]
 
                     just_string = False
                     this_string = ""
                     for elem in metadata_list[n_elem][dict_key]:
                         separated_elements = elem.split(": ")
                         if len(separated_elements) >= 2:
-                            list_of_elem = [
-                                separated_elements[0],
-                                ": ".join(separated_elements[1:]),
-                            ]
-                            sample_char = dict([list_of_elem])
-                            metadata_list[n_elem].update(sample_char)
+
+                            # if first element is larger than 40 then treat it like simple string
+                            if len(separated_elements[0]) > 40:
+                                just_string = True
+                                if this_string != "":
+                                    this_string = ", ".join([this_string, elem])
+                                else:
+                                    this_string = elem
+                            # additional elem for all bed files
+                            elif len(separated_elements[0].split("(")) > 1:
+                                just_string = True
+                                if this_string != "":
+                                    this_string = "(".join([this_string, elem])
+                                else:
+                                    this_string = elem
+                            else:
+                                list_of_elem = [
+                                    separated_elements[0],
+                                    ": ".join(separated_elements[1:]),
+                                ]
+                                sample_char = dict([list_of_elem])
+                                metadata_list[n_elem].update(sample_char)
                         else:
                             just_string = True
                             if this_string != "":
                                 this_string = ", ".join([this_string, elem])
                             else:
                                 this_string = elem
 
@@ -778,14 +777,32 @@
         list_of_keys = self.get_list_of_keys(processed_meta_list)
         for k in list_of_keys:
             for list_elem in range(len(processed_meta_list)):
                 if k not in processed_meta_list[list_elem]:
                     processed_meta_list[list_elem][k] = ""
         return processed_meta_list
 
+    def find_genome(self, metadata_list):
+        """
+        Create new genome table by joining few columns
+        """
+        list_keys = self.get_list_of_keys(metadata_list)
+        genome_keys = [
+            "assembly",
+            "genome_build",
+        ]
+        proj_gen_keys = list(set(list_keys).intersection(genome_keys))
+
+        for sample in enumerate(metadata_list):
+            sample_genome = ""
+            for key in proj_gen_keys:
+                sample_genome = " ".join([sample_genome, sample[1][key]])
+            metadata_list[sample[0]]["sample_genome"] = sample_genome
+        return metadata_list
+
     def write_gsm_annotation(self, gsm_metadata, file_annotation, use_key_subset=False):
         """
         Write metadata sheet out as an annotation file.
 
         :param Mapping gsm_metadata: the data to write, parsed from a file
             with metadata/annotation information
         :param str file_annotation: the path to the file to write
@@ -819,22 +836,37 @@
         if len(processed_metadata) == 0:
             self._LOGGER.info(
                 "No files found. No data to save. File %s won't be created"
                 % file_annotation_path
             )
             return False
 
-        # create folder if does not exist
+        # create folder if it does not exist
         pep_file_folder = os.path.split(file_annotation_path)[0]
         if not os.path.exists(pep_file_folder):
             os.makedirs(pep_file_folder)
 
         self._LOGGER.info("Unifying and saving of metadata... ")
         processed_metadata = self.unify_list_keys(processed_metadata)
 
+        # delete rare keys
+        processed_metadata = self.find_genome(processed_metadata)
+
+        # filtering huge annotation strings that are repeating for each sample
+        processed_metadata, proj_meta = self.separate_common_meta(
+            processed_metadata,
+            self.const_limit_project,
+            self.const_limit_discard,
+            self.attr_limit_truncate,
+        )
+        meta_list_str = [
+            f"{list(i.keys())[0]}: {list(i.values())[0]}" for i in proj_meta
+        ]
+        modifiers_str = "\n    ".join(d for d in meta_list_str)
+
         with open(file_annotation_path, "w") as m_file:
             dict_writer = csv.DictWriter(m_file, processed_metadata[0].keys())
             dict_writer.writeheader()
             dict_writer.writerows(processed_metadata)
         self._LOGGER.info(
             "\033[92mFile %s has been saved successfully\033[0m" % file_annotation_path
         )
@@ -845,27 +877,284 @@
         with open(config_template, "r") as template_file:
             template = template_file.read()
 
         template_values = {
             "project_name": self.project_name,
             "sample_table": os.path.basename(file_annotation_path),
             "geo_folder": self.geo_folder,
-            "pipeline_interfaces": self.file_pipeline_interfaces,
+            "pipeline_samples": self.file_pipeline_samples,
+            "pipeline_project": self.file_pipeline_project,
+            "additional_columns": modifiers_str,
         }
 
         for k, v in template_values.items():
             placeholder = "{" + str(k) + "}"
             template = template.replace(placeholder, str(v))
 
         # save .yaml file
         yaml_name = os.path.split(file_annotation_path)[1][:-4] + ".yaml"
         config = os.path.join(pep_file_folder, yaml_name)
         self._write(config, template, msg_pre="  Config file: ")
+
+        # save .pep.yaml file
+        if self.add_dotfile:
+            dot_yaml_path = os.path.join(pep_file_folder, ".pep.yaml")
+            self.create_dot_yaml(dot_yaml_path, yaml_name)
+
         return True
 
+    @staticmethod
+    def sanitize_name(name_str: str):
+        """
+        Function that sanitizing strings. (Replace all odd characters)
+        :param str names_str: Any string value that has to be sanitized.
+        :return: sanitized strings
+        """
+        new_str = name_str
+        for odd_char in list(punctuation):
+            new_str = new_str.replace(odd_char, "_")
+        new_str = new_str.replace(" ", "_").replace("__", "_")
+        return new_str
+
+    def write_raw_annotation(self, metadata_dict, subannotation_dict):
+        """
+        Combining individual accessions into project-level annotations, and writeing
+        individual accession files (if requested)
+        :param dict metadata_dict: dictionary of metadata
+        :param dict subannotation_dict: dictionary of sub-annotation metadata
+        """
+
+        if self.discard_soft:
+            clean_soft_files(os.path.join(self.metadata_raw))
+
+        try:
+            assert len(metadata_dict) > 0
+        except AssertionError:
+            self._LOGGER.warning(
+                "\033[33mNo PEP created, as no raw data was found!!!\033[0m"
+            )
+            return False
+
+        # checking sample_name value if it's not empty,
+        # otherwise pulling from title
+        for key, value in metadata_dict.items():
+            fixed_dict = {}
+            for key_sample, value_sample in value.items():
+                fixed_dict[key_sample] = value_sample
+                if (
+                    value_sample["sample_name"] == ""
+                    or value_sample["sample_name"] is None
+                ):
+                    fixed_dict[key_sample]["sample_name"] = value_sample["Sample_title"]
+
+                # sanitize sample names
+                fixed_dict[key_sample]["sample_name"] = self.sanitize_name(
+                    fixed_dict[key_sample]["sample_name"]
+                )
+
+            metadata_dict[key] = fixed_dict
+
+        metadata_dict_combined = {}
+        for acc_GSE, gsm_metadata in metadata_dict.items():
+            file_annotation = os.path.join(
+                self.metadata_expanded, acc_GSE + "_annotation.csv"
+            )
+            if self.acc_anno:
+                self.write_gsm_annotation(
+                    gsm_metadata,
+                    file_annotation,
+                    use_key_subset=self.use_key_subset,
+                )
+            metadata_dict_combined.update(gsm_metadata)
+
+        # filtering huge annotation strings that are repeating for each sample
+        metadata_dict_combined, proj_meta = self.separate_common_meta(
+            metadata_dict_combined,
+            self.const_limit_project,
+            self.const_limit_discard,
+            self.attr_limit_truncate,
+        )
+        meta_list_str = [
+            f"{list(i.keys())[0]}: {list(i.values())[0]}" for i in proj_meta
+        ]
+        modifiers_str = "\n    ".join(d for d in meta_list_str)
+
+        subannotation_dict_combined = {}
+        for acc_GSE, gsm_multi_table in subannotation_dict.items():
+            file_subannotation = os.path.join(
+                self.metadata_expanded, acc_GSE + "_subannotation.csv"
+            )
+            if self.acc_anno:
+                self.write_subannotation(gsm_multi_table, file_subannotation)
+            subannotation_dict_combined.update(gsm_multi_table)
+        self._LOGGER.info(
+            "Creating complete project annotation sheets and config file..."
+        )
+        # If the project included more than one GSE, we can now output combined
+        # annotation tables for the entire project.
+        # Write combined annotation sheet
+        file_annotation = os.path.join(
+            self.metadata_raw, self.project_name + "_annotation.csv"
+        )
+        self.write_gsm_annotation(
+            metadata_dict_combined,
+            file_annotation,
+            use_key_subset=self.use_key_subset,
+        )
+        # Write combined subannotation table
+        if len(subannotation_dict_combined) > 0:
+            file_subannotation = os.path.join(
+                self.metadata_raw, self.project_name + "_subannotation.csv"
+            )
+            self.write_subannotation(subannotation_dict_combined, file_subannotation)
+        else:
+            file_subannotation = "null"
+        # Write project config file
+        if not self.config_template:
+            geofetchdir = os.path.dirname(__file__)
+            self.config_template = os.path.join(geofetchdir, "config_template.yaml")
+        with open(self.config_template, "r") as template_file:
+            template = template_file.read()
+
+        template_values = {
+            "project_name": self.project_name,
+            "annotation": os.path.basename(file_annotation),
+            "subannotation": os.path.basename(file_subannotation),
+            "pipeline_samples": self.file_pipeline_samples,
+            "pipeline_project": self.file_pipeline_project,
+            "additional_columns": modifiers_str,
+        }
+        for k, v in template_values.items():
+            placeholder = "{" + str(k) + "}"
+            template = template.replace(placeholder, str(v))
+        # save .yaml file
+        yaml_name = self.project_name + "_config.yaml"
+        config = os.path.join(self.metadata_raw, yaml_name)
+        self._write(config, template, msg_pre="  Config file: ")
+
+        # save .pep.yaml file
+        if self.add_dotfile:
+            dot_yaml_path = os.path.join(self.metadata_raw, ".pep.yaml")
+            self.create_dot_yaml(dot_yaml_path, yaml_name)
+
+    @staticmethod
+    def create_dot_yaml(file_path: str, yaml_path: str):
+        """
+        Function that creates .pep.yaml file that points to actual yaml file
+        :param str file_path: Path to the .pep.yaml file that we want to create
+        :param str yaml_path: path or name of the actual yaml file
+        """
+        with open(file_path, "w+") as file:
+            file.writelines(f"config_file: {yaml_path}")
+
+    def separate_common_meta(
+        self, meta_list, max_len=50, del_limit=250, attr_limit_truncate=500
+    ):
+        """
+        This function is separating information for the experiment from a sample
+        :param list or dict meta_list: list of dictionaries of samples
+        :param int max_len: threshold of the length of the common value that can be stored in the sample table
+        :param int del_limit: threshold of the length of the common value that have to be deleted
+        :param int attr_limit_truncate: max length of the attribute in the sample csv
+        :return set: Return is a set of list, where 1 list (or dict) is
+        list of samples metadata dictionaries and 2: list of common samples metadata
+        dictionaries that are linked to the project.
+        """
+        input_is_dict = False
+        if isinstance(meta_list, dict):
+            input_is_dict = True
+            new_meta_list = []
+            for key in meta_list:
+                new_dict = meta_list[key]
+                new_dict["big_key"] = key
+                new_meta_list.append(new_dict)
+
+            meta_list = new_meta_list
+
+        list_of_keys = self.get_list_of_keys(meta_list)
+        list_keys_diff = []
+        # finding columns with common values
+        for this_key in list_of_keys:
+            value = ""
+            for nb_sample in enumerate(meta_list):
+                try:
+                    if nb_sample[0] == 0:
+                        value = meta_list[nb_sample[0]][this_key]
+                        if len(str(value)) < max_len and len(str(value)) < del_limit:
+                            list_keys_diff.append(this_key)
+                            break
+                    else:
+                        if value != meta_list[nb_sample[0]][this_key]:
+                            list_keys_diff.append(this_key)
+                            break
+                except KeyError:
+                    pass
+
+        list_keys_diff = set(list_keys_diff)
+
+        # separating sample and common metadata and creating 2 lists
+        new_meta_project = []
+        for this_key in list_of_keys:
+            first_key = True
+            for nb_sample in enumerate(meta_list):
+                try:
+                    if this_key not in list_keys_diff:
+                        if first_key:
+                            if len(str(nb_sample[1][this_key])) <= del_limit:
+                                new_meta_project.append(
+                                    {this_key: nb_sample[1][this_key]}
+                                )
+                            first_key = False
+                        del meta_list[nb_sample[0]][this_key]
+                except KeyError:
+                    pass
+
+        # Truncate huge information in metadata
+        new_list = []
+        for this_item in meta_list:
+            new_item_list = {}
+            for key, value in this_item.items():
+                if len(str(value)) < attr_limit_truncate:
+                    new_item_list[key] = value
+                else:
+                    new_item_list[key] = value[0:attr_limit_truncate] + " ..."
+            new_list.append(new_item_list)
+
+        meta_list = new_list
+
+        if input_is_dict:
+            new_sample_dict = {}
+            for sample in meta_list:
+                new_sample_dict[sample["big_key"]] = sample
+            meta_list = new_sample_dict
+
+        return meta_list, new_meta_project
+
+    def standardize_colnames(self, meta_list):
+        """
+        Standardize column names by lower-casing and underscore
+        :param list meta_list: list of dictionaries of samples
+        :return : list of dictionaries of samples with standard colnames
+        """
+        new_metalist = []
+        list_keys = self.get_list_of_keys(meta_list)
+        for item_nb, values in enumerate(meta_list):
+            new_metalist.append({})
+            for key in list_keys:
+                try:
+                    new_key_name = key.lower().strip()
+                    new_key_name = self.sanitize_name(new_key_name)
+
+                    new_metalist[item_nb][new_key_name] = values[key]
+
+                except KeyError:
+                    pass
+
+        return new_metalist
+
     def download_SRA_file(self, run_name):
         """
         Downloading SRA file by ising 'prefetch' utility from the SRA Toolkit
         more info: (http://www.ncbi.nlm.nih.gov/books/NBK242621/)
         :param str run_name: SRR number of the SRA file
         """
 
@@ -1255,29 +1544,34 @@
                 new_dict["file"] = file_elem
                 separated_list.append(new_dict)
         else:
             return TypeError("Incorrect type")
 
         return separated_list
 
-    @staticmethod
-    def separate_file_url(meta_list):
+    def separate_file_url(self, meta_list):
         """
         This method is adding dict key without file_name without path
         """
         separated_list = []
         for meta_elem in meta_list:
             new_dict = meta_elem.copy()
             new_dict["file_url"] = meta_elem["file"]
             new_dict["file"] = os.path.basename(meta_elem["file"])
             # new_dict["sample_name"] = os.path.basename(meta_elem["file"])
             try:
                 new_dict["sample_name"] = str(meta_elem["Sample_title"])
+                if new_dict["sample_name"] == "" or new_dict["sample_name"] is None:
+                    raise KeyError("sample_name Does not exist. Creating .. ")
             except KeyError:
                 new_dict["sample_name"] = os.path.basename(meta_elem["file"])
+
+            # sanitize sample names
+            new_dict["sample_name"] = self.sanitize_name(new_dict["sample_name"])
+
             separated_list.append(new_dict)
         return separated_list
 
     def run_filter(self, meta_list, col_name="file"):
         """
         If user specified filter it will filter all this files here by col_name
         """
@@ -1295,15 +1589,15 @@
     def run_size_filter(self, meta_list, col_name="file_size"):
         """
         function for filtering file size
         """
         if self.filter_size is not None:
             filtered_list = []
             for meta_elem in meta_list:
-                if meta_elem[col_name] <= self.filter_size:
+                if int(meta_elem[col_name]) <= self.filter_size:
                     filtered_list.append(meta_elem)
         else:
             self._LOGGER.info(
                 "\033[32mTotal number of files after size filter NONE?? \033[0m"
             )
             return meta_list
         self._LOGGER.info(
@@ -1586,62 +1880,103 @@
         help="If set, re-download metadata even if it exists.",
     )
 
     parser.add_argument(
         "--config-template", default=None, help="Project config yaml file template."
     )
 
+    # Optional
+    parser.add_argument(
+        "--pipeline-samples",
+        default=None,
+        help="Optional: Specify one or more filepaths to SAMPLES pipeline interface yaml files. "
+        "These will be added to the project config file to make it immediately "
+        "compatible with looper. [Default: null]",
+    )
+
+    # Optional
     parser.add_argument(
-        "-P",
-        "--pipeline_interfaces",
+        "--pipeline-project",
         default=None,
-        help="Optional: Specify one or more filepaths to pipeline interface yaml files. "
+        help="Optional: Specify one or more filepaths to PROJECT pipeline interface yaml files. "
         "These will be added to the project config file to make it immediately "
         "compatible with looper. [Default: null]",
     )
 
+    # Optional
     parser.add_argument(
         "-k",
         "--skip",
         default=0,
         type=int,
         help="Skip some accessions. [Default: no skip].",
     )
 
     parser.add_argument(
         "--acc-anno",
         action="store_true",
-        help="Also produce annotation sheets for each accession, not just"
-        " for the whole project combined",
+        help="Optional: Produce annotation sheets for each accession."
+        " Project combined PEP for the whole project won't be produced.",
     )
 
     parser.add_argument(
-        "--use-key-subset",
+        "--discard-soft",
         action="store_true",
-        help="Use just the keys defined in this module when writing out metadata.",
+        help="Optional: After creation of PEP files, all soft and additional files will be deleted",
+    )
+
+    parser.add_argument(
+        "--const-limit-project",
+        type=int,
+        default=50,
+        help="Optional: Limit of the number of the constant sample characters "
+        "that should not be in project yaml. [Default: 50]",
+    )
+
+    parser.add_argument(
+        "--const-limit-discard",
+        type=int,
+        default=250,
+        help="Optional: Limit of the number of the constant sample characters "
+        "that should not be discarded [Default: 250]",
+    )
+
+    parser.add_argument(
+        "--attr-limit-truncate",
+        type=int,
+        default=500,
+        help="Optional: Limit of the number of sample characters."
+        "Any attribute with more than X characters will truncate to the first X,"
+        " where X is a number of characters [Default: 500]",
+    )
+
+    parser.add_argument(
+        "--add-dotfile",
+        action="store_true",
+        help="Optional: Add .pep.yaml file that points .yaml PEP file",
     )
 
     processed_group.add_argument(
         "-p",
         "--processed",
         default=False,
         action="store_true",
         help="Download processed data [Default: download raw data].",
     )
 
     processed_group.add_argument(
         "--data-source",
-        dest="supp_by",
+        dest="data_source",
         choices=["all", "samples", "series"],
         default="samples",
         help="Optional: Specifies the source of data on the GEO record"
         " to retrieve processed data, which may be attached to the"
         " collective series entity, or to individual samples. "
         "Allowable values are: samples, series or both (all). "
-        "Ignored unless 'processed' flag is set. [Default: all]",
+        "Ignored unless 'processed' flag is set. [Default: samples]",
     )
 
     processed_group.add_argument(
         "--filter",
         default=None,
         help="Optional: Filter regex for processed filenames [Default: None]."
         "Ignored unless 'processed' flag is set.",
@@ -1649,14 +1984,15 @@
 
     processed_group.add_argument(
         "--filter-size",
         dest="filter_size",
         default=None,
         help="""Optional: Filter size for processed files
                 that are stored as sample repository [Default: None].
+                Works only for sample data.
                 Supported input formats : 12B, 12KB, 12MB, 12GB. 
                 Ignored unless 'processed' flag is set.""",
     )
 
     processed_group.add_argument(
         "-g",
         "--geo-folder",
@@ -1724,14 +2060,20 @@
         dest="picard_path",
         default=safe_echo("PICARD"),
         # help="Specify a path to the picard jar, if you want to convert "
         # "fastq to bam [Default: $PICARD:" + safe_echo("PICARD") + "]",
         help=argparse.SUPPRESS,
     )
 
+    raw_group.add_argument(
+        "--use-key-subset",
+        action="store_true",
+        help="Use just the keys defined in this module when writing out metadata.",
+    )
+
     parser = add_logging_options(parser)
     return parser.parse_args(cmdl)
 
 
 def safe_echo(var):
     """Returns an environment variable if it exists, or an empty string if not"""
     return os.getenv(var, "")
@@ -1749,17 +2091,15 @@
         super(self, f"{l}")
 
 
 def main():
     """Run the script."""
     args = _parse_cmdl(sys.argv[1:])
     args_dict = vars(args)
-    print(args_dict)
     Geofetcher(**args_dict).fetch_all(args_dict["input"])
-    # print(ab.get_list_of_processed_files())
 
 
 if __name__ == "__main__":
     try:
         sys.exit(main())
 
     except KeyboardInterrupt:
```

### Comparing `geofetch-0.8.0/geofetch/sraconvert.py` & `geofetch-0.9.0/geofetch/sraconvert.py`

 * *Files identical despite different names*

### Comparing `geofetch-0.8.0/geofetch/utils.py` & `geofetch-0.9.0/geofetch/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -275,21 +275,49 @@
     :return str, str: prefix and integral suffix
     """
     typename, number_text = accn[:3], accn[3:]
     return typename.upper(), number_text
 
 
 def convert_size(size_str: str) -> int:
+    """
+    Converting size, that was provided as string with suffix
+    :param str size_str: size as string with suffix: gb, mb, kb or b
+    :return int: size as int value in bytes
+    """
     abbreviation_dict = {"gb": 1073741824, "mb": 1048576, "kb": 1024, "b": 1}
     supported_formats = r"(\dgb|\dmb|\db|\dkb)$"
     reg_number = r"^\d+"
     abbreviation = re.findall(supported_formats, size_str)
     size_numb = re.findall(reg_number, size_str)
 
     # check if list is empty
     if len(abbreviation) == 0:
         size_in_bytes = size_numb[0]
     else:
         abb = abbreviation[0][1:]
         size_in_bytes = int(size_numb[0]) * abbreviation_dict[abb]
 
+    if not isinstance(size_in_bytes, int):
+        raise ValueError(
+            f"Incorrect type of file size was provided! You provided:'{size_str}'"
+        )
+
     return size_in_bytes
+
+
+def clean_soft_files(meta_dir: str):
+    """
+    Cleaning, deleting all soft files after downloading files
+    and creating PEPs
+    :param str meta_dir: Path to the metadata files
+    """
+    dir_files = os.listdir(meta_dir)
+
+    for item in dir_files:
+        if (
+            item.endswith(".soft")
+            or item.endswith("_file_list.txt")
+            or item.endswith("SRA.csv")
+            or item.endswith("SRA_filt.csv")
+        ):
+            os.remove(os.path.join(meta_dir, item))
```

### Comparing `geofetch-0.8.0/geofetch.egg-info/PKG-INFO` & `geofetch-0.9.0/geofetch.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: geofetch
-Version: 0.8.0
+Version: 0.9.0
 Summary: Downloads data and metadata from GEO and SRA and creates standard PEPs.
 Home-page: https://github.com/pepkit/geofetch/
 Author: Nathan Sheffield, Vince Reuter, Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,bioinformatics,sequencing,ngs,workflow,GUI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # <img src="docs/img/geofetch_logo.svg" alt="geofetch logo" height="70">
 
+![Run pytests](https://github.com/pepkit/geofetch/workflows/Run%20pytests/badge.svg)
 [![PEP compatible](http://pepkit.github.io/img/PEP-compatible-green.svg)](http://pepkit.github.io)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-`geofetch` is a command-line tool that downloads sequencing data and metadata from GEO and SRA and creates [standard PEPs](http://pepkit.github.io). `geofetch` is hosted at [pypi](https://pypi.org/project/geofetch/) and documentation is hosted at [geofetch.databio.org](http://geofetch.databio.org) (source in the [/docs](/docs) folder).
+`geofetch` is a command-line tool that downloads sequencing data and metadata from GEO and SRA and creates [standard PEPs](http://pep.databio.org/). `geofetch` is hosted at [pypi](https://pypi.org/project/geofetch/) and documentation is hosted at [geofetch.databio.org](http://geofetch.databio.org) (source in the [/docs](/docs) folder).
 
 You can convert the result of geofetch into unmapped `bam` or `fastq` files with the included `sraconvert` command.
```

### Comparing `geofetch-0.8.0/geofetch.egg-info/SOURCES.txt` & `geofetch-0.9.0/geofetch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geofetch-0.8.0/setup.py` & `geofetch-0.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 setup(
     name=PACKAGE,
     packages=[PACKAGE],
     version=version,
     description="Downloads data and metadata from GEO and SRA and creates standard PEPs.",
     long_description=long_description,
+    long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
```

