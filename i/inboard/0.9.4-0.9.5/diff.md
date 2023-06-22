# Comparing `tmp/inboard-0.9.4.tar.gz` & `tmp/inboard-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inboard-0.9.4.tar", max compression
+gzip compressed data, was "inboard-0.9.5.tar", max compression
```

## Comparing `inboard-0.9.4.tar` & `inboard-0.9.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1070 2021-05-16 23:32:55.632385 inboard-0.9.4/LICENSE
--rw-r--r--   0        0        0     2648 2021-05-16 23:32:55.632385 inboard-0.9.4/README.md
--rw-r--r--   0        0        0      647 2021-05-16 23:32:55.636385 inboard-0.9.4/inboard/__init__.py
--rw-r--r--   0        0        0        0 2021-05-16 23:32:55.636385 inboard-0.9.4/inboard/app/__init__.py
--rw-r--r--   0        0        0     1276 2021-05-16 23:32:55.636385 inboard-0.9.4/inboard/app/main_base.py
--rw-r--r--   0        0        0     1621 2021-05-16 23:32:55.636385 inboard-0.9.4/inboard/app/main_fastapi.py
--rw-r--r--   0        0        0     1916 2021-05-16 23:32:55.636385 inboard-0.9.4/inboard/app/main_starlette.py
--rw-r--r--   0        0        0      176 2021-05-16 23:32:55.636385 inboard-0.9.4/inboard/app/prestart.py
--rw-r--r--   0        0        0     2886 2021-05-16 23:32:55.636385 inboard-0.9.4/inboard/app/utilities_fastapi.py
--rw-r--r--   0        0        0     1572 2021-05-16 23:32:55.636385 inboard-0.9.4/inboard/app/utilities_starlette.py
--rw-r--r--   0        0        0     1363 2021-05-16 23:32:55.636385 inboard-0.9.4/inboard/gunicorn_conf.py
--rw-r--r--   0        0        0     3700 2021-05-16 23:32:55.636385 inboard-0.9.4/inboard/logging_conf.py
--rw-r--r--   0        0        0        0 2021-05-16 23:32:55.636385 inboard-0.9.4/inboard/py.typed
--rw-r--r--   0        0        0     4002 2021-05-16 23:32:55.636385 inboard-0.9.4/inboard/start.py
--rw-r--r--   0        0        0     1953 2021-05-16 23:32:55.636385 inboard-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     3698 2021-05-16 23:34:03.399501 inboard-0.9.4/setup.py
--rw-r--r--   0        0        0     4280 2021-05-16 23:34:03.399920 inboard-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2021-05-16 23:54:35.650633 inboard-0.9.5/LICENSE
+-rw-r--r--   0        0        0     2648 2021-05-16 23:54:35.650633 inboard-0.9.5/README.md
+-rw-r--r--   0        0        0    89898 2021-05-16 23:54:35.654633 inboard-0.9.5/docs/assets/images/inboard-logo.svg
+-rw-r--r--   0        0        0      647 2021-05-16 23:54:35.654633 inboard-0.9.5/inboard/__init__.py
+-rw-r--r--   0        0        0        0 2021-05-16 23:54:35.654633 inboard-0.9.5/inboard/app/__init__.py
+-rw-r--r--   0        0        0     1276 2021-05-16 23:54:35.654633 inboard-0.9.5/inboard/app/main_base.py
+-rw-r--r--   0        0        0     1621 2021-05-16 23:54:35.654633 inboard-0.9.5/inboard/app/main_fastapi.py
+-rw-r--r--   0        0        0     1916 2021-05-16 23:54:35.654633 inboard-0.9.5/inboard/app/main_starlette.py
+-rw-r--r--   0        0        0      176 2021-05-16 23:54:35.654633 inboard-0.9.5/inboard/app/prestart.py
+-rw-r--r--   0        0        0     2886 2021-05-16 23:54:35.654633 inboard-0.9.5/inboard/app/utilities_fastapi.py
+-rw-r--r--   0        0        0     1572 2021-05-16 23:54:35.654633 inboard-0.9.5/inboard/app/utilities_starlette.py
+-rw-r--r--   0        0        0     1363 2021-05-16 23:54:35.654633 inboard-0.9.5/inboard/gunicorn_conf.py
+-rw-r--r--   0        0        0     3700 2021-05-16 23:54:35.654633 inboard-0.9.5/inboard/logging_conf.py
+-rw-r--r--   0        0        0        0 2021-05-16 23:54:35.654633 inboard-0.9.5/inboard/py.typed
+-rw-r--r--   0        0        0     4002 2021-05-16 23:54:35.654633 inboard-0.9.5/inboard/start.py
+-rw-r--r--   0        0        0     1992 2021-05-16 23:54:35.654633 inboard-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     3698 2021-05-16 23:55:41.973160 inboard-0.9.5/setup.py
+-rw-r--r--   0        0        0     4280 2021-05-16 23:55:41.973556 inboard-0.9.5/PKG-INFO
```

### Comparing `inboard-0.9.4/LICENSE` & `inboard-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `inboard-0.9.4/README.md` & `inboard-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `inboard-0.9.4/inboard/__init__.py` & `inboard-0.9.5/inboard/__init__.py`

 * *Files identical despite different names*

### Comparing `inboard-0.9.4/inboard/app/main_base.py` & `inboard-0.9.5/inboard/app/main_base.py`

 * *Files identical despite different names*

### Comparing `inboard-0.9.4/inboard/app/main_fastapi.py` & `inboard-0.9.5/inboard/app/main_fastapi.py`

 * *Files identical despite different names*

### Comparing `inboard-0.9.4/inboard/app/main_starlette.py` & `inboard-0.9.5/inboard/app/main_starlette.py`

 * *Files identical despite different names*

### Comparing `inboard-0.9.4/inboard/app/utilities_fastapi.py` & `inboard-0.9.5/inboard/app/utilities_fastapi.py`

 * *Files identical despite different names*

### Comparing `inboard-0.9.4/inboard/app/utilities_starlette.py` & `inboard-0.9.5/inboard/app/utilities_starlette.py`

 * *Files identical despite different names*

### Comparing `inboard-0.9.4/inboard/gunicorn_conf.py` & `inboard-0.9.5/inboard/gunicorn_conf.py`

 * *Files identical despite different names*

### Comparing `inboard-0.9.4/inboard/logging_conf.py` & `inboard-0.9.5/inboard/logging_conf.py`

 * *Files identical despite different names*

### Comparing `inboard-0.9.4/inboard/start.py` & `inboard-0.9.5/inboard/start.py`

 * *Files identical despite different names*

### Comparing `inboard-0.9.4/pyproject.toml` & `inboard-0.9.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 [tool.isort]
 profile = "black"
 src_paths = ["inboard", "tests"]
 
 [tool.poetry]
 name = "inboard"
