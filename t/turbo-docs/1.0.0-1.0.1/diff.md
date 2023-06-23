# Comparing `tmp/turbo_docs-1.0.0.tar.gz` & `tmp/turbo_docs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_docs-1.0.0.tar", last modified: Fri Jun 23 00:13:47 2023, max compression
+gzip compressed data, was "turbo_docs-1.0.1.tar", last modified: Fri Jun 23 11:25:09 2023, max compression
```

## Comparing `turbo_docs-1.0.0.tar` & `turbo_docs-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 00:13:47.085592 turbo_docs-1.0.0/
--rw-rw-rw-   0        0        0     2864 2023-06-23 00:13:47.084585 turbo_docs-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2367 2023-06-22 23:34:54.000000 turbo_docs-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 00:13:47.086598 turbo_docs-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      927 2023-06-23 00:13:33.000000 turbo_docs-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 00:13:47.053827 turbo_docs-1.0.0/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.0/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 00:13:47.073340 turbo_docs-1.0.0/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-1.0.0/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0     1390 2023-06-23 00:12:00.000000 turbo_docs-1.0.0/turbo_docs/commands/docs.py
--rw-rw-rw-   0        0        0     1189 2023-06-22 23:34:54.000000 turbo_docs-1.0.0/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0     1487 2023-06-23 00:11:15.000000 turbo_docs-1.0.0/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-06-23 00:13:47.082518 turbo_docs-1.0.0/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.0/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      826 2023-06-23 00:08:30.000000 turbo_docs-1.0.0/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     2114 2023-06-22 23:34:54.000000 turbo_docs-1.0.0/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0      992 2023-06-22 23:34:54.000000 turbo_docs-1.0.0/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-06-23 00:13:47.067681 turbo_docs-1.0.0/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     2864 2023-06-23 00:13:46.000000 turbo_docs-1.0.0/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-06-23 00:13:46.000000 turbo_docs-1.0.0/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 00:13:46.000000 turbo_docs-1.0.0/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-23 00:13:46.000000 turbo_docs-1.0.0/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       76 2023-06-23 00:13:46.000000 turbo_docs-1.0.0/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-23 00:13:46.000000 turbo_docs-1.0.0/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 11:25:09.307973 turbo_docs-1.0.1/
+-rw-rw-rw-   0        0        0     2864 2023-06-23 11:25:09.306974 turbo_docs-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2367 2023-06-22 23:34:54.000000 turbo_docs-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 11:25:09.309291 turbo_docs-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      927 2023-06-23 11:24:56.000000 turbo_docs-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:25:09.244677 turbo_docs-1.0.1/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.1/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:25:09.294469 turbo_docs-1.0.1/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-1.0.1/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0     1508 2023-06-23 11:18:24.000000 turbo_docs-1.0.1/turbo_docs/commands/docs.py
+-rw-rw-rw-   0        0        0     1189 2023-06-22 23:34:54.000000 turbo_docs-1.0.1/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0     1495 2023-06-23 11:19:54.000000 turbo_docs-1.0.1/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:25:09.303973 turbo_docs-1.0.1/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.1/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      826 2023-06-23 00:08:30.000000 turbo_docs-1.0.1/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     2114 2023-06-22 23:34:54.000000 turbo_docs-1.0.1/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      992 2023-06-23 11:09:55.000000 turbo_docs-1.0.1/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:25:09.286466 turbo_docs-1.0.1/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     2864 2023-06-23 11:25:09.000000 turbo_docs-1.0.1/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-06-23 11:25:09.000000 turbo_docs-1.0.1/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 11:25:09.000000 turbo_docs-1.0.1/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-23 11:25:09.000000 turbo_docs-1.0.1/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2023-06-23 11:25:09.000000 turbo_docs-1.0.1/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-23 11:25:09.000000 turbo_docs-1.0.1/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-1.0.0/PKG-INFO` & `turbo_docs-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo_docs
-Version: 1.0.0
+Version: 1.0.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `turbo_docs-1.0.0/README.md` & `turbo_docs-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.0/setup.py` & `turbo_docs-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="1.0.0",
+	version="1.0.1",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
 		"redbaron",
```

