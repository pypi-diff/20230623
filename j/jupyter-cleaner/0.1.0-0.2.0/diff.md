# Comparing `tmp/jupyter_cleaner-0.1.0.tar.gz` & `tmp/jupyter_cleaner-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_cleaner-0.1.0.tar", max compression
+gzip compressed data, was "jupyter_cleaner-0.2.0.tar", max compression
```

## Comparing `jupyter_cleaner-0.1.0.tar` & `jupyter_cleaner-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-21 17:07:31.522031 jupyter_cleaner-0.1.0/jupyter_cleaner/__init__.py
--rw-r--r--   0        0        0    13019 2023-06-21 17:07:31.522540 jupyter_cleaner-0.1.0/jupyter_cleaner/jupyter_cleaner.py
--rw-r--r--   0        0        0     1092 2023-06-21 17:40:20.719190 jupyter_cleaner-0.1.0/LICENSE
--rw-r--r--   0        0        0      936 2023-06-21 18:44:11.264538 jupyter_cleaner-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1415 2023-06-21 17:07:31.506204 jupyter_cleaner-0.1.0/README.md
--rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 jupyter_cleaner-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 17:07:31.522031 jupyter_cleaner-0.2.0/jupyter_cleaner/__init__.py
+-rw-r--r--   0        0        0    16233 2023-06-23 07:52:40.510421 jupyter_cleaner-0.2.0/jupyter_cleaner/jupyter_cleaner.py
+-rw-r--r--   0        0        0     1092 2023-06-21 17:40:20.719190 jupyter_cleaner-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1795 2023-06-23 07:54:53.033923 jupyter_cleaner-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1991 2023-06-23 07:54:37.232156 jupyter_cleaner-0.2.0/README.md
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 jupyter_cleaner-0.2.0/PKG-INFO
```

### Comparing `jupyter_cleaner-0.1.0/jupyter_cleaner/jupyter_cleaner.py` & `jupyter_cleaner-0.2.0/jupyter_cleaner/jupyter_cleaner.py`

 * *Files 25% similar despite different names*

```diff
@@ -34,43 +34,54 @@
 
 def run(
     files: Sequence[Path],
     execution_count: int = 0,
     remove_code_output: bool = True,
     format: bool = True,
     reorder_imports: bool = True,
+    indent_level: int = 4,
+    exclude_files: Sequence[Path] = [],
     black_config: Optional[Dict[str, str]] = None,
 ) -> None:
     """Format Jupyter lab files.
 
-    :param Union[str, Path, Sequence[Union[str, Path]]] files: file(s) to be formatted
-    :param int execution_count: sets execution count, defaults to 0
+    :param Sequence[Path] files: file(s) to be formatted
+    :param Sequence[Path] exclude_files: file(s) to be excluded from formatting
+    :param int execution_count: sets execution count. If the integer is greater than zero the count will be printed, else `null` will be printed. Defaults to 0.
     :param bool remove_code_output: remove output from code cells, defaults to True
     :param bool format: format cells using black, defaults to True
     :param bool reorder_imports: reorder imports using reoder-python-imports, defaults to True
+    :param int indent_level: integer greater than zero will pretty-print the JSON array with that indent level. An indent level of 0 or negative will only insert newlines.
     :param Optional[Dict[str, str]] black_config: configuration from black formatting, defaults to None
     :raises TypeError: when file input is unrecognised
     """
     if black_config is None:
         black_config = {}
 
     for file in files:
-        if not file.is_file() and not file.exists() and file.suffix != ".ipynb":
+        if (
+            not file.is_file()
+            or not file.exists()
+            or file.suffix != ".ipynb"
+            or file in exclude_files
+        ):
             continue
 
         with open(file) as f:
             data = json.load(f)
             python_version = data["metadata"]["language_info"]["version"]
             min_python_version = tuple(map(int, re.findall(r"(\d+)", python_version)))
             if len(min_python_version) > 2:
                 min_python_version = min_python_version[:2]
 
             for cell in data["cells"]:
                 if "execution_count" in cell.keys() and cell["cell_type"] == "code":
-                    cell["execution_count"] = execution_count
+                    cell["execution_count"] = (
+                        execution_count if execution_count > 0 else "null"
+                    )
                     if remove_code_output:
                         cell["outputs"] = []
 
                     if format:
                         try:
                             mode = black.Mode(is_ipynb=True, **black_config)  # type: ignore
                             str_cell_content = black.format_cell(
@@ -106,16 +117,22 @@
                             to_replace=to_replace,
                             to_remove=to_remove,
                         )[:-1]
                         cell_content = [f"{c}\n" for c in str_cell_content.split("\n")]
                         cell_content[-1] = cell_content[-1][:-1]
                         cell["source"] = cell_content
 
