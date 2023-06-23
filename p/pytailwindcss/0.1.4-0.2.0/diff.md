# Comparing `tmp/pytailwindcss-0.1.4.tar.gz` & `tmp/pytailwindcss-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytailwindcss-0.1.4.tar", last modified: Mon Feb 14 11:56:27 2022, max compression
+gzip compressed data, was "pytailwindcss-0.2.0.tar", max compression
```

## Comparing `pytailwindcss-0.1.4.tar` & `pytailwindcss-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1078 2021-12-19 19:22:21.532111 pytailwindcss-0.1.4/LICENSE
--rw-r--r--   0        0        0     3306 2021-12-22 21:15:41.589587 pytailwindcss-0.1.4/README.md
--rw-r--r--   0        0        0     1157 2022-02-14 11:54:42.129415 pytailwindcss-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2549 2021-12-22 21:09:00.046707 pytailwindcss-0.1.4/src/pytailwindcss/__init__.py
--rw-r--r--   0        0        0      382 2021-12-19 20:57:58.758176 pytailwindcss-0.1.4/src/pytailwindcss/__main__.py
--rw-r--r--   0        0        0      191 2021-12-19 19:59:59.444096 pytailwindcss-0.1.4/src/pytailwindcss/exceptions.py
--rw-r--r--   0        0        0     2663 2022-02-14 11:54:09.012418 pytailwindcss-0.1.4/src/pytailwindcss/installation.py
--rw-r--r--   0        0        0     1281 2021-12-22 20:36:42.516449 pytailwindcss-0.1.4/src/pytailwindcss/utils.py
--rw-r--r--   0        0        0     4197 2022-02-14 11:56:27.605883 pytailwindcss-0.1.4/setup.py
--rw-r--r--   0        0        0     4183 2022-02-14 11:56:27.606213 pytailwindcss-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-23 20:23:51.702866 pytailwindcss-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3525 2023-06-23 21:20:24.241588 pytailwindcss-0.2.0/README.md
+-rw-r--r--   0        0        0     1156 2023-06-23 21:22:37.439245 pytailwindcss-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2563 2023-06-23 20:39:25.361541 pytailwindcss-0.2.0/src/pytailwindcss/__init__.py
+-rw-r--r--   0        0        0      482 2023-06-23 21:20:24.458021 pytailwindcss-0.2.0/src/pytailwindcss/__main__.py
+-rw-r--r--   0        0        0      191 2023-06-23 20:23:51.703949 pytailwindcss-0.2.0/src/pytailwindcss/exceptions.py
+-rw-r--r--   0        0        0     2663 2023-06-23 20:23:51.704060 pytailwindcss-0.2.0/src/pytailwindcss/installation.py
+-rw-r--r--   0        0        0     1307 2023-06-23 20:31:08.537606 pytailwindcss-0.2.0/src/pytailwindcss/utils.py
+-rw-r--r--   0        0        0     4604 1970-01-01 00:00:00.000000 pytailwindcss-0.2.0/PKG-INFO
```

### Comparing `pytailwindcss-0.1.4/LICENSE` & `pytailwindcss-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytailwindcss-0.1.4/README.md` & `pytailwindcss-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,39 +32,47 @@
 
 1. Install `tailwindcss` via `pip` by executing the following command:
 
    ```
    pip install pytailwindcss
    ```
 
-2. The `tailwindcss` command should now be available in your terminal. Try to run it:
+2. [Optional] Preinstall `tailwindcss` binary by running the following command:
+
+   ```
+   tailwindcss_install
+   ```
+
+   If you skip this step, the binary will be downloaded on the first run of `tailwindcss` command.
+
+3. The `tailwindcss` command should now be available in your terminal. Try to run it:
 
    ```
    tailwindcss
    ```
 
    If the installation was successful, you should see the message about binary being downloaded on the first run. When download is complete, you should see the help output for the `tailwindcss` command. Use `tailwindcss`
    to create a new project or work with an existing *Tailwind CSS* project.
 