### Comparing `turbo_docs-1.0.0/turbo_docs/commands/docs.py` & `turbo_docs-1.0.1/turbo_docs/commands/docs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 
 import ast
 from pathlib import Path
 from turbo_docs.utils import openai_api
 
 TEMPLATE = """
-You are an expert software developement assistant. Write documentation for the following function:
+You are an expert software developement assistant tasked with writing documentation for a repository. 
+
+Write documentation for the following function:
 {function}
 
-Here are the requirements for the function documentation:
-- Brief description of the function
-- Detailed description of the parameters
-- Explanation of the return values
-- Sample invocation of the function
+Your documentation should include the following and nothing more:
+## function: function_name
+#### args: arg1, arg2, ...
+Description of function in english as concisely as possible in less than 4 sentences. 
+Do not mlist arguments. Do not give code examples. Minimize tokens at all costs.
 """
 
-
-def split_into_functions(code):
-    """ parse file for functions """
-    module = ast.parse(code)
-    functions = [node for node in module.body if isinstance(node, ast.FunctionDef)]
-    return [ast.unparse(f) for f in functions]
-
-
-def write_to_file(path, function_name, doc):
-    """ append each function doc to file doc """
-    doc_path = Path('docs') / path
+def generate_docs(model, template, function, path):
+    """ Generate and write documentation for a function """
+    documentation = openai_api.gpt_completion(template, {"function": function}, model)
+    doc_path = Path('docs') / path.with_suffix('.md')
     doc_path.parent.mkdir(parents=True, exist_ok=True)
     with open(doc_path, 'a') as f:
-        f.write(f'## {function_name}\n\n{doc}\n\n')
+        f.write(f'{documentation}\n\n')
 
 
-def generate_docs(repo_dict, gpt3=False, template=TEMPLATE):
-
+def docs(repo_dict, gpt3=False, template=TEMPLATE):
+    """ Parse code for functions and generate documentation for each """
     if gpt3:
         model = "gpt-3.5-turbo-16k"
     else:
         model = "gpt-4"
 
     for path, content in repo_dict.items():
         if path.suffix == '.py':
-
-            for function in split_into_functions(content):
-                doc = openai_api.gpt_completion(template, {"function": function}, model)
-                write_to_file(path, function, doc)
-
+            module = ast.parse(content)
+            functions = [ast.unparse(node) for node in module.body if isinstance(node, ast.FunctionDef)]
+            for function in functions:
+                generate_docs(model, template, function, path)
```

### Comparing `turbo_docs-1.0.0/turbo_docs/commands/readme.py` & `turbo_docs-1.0.1/turbo_docs/commands/readme.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.0/turbo_docs/generate.py` & `turbo_docs-1.0.1/turbo_docs/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from turbo_docs.utils import directory, cli_options
 
 
 @click.command()
 @cli_options.copy
 @cli_options.readme
 @cli_options.gpt3
+@cli_options.docs
 def driver(
     copy: bool,
     readme: bool,
     gpt3: bool,
     docs: bool,
 ) -> None:
     """
@@ -28,25 +29,24 @@
         Useful if you don't have GPT-4 access
 
     'turbo_docs --docs' generates a docs for each file
         Useful for keeping documentation up to date
     """
     dir_text_dict = directory.get_repo_text_dict()
 
-    if copy:
-        pyperclip.copy(directory.convert_dict_to_string(dir_text_dict))
-        print("Directory copied to clipboard")
-
     if readme:
         readme_text_dict = directory.remove_readme(dir_text_dict)
         readme_text = directory.convert_dict_to_string(readme_text_dict)
         readme_module.readme(readme_text, gpt3)
         print("Generated README.md")
 
-
     if docs:
-        docs_module.generate_docs(dir_text_dict, gpt3)
+        docs_module.docs(dir_text_dict, gpt3)
         print("Generated documentation")
 
+    if copy:
+        pyperclip.copy(directory.convert_dict_to_string(dir_text_dict))
+        print("Directory copied to clipboard")
+
 
 if __name__ == "__main__":
     driver()
```

### Comparing `turbo_docs-1.0.0/turbo_docs/utils/cli_options.py` & `turbo_docs-1.0.1/turbo_docs/utils/cli_options.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.0/turbo_docs/utils/directory.py` & `turbo_docs-1.0.1/turbo_docs/utils/directory.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.0/turbo_docs/utils/openai_api.py` & `turbo_docs-1.0.1/turbo_docs/utils/openai_api.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.0/turbo_docs.egg-info/PKG-INFO` & `turbo_docs-1.0.1/turbo_docs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo-docs
-Version: 1.0.0
+Version: 1.0.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