+        with open(file) as f:
+            original_data = json.load(f)
+            if data == original_data:
+                continue
+
         with open(file, "w") as f:
-            json.dump(data, f)
+            json.dump(data, f, indent=indent_level)
+        print(f"Reformatted {str(file)}")
 
 
 @lru_cache
 def find_project_root(
     srcs: Sequence[str], stdin_filename: Optional[str] = None
 ) -> Path:
     """Modified version of black's find_project_root():
@@ -164,136 +181,179 @@
 def parse_pyproject() -> (
     Tuple[
         Union[List[str], str, None],
         Union[int, None],
         Union[bool, None],
         Union[bool, None],
         Union[bool, None],
+        Union[int, None],
+        Union[List[str], str, None],
     ]
 ):
     """Parse inputs from pyproject.toml
 
-    :return Tuple[ Union[List[str], None], Union[int, None], Union[bool, None], Union[bool, None], Union[bool, None], ]: returns parsed pyproject information
+    :return _type_: Parse inputs from pyproject.toml
     """
     project_root = find_project_root((str(Path.cwd().resolve()),))
     pyproject_path = project_root / "pyproject.toml"
     if not pyproject_path.exists():
         return (
             None,
             None,
             None,
             None,
             None,
+            None,
+            None,
         )
 
     with open(pyproject_path, "rb") as f:
         pyproject_toml = tomllib.load(f)
 
-    config: Dict[str, Any] = pyproject_toml.get("tool", {}).get("jupyter_cleaner", {})
+    config: Dict[str, Any] = pyproject_toml.get("tool", {}).get("jupyter-cleaner", {})
 
-    files = config["files"] if "files" in config else None
+    files_or_dirs = config["files_or_dirs"] if "files_or_dirs" in config else None
+    if isinstance(files_or_dirs, str):
+        files_or_dirs = [files_or_dirs]
+    exclude_files_or_dirs = (
+        config["exclude_files_or_dirs"] if "exclude_files_or_dirs" in config else None
+    )
+    if isinstance(exclude_files_or_dirs, str):
+        exclude_files_or_dirs = [exclude_files_or_dirs]
     execution_count = config["execution_count"] if "execution_count" in config else None
     remove_code_output = (
         config["remove_code_output"] if "remove_code_output" in config else None
     )
     format = config["format"] if "format" in config else None
     reorder_imports = config["reorder_imports"] if "reorder_imports" in config else None
+    indent_level = config["indent_level"] if "indent_level" in config else None
     return (
-        files,
+        files_or_dirs,
         execution_count,
         remove_code_output,
         format,
         reorder_imports,
+        indent_level,
+        exclude_files_or_dirs,
     )
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="jupyter_cleaner")
     parser.add_argument(
-        "files_or_dir",
+        "files_or_dirs",
         type=str,
-        nargs="*",
+        nargs="+",
         help="Jupyter lab files to format or directories to search for lab files",
     )
     parser.add_argument(
+        "--exclude_files_or_dirs",
+        type=str,
+        nargs="+",
+        help="Jupyter lab files or directories to exclude from formatting and search",
+    )
+    parser.add_argument(
         "--execution_count",
         type=int,
         default=0,
         help="Number to set for the execution count of every cell",
     )
     parser.add_argument(
+        "--indent_level",
+        type=int,
+        default=4,
+        help="Integer greater than zero will pretty-print the JSON array with that indent level. An indent level of 0 or negative will only insert newlines.",
+    )
+    parser.add_argument(
         "--remove_code_output",
         action="store_false",
-        help="Number to set for the execution count of every cell",
+        help="Remove output of cell",
     )
     parser.add_argument(
         "--format",
         action="store_false",
         help="Format code of every cell (uses black)",
     )
     parser.add_argument(
         "--reorder_imports",
         action="store_false",
         help="Reorder imports of every cell (uses reorder-python-imports)",
     )
     args = parser.parse_args()
     return (
-        args.files_or_dir,
+        args.files_or_dirs,
         args.execution_count,
         args.remove_code_output,
         args.format,
         args.reorder_imports,
+        args.indent_level,
+        args.exclude_files_or_dirs,
     )
 
 
-def get_lab_files(files_or_dirs: List[Path]) -> List[Path]:
+def get_lab_files(files_or_dirss: List[Path]) -> List[Path]:
     files = []
-    for file_or_dir in files_or_dirs:
+    for file_or_dir in files_or_dirss:
         if file_or_dir.is_dir():
-            files.extend([p for p in file_or_dir.rglob("*") if p.suffix == ".ipynb"])
+            files.extend([p for p in file_or_dir.rglob("*.ipynb")])
         elif file_or_dir.is_file() and file_or_dir.suffix == ".ipynb":
             files.append(file_or_dir)
         else:
-            raise ValueError("Files or directories do not exist or could not be found")
-    return files
+            raise ValueError("File or directory does not exist or could not be found")
+    return list(set(files))
 
 
 def process_inputs(
-    args_files_or_dirs: List[str],
+    args_files_or_dirss: List[str],
     args_execution_count: int,
     args_remove_code_output: bool,
     args_format: bool,
     args_reorder_imports: bool,
-    project_files_or_dirs: Union[List[str], str, None],
+    args_indent_level: int,
+    args_exclude_files_or_dirs: Union[List[str], None],
+    project_files_or_dirss: Union[List[str], str, None],
     project_execution_count: Union[int, None],
     project_remove_code_output: Union[bool, None],
     project_format: Union[bool, None],
     project_reorder_imports: Union[bool, None],
-) -> Tuple[List[Path], int, bool, bool, bool]:
+    project_indent_level: Union[int, None],
+    project_exclude_files_or_dirs: Union[List[str], str, None],
+) -> Tuple[List[Path], int, bool, bool, bool, int, List[Path]]:
     """Creates inputs of the right format and prioritises pyproject inputs over argparse inputs, outside of files and directories where all inputs are combined.
 
