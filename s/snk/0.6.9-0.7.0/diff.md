# Comparing `tmp/snk-0.6.9.tar.gz` & `tmp/snk-0.7.0.tar.gz`

## Comparing `snk-0.6.9.tar` & `snk-0.7.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.9/Dockerfile
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 snk-0.6.9/mkdocs.yml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.9/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.9/.github/workflows/publish.yml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.9/.github/workflows/tests.yml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.9/docs/CNAME
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 snk-0.6.9/docs/index.md
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 snk-0.6.9/docs/managing_pipelines.md
--rw-r--r--   0        0        0     8963 2020-02-02 00:00:00.000000 snk-0.6.9/docs/pipeline_packages.md
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 snk-0.6.9/docs/reference/cli.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.9/docs/reference/errors.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.9/docs/reference/main.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.9/docs/reference/nest.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 snk-0.6.9/docs/reference/pipeline.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.9/snk/__about__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.6.9/snk/__init__.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.6.9/snk/errors.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 snk-0.6.9/snk/main.py
--rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 snk-0.6.9/snk/nest.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 snk-0.6.9/snk/pipeline.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.6.9/snk/cli/__init__.py
--rw-r--r--   0        0        0    19654 2020-02-02 00:00:00.000000 snk-0.6.9/snk/cli/cli.py
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 snk-0.6.9/snk/cli/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.9/snk/cli/options.py
--rw-r--r--   0        0        0     8933 2020-02-02 00:00:00.000000 snk-0.6.9/snk/cli/utils.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.9/tests/.DS_Store
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.9/tests/__init__.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 snk-0.6.9/tests/conftest.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.9/tests/test_nest.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 snk-0.6.9/tests/test_pipline_cli.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.6.9/tests/test_snk.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.9/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/cov.fasta
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/bin/snk-basic-pipeline
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/pipeline/.snk
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/pipeline/cli.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/pipeline/config.yaml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/pipeline/resources/data.txt
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/pipeline/workflow/Snakefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/pipeline/workflow/envs/base.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.9/tests/data/pipeline/workflow/profiles/base/config.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snk-0.6.9/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.9/LICENSE.txt
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 snk-0.6.9/README.md
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 snk-0.6.9/pyproject.toml
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 snk-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.7.0/Dockerfile
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 snk-0.7.0/mkdocs.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.7.0/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.7.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 snk-0.7.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.7.0/docs/CNAME
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 snk-0.7.0/docs/index.md
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 snk-0.7.0/docs/managing_pipelines.md
+-rw-r--r--   0        0        0     8963 2020-02-02 00:00:00.000000 snk-0.7.0/docs/pipeline_packages.md
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 snk-0.7.0/docs/reference/cli.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.7.0/docs/reference/errors.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.7.0/docs/reference/main.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.7.0/docs/reference/nest.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 snk-0.7.0/docs/reference/pipeline.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.7.0/snk/__about__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.7.0/snk/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.7.0/snk/errors.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 snk-0.7.0/snk/main.py
+-rw-r--r--   0        0        0    16501 2020-02-02 00:00:00.000000 snk-0.7.0/snk/nest.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 snk-0.7.0/snk/pipeline.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.7.0/snk/cli/__init__.py
+-rw-r--r--   0        0        0    20027 2020-02-02 00:00:00.000000 snk-0.7.0/snk/cli/cli.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 snk-0.7.0/snk/cli/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.7.0/snk/cli/options.py
+-rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 snk-0.7.0/snk/cli/utils.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.7.0/tests/.DS_Store
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 snk-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 snk-0.7.0/tests/test_nest.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 snk-0.7.0/tests/test_pipline_cli.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.7.0/tests/test_snk.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.7.0/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/cov.fasta
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/bin/snk-basic-pipeline
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/pipeline/.snk
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/pipeline/cli.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/pipeline/config.yaml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/pipeline/resources/data.txt
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/pipeline/workflow/Snakefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/pipeline/workflow/envs/base.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/pipeline/workflow/profiles/base/config.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snk-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 snk-0.7.0/README.md
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 snk-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 snk-0.7.0/PKG-INFO
```

### Comparing `snk-0.6.9/mkdocs.yml` & `snk-0.7.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.9/.github/workflows/publish.yml` & `snk-0.7.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.9/.github/workflows/tests.yml` & `snk-0.7.0/.github/workflows/tests.yml`

 * *Files 18% similar despite different names*

```diff
@@ -16,12 +16,13 @@
         with:
           python-version: 3.x
       - uses: actions/cache@v2
         with:
           key: ${{ github.ref }}
           path: .cache
       - run: pip install hatch
