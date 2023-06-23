# Comparing `tmp/turbo_docs-0.9.3.tar.gz` & `tmp/turbo_docs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_docs-0.9.3.tar", last modified: Tue Jun 20 00:33:51 2023, max compression
+gzip compressed data, was "turbo_docs-1.0.0.tar", last modified: Fri Jun 23 00:13:47 2023, max compression
```

## Comparing `turbo_docs-0.9.3.tar` & `turbo_docs-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 00:33:51.481467 turbo_docs-0.9.3/
--rw-rw-rw-   0        0        0     2677 2023-06-20 00:33:51.480465 turbo_docs-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     2180 2023-06-19 23:48:10.000000 turbo_docs-0.9.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 00:33:51.482463 turbo_docs-0.9.3/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-06-20 00:33:42.000000 turbo_docs-0.9.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 00:33:51.454308 turbo_docs-0.9.3/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.3/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 00:33:51.469484 turbo_docs-0.9.3/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.9.3/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0     1214 2023-06-19 23:47:07.000000 turbo_docs-0.9.3/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0      914 2023-06-14 00:14:25.000000 turbo_docs-0.9.3/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-06-20 00:33:51.477464 turbo_docs-0.9.3/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.3/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      622 2023-06-14 00:14:25.000000 turbo_docs-0.9.3/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     2022 2023-06-12 21:03:28.000000 turbo_docs-0.9.3/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0      992 2023-06-14 00:20:44.000000 turbo_docs-0.9.3/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-06-20 00:33:51.466066 turbo_docs-0.9.3/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     2677 2023-06-20 00:33:51.000000 turbo_docs-0.9.3/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-06-20 00:33:51.000000 turbo_docs-0.9.3/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 00:33:51.000000 turbo_docs-0.9.3/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-20 00:33:51.000000 turbo_docs-0.9.3/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       65 2023-06-20 00:33:51.000000 turbo_docs-0.9.3/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-20 00:33:51.000000 turbo_docs-0.9.3/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 00:13:47.085592 turbo_docs-1.0.0/
+-rw-rw-rw-   0        0        0     2864 2023-06-23 00:13:47.084585 turbo_docs-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2367 2023-06-22 23:34:54.000000 turbo_docs-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 00:13:47.086598 turbo_docs-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      927 2023-06-23 00:13:33.000000 turbo_docs-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:13:47.053827 turbo_docs-1.0.0/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.0/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:13:47.073340 turbo_docs-1.0.0/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-1.0.0/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0     1390 2023-06-23 00:12:00.000000 turbo_docs-1.0.0/turbo_docs/commands/docs.py
+-rw-rw-rw-   0        0        0     1189 2023-06-22 23:34:54.000000 turbo_docs-1.0.0/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0     1487 2023-06-23 00:11:15.000000 turbo_docs-1.0.0/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:13:47.082518 turbo_docs-1.0.0/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.0/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      826 2023-06-23 00:08:30.000000 turbo_docs-1.0.0/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     2114 2023-06-22 23:34:54.000000 turbo_docs-1.0.0/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      992 2023-06-22 23:34:54.000000 turbo_docs-1.0.0/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:13:47.067681 turbo_docs-1.0.0/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     2864 2023-06-23 00:13:46.000000 turbo_docs-1.0.0/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-06-23 00:13:46.000000 turbo_docs-1.0.0/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 00:13:46.000000 turbo_docs-1.0.0/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-23 00:13:46.000000 turbo_docs-1.0.0/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2023-06-23 00:13:46.000000 turbo_docs-1.0.0/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-23 00:13:46.000000 turbo_docs-1.0.0/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.9.3/PKG-INFO` & `turbo_docs-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,105 @@
 Metadata-Version: 2.1
 Name: turbo_docs
-Version: 0.9.3
+Version: 1.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # Turbo Docs 🚀
 
