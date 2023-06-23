# Comparing `tmp/pymetasnap-0.2.2.tar.gz` & `tmp/pymetasnap-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetasnap-0.2.2.tar", max compression
+gzip compressed data, was "pymetasnap-0.2.3.tar", max compression
```

## Comparing `pymetasnap-0.2.2.tar` & `pymetasnap-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/LICENSE
--rw-r--r--   0        0        0     2927 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/extractor/__init__.py
--rw-r--r--   0        0        0     2492 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/extractor/checks.py
--rw-r--r--   0        0        0     2998 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/extractor/core.py
--rw-r--r--   0        0        0      227 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/extractor/logger.py
--rw-r--r--   0        0        0     1253 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/extractor/main.py
--rw-r--r--   0        0        0     3262 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/extractor/render.py
--rw-r--r--   0        0        0     1669 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/extractor/utils.py
--rw-r--r--   0        0        0      845 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3888 1970-01-01 00:00:00.000000 pymetasnap-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-23 17:11:20.041671 pymetasnap-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2927 2023-06-23 17:11:20.041671 pymetasnap-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 17:11:20.041671 pymetasnap-0.2.3/extractor/__init__.py
+-rw-r--r--   0        0        0     2189 2023-06-23 17:11:20.041671 pymetasnap-0.2.3/extractor/checks.py
+-rw-r--r--   0        0        0     3216 2023-06-23 17:11:20.041671 pymetasnap-0.2.3/extractor/core.py
+-rw-r--r--   0        0        0      227 2023-06-23 17:11:20.041671 pymetasnap-0.2.3/extractor/logger.py
+-rw-r--r--   0        0        0     1253 2023-06-23 17:11:20.041671 pymetasnap-0.2.3/extractor/main.py
+-rw-r--r--   0        0        0     3262 2023-06-23 17:11:20.041671 pymetasnap-0.2.3/extractor/render.py
+-rw-r--r--   0        0        0     1669 2023-06-23 17:11:20.041671 pymetasnap-0.2.3/extractor/utils.py
+-rw-r--r--   0        0        0      845 2023-06-23 17:11:20.045672 pymetasnap-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3888 1970-01-01 00:00:00.000000 pymetasnap-0.2.3/PKG-INFO
```

### Comparing `pymetasnap-0.2.2/LICENSE` & `pymetasnap-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.2.2/README.md` & `pymetasnap-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.2.2/extractor/checks.py` & `pymetasnap-0.2.3/extractor/checks.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,27 +45,21 @@
         if project_url != "" and self.gh_pattern(pattern, project_url):
             return project_url
 
         if project_urls:
             logger.debug("Nested metadata found")
             return self.additional_urls(pattern, project_urls)
 
-    def version(
-        self, version: str, pattern: str, raw_data: Dict, filtered_data: Dict
-    ) -> Dict:
+    def version(self, version: str, pattern: str, filtered_data: Dict) -> Dict:
         project_default_error = "No project url found, please check manually"
-        version_default_error = "No version url found, please check manually"
         if version and self.gh_pattern(
             pattern, filtered_data.get("project_url"), project_default_error
         ):
             filtered_data[
                 "version_url"
             ] = f"{filtered_data['project_url']}/tree/{version}/"
-        elif raw_data["release_url"] and self.gh_pattern(
-            pattern, filtered_data.get("project_url"), version_default_error
-        ):
-            filtered_data["version_url"] = raw_data["release_url"]
 
         else:
+            version_default_error = "No version url found, please check manually"
             filtered_data["version_url"] = version_default_error
-            filtered_data["project_url"] = project_default_error
+
         return filtered_data
```

### Comparing `pymetasnap-0.2.2/extractor/core.py` & `pymetasnap-0.2.3/extractor/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,32 +42,35 @@
 
     Returns:
         A dictionary containing filtered metadata.
     """
     project_name = raw_data["name"]
     project_url = raw_data["project_url"]
     project_urls = raw_data["project_urls"]
+    project_version = version or raw_data["version"]
     check = StandardCheck()
+    pypi_url = f"https://pypi.org/project/{project_name}/{project_version}/"
     gh_url_pattern = r"(https:\/\/|http:\/\/)github\.com"
     filtered_data = {
         "name": project_name,
-        "version": version or raw_data["version"],
+        "version": project_version,
         "license": check.licenses(raw_data),
-        "homepage": raw_data["home_page"],
-        "release_url": raw_data["release_url"],
+        # "homepage": raw_data["home_page"],
+        "pypi_release_url": pypi_url,
         "project_url": check.project_url(gh_url_pattern, project_url, project_urls),
     }
 
     logger.info(f"Searching GitHub url for: {project_name}")
 
     if project_name == "pandas":
         version = f"v{filtered_data['version']}"
         filtered_data["version"] = version
 
-    filtered_data = check.version(version, gh_url_pattern, raw_data, filtered_data)
+    filtered_data = check.version(version, gh_url_pattern, filtered_data)
+    del filtered_data["project_url"]
     return filtered_data
 
 
 def extract_data(source_path: Path, format: str) -> None:
     """
     Extract data based on the specified requirements format.
 
@@ -77,21 +80,22 @@
 
     Returns:
         pd.DataFrame
     """
     logger.info("Starting process")
     logger.debug(f"Retrieving: {source_path}")
     result = Requirements().render(source_path, format)
+    custom_columns_order = ["license", "name"]
     pkgs_raw_metadata = []
     for pkg in track(result):
         filtered_data = filter_data(
             get_raw_data(pkg[0]), pkg[1] if len(pkg) > 1 else None
         )
         pkgs_raw_metadata.append(filtered_data)
-    return pd.DataFrame(pkgs_raw_metadata)
+    return pd.DataFrame(pkgs_raw_metadata).sort_values(by=custom_columns_order)
 
 
 def save_data(data: pd.DataFrame, output: Path):
     logger.info(f"Storing into: {output}")
     if str(output).endswith(".csv"):
         data.to_csv(output, index=False)
         logger.info("All done! Have a Great day")
```

### Comparing `pymetasnap-0.2.2/extractor/main.py` & `pymetasnap-0.2.3/extractor/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from rich import print
 from typing_extensions import Annotated
 
 from extractor.core import extract_data, save_data
 from extractor.render import RequirementsFormat
 
 app = typer.Typer()
-VERSION = "0.2.2"
+VERSION = "0.2.3"
 
 
 @app.command(name="version")
 def version():
     return print(VERSION)
```

### Comparing `pymetasnap-0.2.2/extractor/render.py` & `pymetasnap-0.2.3/extractor/render.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.2.2/extractor/utils.py` & `pymetasnap-0.2.3/extractor/utils.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.2.2/pyproject.toml` & `pymetasnap-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymetasnap"
-version = "0.2.2"
+version = "0.2.3"
 description = "This package allows you to scrape metadata from the Python Package Index"
 authors = ["cristian-rincon <cristian.o.rincon.b@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "extractor"}]
 
 [tool.poetry.scripts]
```

### Comparing `pymetasnap-0.2.2/PKG-INFO` & `pymetasnap-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetasnap
-Version: 0.2.2
+Version: 0.2.3
 Summary: This package allows you to scrape metadata from the Python Package Index
 License: MIT
 Author: cristian-rincon
 Author-email: cristian.o.rincon.b@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