-3. Let's create a new project. Go to the directory where you want to host your *Tailwind CSS* project and initialize it
+4. Let's create a new project. Go to the directory where you want to host your *Tailwind CSS* project and initialize it
    by running:
 
    ```
    tailwindcss init
    ```
 
    This command will create the default *tailwind.config.js* file.
 
-4. Start a watcher by running:
+5. Start a watcher by running:
 
    ```
    tailwindcss -i input.css -o output.css --watch
    ```
 
-5. Compile and minify your CSS for production by running:
+6. Compile and minify your CSS for production by running:
 
    ```
    tailwindcss -i input.css -o output.css --minify
    ```
 
 You got it. Please refer to [official Tailwind documentation](https://tailwindcss.com/docs) for more information on
 using *Tailwind CSS* and its CLI.
```

### Comparing `pytailwindcss-0.1.4/pyproject.toml` & `pytailwindcss-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytailwindcss"
-version = "0.1.4"
+version = "0.2.0"
 description = "Standalone Tailwind CSS CLI, installable via pip. Use Tailwind CSS without Node.js."
 authors = ["Tim Kamanin <tim@timonweb.com>"]
 homepage = "https://github.com/timonweb/pytailwindcss"
 readme = "README.md"
 license = "MIT"
 keywords = ["cli", "tailwind", "css"]
 classifiers = [
@@ -22,21 +22,19 @@
 
 packages = [
     { include = "pytailwindcss", from = "src" }
 ]
 
 [tool.poetry.scripts]
 tailwindcss = "pytailwindcss.__main__:main"
+tailwindcss_install = "pytailwindcss.__main__:install"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-isort = "^5.10.1"
-flake8 = "^4.0.1"
-black = "^21.12b0"
-pre-commit = "^2.16.0"
+pytest = "^7.4.0"
+pre-commit = "^3.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pytailwindcss-0.1.4/src/pytailwindcss/__init__.py` & `pytailwindcss-0.2.0/src/pytailwindcss/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     @param version: sets version of the tailwindcss binary.
     Defaults to the 'latest' if not provided.
     """
     if version is None:
         version = env.get("TAILWINDCSS_VERSION", "latest") if env else "latest"
 
     if bin_path is None:
-        bin_path = get_bin_path()
+        bin_path = get_bin_path(version)
 
     if auto_install and not bin_path.exists():
         install(version, bin_path)
 
     try:
         tailwindcss_cli_args = format_cli_args(tailwindcss_cli_args or "")
         kwargs = make_subprocess_run_kwargs(cwd, env, live_output)
@@ -61,9 +61,9 @@
     @param version: sets version of the tailwindcss binary. Defaults to the 'latest' if not provided.
     @param bin_path: sets bin path for the tailwindcss binary. Sets default location is not provided.
     @return:
     """
     if version is None:
         version = "latest"
     if bin_path is None:
-        bin_path = get_bin_path()
+        bin_path = get_bin_path(version)
     return install_binary(version, ensure_is_pathlib_path(bin_path))
```

### Comparing `pytailwindcss-0.1.4/src/pytailwindcss/installation.py` & `pytailwindcss-0.2.0/src/pytailwindcss/installation.py`

 * *Files identical despite different names*

### Comparing `pytailwindcss-0.1.4/src/pytailwindcss/utils.py` & `pytailwindcss-0.2.0/src/pytailwindcss/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     Formats cli_args as list if they're string.
     """
     if isinstance(cli_args, str):
         return shlex.split(cli_args)
     return cli_args
 
 
-def get_bin_path():
+def get_bin_path(version="latest"):
     """
     Returns a path for the tailwindcss binary.
     """
-    return pathlib.Path(__file__).parent.resolve() / "bin" / "tailwindcss"
+    return pathlib.Path(__file__).parent.resolve() / "bin" / version / "tailwindcss"
 
 
 def ensure_is_pathlib_path(path):
     if isinstance(path, str):
         return pathlib.Path(path)
     return path
```

### Comparing `pytailwindcss-0.1.4/setup.py` & `pytailwindcss-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,125 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pytailwindcss
+Version: 0.2.0
+Summary: Standalone Tailwind CSS CLI, installable via pip. Use Tailwind CSS without Node.js.
+Home-page: https://github.com/timonweb/pytailwindcss
+License: MIT
+Keywords: cli,tailwind,css
+Author: Tim Kamanin
+Author-email: tim@timonweb.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Standalone Tailwind CSS CLI, installable via pip
 
-packages = \
-['pytailwindcss']
+Use *Tailwind CSS* without *Node.js* and install it via pip.
 
-package_data = \
-{'': ['*']}
-
-entry_points = \
-{'console_scripts': ['tailwindcss = pytailwindcss.__main__:main']}
-
-setup_kwargs = {
-    'name': 'pytailwindcss',
-    'version': '0.1.4',
-    'description': 'Standalone Tailwind CSS CLI, installable via pip. Use Tailwind CSS without Node.js.',
-    'long_description': "# Standalone Tailwind CSS CLI, installable via pip\n\nUse *Tailwind CSS* without *Node.js* and install it via pip.\n\n## Why\n\n*Tailwind CSS* is notoriously dependent on *Node.js*. If you're a *Python* developer, this dependency may not be welcome\nin your team, your Docker container, or your inner circle.\n\nThe *Tailwind CSS* team recently announced a new standalone CLI build that gives you the full power of *Tailwind CLI* in\na self-contained executable — no *Node.js* or `npm` required.\n\nHowever, installing such a standalone CLI isn't as easy as running `npm install`, the installation command for *Node.js*\n.\n\nThat's why I decided to make it as simple as running `pip install` command. As a result you can install the standalone *\nTailwind CLI* via `pip` by running the following command:\n\n```bash\npip install pytailwindcss\n```\n\nNow you can run `tailwindcss` in your terminal as:\n\n```\ntailwindcss -i input.css -o output.css --minify\n```\n\nVoila!\n\n## Get started\n\n1. Install `tailwindcss` via `pip` by executing the following command:\n\n   ```\n   pip install pytailwindcss\n   ```\n\n2. The `tailwindcss` command should now be available in your terminal. Try to run it:\n\n   ```\n   tailwindcss\n   ```\n\n   If the installation was successful, you should see the message about binary being downloaded on the first run. When download is complete, you should see the help output for the `tailwindcss` command. Use `tailwindcss`\n   to create a new project or work with an existing *Tailwind CSS* project.\n\n3. Let's create a new project. Go to the directory where you want to host your *Tailwind CSS* project and initialize it\n   by running:\n\n   ```\n   tailwindcss init\n   ```\n\n   This command will create the default *tailwind.config.js* file.\n\n4. Start a watcher by running:\n\n   ```\n   tailwindcss -i input.css -o output.css --watch\n   ```\n\n5. Compile and minify your CSS for production by running:\n\n   ```\n   tailwindcss -i input.css -o output.css --minify\n   ```\n\nYou got it. Please refer to [official Tailwind documentation](https://tailwindcss.com/docs) for more information on\nusing *Tailwind CSS* and its CLI.\n\n## Caveats\n\nIt's not all roses, though. Giving up *Node.js* means you won't be able to install plugins or additional dependencies for\nyour *Tailwind CSS* setup. At the same time, that might not be a dealbreaker. You can still customize *Tailwind CSS* via\nthe *tailwind.config.js* file. And the standalone build also comes with all official *Tailwind CSS* plugins\nlike `@tailwindcss/aspect-ratio`, `@tailwindcss/forms`, `@tailwindcss/line-clamp`, and `@tailwindcss/typography`. So in\n90% of *Tailwind CSS* usage cases you should be covered, and the setup is so simplified now.\n\nHere is what the *Tailwind CSS* team says about going the standalone *Tailwind CSS* route:\n> If you’re working on a project where you don’t otherwise need *Node.js* or `npm`, the standalone build can be a great choice. If Tailwind was the only reason you had a package.json file, this is probably going to feel like a nicer solution.\n\n## Bugs and suggestions\n\nIf you have found a bug, please use the issue tracker on GitHub.\n\n[https://github.com/timonweb/pytailwindcss/issues](https://github.com/timonweb/pytailwindcss/issues)\n\n2021 (c) [Tim Kamanin - A Full Stack Django and Wagtail Developer](https://timonweb.com)\n",
-    'author': 'Tim Kamanin',
-    'author_email': 'tim@timonweb.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/timonweb/pytailwindcss',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+## Why
 
+*Tailwind CSS* is notoriously dependent on *Node.js*. If you're a *Python* developer, this dependency may not be welcome
+in your team, your Docker container, or your inner circle.
+
+The *Tailwind CSS* team recently announced a new standalone CLI build that gives you the full power of *Tailwind CLI* in
+a self-contained executable — no *Node.js* or `npm` required.
+
+However, installing such a standalone CLI isn't as easy as running `npm install`, the installation command for *Node.js*
+.
+
+That's why I decided to make it as simple as running `pip install` command. As a result you can install the standalone *
+Tailwind CLI* via `pip` by running the following command:
+
+```bash
+pip install pytailwindcss
+```
+
+Now you can run `tailwindcss` in your terminal as:
+
+```
+tailwindcss -i input.css -o output.css --minify
+```
+
+Voila!
+
+## Get started
+
+1. Install `tailwindcss` via `pip` by executing the following command:
+
+   ```
+   pip install pytailwindcss
+   ```
+
+2. [Optional] Preinstall `tailwindcss` binary by running the following command:
+
+   ```
+   tailwindcss_install
+   ```
+
+   If you skip this step, the binary will be downloaded on the first run of `tailwindcss` command.
+
+3. The `tailwindcss` command should now be available in your terminal. Try to run it:
+
+   ```
+   tailwindcss
+   ```
+
+   If the installation was successful, you should see the message about binary being downloaded on the first run. When download is complete, you should see the help output for the `tailwindcss` command. Use `tailwindcss`
+   to create a new project or work with an existing *Tailwind CSS* project.
+
+4. Let's create a new project. Go to the directory where you want to host your *Tailwind CSS* project and initialize it
+   by running:
+
+   ```
+   tailwindcss init
+   ```
+
+   This command will create the default *tailwind.config.js* file.
+
+5. Start a watcher by running:
+
+   ```
+   tailwindcss -i input.css -o output.css --watch
+   ```
+
+6. Compile and minify your CSS for production by running:
+
+   ```
+   tailwindcss -i input.css -o output.css --minify
+   ```
+
+You got it. Please refer to [official Tailwind documentation](https://tailwindcss.com/docs) for more information on
+using *Tailwind CSS* and its CLI.
+
+## Caveats
+
+It's not all roses, though. Giving up *Node.js* means you won't be able to install plugins or additional dependencies for
+your *Tailwind CSS* setup. At the same time, that might not be a dealbreaker. You can still customize *Tailwind CSS* via
+the *tailwind.config.js* file. And the standalone build also comes with all official *Tailwind CSS* plugins
+like `@tailwindcss/aspect-ratio`, `@tailwindcss/forms`, `@tailwindcss/line-clamp`, and `@tailwindcss/typography`. So in
+90% of *Tailwind CSS* usage cases you should be covered, and the setup is so simplified now.
+
+Here is what the *Tailwind CSS* team says about going the standalone *Tailwind CSS* route:
+> If you’re working on a project where you don’t otherwise need *Node.js* or `npm`, the standalone build can be a great choice. If Tailwind was the only reason you had a package.json file, this is probably going to feel like a nicer solution.
+
+## Bugs and suggestions
+
+If you have found a bug, please use the issue tracker on GitHub.
+
+[https://github.com/timonweb/pytailwindcss/issues](https://github.com/timonweb/pytailwindcss/issues)
+
+2021 (c) [Tim Kamanin - A Full Stack Django and Wagtail Developer](https://timonweb.com)
 
-setup(**setup_kwargs)
```