-    :param List[str] args_files_or_dirs: files or directories from argparse
+    :param List[str] args_files_or_dirss: files or directories from argparse
+    :param List[str] args_exclude_files_or_dirs: files or directories to exclude from argparse
     :param int args_execution_count: execution count from argparse
     :param bool args_remove_code_output: remove code output from argparse
     :param bool args_format: apply formatting from argparse
     :param bool args_reorder_imports: reorder imports from argparse
-    :param Union[List[str], str, None] project_files_or_dirs: files or directories from pyproject
+    :param Union[List[str], str, None] project_files_or_dirss: files or directories from pyproject
+    :param Union[List[str], str, None] project_exclude_files_or_dirs: files or directories to exclude from pyproject
     :param Union[int, None] project_execution_count: execution count from pyproject
     :param Union[bool, None] project_remove_code_output: remove code output from pyproject
     :param Union[bool, None] project_format: apply formatting from pyproject
     :param Union[bool, None] project_reorder_imports: reorder imports from pyproject
     :return Tuple[ Union[List[str], str, None], Union[int, None], Union[bool, None], Union[bool, None], Union[bool, None], ]: inputs to run()
     """
-    if args_files_or_dirs is None:
-        args_files_or_dirs = [Path.cwd().resolve()]
-    if project_files_or_dirs is None:
-        project_files_or_dirs = []
-    elif isinstance(project_files_or_dirs, str):
-        project_files_or_dirs = [project_files_or_dirs]
-    files_or_dirs = [Path(f) for f in project_files_or_dirs + args_files_or_dirs]
+    if args_files_or_dirss is None:
+        args_files_or_dirss = [Path.cwd().resolve()]
+    if project_files_or_dirss is None:
+        project_files_or_dirss = []
+    elif isinstance(project_files_or_dirss, str):
+        project_files_or_dirss = [project_files_or_dirss]
+    files_or_dirss = [Path(f) for f in project_files_or_dirss + args_files_or_dirss]
+    if project_exclude_files_or_dirs is None:
+        project_exclude_files_or_dirs = []
+    elif isinstance(project_exclude_files_or_dirs, str):
+        project_exclude_files_or_dirs = [project_exclude_files_or_dirs]
+    if args_exclude_files_or_dirs is None:
+        args_exclude_files_or_dirs = []
+    exclude_files_or_dirss = [
+        Path(f) for f in project_exclude_files_or_dirs + args_exclude_files_or_dirs
+    ]
     execution_count = (
         project_execution_count
         if project_execution_count is not None
         else args_execution_count
     )
     remove_code_output = (
         project_remove_code_output
@@ -302,62 +362,80 @@
     )
     format = project_format if project_format is not None else args_format
     reorder_imports = (
         project_reorder_imports
         if project_reorder_imports is not None
         else args_reorder_imports
     )
+    indent_level = (
+        project_indent_level if project_indent_level is not None else args_indent_level
+    )
 
     return (
-        files_or_dirs,
+        files_or_dirss,
         execution_count,
         remove_code_output,
         format,
         reorder_imports,
+        indent_level,
+        exclude_files_or_dirss,
     )
 
 
 def main():
     (
-        args_files_or_dirs,
+        args_files_or_dirss,
         args_execution_count,
         args_remove_code_output,
         args_format,
         args_reorder_imports,
+        args_indent_level,
+        args_exclude_files_or_dirs,
     ) = parse_args()
 
     (
-        project_files_or_dirs,
+        project_files_or_dirss,
         project_execution_count,
         project_remove_code_output,
         project_format,
         project_reorder_imports,
+        project_indent_level,
+        project_exclude_files_or_dirs,
     ) = parse_pyproject()
 
     (
-        files_or_dirs,
+        files_or_dirss,
         execution_count,
         remove_code_output,
         format,
         reorder_imports,
+        indent_level,
+        exclude_files_or_dirss,
     ) = process_inputs(
-        args_files_or_dirs,
+        args_files_or_dirss,
         args_execution_count,
         args_remove_code_output,
         args_format,
         args_reorder_imports,
-        project_files_or_dirs,
+        args_indent_level,
+        args_exclude_files_or_dirs,
+        project_files_or_dirss,
         project_execution_count,
         project_remove_code_output,
         project_format,
         project_reorder_imports,
+        project_indent_level,
+        project_exclude_files_or_dirs,
     )
 
-    files = get_lab_files(files_or_dirs)
+    files = get_lab_files(files_or_dirss)
+    exclude_files = get_lab_files(exclude_files_or_dirss)
 
     run(
         files,
         execution_count,
         remove_code_output,
         format,
         reorder_imports,
+        indent_level,
+        exclude_files,
     )
```

### Comparing `jupyter_cleaner-0.1.0/LICENSE` & `jupyter_cleaner-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_cleaner-0.1.0/PKG-INFO` & `jupyter_cleaner-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,70 @@
 Metadata-Version: 2.1
 Name: jupyter-cleaner
-Version: 0.1.0
+Version: 0.2.0
 Summary: Easy git tracking of Jupyter lab files
 Home-page: https://github.com/Stoops-ML/jupyter-cleaner
 License: MIT
 Author: Daniel Stoops
 Author-email: danielstoops25@gmail.com
 Maintainer: Daniel Stoops
 Maintainer-email: danielstoops25@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: black[jupyter]
-Requires-Dist: reorder-python-imports
+Requires-Dist: black[jupyter] (>=23.3.0,<24.0.0)
+Requires-Dist: reorder-python-imports (>=3.10.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # jupyter-cleaner
 
 jupyter-cleaner makes tracking Jupyter lab files in git easy.
 
 This is done by:
-- Removing output of all cells
-- Formatting all cells (using black)
-- Reordering imports in all cells (using reorder-python-imports)
-- Setting the execution count of all cells
+- Removing the output of cells
+- Formatting the source of cells (using black)
+- Reordering imports in the source of cells (using reorder-python-imports)
+- Setting the execution count of cells
+- pretty printing the JSON array
 
-It is recommended to run jupyter-cleaner using pre-commit:
-```
-default_language_version:
-  python: python3.11
-repos:
-- repo: local
-  hooks:
-      - id: jupyter_cleaner
-        name: jupyter_cleaner
-        entry: jupyter_cleaner .
-        language: system
-        pass_filenames: false
-        always_run: true
-```
+It is recommended to run jupyter-cleaner before adding the Jupyter lab files to the stage in git. This allows for easier tracking of differences between commits.
 
 ## CLI
-running `jupyter_cleaner -h` displays:
+running `jupyter-cleaner -h` displays:
 ```
+usage: jupyter-cleaner [-h] [--exclude_files_or_dirs EXCLUDE_FILES_OR_DIRS [EXCLUDE_FILES_OR_DIRS ...]] [--execution_count EXECUTION_COUNT]
+                       [--indent_level INDENT_LEVEL] [--remove_code_output] [--format] [--reorder_imports]
+                       files_or_dirs [files_or_dirs ...]
+
 jupyter_cleaner
 
 positional arguments:
-  files_or_dir          Jupyter lab files to format or directories to search for lab files
+  files_or_dirs         Jupyter lab files to format or directories to search for lab files
 
 options:
   -h, --help            show this help message and exit
+  --exclude_files_or_dirs EXCLUDE_FILES_OR_DIRS [EXCLUDE_FILES_OR_DIRS ...]
+                        Jupyter lab files or directories to exclude from formatting and search
   --execution_count EXECUTION_COUNT
                         Number to set for the execution count of every cell
-  --remove_code_output  Number to set for the execution count of every cell
+  --indent_level INDENT_LEVEL
+                        Integer greater than zero will pretty-print the JSON array with that indent level. An indent level of 0 or negative will only insert
+                        newlines.
+  --remove_code_output  Remove output of cell
   --format              Format code of every cell (uses black)
   --reorder_imports     Reorder imports of every cell (uses reorder-python-imports)
 ```
 
 ## pyproject.toml
 Inputs to jupyter-cleaner can be supplied via pyproject.toml:
 ```
 [tool.jupyter_cleaner]
 execution_count=0
 remove_code_output=true
 format=true
 reorder_imports=true
+indent_level=4
 ```
```