-Turbo Docs is a powerful Python tool that helps developers generate high-quality README.md files for their repositories. It uses OpenAI's GPT-3.5 Turbo and GPT-4 models to create well-structured and informative documentation.
+[![PyPI version](https://badge.fury.io/py/turbo_docs.svg)](https://badge.fury.io/py/turbo_docs)
+[![GitHub stars](https://img.shields.io/github/stars/voynow/turbo-docs.svg)](https://github.com/voynow/turbo-docs/stargazers)
+
+Turbo Docs is a powerful Python tool that helps developers automatically generate high-quality README.md files for their repositories. It leverages the power of OpenAI's GPT-3.5 Turbo and GPT-4 models to create well-structured, informative, and engaging documentation.
 
 ## Why Turbo Docs? 🤔
 
-Writing a good README.md file is essential for any software project, as it provides an overview of the project, its purpose, and how to use it. However, creating a comprehensive and well-structured README.md can be time-consuming. Turbo Docs automates this process, allowing developers to focus on writing code while ensuring their documentation is up-to-date and professional.
+Writing good documentation is essential for any software project, but it can be time-consuming and tedious. Turbo Docs simplifies this process by generating a README.md file that meets all your requirements, allowing you to focus on writing great code.
 
 ## Table of Contents 📚
 
 - [Installation](#installation)
 - [Usage](#usage)
-  - [Generate README.md](#generate-readmemd)
-  - [Copy Directory Text](#copy-directory-text)
-- [Requirements](#requirements)
-- [Contributing](#contributing)
-- [License](#license)
+- [Repo Structure](#repo-structure)
+- [Example Usage](#example-usage)
+- [Badges](#badges)
 
 ## Installation 💻
 
-To install Turbo Docs, simply run the following command:
+To install Turbo Docs, simply run:
 
 ```bash
 pip install turbo_docs
 ```
 
 ## Usage 🛠️
 
-### Generate README.md 📝
-
-To generate a README.md file for your repository, navigate to the root directory of your project and run the following command:
+To use Turbo Docs, navigate to your project's root directory and run:
 
 ```bash
 turbo_docs --readme
 ```
 
-By default, Turbo Docs uses the GPT-4 model. To use the GPT-3.5 Turbo model instead, add the `--gpt3` flag:
+This will generate a README.md file for your project. You can also use the `--gpt3` flag to use the GPT-3.5 Turbo model:
 
 ```bash
 turbo_docs --readme --gpt3
 ```
 
-### Copy Directory Text 📋
-
-To copy the text from all files in the current directory to your clipboard, run the following command:
+Additionally, you can copy the directory text to the clipboard by using the `--copy` flag:
 
 ```bash
 turbo_docs --copy
 ```
 
-This can be useful when working with ChatGPT.
+## Repo Structure 🏗️
 
-## Requirements 📦
+```
+turbo_docs/
+│
+├── commands/
+│   ├── __init__.py
+│   └── readme.py
+│
+├── utils/
+│   ├── __init__.py
+│   ├── cli_options.py
+│   ├── directory.py
+│   └── openai_api.py
+│
+├── __init__.py
+├── generate.py
+├── setup.py
+└── turbo_docs.toml
+```
 
-Turbo Docs requires the following packages:
+## Example Usage 📖
 
-- requests
-- openai
-- llm-blocks
-- click
-- pyperclip
-- redbaron
-- gitpython
-- toml
-- pathspec
+Here's an example of how to use Turbo Docs to generate a README.md file:
 
-These dependencies are automatically installed when you install Turbo Docs using pip.
+```python
+from turbo_docs.commands import readme
 
-## Contributing 🤝
+# Define your repo structure as a string
+repo = """
+{'repo': 'example_repo',
+ 'files': {
+     'main.py': 'print("Hello, World!")',
+     'README.md': ''
+ }
+}
+"""
 
-Contributions are welcome! If you'd like to improve Turbo Docs, please feel free to submit a pull request or open an issue on GitHub.
+# Generate the README.md file
+readme(repo)
+```
 
 ## License 📄
 
-Turbo Docs is released under the MIT License. See [LICENSE](LICENSE) for more information.
+Turbo Docs is released under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `turbo_docs-0.9.3/README.md` & `turbo_docs-1.0.0/turbo_docs.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,105 @@
+Metadata-Version: 2.1
+Name: turbo-docs
+Version: 1.0.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+
 # Turbo Docs 🚀
 
-Turbo Docs is a powerful Python tool that helps developers generate high-quality README.md files for their repositories. It uses OpenAI's GPT-3.5 Turbo and GPT-4 models to create well-structured and informative documentation.
+[![PyPI version](https://badge.fury.io/py/turbo_docs.svg)](https://badge.fury.io/py/turbo_docs)
+[![GitHub stars](https://img.shields.io/github/stars/voynow/turbo-docs.svg)](https://github.com/voynow/turbo-docs/stargazers)
+
+Turbo Docs is a powerful Python tool that helps developers automatically generate high-quality README.md files for their repositories. It leverages the power of OpenAI's GPT-3.5 Turbo and GPT-4 models to create well-structured, informative, and engaging documentation.
 
 ## Why Turbo Docs? 🤔
 
-Writing a good README.md file is essential for any software project, as it provides an overview of the project, its purpose, and how to use it. However, creating a comprehensive and well-structured README.md can be time-consuming. Turbo Docs automates this process, allowing developers to focus on writing code while ensuring their documentation is up-to-date and professional.
+Writing good documentation is essential for any software project, but it can be time-consuming and tedious. Turbo Docs simplifies this process by generating a README.md file that meets all your requirements, allowing you to focus on writing great code.
 
 ## Table of Contents 📚
 
 - [Installation](#installation)
 - [Usage](#usage)
-  - [Generate README.md](#generate-readmemd)
-  - [Copy Directory Text](#copy-directory-text)
-- [Requirements](#requirements)
-- [Contributing](#contributing)
-- [License](#license)
+- [Repo Structure](#repo-structure)
+- [Example Usage](#example-usage)
+- [Badges](#badges)
 
 ## Installation 💻
 
-To install Turbo Docs, simply run the following command:
+To install Turbo Docs, simply run:
 
 ```bash
 pip install turbo_docs
 ```
 
 ## Usage 🛠️
 
-### Generate README.md 📝
-
-To generate a README.md file for your repository, navigate to the root directory of your project and run the following command:
+To use Turbo Docs, navigate to your project's root directory and run:
 
 ```bash
 turbo_docs --readme
 ```
 
-By default, Turbo Docs uses the GPT-4 model. To use the GPT-3.5 Turbo model instead, add the `--gpt3` flag:
+This will generate a README.md file for your project. You can also use the `--gpt3` flag to use the GPT-3.5 Turbo model:
 
 ```bash
 turbo_docs --readme --gpt3
 ```
 
-### Copy Directory Text 📋
-
-To copy the text from all files in the current directory to your clipboard, run the following command:
+Additionally, you can copy the directory text to the clipboard by using the `--copy` flag:
 
 ```bash
 turbo_docs --copy
 ```
 
-This can be useful when working with ChatGPT.
+## Repo Structure 🏗️
 
-## Requirements 📦
+```
+turbo_docs/
+│
+├── commands/
+│   ├── __init__.py
+│   └── readme.py
+│
+├── utils/
+│   ├── __init__.py
+│   ├── cli_options.py
+│   ├── directory.py
+│   └── openai_api.py
+│
+├── __init__.py
+├── generate.py
+├── setup.py
+└── turbo_docs.toml
+```
 
-Turbo Docs requires the following packages:
+## Example Usage 📖
 
-- requests
-- openai
-- llm-blocks
-- click
-- pyperclip
-- redbaron
-- gitpython
-- toml
-- pathspec
+Here's an example of how to use Turbo Docs to generate a README.md file:
 
-These dependencies are automatically installed when you install Turbo Docs using pip.
+```python
+from turbo_docs.commands import readme
 
-## Contributing 🤝
+# Define your repo structure as a string
+repo = """
+{'repo': 'example_repo',
+ 'files': {
+     'main.py': 'print("Hello, World!")',
+     'README.md': ''
+ }
+}
+"""
 
-Contributions are welcome! If you'd like to improve Turbo Docs, please feel free to submit a pull request or open an issue on GitHub.
+# Generate the README.md file
+readme(repo)
+```
 
 ## License 📄
 
-Turbo Docs is released under the MIT License. See [LICENSE](LICENSE) for more information.
+Turbo Docs is released under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `turbo_docs-0.9.3/setup.py` & `turbo_docs-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="0.9.3",
+	version="1.0.0",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
 		"redbaron",
 		"gitpython",
     	"toml",
         "pathspec",
+        "llm-blocks",
 	],
 	entry_points={
 		"console_scripts": [
 			"turbo_docs=turbo_docs.generate:driver"
 		],
 	},
 	classifiers=[
```

### Comparing `turbo_docs-0.9.3/turbo_docs/commands/readme.py` & `turbo_docs-1.0.0/turbo_docs/commands/readme.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,10 +26,9 @@
     else:
         model = "gpt-4"
 
     response = openai_api.gpt_completion(template, {"repo": repo}, model)
     if response is None:
         print("Unable to generate README.md, it seems like you have uploaded too many tokens.")
     else:
-        print(response)
         with open(readme, "w", encoding="utf-8") as readme_file:
             readme_file.write(response)
```

### Comparing `turbo_docs-0.9.3/turbo_docs/generate.py` & `turbo_docs-1.0.0/turbo_docs/generate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,52 @@
 import click
 import pyperclip
 from turbo_docs.commands import readme as readme_module
+from turbo_docs.commands import docs as docs_module
 from turbo_docs.utils import directory, cli_options
 
 
 @click.command()
 @cli_options.copy
 @cli_options.readme
 @cli_options.gpt3
 def driver(
-        copy: bool,
-        readme: bool,
-        gpt3: bool,
+    copy: bool,
+    readme: bool,
+    gpt3: bool,
+    docs: bool,
 ) -> None:
     """
     Pull text from all files in the current directory and apply the following commands:
 
     'turbo_docs --copy' copies the text to clipboard
         Useful for wokring with ChatGPT
 
     'turbo_docs --readme' generates a README.md file
         Useful for keeping documentation up to date
+
+    'turbo_docs --gpt3' uses GPT-3.5-turbo-16k
+        Useful if you don't have GPT-4 access
+
+    'turbo_docs --docs' generates a docs for each file
+        Useful for keeping documentation up to date
     """
-    dir_text = directory.get_repo_text()
+    dir_text_dict = directory.get_repo_text_dict()
 
     if copy:
-        pyperclip.copy(dir_text)
+        pyperclip.copy(directory.convert_dict_to_string(dir_text_dict))
         print("Directory copied to clipboard")
 
     if readme:
-        readme_module.readme(dir_text, gpt3)
+        readme_text_dict = directory.remove_readme(dir_text_dict)
+        readme_text = directory.convert_dict_to_string(readme_text_dict)
+        readme_module.readme(readme_text, gpt3)
         print("Generated README.md")
 
 
-if __name__ == '__main__':
-    driver()
+    if docs:
+        docs_module.generate_docs(dir_text_dict, gpt3)
+        print("Generated documentation")
+
+
+if __name__ == "__main__":
+    driver()
```

### Comparing `turbo_docs-0.9.3/turbo_docs/utils/cli_options.py` & `turbo_docs-1.0.0/turbo_docs/utils/cli_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,7 +20,15 @@
 def gpt3(func: Callable) -> Callable:
     return click.option(
         '--gpt3',
         default=False,
         is_flag=True,
         help='Use the GPT-3.5 Turbo model'
     )(func)
+
+def docs(func: Callable) -> Callable:
+    return click.option(
+        '--docs',
+        default=False,
+        is_flag=True,
+        help='Generate documentation for all code files'
+    )(func)
```

### Comparing `turbo_docs-0.9.3/turbo_docs/utils/directory.py` & `turbo_docs-1.0.0/turbo_docs/utils/directory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 from pathspec import PathSpec
 from pathspec.patterns import GitWildMatchPattern
 from pathlib import Path
 import toml
 
+
 def read_text(path: Path) -> str:
-    """ 
-    Read the text from a file and return it as a string. We are assuming that
-    all non-textual files are in the ignore list in 'turbo_docs.toml'.
-    """
+    """Assuming all non-textual files are in the turbo_docs.toml ignore list"""
     try:
-        with open(path, 'r') as file:
-            return f'filename: {path.name}\npath: {path}\n\n{file.read()}\n\n'
+        with open(path, "r") as file:
+            return file.read()
+        
     except UnicodeDecodeError:
-        raise ValueError(f"File {path} contains non-textual content. Please add it to the ignore list in 'turbo_docs.toml'.")
+        print(f"File {path} contains non-textual content. Add to 'turbo_docs.toml' if this file should be ignored.")
+        with open(path, 'r', encoding='utf-8', errors='replace') as file:
+            return file.read()
+        
     except Exception as e:
         raise e
 
-def collect_text_from_files(dir_path: Path, pathspec: PathSpec) -> str:
-    """
-    Traverse through all files in a directory (and its subdirectories), 
-    collect the text from each file and return it as a single string.
-    """
-    result = ''
-    
+
+def collect_text_from_files(dir_path: Path, pathspec: PathSpec) -> dict:
+    """recursively collect text from all files in a directory"""
+    result = {}
     for path in dir_path.iterdir():
         if path.is_file():
             if not pathspec.match_file(str(path)):
-                result += read_text(path)
+                result[path] = read_text(path)
         elif path.is_dir():
-            result += collect_text_from_files(path, pathspec)
+            result.update(collect_text_from_files(path, pathspec))
 
     return result
 
 
-def get_repo_text():
-    """
-    Recursively get all text from files in the current directory, ignoring files 
-    specified in the exclude list in turbo_docs.toml
-
-    Text returned in the following format for each document:
-    filename: <filename>
-    path: <path>
-    <text>
-    ...
-    """
-    if not Path('turbo_docs.toml').exists():
+def get_repo_text_dict():
+    """Return a dictionary of all text in the current repo"""
+    if not Path("turbo_docs.toml").exists():
         ignored_patterns = []
         print("Warning: 'turbo_docs.toml' not found. All files will be included.")
     else:
-        config = toml.load('turbo_docs.toml')
-        ignored_patterns = config.get('ignore', [])
-    print(f"Ignoring files and folders matching the following patterns: {ignored_patterns}")
+        config = toml.load("turbo_docs.toml")
+        ignored_patterns = config.get("ignore", [])
+    print(
+        f"Ignoring files and folders matching the following patterns: {ignored_patterns}"
+    )
 
     pathspec = PathSpec.from_lines(GitWildMatchPattern, ignored_patterns)
-    text = collect_text_from_files(Path("."), pathspec)
+    return collect_text_from_files(Path("."), pathspec)
+
 
-    return text
+def remove_readme(file_dict: dict):
+    str_dict = {str(key): value for key, value in file_dict.items()}
+    return {
+        Path(key): value
+        for key, value in str_dict.items()
+        if not key.endswith("README.md")
+    }
+
+
+def convert_dict_to_string(file_dict: dict):
+    text = ""
+    for path, content in file_dict.items():
+        text += f"{path}:\n\n{content}\n\n"
+    return text
```

### Comparing `turbo_docs-0.9.3/turbo_docs/utils/openai_api.py` & `turbo_docs-1.0.0/turbo_docs/utils/openai_api.py`

 * *Files identical despite different names*