+      - run: sudo apt-get -y install graphviz
       - run: hatch run cov
       - name: Upload coverage reports to Codecov
         uses: codecov/codecov-action@v3
```

### Comparing `snk-0.6.9/docs/index.md` & `snk-0.7.0/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 **Documentation**: <a href="https://snk.wytamma.com" target="_blank">https://snk.wytamma.com</a>
 
 **Source Code**: <a href="https://github.com/Wytamma/snk" target="_blank">https://github.com/Wytamma/snk</a>
 
 ---
 
-Snk (pronounced snek) is a SNaKemake pipeline management system. Snk allows you to install Snakemake pipelines as Command Line Interfaces (CLIs). Using a pipeline as a CLI increases its interoperability and allows complex pipelines to be used as modular components in a larger system. Snk, using python magic, will dynamic genrate the pipeline CLI using the pipeline configuration file.
+Snk (pronounced snek) is a SNaKemake pipeline management system. Snk allows you to install Snakemake pipelines as dynamically generated Command Line Interfaces (CLIs). Using a pipeline as a CLI increases its interoperability and allows complex pipelines to be used as modular components in a larger system.
 
 ## Installation
 
 ```console
 pip install snk
 ```
```

#### html2text {}

```diff
@@ -5,31 +5,30 @@
 raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)]
 (https://write-the.wytamma.com/) [![Hits](https://hits.seeyoufarm.com/api/
 count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FWytamma%2Fsnk&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)]
 (https://github.com/Wytamma/snk) --- **Documentation**: https://snk.wytamma.com
 **Source Code**: https://github.com/Wytamma/snk --- Snk (pronounced snek) is a
 SNaKemake pipeline management system. Snk allows you to install Snakemake
-pipelines as Command Line Interfaces (CLIs). Using a pipeline as a CLI
-increases its interoperability and allows complex pipelines to be used as
-modular components in a larger system. Snk, using python magic, will dynamic
-genrate the pipeline CLI using the pipeline configuration file. ## Installation
-```console pip install snk ``` ## Basic Use ### Install a pipeline as a CLI
-Install the dna-seq-gatk-variant-calling pipeline (v2.1.1) as `variant-
-calling`. ``` snk install snakemake-workflows/dna-seq-gatk-variant-calling --
-name variant-calling -t v2.1.1 ``` Successfully installed variant-calling
-(v2.1.1)! ### Inspect the CLI ``` variant-calling --help ``` [main cli] ###
-View run options ``` variant-calling run -h ``` [run cli] ### Create a DAG Here
-we use the `.test` resources included in the pipeline to create the DAG. ```
-variant-calling run -r .test/config -r .test/data --dag dag.pdf ``` [dag] ###
-Configure Snk will dynamically generate config options for the CLI. For example
-if your config.yaml file has the option `fasta: null` you can set this option
-with `--fasta`. ``` variant-calling run --fasta example.fa ``` You can also
-configure the pipeline using a config file. ``` variant-calling config --pretty
-# print the config variant-calling config > config.yml # save the config
-variant-calling run --config config.yml # run with config ``` ## how it works
-When installing a pipeline snk will - create directory `$PYTHON_BIN_DIR/../snk/
-pipelines/PIPELINE` - install the pipeline into this directory - expose CLI at
-`$PYTHON_BIN_DIR` that point to pipeline directory in `snk/pipelines/PIPELINE/
-bin` - As long as `$PYTHON_BIN_DIR` is on your PATH, you can now invoke the
-pipeline globally ## License `snk` is distributed under the terms of the [MIT]
-(https://spdx.org/licenses/MIT.html) license.
+pipelines as dynamically generated Command Line Interfaces (CLIs). Using a
+pipeline as a CLI increases its interoperability and allows complex pipelines
+to be used as modular components in a larger system. ## Installation ```console
+pip install snk ``` ## Basic Use ### Install a pipeline as a CLI Install the
+dna-seq-gatk-variant-calling pipeline (v2.1.1) as `variant-calling`. ``` snk
+install snakemake-workflows/dna-seq-gatk-variant-calling --name variant-calling
+-t v2.1.1 ``` Successfully installed variant-calling (v2.1.1)! ### Inspect the
+CLI ``` variant-calling --help ``` [main cli] ### View run options ``` variant-
+calling run -h ``` [run cli] ### Create a DAG Here we use the `.test` resources
+included in the pipeline to create the DAG. ``` variant-calling run -r .test/
+config -r .test/data --dag dag.pdf ``` [dag] ### Configure Snk will dynamically
+generate config options for the CLI. For example if your config.yaml file has
+the option `fasta: null` you can set this option with `--fasta`. ``` variant-
+calling run --fasta example.fa ``` You can also configure the pipeline using a
+config file. ``` variant-calling config --pretty # print the config variant-
+calling config > config.yml # save the config variant-calling run --config
+config.yml # run with config ``` ## how it works When installing a pipeline snk
+will - create directory `$PYTHON_BIN_DIR/../snk/pipelines/PIPELINE` - install
+the pipeline into this directory - expose CLI at `$PYTHON_BIN_DIR` that point
+to pipeline directory in `snk/pipelines/PIPELINE/bin` - As long as
+`$PYTHON_BIN_DIR` is on your PATH, you can now invoke the pipeline globally ##
+License `snk` is distributed under the terms of the [MIT](https://spdx.org/
+licenses/MIT.html) license.
```

### Comparing `snk-0.6.9/docs/managing_pipelines.md` & `snk-0.7.0/docs/managing_pipelines.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.9/docs/pipeline_packages.md` & `snk-0.7.0/docs/pipeline_packages.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.9/snk/main.py` & `snk-0.7.0/snk/main.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.9/snk/nest.py` & `snk-0.7.0/snk/nest.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,36 +140,50 @@
             pipeline_path = self.local(pipeline_local_path, name, editable)
         try:
             pipeline_executable = self.create_package(pipeline_path)
             self.link_pipeline_executable_to_bin(pipeline_executable)
             if config:
                 self.copy_nonstandard_config(pipeline_path, config)
             if additional_resources:
-                self.additional_resources(pipeline_path, additional_resources)
+                self.additional_resources(pipeline_path, additional_resources)            
             self._confirm_installation(name)
         except Exception as e:
             # remove any half completed steps
             to_remove = self.get_paths_to_delete(name)
             self.delete_paths(to_remove)
             raise e
         return Pipeline(pipeline_path)
 
-    def additional_resources(self, pipeline_dir: Path, resources: List[Path]):
+    def modify_snk_config(self, pipeline_path: Path, **kwargs):
+        """
+        Modify the .snk file.
+        Args:
+          pipeline_path (Path): The path to the pipeline directory.
+          name (str): The name of the pipeline.
+        Examples:
+          >>> nest.modify_snk_config(Path('/path/to/pipeline'), 'example')
+        """
+        snk_config = SnkConfig.from_path(pipeline_path / ".snk")
+        for key, value in kwargs.items():
+            setattr(snk_config, key, value)
+        snk_config.to_yaml(pipeline_path / ".snk")
+    
+    def additional_resources(self, pipeline_path: Path, resources: List[Path]):
         """
         Modify the .snk file so that resources will be copied at runtime.
         Args:
-          pipeline_dir (Path): The path to the pipeline directory.
+          pipeline_path (Path): The path to the pipeline directory.
           resources (List[Path]): A list of additional resources to copy.
         Examples:
           >>> nest.additional_resources(Path('/path/to/pipeline'), [Path('/path/to/resource1'), Path('/path/to/resource2')])
         """
         # validate_resources(resources)
-        snk_config = SnkConfig.from_path(pipeline_dir / ".snk")
-        snk_config.add_resources(resources, pipeline_dir)
-        snk_config.to_yaml(pipeline_dir / ".snk")
+        snk_config = SnkConfig.from_path(pipeline_path / ".snk")
+        snk_config.add_resources(resources, pipeline_path)
+        snk_config.to_yaml(pipeline_path / ".snk")
 
     def copy_nonstandard_config(self, pipeline_dir: Path, config_path: Path):
         """
         Copy a nonstandard config file to the pipeline directory.
         Args:
           pipeline_dir (Path): The path to the pipeline directory.
           config_path (Path): The path to the config file.
@@ -348,25 +362,14 @@
         try:
             Repo(location)
         except InvalidGitRepositoryError:
             Repo.init(location, mkdir=False)
         return location
 
     def create_package(self, pipeline_dir: Path) -> Path:
-        """
-        Creates a package in the local environment.
-        Args:
-          package_name (str): The name of the package to create.
-        Returns:
-          None
-        Side Effects:
-          Creates a package in the local environment.
-        Examples:
-          >>> Nest.create_package('my_package')
-        """
         self.validate_SnakeMake_repo(pipeline_dir)
 
         template = inspect.cleandoc(
             f"""
             #!/bin/sh
             '''exec' "{self.python_interpreter_path}" "$0" "$@"
             ' '''
```

### Comparing `snk-0.6.9/snk/pipeline.py` & `snk-0.7.0/snk/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 import sys
 from typing import Optional
-from git import Repo, GitCommandError, InvalidGitRepositoryError
+from git import Repo, InvalidGitRepositoryError
 
 
 class Pipeline:
     """
     Represents a pipeline.
     Attributes:
       path (Path): The path to the pipeline.
```

### Comparing `snk-0.6.9/snk/cli/cli.py` & `snk-0.7.0/snk/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,17 +88,20 @@
                 is_eager=True,
                 callback=_print_pipline_path,
                 show_default=False,
             ),
         ):
             if ctx.invoked_subcommand is None:
                 typer.echo(f"{ctx.get_help()}")
-
+        
         # dynamically create the logo
-        callback.__doc__ = f"{self.create_logo()}"
+        tagline: str = self.snk_config.tagline
+        font: str = self.snk_config.font
+        self.logo = self.create_logo(tagline=tagline, font=font)
+        callback.__doc__ = self.logo
 
         # registration
         self.register_callback(
             callback,
             invoke_without_command=True,
             context_settings={"help_option_names": ["-h", "--help"]},
         )
@@ -148,26 +151,30 @@
         Side Effects:
           Registers the callback to the CLI.
         Examples:
           >>> CLI.register_callback(my_callback)
         """
         self.app.callback(**command_kwargs)(command)
 
-    def create_logo(self, font="small"):
+    def create_logo(self, tagline="A Snakemake pipeline CLI generated with snk", font="small"):
         """
         Create a logo for the CLI.
         Args:
           font (str): The font to use for the logo.
         Returns:
           str: The logo.
         Examples:
           >>> CLI.create_logo()
         """
-        logo = text2art(self.name, font=font)
-        doc = f"""\b{logo}\bA Snakemake pipeline CLI generated with snk"""
+        if self.snk_config.art:
+            art = self.snk_config.art
+        else:
+            logo = self.snk_config.logo if self.snk_config.logo else self.name
+            art = text2art(logo, font=font)
+        doc = f"""\b{art}\b{tagline}"""
         return doc
 
     def _print_snakemake_help(value: bool):
         """
         Print the snakemake help and exit.
         Args:
           value (bool): If True, print the snakemake help and exit.
@@ -404,15 +411,15 @@
             typer.secho(
                 "Mamba not found! Install for speed up.", fg=typer.colors.YELLOW
             )
             mamba_found = False
         if not mamba_found:
             args.append("--conda-frontend=conda")
 
-        typer.echo(self.create_logo())
+        typer.echo(self.logo)
         typer.echo()
 
         if verbose:
             args.insert(0, "--verbose")
 
         if force:
             args.append("--forceall")
@@ -553,10 +560,12 @@
             with open(filename, 'w') as output_file:
                 if self.verbose:
                     typer.secho(
                         f"Saving dag to {filename}", fg=typer.colors.YELLOW
                     )
                 subprocess.run(['cat'], stdin=dot_process.stdout, stdout=output_file)
         except (subprocess.CalledProcessError, FileNotFoundError):
-            typer.secho(
-                "dot command not found!", fg=typer.colors.RED
-            )
+            typer.echo(
+                "dot command not found!", fg=typer.colors.RED, err=True
+            )
+            raise typer.Exit(1)
+
```

### Comparing `snk-0.6.9/snk/cli/config.py` & `snk-0.7.0/snk/cli/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 @dataclass
 class SnkConfig:
     """
     SNK config holds dynamic cli config and option annotations.
     """
 
+    art: str = None
+    logo: str = None
+    tagline: str = "A Snakemake pipeline CLI generated with Snk"
+    font: str = "small"
     resources: List[Path] = field(default_factory=list)
     annotations: dict = field(default_factory=dict)
     symlink_resources: bool = False
 
     @classmethod
     def from_path(cls, snk_config_path: Path):
         """
```

### Comparing `snk-0.6.9/snk/cli/utils.py` & `snk-0.7.0/snk/cli/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "integer": int,
     "str": str,
     "string": str,
     "path": Path,
     "bool": bool,
     "boolean": bool,
     "list": List[str],
+    "list[str]": List[str],
     "list[path]": List[Path],
     "list[int]": List[int],
 }
 
 
 def create_cli_parameter(option):
     """
@@ -43,15 +44,18 @@
     return Parameter(
         option["name"],
         kind=Parameter.POSITIONAL_OR_KEYWORD,
         default=typer.Option(
             ... if option["required"] else option["default"],
             help=f"[CONFIG] {option['help']}",
         ),
-        annotation=types.get(option["type"].lower(), str),
+        annotation=types.get(
+            option["type"].lower(), 
+            List[str] if 'list' in option["type"].lower() else str
+        ),
     )
 
 
 def add_dynamic_options(options: List[dict]):
     """
     Decorator to add dynamic options to a function.
     Args:
@@ -205,14 +209,19 @@
             continue
         if arg.startswith("-") and arg.lstrip("-") in names:
             flag = arg
             continue
         parsed.append(arg)
     return parsed, config
 
+def get_default_type(v):
+    default_type = type(v)
+    if default_type == list and len(v) > 0:
+        return f"List[{type(v[0]).__name__}]"
+    return str(default_type.__name__)
 
 def build_dynamic_cli_options(snakemake_config, snk_config: SnkConfig):
     """
     Builds a list of options from a snakemake config and a snk config.
     Args:
       snakemake_config (dict): A snakemake config.
       snk_config (SnkConfig): A snk config.
@@ -228,15 +237,15 @@
     for op in flat_config:
         name = flat_snk_annotations.get(f"{op}:name", op.replace(":", "_"))
         help = flat_snk_annotations.get(f"{op}:help", "")
         # TODO be smarter here
         # look up the List type e.g. if type == list then check the frist index type
         # also can probably just pass the type around instead of the string?
         param_type = flat_snk_annotations.get(
-            f"{op}:type", f"{type(flat_config[op]).__name__}"
+            f"{op}:type", get_default_type(flat_config[op])
         )  # TODO refactor
         required = flat_snk_annotations.get(f"{op}:required", False)
         options.append(
             {
                 "name": name.replace("-", "_"),
                 "original_key": op,
                 "default": flat_config[op],
```

### Comparing `snk-0.6.9/tests/.DS_Store` & `snk-0.7.0/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `snk-0.6.9/tests/conftest.py` & `snk-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.9/tests/test_nest.py` & `snk-0.7.0/tests/test_nest.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,22 @@
 
 def test_create_package(nest: Nest):
     test_pipeline_path = nest.pipelines_dir / 'pipeline-name'
     test_pipeline_path.mkdir()
     path = nest.create_package(pipeline_dir=test_pipeline_path)
     assert path == test_pipeline_path / 'bin' / 'pipeline-name'
 
+def test_install(nest: Nest):
+    pipeline = nest.install('tests/data/pipeline')
+    assert pipeline.name == 'pipeline'
+    pipeline = nest.install('tests/data/pipeline', name='new-pipeline-name')
+    assert pipeline.name == 'new-pipeline-name'
+    assert pipeline.path.name == 'new-pipeline-name'
+
+
 def test_link_pipeline_executable_to_bin(nest: Nest):
     pipeline_executable_path = Path('tests/data/bin/snk-basic-pipeline')
     executable_path = nest.link_pipeline_executable_to_bin(pipeline_executable_path)
-    assert executable_path.exists() == True and executable_path.is_symlink() == True
+    assert executable_path.exists() is True and executable_path.is_symlink() is True
 
 def test_uninstall(nest:Nest):
     pass
```

### Comparing `snk-0.6.9/tests/test_pipline_cli.py` & `snk-0.7.0/tests/test_pipline_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 from snk.cli.utils import flatten, convert_key_to_snakemake_format
 import snakemake
 import pytest
+from .utils import CLIRunner
 
 def test_flatten(example_config: Path):
     config = snakemake.load_configfile(example_config)
     flat_config = flatten(config)
     assert flat_config['diffexp:contrasts:A-vs-B'] == ['A', 'B']
 
 
@@ -16,26 +17,30 @@
     ("h", "world", {"h": "world"}),
 ])
 def test_convert_key_to_snakemake_format(key, value, expected):
     assert convert_key_to_snakemake_format(key, value) == expected
 
 def test_installation(basic_runner):
     res = basic_runner(['--help'])
+    assert res.code == 0, res.stderr
     assert 'snk-basic-pipeline' in res.stdout
 
 def test_info(basic_runner):
     res = basic_runner(['info'])
+    assert res.code == 0, res.stderr
     assert 'snk-basic-pipeline' in res.stdout, res.stderr
     assert 'version' in res.stdout
     assert 'pipeline_dir_path' in res.stdout
 
 def test_run_cli(basic_runner):
     res = basic_runner(['run', '-h'])
+    assert res.code == 0, res.stderr
     assert 'snk-basic-pipeline' in res.stdout, res.stderr
     assert 'samples' in res.stdout
     assert 'genome' in res.stdout
 
 @pytest.mark.parametrize("filetype", ['pdf', 'svg', 'png'])
-def test_dag(local_runner, tmp_path, filetype):
+def test_dag(local_runner: CLIRunner, tmp_path, filetype):
     res = local_runner(['run', '--dag', f'{tmp_path}/dag.{filetype}'])
+    assert res.code == 0, res.stderr
     assert 'DAG' in res.stderr, res.stderr
     assert Path(f'{tmp_path}/dag.{filetype}').exists()
```

### Comparing `snk-0.6.9/tests/test_snk.py` & `snk-0.7.0/tests/test_snk.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.9/tests/utils.py` & `snk-0.7.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.9/tests/data/artic_v4.1.bed` & `snk-0.7.0/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk-0.6.9/tests/data/config.yaml` & `snk-0.7.0/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk-0.6.9/tests/data/cov.fasta` & `snk-0.7.0/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk-0.6.9/LICENSE.txt` & `snk-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snk-0.6.9/README.md` & `snk-0.7.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 **Documentation**: <a href="https://snk.wytamma.com" target="_blank">https://snk.wytamma.com</a>
 
 **Source Code**: <a href="https://github.com/Wytamma/snk" target="_blank">https://github.com/Wytamma/snk</a>
 
 ---
 
-Snk (pronounced snek) is a SNaKemake pipeline management system. Snk allows you to install Snakemake pipelines as Command Line Interfaces (CLIs). Using a pipeline as a CLI increases its interoperability and allows complex pipelines to be used as modular components in a larger system. Snk, using python magic, will dynamic genrate the pipeline CLI using the pipeline configuration file.
+Snk (pronounced snek) is a SNaKemake pipeline management system. Snk allows you to install Snakemake pipelines as dynamically generated Command Line Interfaces (CLIs). Using a pipeline as a CLI increases its interoperability and allows complex pipelines to be used as modular components in a larger system.
 
 ## Installation
 
 ```console
 pip install snk
 ```
 
 ## Basic Use
 
 ### Install a pipeline as a CLI
 
-Install the dna-seq-gatk-variant-calling pipeline (v2.1.1) as `variant-calling`.
+Install the [dna-seq-gatk-variant-calling](https://github.com/snakemake-workflows/dna-seq-gatk-variant-calling) pipeline (v2.1.1) as `variant-calling`.
 
 ```
 snk install snakemake-workflows/dna-seq-gatk-variant-calling --name variant-calling -t v2.1.1
 ```
 Successfully installed variant-calling (v2.1.1)!
 
 ### Inspect the CLI   
@@ -69,20 +69,12 @@
 
 ```
 variant-calling config --pretty # print the config 
 variant-calling config > config.yml # save the config 
 variant-calling run --config config.yml # run with config 
 ```
 
-## how it works
-
-When installing a pipeline snk will
-
-- create directory `$PYTHON_BIN_DIR/../snk/pipelines/PIPELINE`
-- install the pipeline into this directory
-- expose CLI at `$PYTHON_BIN_DIR` that point to pipeline directory in `snk/pipelines/PIPELINE/bin`
-- As long as `$PYTHON_BIN_DIR` is on your PATH, you can now invoke the pipeline globally
-
+Read the [documentation](https://snk.wytamma.com") for more information.
 
 ## License
 
 `snk` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

#### html2text {}

```diff
@@ -4,31 +4,27 @@
 /badgen.net/badge/write-the/docs/blue?icon=https://raw.githubusercontent.com/
 Wytamma/write-the/master/images/write-the-icon.svg)](https://write-
 the.wytamma.com/) [![Hits](https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FWytamma%2Fsnk&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)]
 (https://github.com/Wytamma/snk) --- **Documentation**: https://snk.wytamma.com
 **Source Code**: https://github.com/Wytamma/snk --- Snk (pronounced snek) is a
 SNaKemake pipeline management system. Snk allows you to install Snakemake
-pipelines as Command Line Interfaces (CLIs). Using a pipeline as a CLI
-increases its interoperability and allows complex pipelines to be used as
-modular components in a larger system. Snk, using python magic, will dynamic
-genrate the pipeline CLI using the pipeline configuration file. ## Installation
-```console pip install snk ``` ## Basic Use ### Install a pipeline as a CLI
-Install the dna-seq-gatk-variant-calling pipeline (v2.1.1) as `variant-
-calling`. ``` snk install snakemake-workflows/dna-seq-gatk-variant-calling --
-name variant-calling -t v2.1.1 ``` Successfully installed variant-calling
-(v2.1.1)! ### Inspect the CLI ``` variant-calling --help ``` [main cli] ###
-View run options ``` variant-calling run -h ``` [run cli] ### Create a DAG Here
-we use the `.test` resources included in the pipeline to create the DAG. ```
-variant-calling run -r .test/config -r .test/data --dag dag.pdf ``` [dag] ###
-Configure Snk will dynamically generate config options for the CLI. For example
-if your config.yaml file has the option `fasta: null` you can set this option
-with `--fasta`. ``` variant-calling run --fasta example.fa ``` You can also
-configure the pipeline using a config file. ``` variant-calling config --pretty
-# print the config variant-calling config > config.yml # save the config
-variant-calling run --config config.yml # run with config ``` ## how it works
-When installing a pipeline snk will - create directory `$PYTHON_BIN_DIR/../snk/
-pipelines/PIPELINE` - install the pipeline into this directory - expose CLI at
-`$PYTHON_BIN_DIR` that point to pipeline directory in `snk/pipelines/PIPELINE/
-bin` - As long as `$PYTHON_BIN_DIR` is on your PATH, you can now invoke the
-pipeline globally ## License `snk` is distributed under the terms of the [MIT]
-(https://spdx.org/licenses/MIT.html) license.
+pipelines as dynamically generated Command Line Interfaces (CLIs). Using a
+pipeline as a CLI increases its interoperability and allows complex pipelines
+to be used as modular components in a larger system. ## Installation ```console
+pip install snk ``` ## Basic Use ### Install a pipeline as a CLI Install the
+[dna-seq-gatk-variant-calling](https://github.com/snakemake-workflows/dna-seq-
+gatk-variant-calling) pipeline (v2.1.1) as `variant-calling`. ``` snk install
+snakemake-workflows/dna-seq-gatk-variant-calling --name variant-calling -
+t v2.1.1 ``` Successfully installed variant-calling (v2.1.1)! ### Inspect the
+CLI ``` variant-calling --help ``` [main cli] ### View run options ``` variant-
+calling run -h ``` [run cli] ### Create a DAG Here we use the `.test` resources
+included in the pipeline to create the DAG. ``` variant-calling run -r .test/
+config -r .test/data --dag dag.pdf ``` [dag] ### Configure Snk will dynamically
+generate config options for the CLI. For example if your config.yaml file has
+the option `fasta: null` you can set this option with `--fasta`. ``` variant-
+calling run --fasta example.fa ``` You can also configure the pipeline using a
+config file. ``` variant-calling config --pretty # print the config variant-
+calling config > config.yml # save the config variant-calling run --config
+config.yml # run with config ``` Read the [documentation](https://
+snk.wytamma.com") for more information. ## License `snk` is distributed under
+the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `snk-0.6.9/pyproject.toml` & `snk-0.7.0/pyproject.toml`

 * *Files identical despite different names*