-version = "0.9.4"
+version = "0.9.5"
 description = "Docker images and utilities to power your Python APIs and help you ship faster."
 authors = ["Brendon Smith <br3ndonland@protonmail.com>"]
 license = "MIT"
 homepage = "https://github.com/br3ndonland/inboard"
 repository = "https://github.com/br3ndonland/inboard"
 documentation = "https://inboard.bws.bio"
 readme = "README.md"
-include = ["inboard/py.typed"]
+include = ["docs/assets/images/inboard-logo.svg", "inboard/py.typed"]
 keywords = ["asgi", "docker", "fastapi", "gunicorn", "uvicorn"]
 classifiers = [
   "Natural Language :: English",
   "Topic :: Internet :: Log Analysis",
   "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
   "Topic :: Internet :: WWW/HTTP :: WSGI",
   "Topic :: Software Development :: Libraries :: Application Frameworks",
@@ -52,15 +52,15 @@
 [tool.poetry.extras]
 all = ["fastapi", "mkdocs-material", "toml"]
 docs = ["mkdocs-material"]
 fastapi = ["fastapi", "toml"]
 starlette = ["starlette"]
 
 [tool.poetry.urls]
-docker = "https://github.com/users/br3ndonland/packages/container/package/inboard"
+Docker = "https://github.com/users/br3ndonland/packages/container/package/inboard"
 
 [tool.pytest.ini_options]
 addopts = "--cov=inboard -q"
 minversion = "6.0"
 testpaths = ["tests"]
 
 [build-system]
```

### Comparing `inboard-0.9.4/setup.py` & `inboard-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 {'all': ['fastapi>=0.64,<0.65', 'mkdocs-material>=7,<8', 'toml>=0.10'],
  'docs': ['mkdocs-material>=7,<8'],
  'fastapi': ['fastapi>=0.64,<0.65', 'toml>=0.10'],
  'starlette': ['starlette>=0.13,<0.14']}
 
 setup_kwargs = {
     'name': 'inboard',
-    'version': '0.9.4',
+    'version': '0.9.5',
     'description': 'Docker images and utilities to power your Python APIs and help you ship faster.',
     'long_description': '# 🚢 inboard 🐳\n\n<img src="docs/assets/images/inboard-logo.svg" alt="inboard logo" width="90%" />\n\n_Docker images and utilities to power your Python APIs and help you ship faster._\n\n[![PyPI](https://img.shields.io/pypi/v/inboard?color=success)](https://pypi.org/project/inboard/)\n[![GitHub Container Registry](https://img.shields.io/badge/github%20container%20registry-inboard-success)](https://github.com/users/br3ndonland/packages/container/package/inboard)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)\n\n[![builds](https://github.com/br3ndonland/inboard/workflows/builds/badge.svg)](https://github.com/br3ndonland/inboard/actions)\n[![hooks](https://github.com/br3ndonland/inboard/workflows/hooks/badge.svg)](https://github.com/br3ndonland/inboard/actions)\n[![tests](https://github.com/br3ndonland/inboard/workflows/tests/badge.svg)](https://github.com/br3ndonland/inboard/actions)\n[![codecov](https://codecov.io/gh/br3ndonland/inboard/branch/develop/graph/badge.svg)](https://codecov.io/gh/br3ndonland/inboard)\n\n[![Mentioned in Awesome FastAPI](https://awesome.re/mentioned-badge-flat.svg)](https://github.com/mjhea0/awesome-fastapi)\n\n## Description\n\nThis repository provides [Docker images](https://github.com/users/br3ndonland/packages/container/package/inboard) and a [PyPI package](https://pypi.org/project/inboard/) with useful utilities for Python web servers. It runs [Uvicorn with Gunicorn](https://www.uvicorn.org/), and can be used to build applications with [Starlette](https://www.starlette.io/) and [FastAPI](https://fastapi.tiangolo.com/).\n\n## Quickstart\n\n[Get started with Docker](https://www.docker.com/get-started), pull and run an image, and try an API endpoint.\n\n```sh\ndocker pull ghcr.io/br3ndonland/inboard\ndocker run -d -p 80:80 ghcr.io/br3ndonland/inboard\nhttp :80  # HTTPie: https://httpie.io/\n```\n\n## Documentation\n\nDocumentation is built with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/), deployed on [Vercel](https://vercel.com/), and available at [inboard.bws.bio](https://inboard.bws.bio) and [inboard.vercel.app](https://inboard.vercel.app).\n\n[Vercel build configuration](https://vercel.com/docs/build-step):\n\n- Build command: `python3 -m pip install \'mkdocs-material>=7.0.0,<=8.0.0\' && mkdocs build --site-dir public`\n- Output directory: `public` (default)\n\n[Vercel site configuration](https://vercel.com/docs/configuration) is specified in _[vercel.json](vercel.json)_.\n',
     'author': 'Brendon Smith',
     'author_email': 'br3ndonland@protonmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/br3ndonland/inboard',
```

### Comparing `inboard-0.9.4/PKG-INFO` & `inboard-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inboard
-Version: 0.9.4
+Version: 0.9.5
 Summary: Docker images and utilities to power your Python APIs and help you ship faster.
 Home-page: https://github.com/br3ndonland/inboard
 License: MIT
 Keywords: asgi,docker,fastapi,gunicorn,uvicorn
 Author: Brendon Smith
 Author-email: br3ndonland@protonmail.com
 Requires-Python: >=3.8,<4.0
@@ -27,16 +27,16 @@
 Requires-Dist: fastapi (>=0.64,<0.65); extra == "all" or extra == "fastapi"
 Requires-Dist: gunicorn (>=20,<21)
 Requires-Dist: mkdocs-material (>=7,<8); extra == "all" or extra == "docs"
 Requires-Dist: starlette (>=0.13,<0.14); extra == "starlette"
 Requires-Dist: toml (>=0.10); extra == "all" or extra == "fastapi"
 Requires-Dist: uvicorn[standard] (>=0.13,<0.14)
 Project-URL: Documentation, https://inboard.bws.bio
+Project-URL: Docker, https://github.com/users/br3ndonland/packages/container/package/inboard
 Project-URL: Repository, https://github.com/br3ndonland/inboard
-Project-URL: docker, https://github.com/users/br3ndonland/packages/container/package/inboard
 Description-Content-Type: text/markdown
 
 # 🚢 inboard 🐳
 
 <img src="docs/assets/images/inboard-logo.svg" alt="inboard logo" width="90%" />
 
 _Docker images and utilities to power your Python APIs and help you ship faster._
```

