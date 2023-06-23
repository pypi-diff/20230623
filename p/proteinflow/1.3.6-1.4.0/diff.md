# Comparing `tmp/proteinflow-1.3.6.tar.gz` & `tmp/proteinflow-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-1.3.6.tar", last modified: Mon Jun  5 12:59:15 2023, max compression
+gzip compressed data, was "proteinflow-1.4.0.tar", last modified: Fri Jun 23 17:06:22 2023, max compression
```

## Comparing `proteinflow-1.3.6.tar` & `proteinflow-1.4.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:15.711494 proteinflow-1.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-05 12:59:03.000000 proteinflow-1.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-06-05 12:59:15.711494 proteinflow-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-06-05 12:59:03.000000 proteinflow-1.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:15.703494 proteinflow-1.3.6/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)   101608 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:15.707494 proteinflow-1.3.6/proteinflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/scripts/proteinflow_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:15.707494 proteinflow-1.3.6/proteinflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/async_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/biotite_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/build_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    41081 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/cluster_and_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/filter_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/mmcif_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/process_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-06-05 12:59:03.000000 proteinflow-1.3.6/proteinflow/utils/split_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:15.707494 proteinflow-1.3.6/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-06-05 12:59:15.000000 proteinflow-1.3.6/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-05 12:59:15.000000 proteinflow-1.3.6/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:59:15.000000 proteinflow-1.3.6/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-05 12:59:15.000000 proteinflow-1.3.6/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-05 12:59:15.000000 proteinflow-1.3.6/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-05 12:59:15.000000 proteinflow-1.3.6/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-05 12:59:03.000000 proteinflow-1.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 12:59:15.711494 proteinflow-1.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:59:15.711494 proteinflow-1.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-05 12:59:03.000000 proteinflow-1.3.6/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-05 12:59:03.000000 proteinflow-1.3.6/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-05 12:59:03.000000 proteinflow-1.3.6/tests/test_sabdab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:22.546243 proteinflow-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-23 17:06:10.000000 proteinflow-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-23 17:06:22.546243 proteinflow-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-06-23 17:06:10.000000 proteinflow-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:22.542243 proteinflow-1.4.0/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    50281 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/custom_mmcif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21978 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39439 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/protein_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/protein_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:22.546243 proteinflow-1.4.0/proteinflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/scripts/proteinflow_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/sequences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:22.546243 proteinflow-1.4.0/proteinflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/utils/biotite_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/utils/boto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/utils/cluster_and_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-23 17:06:10.000000 proteinflow-1.4.0/proteinflow/utils/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:22.546243 proteinflow-1.4.0/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-23 17:06:22.000000 proteinflow-1.4.0/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-23 17:06:22.000000 proteinflow-1.4.0/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 17:06:22.000000 proteinflow-1.4.0/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-23 17:06:22.000000 proteinflow-1.4.0/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-23 17:06:22.000000 proteinflow-1.4.0/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 17:06:22.000000 proteinflow-1.4.0/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-23 17:06:10.000000 proteinflow-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-23 17:06:22.546243 proteinflow-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:06:22.546243 proteinflow-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-23 17:06:10.000000 proteinflow-1.4.0/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-23 17:06:10.000000 proteinflow-1.4.0/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-23 17:06:10.000000 proteinflow-1.4.0/tests/test_sabdab.py
```

### Comparing `proteinflow-1.3.6/LICENSE` & `proteinflow-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.6/PKG-INFO` & `proteinflow-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.3.6
+Version: 1.4.0
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,15 +22,15 @@
 ---
 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/proteinflow)](https://pypi.org/project/proteinflow/)
 [![Conda](https://img.shields.io/conda/v/adaptyvbio/proteinflow)](https://anaconda.org/adaptyvbio/proteinflow)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/tags)
-![Generic badge](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)
+[![Generic badge](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](CONTRIBUTING.md)
 
 
 ProteinFlow is an open-source Python library that streamlines the pre-processing of protein structure data for deep learning applications. ProteinFlow enables users to efficiently filter, cluster, and generate new datasets from resources like the Protein Data Bank (PDB) and SAbDab (The Structural Antibody Database).
 
 Here are some of the key features we currently support:
 
 - ⛓️ Processing of both single-chain and multi-chain protein structures (Biounit PDB definition)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.3.6 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 1.4.0 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
@@ -11,126 +11,127 @@
 (https://opensource.org/licenses/BSD-3-Clause) [![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
 black) [![PyPI](https://img.shields.io/pypi/v/proteinflow)](https://pypi.org/
 project/proteinflow/) [![Conda](https://img.shields.io/conda/v/adaptyvbio/
 proteinflow)](https://anaconda.org/adaptyvbio/proteinflow) [![Docker Image
 Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/
 proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/
-tags) ![Generic badge](https://img.shields.io/badge/Contributions-Welcome-
-brightgreen.svg) ProteinFlow is an open-source Python library that streamlines
-the pre-processing of protein structure data for deep learning applications.
-ProteinFlow enables users to efficiently filter, cluster, and generate new
-datasets from resources like the Protein Data Bank (PDB) and SAbDab (The
-Structural Antibody Database). Here are some of the key features we currently
-support: - âï¸ Processing of both single-chain and multi-chain protein
-structures (Biounit PDB definition) - ð·ï¸ Various featurization options can
-be computed, including secondary structure features, torsion angles, etc. -
-ð¾ A variety of data loading options and conversions to cater to different
-downstream training frameworks - ð§¬ Access to up-to-date, pre-computed
-protein structure datasets ![overview](https://raw.githubusercontent.com/
-adaptyvbio/ProteinFlow/main/media/pf-1.png) --- ## Installation conda: ```bash
-# This should take a few minutes, be patient conda install -c conda-forge -
-c bioconda -c adaptyvbio proteinflow ``` pip: ```bash pip install proteinflow
-``` docker: ```bash docker pull adaptyvbio/proteinflow ``` ### Troubleshooting
-- If you are using python 3.10 and encountering installation problems, try
-running `python -m pip install prody==2.4.0` before installing `proteinflow`. -
-If you are planning to generate new datasets and installed `proteinflow` with
-`pip`, you will need to additionally install [`mmseqs`](https://github.com/
-soedinglab/MMseqs2). - Generating new datasets also depends on the `rcsbsearch`
-package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/
-releases/tag/v0.2.3) is currently not working correctly. The recommended fix is
-installing the version from [this pull request](https://github.com/sbliven/
-rcsbsearch/pull/6). ```bash python -m pip install "rcsbsearch @ git+https://
-github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` -
-The docker image can be accessed in interactive mode with this command. ```bash
-docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage
-### Downloading pre-computed datasets (stable) Already precomputed datasets
-with consensus set of parameters and can be accessed and downloaded using the
-`proteinflow`. package. Check the output of `proteinflow check_tags` for a list
-of available tags. ```bash proteinflow download --tag 20230102_stable ``` ###
-Running the pipeline (PDB) You can also run `proteinflow` with your own
-parameters. Check the output of `proteinflow check_snapshots` for a list of
-available PDB snapshots (naming rule: `yyyymmdd`). For instance, let's generate
-a dataset with the following description: - resolution threshold: 5 angstrom, -
-PDB snapshot: 20190101, - structure methods accepted: all (x-ray
-christolography, NRM, Cryo-EM), - sequence identity threshold for clustering:
-40% sequence similarity, - maximum length per sequence: 1000 residues, -
-minimum length per sequence: 5 residues, - maximum fraction of missing values
-at the ends: 10%, - size of validation subset: 10%. ```bash proteinflow
-generate --tag new --resolution_thr 5 --pdb_snapshot 20190101 --
-not_filter_methods --min_seq_id 0.4 --max_length 1000 --min_length 5 --
-missing_ends_thr 0.1 --valid_split 0.1 ``` See the [docs](https://
-adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`) for the
-full list of parameters and more information. A registry of all the files that
-are removed during the filtering as well as description with the reason for
-their removal is created automatically for each `generate` command. The log
-files are save (at `data/logs` by default) and a summary can be accessed
-running `proteinflow get_summary {log_path}`. ### Running the pipeline (SAbDab)
-You can also use the `--sabdab` option in `proteinflow generate` to load files
-from SAbDab and cluster them based on CDRs. By default the `--sabdab` tag will
-download the latest up-to-date version of the SabDab dataset and cluster the
-antibodies based on their CDR sequence. Alternatively, it can be used together
-with the tag `--sabdab_data_path` to process a custom SAbDab-like zip file or
-folder. This allows you to use search and query tools from the [SabDab web
-interface](https://opig.stats.ox.ac.uk/webapps/newsabdab/sabdab/) to create a
-custom dataset by downloading the archived zip file of the structures selected.
-(Under Downloads section of your SabDab query). SAbDab sequences clustering is
-done across all 6 Complementary Determining Regions (CDRs) - H1, H2, H3, L1,
-L2, L3, based on the [Chothia numbering](https://pubmed.ncbi.nlm.nih.gov/
-9367782/) implemented by SabDab. CDRs from nanobodies and other synthetic
-constructs are clustered together with other heavy chain CDRs. The resulting
-CDR clusters are split into training, test and validation in a way that ensures
-that every PDB file only appears in one subset. Individual output pickle files
-represent heavy chain - light chain - antigen complexes (created from SAbDab
-annotation, sometimes more than one per PDB entry). Each of the elements (heavy
-chain, light chain, antigen) can be missing in specific entries and there can
-be multiple antigen chains. In order to filter for at least one antigen chain,
-use the `--require_antigen` option. For instance, let's generate a dataset with
-the following description: - SabDab version: latest (up-to-date), - resolution
-threshold: 5 angstrom, - structure methods accepted: all (x-ray
-christolography, NRM, Cryo-EM), - sequence identity threshold for clustering
-(CDRs): 40%, - size of validation subset: 10%. ```bash proteinflow generate --
-sabdab --resolution_thr 5 --not_filter_methods --min_seq_id 0.4 --valid_split
-0.1 ``` ### Splitting By default, both `proteinflow generate` and `proteinflow
-download` will also split your data into training, test and validation
-according to MMseqs2 clustering and homomer/heteromer/single chain proportions.
-However, you can skip this step with a `--skip_splitting` flag and then perform
-it separately with the `proteinflow split` command. The following command will
-perform the splitting with a 10% validation set, a 5% test set and a 50%
-threshold for sequence identity clusters. ```bash proteinflow split --tag new -
--valid_split 0.1 --test_split 0.5 --min_seq_id 0.5 ``` Use the `--
-exclude_chains` and `--exclude_threshold` parameters to move all biounits that
-contain chains similar to what you specify to a separate folder. ### Using the
-data The output files are pickled nested dictionaries where first-level keys
-are chain Ids and second-level keys are the following: - `'crd_bb'`: a `numpy`
-array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O), -
-`'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom
-coordinates (check `proteinflow.sidechain_order()` for the order of atoms), -
-`'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with
-known coordinates and zeros to missing values, - `'seq'`: a string of length
-`L` with residue types. In a SAbDab datasets, an additional key is added to the
-dictionary: - `'cdr'`: a `numpy` array of shape `(L,)` where CDR residues are
-marked with the corresponding type (`'H1'`, `'L1'`, ...) and non-CDR residues
-are marked with `'-'`. Note that the sequence information in the PDB files is
-aligned to the FASTA sequences to identify the missing residues. Once your data
-is ready, you can open the files with `pickle` directly. ```python import
-pickle import os train_folder = "./data/proteinflow_new/training" for filename
-in os.listdir(train_folder): with open(os.path.join(train_folder, filename),
-"rb") as f: data = pickle.load(f) crd_bb = data["crd_bb"] seq = data["seq"] ...
-``` Alternatively, you can use our `ProteinDataset` or `ProteinLoader` classes
-for convenient processing. Among other things, they allow for feature
-extraction, single chain / homomer / heteromer filtering and randomized
-sampling from sequence identity clusters. For example, here is how we can
-create a data loader that: - samples a different cluster representative at
-every epoch, - extracts dihedral angles, sidechain orientation and secondary
-structure features, - only loads pairs of interacting proteins (larger biounits
-are broken up into pairs), - has batch size 8. ```python from proteinflow
-import ProteinLoader train_loader = ProteinLoader.from_args( "./data/
-proteinflow_new/training", clustering_dict_path="./data/proteinflow_new/
-splits_dict/train.pickle",
+tags) [![Generic badge](https://img.shields.io/badge/Contributions-Welcome-
+brightgreen.svg)](CONTRIBUTING.md) ProteinFlow is an open-source Python library
+that streamlines the pre-processing of protein structure data for deep learning
+applications. ProteinFlow enables users to efficiently filter, cluster, and
+generate new datasets from resources like the Protein Data Bank (PDB) and
+SAbDab (The Structural Antibody Database). Here are some of the key features we
+currently support: - âï¸ Processing of both single-chain and multi-chain
+protein structures (Biounit PDB definition) - ð·ï¸ Various featurization
+options can be computed, including secondary structure features, torsion
+angles, etc. - ð¾ A variety of data loading options and conversions to cater
+to different downstream training frameworks - ð§¬ Access to up-to-date, pre-
+computed protein structure datasets ![overview](https://
+raw.githubusercontent.com/adaptyvbio/ProteinFlow/main/media/pf-1.png) --- ##
+Installation conda: ```bash # This should take a few minutes, be patient conda
+install -c conda-forge -c bioconda -c adaptyvbio proteinflow ``` pip: ```bash
+pip install proteinflow ``` docker: ```bash docker pull adaptyvbio/proteinflow
+``` ### Troubleshooting - If you are using python 3.10 and encountering
+installation problems, try running `python -m pip install prody==2.4.0` before
+installing `proteinflow`. - If you are planning to generate new datasets and
+installed `proteinflow` with `pip`, you will need to additionally install
+[`mmseqs`](https://github.com/soedinglab/MMseqs2). - Generating new datasets
+also depends on the `rcsbsearch` package and the latest release [v0.2.3](https:
+//github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working
+correctly. The recommended fix is installing the version from [this pull
+request](https://github.com/sbliven/rcsbsearch/pull/6). ```bash python -m pip
+install "rcsbsearch @ git+https://github.com/sbliven/
+rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` - The docker image can
+be accessed in interactive mode with this command. ```bash docker run -it -v /
+path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage ### Downloading
+pre-computed datasets (stable) Already precomputed datasets with consensus set
+of parameters and can be accessed and downloaded using the `proteinflow`.
+package. Check the output of `proteinflow check_tags` for a list of available
+tags. ```bash proteinflow download --tag 20230102_stable ``` ### Running the
+pipeline (PDB) You can also run `proteinflow` with your own parameters. Check
+the output of `proteinflow check_snapshots` for a list of available PDB
+snapshots (naming rule: `yyyymmdd`). For instance, let's generate a dataset
+with the following description: - resolution threshold: 5 angstrom, - PDB
+snapshot: 20190101, - structure methods accepted: all (x-ray christolography,
+NRM, Cryo-EM), - sequence identity threshold for clustering: 40% sequence
+similarity, - maximum length per sequence: 1000 residues, - minimum length per
+sequence: 5 residues, - maximum fraction of missing values at the ends: 10%, -
+size of validation subset: 10%. ```bash proteinflow generate --tag new --
+resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4
+--max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1 ```
+See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow
+generate --help`) for the full list of parameters and more information. A
+registry of all the files that are removed during the filtering as well as
+description with the reason for their removal is created automatically for each
+`generate` command. The log files are save (at `data/logs` by default) and a
+summary can be accessed running `proteinflow get_summary {log_path}`. ###
+Running the pipeline (SAbDab) You can also use the `--sabdab` option in
+`proteinflow generate` to load files from SAbDab and cluster them based on
+CDRs. By default the `--sabdab` tag will download the latest up-to-date version
+of the SabDab dataset and cluster the antibodies based on their CDR sequence.
+Alternatively, it can be used together with the tag `--sabdab_data_path` to
+process a custom SAbDab-like zip file or folder. This allows you to use search
+and query tools from the [SabDab web interface](https://opig.stats.ox.ac.uk/
+webapps/newsabdab/sabdab/) to create a custom dataset by downloading the
+archived zip file of the structures selected. (Under Downloads section of your
+SabDab query). SAbDab sequences clustering is done across all 6 Complementary
+Determining Regions (CDRs) - H1, H2, H3, L1, L2, L3, based on the [Chothia
+numbering](https://pubmed.ncbi.nlm.nih.gov/9367782/) implemented by SabDab.
+CDRs from nanobodies and other synthetic constructs are clustered together with
+other heavy chain CDRs. The resulting CDR clusters are split into training,
+test and validation in a way that ensures that every PDB file only appears in
+one subset. Individual output pickle files represent heavy chain - light chain
+- antigen complexes (created from SAbDab annotation, sometimes more than one
+per PDB entry). Each of the elements (heavy chain, light chain, antigen) can be
+missing in specific entries and there can be multiple antigen chains. In order
+to filter for at least one antigen chain, use the `--require_antigen` option.
+For instance, let's generate a dataset with the following description: - SabDab
+version: latest (up-to-date), - resolution threshold: 5 angstrom, - structure
+methods accepted: all (x-ray christolography, NRM, Cryo-EM), - sequence
+identity threshold for clustering (CDRs): 40%, - size of validation subset:
+10%. ```bash proteinflow generate --sabdab --resolution_thr 5 --
+not_filter_methods --min_seq_id 0.4 --valid_split 0.1 ``` ### Splitting By
+default, both `proteinflow generate` and `proteinflow download` will also split
+your data into training, test and validation according to MMseqs2 clustering
+and homomer/heteromer/single chain proportions. However, you can skip this step
+with a `--skip_splitting` flag and then perform it separately with the
+`proteinflow split` command. The following command will perform the splitting
+with a 10% validation set, a 5% test set and a 50% threshold for sequence
+identity clusters. ```bash proteinflow split --tag new --valid_split 0.1 --
+test_split 0.5 --min_seq_id 0.5 ``` Use the `--exclude_chains` and `--
+exclude_threshold` parameters to move all biounits that contain chains similar
+to what you specify to a separate folder. ### Using the data The output files
+are pickled nested dictionaries where first-level keys are chain Ids and
+second-level keys are the following: - `'crd_bb'`: a `numpy` array of shape `
+(L, 4, 3)` with backbone atom coordinates (N, C, CA, O), - `'crd_sc'`: a
+`numpy` array of shape `(L, 10, 3)` with sidechain atom coordinates (check
+`proteinflow.sidechain_order()` for the order of atoms), - `'msk'`: a `numpy`
+array of shape `(L,)` where ones correspond to residues with known coordinates
+and zeros to missing values, - `'seq'`: a string of length `L` with residue
+types. In a SAbDab datasets, an additional key is added to the dictionary: -
+`'cdr'`: a `numpy` array of shape `(L,)` where CDR residues are marked with the
+corresponding type (`'H1'`, `'L1'`, ...) and non-CDR residues are marked with
+`'-'`. Note that the sequence information in the PDB files is aligned to the
+FASTA sequences to identify the missing residues. Once your data is ready, you
+can open the files with `pickle` directly. ```python import pickle import os
+train_folder = "./data/proteinflow_new/training" for filename in os.listdir
+(train_folder): with open(os.path.join(train_folder, filename), "rb") as f:
+data = pickle.load(f) crd_bb = data["crd_bb"] seq = data["seq"] ... ```
+Alternatively, you can use our `ProteinDataset` or `ProteinLoader` classes for
+convenient processing. Among other things, they allow for feature extraction,
+single chain / homomer / heteromer filtering and randomized sampling from
+sequence identity clusters. For example, here is how we can create a data
+loader that: - samples a different cluster representative at every epoch, -
+extracts dihedral angles, sidechain orientation and secondary structure
+features, - only loads pairs of interacting proteins (larger biounits are
+broken up into pairs), - has batch size 8. ```python from proteinflow import
+ProteinLoader train_loader = ProteinLoader.from_args( "./data/proteinflow_new/
+training", clustering_dict_path="./data/proteinflow_new/splits_dict/
+train.pickle",
 node_features_type="dihedral+sidechain_orientation+secondary_structure",
 entry_type="pair", batch_size=8, ) for batch in train_loader: crd_bb = batch
 ["X"] #(B, L, 4, 3) seq = batch["S"] #(B, L) sse = batch["secondary_structure"]
 #(B, L, 3) to_predict = batch["masked_res"] #(B, L), 1 where the residues
 should be masked, 0 otherwise ... ``` See more details on available parameters
 and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) +
 [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use
```

### Comparing `proteinflow-1.3.6/README.md` & `proteinflow-1.4.0/proteinflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: proteinflow
+Version: 1.4.0
+Summary: Versatile pipeline for processing protein structure data for deep learning applications.
+Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
+License: BSD-3-Clause
+Keywords: bioinformatics,dataset,protein,PDB,deep learning
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
     <b> ProteinFlow - A data processing pipeline for all your protein design needs </b> <br />
 </p>
 
 <p align="center">
   <a href="https://adaptyvbio.github.io/ProteinFlow/" target="_blank">
       Docs
@@ -11,15 +22,15 @@
 ---
 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/proteinflow)](https://pypi.org/project/proteinflow/)
 [![Conda](https://img.shields.io/conda/v/adaptyvbio/proteinflow)](https://anaconda.org/adaptyvbio/proteinflow)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/tags)
-![Generic badge](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)
+[![Generic badge](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](CONTRIBUTING.md)
 
 
 ProteinFlow is an open-source Python library that streamlines the pre-processing of protein structure data for deep learning applications. ProteinFlow enables users to efficiently filter, cluster, and generate new datasets from resources like the Protein Data Bank (PDB) and SAbDab (The Structural Antibody Database).
 
 Here are some of the key features we currently support:
 
 - ⛓️ Processing of both single-chain and multi-chain protein structures (Biounit PDB definition)
```

#### html2text {}

```diff
@@ -1,129 +1,137 @@
+Metadata-Version: 2.1 Name: proteinflow Version: 1.4.0 Summary: Versatile
+pipeline for processing protein structure data for deep learning applications.
+Author-email: Liza Kozlova
+adaptyvbio.com>, Arthur Valentin
+adaptyvbio.com> License: BSD-3-Clause Keywords:
+bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
                                      Docs
 --- [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)]
 (https://opensource.org/licenses/BSD-3-Clause) [![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
 black) [![PyPI](https://img.shields.io/pypi/v/proteinflow)](https://pypi.org/
 project/proteinflow/) [![Conda](https://img.shields.io/conda/v/adaptyvbio/
 proteinflow)](https://anaconda.org/adaptyvbio/proteinflow) [![Docker Image
 Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/
 proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/
-tags) ![Generic badge](https://img.shields.io/badge/Contributions-Welcome-
-brightgreen.svg) ProteinFlow is an open-source Python library that streamlines
-the pre-processing of protein structure data for deep learning applications.
-ProteinFlow enables users to efficiently filter, cluster, and generate new
-datasets from resources like the Protein Data Bank (PDB) and SAbDab (The
-Structural Antibody Database). Here are some of the key features we currently
-support: - âï¸ Processing of both single-chain and multi-chain protein
-structures (Biounit PDB definition) - ð·ï¸ Various featurization options can
-be computed, including secondary structure features, torsion angles, etc. -
-ð¾ A variety of data loading options and conversions to cater to different
-downstream training frameworks - ð§¬ Access to up-to-date, pre-computed
-protein structure datasets ![overview](https://raw.githubusercontent.com/
-adaptyvbio/ProteinFlow/main/media/pf-1.png) --- ## Installation conda: ```bash
-# This should take a few minutes, be patient conda install -c conda-forge -
-c bioconda -c adaptyvbio proteinflow ``` pip: ```bash pip install proteinflow
-``` docker: ```bash docker pull adaptyvbio/proteinflow ``` ### Troubleshooting
-- If you are using python 3.10 and encountering installation problems, try
-running `python -m pip install prody==2.4.0` before installing `proteinflow`. -
-If you are planning to generate new datasets and installed `proteinflow` with
-`pip`, you will need to additionally install [`mmseqs`](https://github.com/
-soedinglab/MMseqs2). - Generating new datasets also depends on the `rcsbsearch`
-package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/
-releases/tag/v0.2.3) is currently not working correctly. The recommended fix is
-installing the version from [this pull request](https://github.com/sbliven/
-rcsbsearch/pull/6). ```bash python -m pip install "rcsbsearch @ git+https://
-github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` -
-The docker image can be accessed in interactive mode with this command. ```bash
-docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage
-### Downloading pre-computed datasets (stable) Already precomputed datasets
-with consensus set of parameters and can be accessed and downloaded using the
-`proteinflow`. package. Check the output of `proteinflow check_tags` for a list
-of available tags. ```bash proteinflow download --tag 20230102_stable ``` ###
-Running the pipeline (PDB) You can also run `proteinflow` with your own
-parameters. Check the output of `proteinflow check_snapshots` for a list of
-available PDB snapshots (naming rule: `yyyymmdd`). For instance, let's generate
-a dataset with the following description: - resolution threshold: 5 angstrom, -
-PDB snapshot: 20190101, - structure methods accepted: all (x-ray
-christolography, NRM, Cryo-EM), - sequence identity threshold for clustering:
-40% sequence similarity, - maximum length per sequence: 1000 residues, -
-minimum length per sequence: 5 residues, - maximum fraction of missing values
-at the ends: 10%, - size of validation subset: 10%. ```bash proteinflow
-generate --tag new --resolution_thr 5 --pdb_snapshot 20190101 --
-not_filter_methods --min_seq_id 0.4 --max_length 1000 --min_length 5 --
-missing_ends_thr 0.1 --valid_split 0.1 ``` See the [docs](https://
-adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`) for the
-full list of parameters and more information. A registry of all the files that
-are removed during the filtering as well as description with the reason for
-their removal is created automatically for each `generate` command. The log
-files are save (at `data/logs` by default) and a summary can be accessed
-running `proteinflow get_summary {log_path}`. ### Running the pipeline (SAbDab)
-You can also use the `--sabdab` option in `proteinflow generate` to load files
-from SAbDab and cluster them based on CDRs. By default the `--sabdab` tag will
-download the latest up-to-date version of the SabDab dataset and cluster the
-antibodies based on their CDR sequence. Alternatively, it can be used together
-with the tag `--sabdab_data_path` to process a custom SAbDab-like zip file or
-folder. This allows you to use search and query tools from the [SabDab web
-interface](https://opig.stats.ox.ac.uk/webapps/newsabdab/sabdab/) to create a
-custom dataset by downloading the archived zip file of the structures selected.
-(Under Downloads section of your SabDab query). SAbDab sequences clustering is
-done across all 6 Complementary Determining Regions (CDRs) - H1, H2, H3, L1,
-L2, L3, based on the [Chothia numbering](https://pubmed.ncbi.nlm.nih.gov/
-9367782/) implemented by SabDab. CDRs from nanobodies and other synthetic
-constructs are clustered together with other heavy chain CDRs. The resulting
-CDR clusters are split into training, test and validation in a way that ensures
-that every PDB file only appears in one subset. Individual output pickle files
-represent heavy chain - light chain - antigen complexes (created from SAbDab
-annotation, sometimes more than one per PDB entry). Each of the elements (heavy
-chain, light chain, antigen) can be missing in specific entries and there can
-be multiple antigen chains. In order to filter for at least one antigen chain,
-use the `--require_antigen` option. For instance, let's generate a dataset with
-the following description: - SabDab version: latest (up-to-date), - resolution
-threshold: 5 angstrom, - structure methods accepted: all (x-ray
-christolography, NRM, Cryo-EM), - sequence identity threshold for clustering
-(CDRs): 40%, - size of validation subset: 10%. ```bash proteinflow generate --
-sabdab --resolution_thr 5 --not_filter_methods --min_seq_id 0.4 --valid_split
-0.1 ``` ### Splitting By default, both `proteinflow generate` and `proteinflow
-download` will also split your data into training, test and validation
-according to MMseqs2 clustering and homomer/heteromer/single chain proportions.
-However, you can skip this step with a `--skip_splitting` flag and then perform
-it separately with the `proteinflow split` command. The following command will
-perform the splitting with a 10% validation set, a 5% test set and a 50%
-threshold for sequence identity clusters. ```bash proteinflow split --tag new -
--valid_split 0.1 --test_split 0.5 --min_seq_id 0.5 ``` Use the `--
-exclude_chains` and `--exclude_threshold` parameters to move all biounits that
-contain chains similar to what you specify to a separate folder. ### Using the
-data The output files are pickled nested dictionaries where first-level keys
-are chain Ids and second-level keys are the following: - `'crd_bb'`: a `numpy`
-array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O), -
-`'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom
-coordinates (check `proteinflow.sidechain_order()` for the order of atoms), -
-`'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with
-known coordinates and zeros to missing values, - `'seq'`: a string of length
-`L` with residue types. In a SAbDab datasets, an additional key is added to the
-dictionary: - `'cdr'`: a `numpy` array of shape `(L,)` where CDR residues are
-marked with the corresponding type (`'H1'`, `'L1'`, ...) and non-CDR residues
-are marked with `'-'`. Note that the sequence information in the PDB files is
-aligned to the FASTA sequences to identify the missing residues. Once your data
-is ready, you can open the files with `pickle` directly. ```python import
-pickle import os train_folder = "./data/proteinflow_new/training" for filename
-in os.listdir(train_folder): with open(os.path.join(train_folder, filename),
-"rb") as f: data = pickle.load(f) crd_bb = data["crd_bb"] seq = data["seq"] ...
-``` Alternatively, you can use our `ProteinDataset` or `ProteinLoader` classes
-for convenient processing. Among other things, they allow for feature
-extraction, single chain / homomer / heteromer filtering and randomized
-sampling from sequence identity clusters. For example, here is how we can
-create a data loader that: - samples a different cluster representative at
-every epoch, - extracts dihedral angles, sidechain orientation and secondary
-structure features, - only loads pairs of interacting proteins (larger biounits
-are broken up into pairs), - has batch size 8. ```python from proteinflow
-import ProteinLoader train_loader = ProteinLoader.from_args( "./data/
-proteinflow_new/training", clustering_dict_path="./data/proteinflow_new/
-splits_dict/train.pickle",
+tags) [![Generic badge](https://img.shields.io/badge/Contributions-Welcome-
+brightgreen.svg)](CONTRIBUTING.md) ProteinFlow is an open-source Python library
+that streamlines the pre-processing of protein structure data for deep learning
+applications. ProteinFlow enables users to efficiently filter, cluster, and
+generate new datasets from resources like the Protein Data Bank (PDB) and
+SAbDab (The Structural Antibody Database). Here are some of the key features we
+currently support: - âï¸ Processing of both single-chain and multi-chain
+protein structures (Biounit PDB definition) - ð·ï¸ Various featurization
+options can be computed, including secondary structure features, torsion
+angles, etc. - ð¾ A variety of data loading options and conversions to cater
+to different downstream training frameworks - ð§¬ Access to up-to-date, pre-
+computed protein structure datasets ![overview](https://
+raw.githubusercontent.com/adaptyvbio/ProteinFlow/main/media/pf-1.png) --- ##
+Installation conda: ```bash # This should take a few minutes, be patient conda
+install -c conda-forge -c bioconda -c adaptyvbio proteinflow ``` pip: ```bash
+pip install proteinflow ``` docker: ```bash docker pull adaptyvbio/proteinflow
+``` ### Troubleshooting - If you are using python 3.10 and encountering
+installation problems, try running `python -m pip install prody==2.4.0` before
+installing `proteinflow`. - If you are planning to generate new datasets and
+installed `proteinflow` with `pip`, you will need to additionally install
+[`mmseqs`](https://github.com/soedinglab/MMseqs2). - Generating new datasets
+also depends on the `rcsbsearch` package and the latest release [v0.2.3](https:
+//github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working
+correctly. The recommended fix is installing the version from [this pull
+request](https://github.com/sbliven/rcsbsearch/pull/6). ```bash python -m pip
+install "rcsbsearch @ git+https://github.com/sbliven/
+rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` - The docker image can
+be accessed in interactive mode with this command. ```bash docker run -it -v /
+path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage ### Downloading
+pre-computed datasets (stable) Already precomputed datasets with consensus set
+of parameters and can be accessed and downloaded using the `proteinflow`.
+package. Check the output of `proteinflow check_tags` for a list of available
+tags. ```bash proteinflow download --tag 20230102_stable ``` ### Running the
+pipeline (PDB) You can also run `proteinflow` with your own parameters. Check
+the output of `proteinflow check_snapshots` for a list of available PDB
+snapshots (naming rule: `yyyymmdd`). For instance, let's generate a dataset
+with the following description: - resolution threshold: 5 angstrom, - PDB
+snapshot: 20190101, - structure methods accepted: all (x-ray christolography,
+NRM, Cryo-EM), - sequence identity threshold for clustering: 40% sequence
+similarity, - maximum length per sequence: 1000 residues, - minimum length per
+sequence: 5 residues, - maximum fraction of missing values at the ends: 10%, -
+size of validation subset: 10%. ```bash proteinflow generate --tag new --
+resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4
+--max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1 ```
+See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow
+generate --help`) for the full list of parameters and more information. A
+registry of all the files that are removed during the filtering as well as
+description with the reason for their removal is created automatically for each
+`generate` command. The log files are save (at `data/logs` by default) and a
+summary can be accessed running `proteinflow get_summary {log_path}`. ###
+Running the pipeline (SAbDab) You can also use the `--sabdab` option in
+`proteinflow generate` to load files from SAbDab and cluster them based on
+CDRs. By default the `--sabdab` tag will download the latest up-to-date version
+of the SabDab dataset and cluster the antibodies based on their CDR sequence.
+Alternatively, it can be used together with the tag `--sabdab_data_path` to
+process a custom SAbDab-like zip file or folder. This allows you to use search
+and query tools from the [SabDab web interface](https://opig.stats.ox.ac.uk/
+webapps/newsabdab/sabdab/) to create a custom dataset by downloading the
+archived zip file of the structures selected. (Under Downloads section of your
+SabDab query). SAbDab sequences clustering is done across all 6 Complementary
+Determining Regions (CDRs) - H1, H2, H3, L1, L2, L3, based on the [Chothia
+numbering](https://pubmed.ncbi.nlm.nih.gov/9367782/) implemented by SabDab.
+CDRs from nanobodies and other synthetic constructs are clustered together with
+other heavy chain CDRs. The resulting CDR clusters are split into training,
+test and validation in a way that ensures that every PDB file only appears in
+one subset. Individual output pickle files represent heavy chain - light chain
+- antigen complexes (created from SAbDab annotation, sometimes more than one
+per PDB entry). Each of the elements (heavy chain, light chain, antigen) can be
+missing in specific entries and there can be multiple antigen chains. In order
+to filter for at least one antigen chain, use the `--require_antigen` option.
+For instance, let's generate a dataset with the following description: - SabDab
+version: latest (up-to-date), - resolution threshold: 5 angstrom, - structure
+methods accepted: all (x-ray christolography, NRM, Cryo-EM), - sequence
+identity threshold for clustering (CDRs): 40%, - size of validation subset:
+10%. ```bash proteinflow generate --sabdab --resolution_thr 5 --
+not_filter_methods --min_seq_id 0.4 --valid_split 0.1 ``` ### Splitting By
+default, both `proteinflow generate` and `proteinflow download` will also split
+your data into training, test and validation according to MMseqs2 clustering
+and homomer/heteromer/single chain proportions. However, you can skip this step
+with a `--skip_splitting` flag and then perform it separately with the
+`proteinflow split` command. The following command will perform the splitting
+with a 10% validation set, a 5% test set and a 50% threshold for sequence
+identity clusters. ```bash proteinflow split --tag new --valid_split 0.1 --
+test_split 0.5 --min_seq_id 0.5 ``` Use the `--exclude_chains` and `--
+exclude_threshold` parameters to move all biounits that contain chains similar
+to what you specify to a separate folder. ### Using the data The output files
+are pickled nested dictionaries where first-level keys are chain Ids and
+second-level keys are the following: - `'crd_bb'`: a `numpy` array of shape `
+(L, 4, 3)` with backbone atom coordinates (N, C, CA, O), - `'crd_sc'`: a
+`numpy` array of shape `(L, 10, 3)` with sidechain atom coordinates (check
+`proteinflow.sidechain_order()` for the order of atoms), - `'msk'`: a `numpy`
+array of shape `(L,)` where ones correspond to residues with known coordinates
+and zeros to missing values, - `'seq'`: a string of length `L` with residue
+types. In a SAbDab datasets, an additional key is added to the dictionary: -
+`'cdr'`: a `numpy` array of shape `(L,)` where CDR residues are marked with the
+corresponding type (`'H1'`, `'L1'`, ...) and non-CDR residues are marked with
+`'-'`. Note that the sequence information in the PDB files is aligned to the
+FASTA sequences to identify the missing residues. Once your data is ready, you
+can open the files with `pickle` directly. ```python import pickle import os
+train_folder = "./data/proteinflow_new/training" for filename in os.listdir
+(train_folder): with open(os.path.join(train_folder, filename), "rb") as f:
+data = pickle.load(f) crd_bb = data["crd_bb"] seq = data["seq"] ... ```
+Alternatively, you can use our `ProteinDataset` or `ProteinLoader` classes for
+convenient processing. Among other things, they allow for feature extraction,
+single chain / homomer / heteromer filtering and randomized sampling from
+sequence identity clusters. For example, here is how we can create a data
+loader that: - samples a different cluster representative at every epoch, -
+extracts dihedral angles, sidechain orientation and secondary structure
+features, - only loads pairs of interacting proteins (larger biounits are
+broken up into pairs), - has batch size 8. ```python from proteinflow import
+ProteinLoader train_loader = ProteinLoader.from_args( "./data/proteinflow_new/
+training", clustering_dict_path="./data/proteinflow_new/splits_dict/
+train.pickle",
 node_features_type="dihedral+sidechain_orientation+secondary_structure",
 entry_type="pair", batch_size=8, ) for batch in train_loader: crd_bb = batch
 ["X"] #(B, L, 4, 3) seq = batch["S"] #(B, L) sse = batch["secondary_structure"]
 #(B, L, 3) to_predict = batch["masked_res"] #(B, L), 1 where the residues
 should be masked, 0 otherwise ... ``` See more details on available parameters
 and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) +
 [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use
```

### Comparing `proteinflow-1.3.6/proteinflow/scripts/proteinflow_cli.py` & `proteinflow-1.4.0/proteinflow/scripts/proteinflow_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+"""Command line interface for proteinflow"""
+
+import click
+
 from proteinflow import (
     check_download_tags,
     check_pdb_snapshots,
     download_data,
     generate_data,
-    split_data,
     get_error_summary,
+    split_data,
     unsplit_data,
 )
-import click
 
 
 @click.group(help="A data processing pipeline for protein design ML tasks")
 def cli():
     pass
 
 
@@ -40,14 +43,15 @@
     help="The folder where proteinflow datasets, temporary files and logs will be stored",
 )
 @click.option(
     "--skip_splitting", is_flag=True, help="Use this flag to skip splitting the data"
 )
 @cli.command("download", help="Download an existing ProteinFlow dataset")
 def download(**kwargs):
+    """Download an existing ProteinFlow dataset"""
     download_data(**kwargs)
 
 
 @click.option(
     "--tag",
     help="The name of the dataset",
 )
@@ -150,16 +154,23 @@
     help="Path to a zip file or a directory containing SAbDab files (only used if `sabdab` is `True`)",
 )
 @click.option(
     "--require_antigen",
     is_flag=True,
     help="Use this flag to require that the SAbDab files contain an antigen",
 )
+@click.option(
+    "--random_seed",
+    default=42,
+    type=int,
+    help="The random seed to use for splitting",
+)
 @cli.command("generate", help="Generate a new ProteinFlow dataset")
 def generate(**kwargs):
+    """Generate a new ProteinFlow dataset"""
     generate_data(**kwargs)
 
 
 @click.option(
     "--tag",
     help="The name of the dataset",
 )
@@ -216,19 +227,26 @@
     help="Exclude clusters that contain chains similar to chains to exclude",
 )
 @click.option(
     "--exclude_based_on_cdr",
     type=click.Choice(["L1", "L2", "L3", "H1", "H2", "H3"]),
     help="if given and exclude_clusters is true + the dataset is SAbDab, exclude files based on only the given CDR clusters",
 )
+@click.option(
+    "--random_seed",
+    default=42,
+    type=int,
+    help="The random seed to use for splitting",
+)
 @cli.command(
     "split",
     help="Split an existing ProteinFlow dataset into training, validation and test subset according to MMseqs clustering and homomer/heteromer/single chain proportions",
 )
 def split(**kwargs):
+    """Split an existing ProteinFlow dataset into training, validation and test subset according to MMseqs clustering and homomer/heteromer/single chain proportions"""
     split_data(**kwargs)
 
 
 @click.option(
     "--tag",
     help="The name of the dataset",
 )
@@ -238,18 +256,20 @@
     help="The folder where proteinflow datasets are stored",
 )
 @cli.command(
     "unsplit",
     help="Move files from train, test, validation and excluded folders back into the main folder",
 )
 def unsplit(**kwargs):
+    """Move files from train, test, validation and excluded folders back into the main folder"""
     unsplit_data(**kwargs)
 
 
 @click.argument("log_path")
 @cli.command("get_summary", help="Get a summary of filtering reasons from a log file")
 def get_summary(log_path):
+    """Get a summary of filtering reasons from a log file"""
     get_error_summary(log_path)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `proteinflow-1.3.6/proteinflow/utils/biotite_sse.py` & `proteinflow-1.4.0/proteinflow/utils/biotite_sse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# Adapted from: https://github.com/biotite-dev/biotite
+"""
+This module contains a function to annotate secondary structure elements (SSEs) in a chain.
+
+Adapted from: https://github.com/biotite-dev/biotite.
+"""
 
-from biotite.structure.geometry import distance, angle, dihedral
 import numpy as np
+from biotite.structure.geometry import angle, dihedral, distance
 
 
 def _annotate_sse(X):
-    """
-    Annotation of secondary structure elements (SSEs) in a chain
-    """
-
+    """Annotation of secondary structure elements (SSEs) in a chain."""
     ca_coord = X[:, 2, :]
     length = ca_coord.shape[0]
 
     _r_helix = (np.deg2rad(89 - 12), np.deg2rad(89 + 12))
     _a_helix = (np.deg2rad(50 - 20), np.deg2rad(50 + 20))
-    _d2_helix = ((5.5 - 0.5), (5.5 + 0.5))  # Not used in the algorithm description
     _d3_helix = ((5.3 - 0.5), (5.3 + 0.5))
     _d4_helix = ((6.4 - 0.6), (6.4 + 0.6))
 
     _r_strand = (np.deg2rad(124 - 14), np.deg2rad(124 + 14))
     _a_strand = (np.deg2rad(-180), np.deg2rad(-125), np.deg2rad(145), np.deg2rad(180))
     _d2_strand = ((6.7 - 0.6), (6.7 + 0.6))
     _d3_strand = ((9.9 - 0.9), (9.9 + 0.9))
```

### Comparing `proteinflow-1.3.6/proteinflow/utils/cluster_and_partition.py` & `proteinflow-1.4.0/proteinflow/utils/cluster_and_partition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,129 +1,25 @@
 import os
-import copy
-import subprocess
-import editdistance
-import numpy as np
 import random as rd
-import pickle as pkl
-import networkx as nx
-from tqdm import tqdm
+import subprocess
 from collections import defaultdict
 from itertools import combinations
 
+import networkx as nx
+import numpy as np
+from tqdm import tqdm
 
-def _unique_chains(seqs_list):
-    """
-    Get unique chains
-    """
-
-    new_seqs_list = [seqs_list[0]]
-    chains = [new_seqs_list[0][0]]
-
-    for seq in seqs_list[1:]:
-        if seq[0] not in chains:
-            new_seqs_list.append(seq)
-            chains.append(seq[0])
-
-    return new_seqs_list
-
-
-def _merge_chains(seqs_dict_):
-    """
-    Look into the chains of each PDB and regroup redundancies (at 90% sequence identity)
-    """
-
-    seqs_dict = copy.deepcopy(seqs_dict_)
-    pdbs_to_delete = []
-
-    for pdb in tqdm(seqs_dict.keys()):
-        if seqs_dict[pdb] == []:
-            pdbs_to_delete.append(pdb)
-            continue
-
-        seqs_dict[pdb] = _unique_chains(seqs_dict[pdb])
-        groups, ref_seqs, indexes = [], [], []
-
-        for k in range(len(seqs_dict[pdb])):
-            if k in indexes:
-                continue
-            group = [seqs_dict[pdb][k][0]]
-            ref_seq = seqs_dict[pdb][k][1]
-            ref_seqs.append(ref_seq)
-            indexes.append(k)
-
-            for l in range(k + 1, len(seqs_dict[pdb])):
-                chain, seq = seqs_dict[pdb][l][0], seqs_dict[pdb][l][1]
-                if (
-                    l in indexes
-                    or len(seq) > 1.1 * len(ref_seq)
-                    or len(seq) < 0.9 * len(ref_seq)
-                    or editdistance.eval(seq, ref_seq) / max(len(seq), len(ref_seq))
-                    > 0.1
-                ):
-                    continue
-                group.append(chain)
-                indexes.append(l)
-
-            groups.append(group)
-
-        new_group = []
-        for group, seq in zip(groups, ref_seqs):
-            new_group.append(("-".join(group), seq))
-        seqs_dict[pdb] = new_group
-
-    for pdb in pdbs_to_delete:
-        del seqs_dict[pdb]
-
-    return seqs_dict
-
-
-def _load_pdbs(dir, cdr=None):
-    """
-    Load biounits and group their sequences by PDB and similarity (90%)
-    """
-
-    seqs_dict = defaultdict(lambda: [])
-
-    for file in tqdm([x for x in os.listdir(dir) if x.endswith(".pickle")]):
-        load_path = os.path.join(dir, file)
-        if os.path.isdir(load_path):
-            continue
-        with open(load_path, "rb") as f:
-            pdb_dict = pkl.load(f)
-        if cdr is None:
-            seqs = [(chain, pdb_dict[chain]["seq"]) for chain in pdb_dict.keys()]
-        else:
-            seqs = [
-                (
-                    chain,
-                    "".join(
-                        np.array(list(pdb_dict[chain]["seq"]))[
-                            pdb_dict[chain]["cdr"] == cdr
-                        ].tolist()
-                    ),
-                )
-                for chain in pdb_dict.keys()
-            ]
-            seqs = [(chain, seq) for chain, seq in seqs if len(seq) > 0]
-        seqs_dict[file[:4]] += seqs
-
-    return seqs_dict
-
-
-def _write_fasta(fasta_path, merged_seqs_dict):
-    """
-    Write a fasta file containing all the sequences contained in the merged_seqs_dict dictionary
-    """
-
-    with open(fasta_path, "w") as f:
-        for k in merged_seqs_dict.keys():
-            for chain, seq in merged_seqs_dict[k]:
-                f.write(">" + k + "_" + chain + "\n")
-                f.write(seq + "\n")
+from proteinflow.sequences import (
+    _create_pdb_seqs_dict,
+    _load_pdbs,
+    _merge_chains,
+    _retrieve_seqs_names_list,
+    _write_fasta,
+)
+from proteinflow.utils.common_utils import _find_correspondences, _test_availability
 
 
 def _run_mmseqs2(fasta_file, tmp_folder, min_seq_id, cdr=None):
     """
     Run the MMSeqs2 command with the parameters we want
 
     Results are stored in the tmp_folder/MMSeqs2 directory.
@@ -168,15 +64,15 @@
         cluster_file_fasta = os.path.join(
             tmp_folder, "MMSeqs2_results", "clusterRes_all_seqs.fasta"
         )
     else:
         cluster_file_fasta = os.path.join(
             tmp_folder, "MMSeqs2_results", cdr, "clusterRes_all_seqs.fasta"
         )
-    with open(cluster_file_fasta, "r") as f:
+    with open(cluster_file_fasta) as f:
         cluster_dict = defaultdict(lambda: [])
         cluster_pdb_dict = defaultdict(lambda: [])
         cluster_name, sequence_name = None, None
         found_header = False
 
         for line in f.readlines():
             if line[0] == ">" and found_header:
@@ -204,15 +100,15 @@
     """
     Produces a graph that relates clusters together
 
     Connections represent a PDB shared by 2 clusters. The more shared PDBs, the stronger the connection.
     """
 
     keys = list(cluster_pdb_dict.keys())
-    keys_mapping = {l: k for l, k in enumerate(keys)}
+    keys_mapping = {length: k for length, k in enumerate(keys)}
     adjacency_matrix = np.zeros((len(keys), len(keys)))
 
     seen_dict = defaultdict(set)
     for i, key in enumerate(keys):
         for pdb in cluster_pdb_dict[key]:
             seen_dict[pdb].add(i)
     for cluster_set in seen_dict.values():
@@ -221,55 +117,14 @@
             adjacency_matrix[j, i] += 1
 
     graph = nx.from_numpy_matrix(adjacency_matrix)
     nx.relabel_nodes(graph, keys_mapping, copy=False)
     return graph
 
 
-def _retrieve_seqs_names_list(merged_seqs_dict):
-    """
-    Retrieve all the sequences names that are contained in the merged_seqs_dict (same names as in the fasta file in input to MMSeqs2)
-    """
-
-    seqs_names = []
-    for k in merged_seqs_dict.keys():
-        for chain, _ in merged_seqs_dict[k]:
-            seqs_names.append(k + "_" + chain)
-
-    return seqs_names
-
-
-def _create_pdb_seqs_dict(seqs_names_list):
-    """
-    Return a dictionary that has the PDB ids as keys and the list of all the chain names that correspond to this PDB
-    """
-
-    pdb_seqs_dict = defaultdict(lambda: [])
-    for name in seqs_names_list:
-        pdb_seqs_dict[name[:4]].append(name[5:])
-
-    return pdb_seqs_dict
-
-
-def _find_correspondances(files, dataset_dir):
-    """
-    Return a dictionary that contains all the biounits in the database (keys) and the list of all the chains that are in these biounits (values)
-    """
-
-    correspondances = defaultdict(lambda: [])
-    for file in files:
-        biounit = file
-        with open(os.path.join(dataset_dir, file), "rb") as f:
-            keys = pkl.load(f)
-            for k in keys:
-                correspondances[biounit].append(k)
-
-    return correspondances
-
-
 def _check_for_heteromers(grouped_seqs, biounit_chains):
     """
     True if the chain names contained in grouped_seqs correspond to at least 2 different sequences
     """
 
     grouped_seqs = [group.split("-") for group in grouped_seqs]
     chain_seqs = [
@@ -300,32 +155,32 @@
                 single_chains.append((file_name, seqs[0]))
 
         elif len(seqs) == 1 and len(file_names) == 1:
             for chain in seqs[0].split("-"):
                 homomers.append((file_names[0], chain))
 
         elif len(seqs) == 1:
-            correspondances = _find_correspondances(file_names, dataset_dir)
-            for biounit in correspondances.keys():
-                if len(correspondances[biounit]) == 1:
-                    single_chains.append((biounit, correspondances[biounit][0]))
+            correspondences = _find_correspondences(file_names, dataset_dir)
+            for biounit in correspondences.keys():
+                if len(correspondences[biounit]) == 1:
+                    single_chains.append((biounit, correspondences[biounit][0]))
                 else:
-                    for chain in correspondances[biounit]:
+                    for chain in correspondences[biounit]:
                         homomers.append((biounit, chain))
 
         else:
-            correspondances = _find_correspondances(file_names, dataset_dir)
-            for biounit in correspondances.keys():
-                if len(correspondances[biounit]) == 1:
-                    single_chains.append((biounit, correspondances[biounit][0]))
-                elif _check_for_heteromers(seqs, correspondances[biounit]):
-                    for chain in correspondances[biounit]:
+            correspondences = _find_correspondences(file_names, dataset_dir)
+            for biounit in correspondences.keys():
+                if len(correspondences[biounit]) == 1:
+                    single_chains.append((biounit, correspondences[biounit][0]))
+                elif _check_for_heteromers(seqs, correspondences[biounit]):
+                    for chain in correspondences[biounit]:
                         heteromers.append((biounit, chain))
                 else:
-                    for chain in correspondances[biounit]:
+                    for chain in correspondences[biounit]:
                         homomers.append((biounit, chain))
 
     return single_chains, homomers, heteromers
 
 
 def _find_chains_in_graph(
     graph, clusters_dict, biounit_chains_array, pdbs_array, chains_array
@@ -360,15 +215,15 @@
 
 
 def _find_repartition(chains_dict, homomers, heteromers):
     """
     Return a dictionary similar to the one created by find_chains_in_graph, with an additional level of classification for single chains, homomers and heteromers
 
     Dictionary structure : `{'single_chains' : {cluster_name : [biounit chains]}, 'homomers' : {cluster_name : [biounit chains]}, 'heteromers' : {cluster_name : [biounit chains]}}`.
-    Additionaly return the number of chains in each class (single chains, ...).
+    Additionally return the number of chains in each class (single chains, ...).
     """
 
     classes_dict = {
         "single_chains": defaultdict(lambda: []),
         "homomers": defaultdict(lambda: []),
         "heteromers": defaultdict(lambda: []),
     }
@@ -476,15 +331,15 @@
     chain_class,
     size_obj,
     current_sizes,
     size_array,
     tolerance=0.2,
 ):
     """
-    Remove values from indices untill we get the required (`size_obj`) number of chains in the class of interest (`chain_class`)
+    Remove values from indices until we get the required (`size_obj`) number of chains in the class of interest (`chain_class`)
 
     Parameter `chain_class` corresponds to the single chain (0), homomer (1) or heteromer (2) class.
     """
 
     sizes = [s[chain_class] for s in size_array[indices]]
     sorted_sizes_indices = np.argsort(sizes)[::-1]
 
@@ -534,15 +389,15 @@
     chain_class,
     size_obj,
     current_sizes,
     size_array,
     tolerance=0.2,
 ):
     """
-    Add values to indices untill we get the required (`size_obj`) number of chains in the class of interest (`chain_class`)
+    Add values to indices until we get the required (`size_obj`) number of chains in the class of interest (`chain_class`)
 
     Parameter `chain_class` corresponds to the single chain (0), homomer (1) or heteromer (2) class.
     """
 
     sizes = [s[chain_class] for s in size_array[remaining_indices]]
     sorted_sizes_indices = np.argsort(sizes)[::-1]
 
@@ -710,26 +565,14 @@
         single_chains_size,
         homomers_size,
         heteromers_size,
         remaining_indices,
     )
 
 
-def test_availability(
-    size_array,
-    n_samples,
-):
-    """
-    Test if there are enough groups in each class to construct a dataset with the required number of samples
-    """
-
-    present = np.sum(size_array != 0, axis=0)
-    return present[0] > n_samples, present[1] > n_samples, present[2] > n_samples
-
-
 def _fill_dataset(
     dict_list,
     size_array,
     n_samples,
     n_single_chains,
     n_homomers,
     n_heteromers,
@@ -742,15 +585,15 @@
 
     Given a list of indices to choose from (`remaining_indices`), choose a list of subgraphs to construct a dataset containing the required number of
     biounits for each class (single chains, ...) within a tolerance.
     Return the same outputs as the construct_dataset function, as long as the list of remaining indices after selection.
     """
 
     single_chains_size, homomers_size, heteromers_size = 0, 0, 0
-    sc_available, hm_available, ht_available = test_availability(
+    sc_available, hm_available, ht_available = _test_availability(
         size_array, n_samples
     )  # rule of thumb to estimate if it is logical to try to fill the dataset with a given class
     distribution_satisfied = False
     n_iter = 0
 
     while not distribution_satisfied and n_iter < n_max_iter:
         n_iter += 1
@@ -879,32 +722,32 @@
             1 - tolerance
         ) and test_sum <= num_clusters_test * (1 + tolerance)
         if valid_ok and test_ok:
             break
     return train_indices, valid_indices, test_indices
 
 
-def _split_dataset(
+def _split_dataset_with_graphs(
     graph,
     clusters_dict,
     merged_seqs_dict,
     dataset_dir,
     valid_split=0.05,
     test_split=0.05,
     tolerance=0.2,
 ):
     """
     Given a graph representing connections between MMSeqs2 clusters, split the dataset between train, validation and test sets.
     Each onnected component of the graph is considered as a group.
-    Then, groups are splitted into the 3 sets so that each set has the right amount of biounits.
+    Then, groups are split into the 3 sets so that each set has the right amount of biounits.
     It has been observed that the biggest group represents about 15-20 % of all the biounits and thus it is automatically assigned to the train set.
     It is difficult to have the exact ratio of biounits in each set since biounits are manipulated by groups.
     However, within an acceptable tolerance (default 20 % of the split ratio - but in theory it can be smaller), the split ratios are respected.
     The process first try to randomly assign the groups to a set.
-    If after 50 trials the partition fails to comply to the requirements, the last partition is kept and small adjustements are made by moving groups from sets one by one untill the ratios are approximately respected.
+    If after 50 trials the partition fails to comply to the requirements, the last partition is kept and small adjustments are made by moving groups from sets one by one until the ratios are approximately respected.
     Note that for very small datasets (around 250 biounits), this method will probably fail. But it also does not make much sense to use it for so few data.
 
     Parameters
     ----------
     graph : networkx graph
         the graph representing connections between MMSeqs2 clusters
     clusters_dict : dict
@@ -1131,16 +974,15 @@
     tmp_folder,
     valid_split=0.05,
     test_split=0.05,
     tolerance=0.2,
     min_seq_id=0.3,
     sabdab=False,
 ):
-    """
-    Build training, validation and test sets from a curated dataset of biounit, using MMSeqs2 for clustering
+    """Build training, validation and test sets from a curated dataset of biounit, using MMSeqs2 for clustering.
 
     Parameters
     ----------
     dataset_dir : str
         the path to the dataset
     valid_split : float in [0, 1], default 0.05
         the validation split ratio
@@ -1163,16 +1005,16 @@
         see train_clusters_dict but for validation set
     valid_classes_dict : dict
         see train_classes_dict but for validation set
     test_clusters_dict : dict
         see train_clusters_dict but for test set
     test_classes_dict : dict
         see train_classes_dict but for test set
-    """
 
+    """
     cdrs = ["L1", "L2", "L3", "H1", "H2", "H3"] if sabdab else [None]
     for cdr in cdrs:
         if cdr is not None:
             print(f"Clustering with MMSeqs2 for CDR {cdr}...")
         else:
             print("Clustering with MMSeqs2...")
         # retrieve all sequences and create a merged_seqs_dict
@@ -1218,15 +1060,15 @@
         train_clusters_dict,
         train_classes_dict,
         valid_clusters_dict,
         valid_classes_dict,
         test_clusters_dict,
         test_classes_dict,
         *_,
-    ) = _split_dataset(
+    ) = _split_dataset_with_graphs(
         graph,
         clusters_dict,
         merged_seqs_dict,
         dataset_dir,
         valid_split=valid_split,
         test_split=test_split,
         tolerance=tolerance,
```

### Comparing `proteinflow-1.3.6/proteinflow/utils/mmcif_fix.py` & `proteinflow-1.4.0/proteinflow/custom_mmcif.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-from biopandas.mmcif import PandasMmcif
 from copy import deepcopy
-import numpy as np
-import pandas as pd
+
+from biopandas.mmcif import PandasMmcif
 
 
 class CustomMmcif(PandasMmcif):
+    """
+    A modification of `PandasMmcif`
+
+    Adds a `get_model` method and renames the columns to match PDB format.
+    """
+
     def read_mmcif(self, path: str):
         x = super().read_mmcif(path)
         x.df["ATOM"].rename(
             {
                 "label_comp_id": "residue_name",
                 "label_seq_id": "residue_number",
                 "label_atom_id": "atom_name",
@@ -26,18 +31,20 @@
     def amino3to1(self):
         df = super().amino3to1()
         df.columns = ["chain_id", "residue_name"]
         return df
 
     def get_model(self, model_index: int):
         """Returns a new PandasPDB object with the dataframes subset to the given model index.
+
         Parameters
         ----------
         model_index : int
             An integer representing the model index to subset to.
+
         Returns
         ---------
         pandas_pdb.PandasPdb : A new PandasPdb object containing the
           structure subsetted to the given model.
         """
 
         df = deepcopy(self)
```

### Comparing `proteinflow-1.3.6/proteinflow.egg-info/PKG-INFO` & `proteinflow-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: proteinflow
-Version: 1.3.6
-Summary: Versatile pipeline for processing protein structure data for deep learning applications.
-Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
-License: BSD-3-Clause
-Keywords: bioinformatics,dataset,protein,PDB,deep learning
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
     <b> ProteinFlow - A data processing pipeline for all your protein design needs </b> <br />
 </p>
 
 <p align="center">
   <a href="https://adaptyvbio.github.io/ProteinFlow/" target="_blank">
       Docs
@@ -22,15 +11,15 @@
 ---
 
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/proteinflow)](https://pypi.org/project/proteinflow/)
 [![Conda](https://img.shields.io/conda/v/adaptyvbio/proteinflow)](https://anaconda.org/adaptyvbio/proteinflow)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/tags)
-![Generic badge](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)
+[![Generic badge](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](CONTRIBUTING.md)
 
 
 ProteinFlow is an open-source Python library that streamlines the pre-processing of protein structure data for deep learning applications. ProteinFlow enables users to efficiently filter, cluster, and generate new datasets from resources like the Protein Data Bank (PDB) and SAbDab (The Structural Antibody Database).
 
 Here are some of the key features we currently support:
 
 - ⛓️ Processing of both single-chain and multi-chain protein structures (Biounit PDB definition)
```

#### html2text {}

```diff
@@ -1,136 +1,130 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.3.6 Summary: Versatile
-pipeline for processing protein structure data for deep learning applications.
-Author-email: Liza Kozlova
-adaptyvbio.com>, Arthur Valentin
-adaptyvbio.com> License: BSD-3-Clause Keywords:
-bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
                                      Docs
 --- [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)]
 (https://opensource.org/licenses/BSD-3-Clause) [![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
 black) [![PyPI](https://img.shields.io/pypi/v/proteinflow)](https://pypi.org/
 project/proteinflow/) [![Conda](https://img.shields.io/conda/v/adaptyvbio/
 proteinflow)](https://anaconda.org/adaptyvbio/proteinflow) [![Docker Image
 Version (latest semver)](https://img.shields.io/docker/v/adaptyvbio/
 proteinflow?label=docker)](https://hub.docker.com/r/adaptyvbio/proteinflow/
-tags) ![Generic badge](https://img.shields.io/badge/Contributions-Welcome-
-brightgreen.svg) ProteinFlow is an open-source Python library that streamlines
-the pre-processing of protein structure data for deep learning applications.
-ProteinFlow enables users to efficiently filter, cluster, and generate new
-datasets from resources like the Protein Data Bank (PDB) and SAbDab (The
-Structural Antibody Database). Here are some of the key features we currently
-support: - âï¸ Processing of both single-chain and multi-chain protein
-structures (Biounit PDB definition) - ð·ï¸ Various featurization options can
-be computed, including secondary structure features, torsion angles, etc. -
-ð¾ A variety of data loading options and conversions to cater to different
-downstream training frameworks - ð§¬ Access to up-to-date, pre-computed
-protein structure datasets ![overview](https://raw.githubusercontent.com/
-adaptyvbio/ProteinFlow/main/media/pf-1.png) --- ## Installation conda: ```bash
-# This should take a few minutes, be patient conda install -c conda-forge -
-c bioconda -c adaptyvbio proteinflow ``` pip: ```bash pip install proteinflow
-``` docker: ```bash docker pull adaptyvbio/proteinflow ``` ### Troubleshooting
-- If you are using python 3.10 and encountering installation problems, try
-running `python -m pip install prody==2.4.0` before installing `proteinflow`. -
-If you are planning to generate new datasets and installed `proteinflow` with
-`pip`, you will need to additionally install [`mmseqs`](https://github.com/
-soedinglab/MMseqs2). - Generating new datasets also depends on the `rcsbsearch`
-package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/
-releases/tag/v0.2.3) is currently not working correctly. The recommended fix is
-installing the version from [this pull request](https://github.com/sbliven/
-rcsbsearch/pull/6). ```bash python -m pip install "rcsbsearch @ git+https://
-github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` -
-The docker image can be accessed in interactive mode with this command. ```bash
-docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage
-### Downloading pre-computed datasets (stable) Already precomputed datasets
-with consensus set of parameters and can be accessed and downloaded using the
-`proteinflow`. package. Check the output of `proteinflow check_tags` for a list
-of available tags. ```bash proteinflow download --tag 20230102_stable ``` ###
-Running the pipeline (PDB) You can also run `proteinflow` with your own
-parameters. Check the output of `proteinflow check_snapshots` for a list of
-available PDB snapshots (naming rule: `yyyymmdd`). For instance, let's generate
-a dataset with the following description: - resolution threshold: 5 angstrom, -
-PDB snapshot: 20190101, - structure methods accepted: all (x-ray
-christolography, NRM, Cryo-EM), - sequence identity threshold for clustering:
-40% sequence similarity, - maximum length per sequence: 1000 residues, -
-minimum length per sequence: 5 residues, - maximum fraction of missing values
-at the ends: 10%, - size of validation subset: 10%. ```bash proteinflow
-generate --tag new --resolution_thr 5 --pdb_snapshot 20190101 --
-not_filter_methods --min_seq_id 0.4 --max_length 1000 --min_length 5 --
-missing_ends_thr 0.1 --valid_split 0.1 ``` See the [docs](https://
-adaptyvbio.github.io/ProteinFlow/) (or `proteinflow generate --help`) for the
-full list of parameters and more information. A registry of all the files that
-are removed during the filtering as well as description with the reason for
-their removal is created automatically for each `generate` command. The log
-files are save (at `data/logs` by default) and a summary can be accessed
-running `proteinflow get_summary {log_path}`. ### Running the pipeline (SAbDab)
-You can also use the `--sabdab` option in `proteinflow generate` to load files
-from SAbDab and cluster them based on CDRs. By default the `--sabdab` tag will
-download the latest up-to-date version of the SabDab dataset and cluster the
-antibodies based on their CDR sequence. Alternatively, it can be used together
-with the tag `--sabdab_data_path` to process a custom SAbDab-like zip file or
-folder. This allows you to use search and query tools from the [SabDab web
-interface](https://opig.stats.ox.ac.uk/webapps/newsabdab/sabdab/) to create a
-custom dataset by downloading the archived zip file of the structures selected.
-(Under Downloads section of your SabDab query). SAbDab sequences clustering is
-done across all 6 Complementary Determining Regions (CDRs) - H1, H2, H3, L1,
-L2, L3, based on the [Chothia numbering](https://pubmed.ncbi.nlm.nih.gov/
-9367782/) implemented by SabDab. CDRs from nanobodies and other synthetic
-constructs are clustered together with other heavy chain CDRs. The resulting
-CDR clusters are split into training, test and validation in a way that ensures
-that every PDB file only appears in one subset. Individual output pickle files
-represent heavy chain - light chain - antigen complexes (created from SAbDab
-annotation, sometimes more than one per PDB entry). Each of the elements (heavy
-chain, light chain, antigen) can be missing in specific entries and there can
-be multiple antigen chains. In order to filter for at least one antigen chain,
-use the `--require_antigen` option. For instance, let's generate a dataset with
-the following description: - SabDab version: latest (up-to-date), - resolution
-threshold: 5 angstrom, - structure methods accepted: all (x-ray
-christolography, NRM, Cryo-EM), - sequence identity threshold for clustering
-(CDRs): 40%, - size of validation subset: 10%. ```bash proteinflow generate --
-sabdab --resolution_thr 5 --not_filter_methods --min_seq_id 0.4 --valid_split
-0.1 ``` ### Splitting By default, both `proteinflow generate` and `proteinflow
-download` will also split your data into training, test and validation
-according to MMseqs2 clustering and homomer/heteromer/single chain proportions.
-However, you can skip this step with a `--skip_splitting` flag and then perform
-it separately with the `proteinflow split` command. The following command will
-perform the splitting with a 10% validation set, a 5% test set and a 50%
-threshold for sequence identity clusters. ```bash proteinflow split --tag new -
--valid_split 0.1 --test_split 0.5 --min_seq_id 0.5 ``` Use the `--
-exclude_chains` and `--exclude_threshold` parameters to move all biounits that
-contain chains similar to what you specify to a separate folder. ### Using the
-data The output files are pickled nested dictionaries where first-level keys
-are chain Ids and second-level keys are the following: - `'crd_bb'`: a `numpy`
-array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O), -
-`'crd_sc'`: a `numpy` array of shape `(L, 10, 3)` with sidechain atom
-coordinates (check `proteinflow.sidechain_order()` for the order of atoms), -
-`'msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues with
-known coordinates and zeros to missing values, - `'seq'`: a string of length
-`L` with residue types. In a SAbDab datasets, an additional key is added to the
-dictionary: - `'cdr'`: a `numpy` array of shape `(L,)` where CDR residues are
-marked with the corresponding type (`'H1'`, `'L1'`, ...) and non-CDR residues
-are marked with `'-'`. Note that the sequence information in the PDB files is
-aligned to the FASTA sequences to identify the missing residues. Once your data
-is ready, you can open the files with `pickle` directly. ```python import
-pickle import os train_folder = "./data/proteinflow_new/training" for filename
-in os.listdir(train_folder): with open(os.path.join(train_folder, filename),
-"rb") as f: data = pickle.load(f) crd_bb = data["crd_bb"] seq = data["seq"] ...
-``` Alternatively, you can use our `ProteinDataset` or `ProteinLoader` classes
-for convenient processing. Among other things, they allow for feature
-extraction, single chain / homomer / heteromer filtering and randomized
-sampling from sequence identity clusters. For example, here is how we can
-create a data loader that: - samples a different cluster representative at
-every epoch, - extracts dihedral angles, sidechain orientation and secondary
-structure features, - only loads pairs of interacting proteins (larger biounits
-are broken up into pairs), - has batch size 8. ```python from proteinflow
-import ProteinLoader train_loader = ProteinLoader.from_args( "./data/
-proteinflow_new/training", clustering_dict_path="./data/proteinflow_new/
-splits_dict/train.pickle",
+tags) [![Generic badge](https://img.shields.io/badge/Contributions-Welcome-
+brightgreen.svg)](CONTRIBUTING.md) ProteinFlow is an open-source Python library
+that streamlines the pre-processing of protein structure data for deep learning
+applications. ProteinFlow enables users to efficiently filter, cluster, and
+generate new datasets from resources like the Protein Data Bank (PDB) and
+SAbDab (The Structural Antibody Database). Here are some of the key features we
+currently support: - âï¸ Processing of both single-chain and multi-chain
+protein structures (Biounit PDB definition) - ð·ï¸ Various featurization
+options can be computed, including secondary structure features, torsion
+angles, etc. - ð¾ A variety of data loading options and conversions to cater
+to different downstream training frameworks - ð§¬ Access to up-to-date, pre-
+computed protein structure datasets ![overview](https://
+raw.githubusercontent.com/adaptyvbio/ProteinFlow/main/media/pf-1.png) --- ##
+Installation conda: ```bash # This should take a few minutes, be patient conda
+install -c conda-forge -c bioconda -c adaptyvbio proteinflow ``` pip: ```bash
+pip install proteinflow ``` docker: ```bash docker pull adaptyvbio/proteinflow
+``` ### Troubleshooting - If you are using python 3.10 and encountering
+installation problems, try running `python -m pip install prody==2.4.0` before
+installing `proteinflow`. - If you are planning to generate new datasets and
+installed `proteinflow` with `pip`, you will need to additionally install
+[`mmseqs`](https://github.com/soedinglab/MMseqs2). - Generating new datasets
+also depends on the `rcsbsearch` package and the latest release [v0.2.3](https:
+//github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working
+correctly. The recommended fix is installing the version from [this pull
+request](https://github.com/sbliven/rcsbsearch/pull/6). ```bash python -m pip
+install "rcsbsearch @ git+https://github.com/sbliven/
+rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` - The docker image can
+be accessed in interactive mode with this command. ```bash docker run -it -v /
+path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage ### Downloading
+pre-computed datasets (stable) Already precomputed datasets with consensus set
+of parameters and can be accessed and downloaded using the `proteinflow`.
+package. Check the output of `proteinflow check_tags` for a list of available
+tags. ```bash proteinflow download --tag 20230102_stable ``` ### Running the
+pipeline (PDB) You can also run `proteinflow` with your own parameters. Check
+the output of `proteinflow check_snapshots` for a list of available PDB
+snapshots (naming rule: `yyyymmdd`). For instance, let's generate a dataset
+with the following description: - resolution threshold: 5 angstrom, - PDB
+snapshot: 20190101, - structure methods accepted: all (x-ray christolography,
+NRM, Cryo-EM), - sequence identity threshold for clustering: 40% sequence
+similarity, - maximum length per sequence: 1000 residues, - minimum length per
+sequence: 5 residues, - maximum fraction of missing values at the ends: 10%, -
+size of validation subset: 10%. ```bash proteinflow generate --tag new --
+resolution_thr 5 --pdb_snapshot 20190101 --not_filter_methods --min_seq_id 0.4
+--max_length 1000 --min_length 5 --missing_ends_thr 0.1 --valid_split 0.1 ```
+See the [docs](https://adaptyvbio.github.io/ProteinFlow/) (or `proteinflow
+generate --help`) for the full list of parameters and more information. A
+registry of all the files that are removed during the filtering as well as
+description with the reason for their removal is created automatically for each
+`generate` command. The log files are save (at `data/logs` by default) and a
+summary can be accessed running `proteinflow get_summary {log_path}`. ###
+Running the pipeline (SAbDab) You can also use the `--sabdab` option in
+`proteinflow generate` to load files from SAbDab and cluster them based on
+CDRs. By default the `--sabdab` tag will download the latest up-to-date version
+of the SabDab dataset and cluster the antibodies based on their CDR sequence.
+Alternatively, it can be used together with the tag `--sabdab_data_path` to
+process a custom SAbDab-like zip file or folder. This allows you to use search
+and query tools from the [SabDab web interface](https://opig.stats.ox.ac.uk/
+webapps/newsabdab/sabdab/) to create a custom dataset by downloading the
+archived zip file of the structures selected. (Under Downloads section of your
+SabDab query). SAbDab sequences clustering is done across all 6 Complementary
+Determining Regions (CDRs) - H1, H2, H3, L1, L2, L3, based on the [Chothia
+numbering](https://pubmed.ncbi.nlm.nih.gov/9367782/) implemented by SabDab.
+CDRs from nanobodies and other synthetic constructs are clustered together with
+other heavy chain CDRs. The resulting CDR clusters are split into training,
+test and validation in a way that ensures that every PDB file only appears in
+one subset. Individual output pickle files represent heavy chain - light chain
+- antigen complexes (created from SAbDab annotation, sometimes more than one
+per PDB entry). Each of the elements (heavy chain, light chain, antigen) can be
+missing in specific entries and there can be multiple antigen chains. In order
+to filter for at least one antigen chain, use the `--require_antigen` option.
+For instance, let's generate a dataset with the following description: - SabDab
+version: latest (up-to-date), - resolution threshold: 5 angstrom, - structure
+methods accepted: all (x-ray christolography, NRM, Cryo-EM), - sequence
+identity threshold for clustering (CDRs): 40%, - size of validation subset:
+10%. ```bash proteinflow generate --sabdab --resolution_thr 5 --
+not_filter_methods --min_seq_id 0.4 --valid_split 0.1 ``` ### Splitting By
+default, both `proteinflow generate` and `proteinflow download` will also split
+your data into training, test and validation according to MMseqs2 clustering
+and homomer/heteromer/single chain proportions. However, you can skip this step
+with a `--skip_splitting` flag and then perform it separately with the
+`proteinflow split` command. The following command will perform the splitting
+with a 10% validation set, a 5% test set and a 50% threshold for sequence
+identity clusters. ```bash proteinflow split --tag new --valid_split 0.1 --
+test_split 0.5 --min_seq_id 0.5 ``` Use the `--exclude_chains` and `--
+exclude_threshold` parameters to move all biounits that contain chains similar
+to what you specify to a separate folder. ### Using the data The output files
+are pickled nested dictionaries where first-level keys are chain Ids and
+second-level keys are the following: - `'crd_bb'`: a `numpy` array of shape `
+(L, 4, 3)` with backbone atom coordinates (N, C, CA, O), - `'crd_sc'`: a
+`numpy` array of shape `(L, 10, 3)` with sidechain atom coordinates (check
+`proteinflow.sidechain_order()` for the order of atoms), - `'msk'`: a `numpy`
+array of shape `(L,)` where ones correspond to residues with known coordinates
+and zeros to missing values, - `'seq'`: a string of length `L` with residue
+types. In a SAbDab datasets, an additional key is added to the dictionary: -
+`'cdr'`: a `numpy` array of shape `(L,)` where CDR residues are marked with the
+corresponding type (`'H1'`, `'L1'`, ...) and non-CDR residues are marked with
+`'-'`. Note that the sequence information in the PDB files is aligned to the
+FASTA sequences to identify the missing residues. Once your data is ready, you
+can open the files with `pickle` directly. ```python import pickle import os
+train_folder = "./data/proteinflow_new/training" for filename in os.listdir
+(train_folder): with open(os.path.join(train_folder, filename), "rb") as f:
+data = pickle.load(f) crd_bb = data["crd_bb"] seq = data["seq"] ... ```
+Alternatively, you can use our `ProteinDataset` or `ProteinLoader` classes for
+convenient processing. Among other things, they allow for feature extraction,
+single chain / homomer / heteromer filtering and randomized sampling from
+sequence identity clusters. For example, here is how we can create a data
+loader that: - samples a different cluster representative at every epoch, -
+extracts dihedral angles, sidechain orientation and secondary structure
+features, - only loads pairs of interacting proteins (larger biounits are
+broken up into pairs), - has batch size 8. ```python from proteinflow import
+ProteinLoader train_loader = ProteinLoader.from_args( "./data/proteinflow_new/
+training", clustering_dict_path="./data/proteinflow_new/splits_dict/
+train.pickle",
 node_features_type="dihedral+sidechain_orientation+secondary_structure",
 entry_type="pair", batch_size=8, ) for batch in train_loader: crd_bb = batch
 ["X"] #(B, L, 4, 3) seq = batch["S"] #(B, L) sse = batch["secondary_structure"]
 #(B, L, 3) to_predict = batch["masked_res"] #(B, L), 1 where the residues
 should be masked, 0 otherwise ... ``` See more details on available parameters
 and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) +
 [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use
```

### Comparing `proteinflow-1.3.6/proteinflow.egg-info/SOURCES.txt` & `proteinflow-1.4.0/proteinflow.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 LICENSE
 README.md
 pyproject.toml
+setup.cfg
 proteinflow/__init__.py
+proteinflow/constants.py
+proteinflow/custom_mmcif.py
+proteinflow/pdb.py
+proteinflow/protein_dataset.py
+proteinflow/protein_loader.py
+proteinflow/sequences.py
 proteinflow.egg-info/PKG-INFO
 proteinflow.egg-info/SOURCES.txt
 proteinflow.egg-info/dependency_links.txt
 proteinflow.egg-info/entry_points.txt
 proteinflow.egg-info/requires.txt
 proteinflow.egg-info/top_level.txt
 proteinflow/scripts/__init__.py
 proteinflow/scripts/proteinflow_cli.py
 proteinflow/utils/__init__.py
-proteinflow/utils/async_download.py
 proteinflow/utils/biotite_sse.py
-proteinflow/utils/build_pdb.py
+proteinflow/utils/boto_utils.py
 proteinflow/utils/cluster_and_partition.py
-proteinflow/utils/filter_database.py
-proteinflow/utils/mmcif_fix.py
-proteinflow/utils/process_pdb.py
-proteinflow/utils/split_dataset.py
+proteinflow/utils/common_utils.py
 tests/test_download.py
 tests/test_generate.py
 tests/test_sabdab.py
```

### Comparing `proteinflow-1.3.6/pyproject.toml` & `proteinflow-1.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proteinflow"
-version = "1.3.6"
+version = "1.4.0"
 authors = [
     {name = "Liza Kozlova", email = "liza@adaptyvbio.com"},
     {name = "Arthur Valentin", email = "arthur@adaptyvbio.com"}
 ]
 description = "Versatile pipeline for processing protein structure data for deep learning applications."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -26,15 +26,21 @@
     "pandas>=1.5.2",
     "torch>=1.10.0",
     "biotite==0.35.0",
     "aiobotocore==2.4.2",
     "awscli==1.25.60",
     "bs4>=0.0.1",
     "rcsbsearch",
+    "pre-commit",
 ]
 keywords = ["bioinformatics", "dataset", "protein", "PDB", "deep learning"]
 
 [project.scripts]
 proteinflow = "proteinflow.scripts.proteinflow_cli:cli"
 
 [tool.setuptools.packages]
 find = {}
+
+[tool.pydocstyle]
+convention = "numpy"
+match_dir = 'proteinflow'
+match = '__init__.py'
```

### Comparing `proteinflow-1.3.6/tests/test_download.py` & `proteinflow-1.4.0/tests/test_download.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,38 @@
-import subprocess
+import os
 import shutil
+import subprocess
+
+import pytest
+
 from proteinflow import ProteinLoader
-import os
 
 
-def test_download():
+@pytest.mark.parametrize("tag", ["test", "test_old"])
+def test_download(tag):
     """Test download_data + split_data + ProteinLoader"""
 
-    folder = "./data/proteinflow_test"
+    folder = f"./data/proteinflow_{tag}"
     if os.path.exists(folder):
         shutil.rmtree(folder)
     subprocess.run(
-        ["proteinflow", "download", "--tag", "test", "--skip_splitting"], check=True
+        ["proteinflow", "download", "--tag", tag, "--skip_splitting"], check=True
     )
-    subprocess.run(["proteinflow", "split", "--tag", "test"], check=True)
+    subprocess.run(["proteinflow", "split", "--tag", tag], check=True)
     for cluster_dict_path, entry_type, classes_to_exclude in [
         (os.path.join(folder, "splits_dict/valid.pickle"), "chain", ["homomers"]),
         (None, "pair", None),
     ]:
         valid_loader = ProteinLoader.from_args(
             dataset_folder=os.path.join(folder, "valid"),
             batch_size=8,
             node_features_type="chemical+sidechain_orientation+dihedral+secondary_structure+sidechain_coords",
             rewrite=True,
             clustering_dict_path=cluster_dict_path,
+            classes_dict_path=os.path.join(folder, "splits_dict", "classes.pickle"),
             entry_type=entry_type,
             classes_to_exclude=classes_to_exclude,
             max_length=1000,
         )
         batch = next(iter(valid_loader))
         assert set(batch.keys()) == {
             "X",
@@ -53,8 +58,8 @@
         assert batch["sidechain_coords"].shape == (8, batch["X"].shape[1], 10, 3)
         assert batch["X"].shape[1] <= 1000
 
     shutil.rmtree(folder)
 
 
 if __name__ == "__main__":
-    test_download()
+    test_download("test_old")
```

### Comparing `proteinflow-1.3.6/tests/test_generate.py` & `proteinflow-1.4.0/tests/test_generate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from proteinflow import generate_data, split_data
 import os
 import pickle
-from collections import defaultdict
-import editdistance
 import shutil
+from collections import defaultdict
 from time import time
-import pytest
+
+import editdistance
+
+from proteinflow import generate_data, split_data
 
 
 def get_class(seqs_dict):
     """Check if the protein is a homomer, a heteromer or a single chain"""
 
     keys = list(seqs_dict.keys())
     if len(keys) == 1:
@@ -34,37 +35,45 @@
     folder = "./data/proteinflow_test"
     if os.path.exists(folder):
         shutil.rmtree(folder)
     start = time()
     generate_data(tag="test", skip_splitting=True, n=50)
     end = time()
     num_files = len(os.listdir(folder))
-    split_data(tag="test", valid_split=0.2, test_split=0.1, ignore_existing=True)
+    split_data(
+        tag="test",
+        valid_split=0.2,
+        test_split=0.1,
+        ignore_existing=True,
+        exclude_chains=["1arx-A"],
+    )
     assert os.path.exists(folder)
-    assert len(os.listdir(folder)) == 5
+    assert len(os.listdir(folder)) == 6
     num_files_split = 0
 
-    for subset in ["train", "valid", "test"]:
+    with open(
+        os.path.join(folder, "splits_dict", "classes.pickle"),
+        "rb",
+    ) as f:
+        class_data = pickle.load(f)
+    classes = defaultdict(int)
+    for subset in ["train", "valid", "test", "excluded"]:
         num_files_split += len(os.listdir(os.path.join(folder, subset)))
         subset_folder = os.path.join(folder, subset)
-        with open(os.path.join(folder, "splits_dict", f"{subset}.pickle"), "rb") as f:
-            for _ in range(2):
-                class_data = pickle.load(f)
-        classes = defaultdict(int)
         for file in os.listdir(subset_folder):
             with open(os.path.join(subset_folder, file), "rb") as f:
                 data = pickle.load(f)
             c = get_class(data)
             classes[c] += 1
-        for c in class_data:
-            class_files = set()
-            for chain_arr in class_data[c].values():
-                for file, _ in chain_arr:
-                    class_files.add(file)
-            assert classes[c] == len(class_files)
+    for c in class_data:
+        class_files = set()
+        for chain_arr in class_data[c].values():
+            for file, _ in chain_arr:
+                class_files.add(file)
+        assert classes[c] == len(class_files)
     assert num_files == num_files_split + 1
     shutil.rmtree(folder)
     print(f"generation time: {end - start} sec")
 
 
 if __name__ == "__main__":
     test_generate()
```

### Comparing `proteinflow-1.3.6/tests/test_sabdab.py` & `proteinflow-1.4.0/tests/test_sabdab.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-from proteinflow import generate_data, split_data
 import os
-import pickle
-from collections import defaultdict
-import editdistance
 import shutil
 from time import time
-import pytest
-from proteinflow import ProteinLoader
+
+from proteinflow import ProteinLoader, generate_data
 
 
 # @pytest.mark.skip()
 def test_generate_sabdab():
     """Test generate_data with `sabdab=True`"""
 
     folder = "./data/proteinflow_test"
```

