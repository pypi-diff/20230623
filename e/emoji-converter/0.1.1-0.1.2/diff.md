# Comparing `tmp/emoji_converter-0.1.1.tar.gz` & `tmp/emoji_converter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emoji_converter-0.1.1.tar", max compression
+gzip compressed data, was "emoji_converter-0.1.2.tar", max compression
```

## Comparing `emoji_converter-0.1.1.tar` & `emoji_converter-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       58 2023-06-19 10:21:24.628659 emoji_converter-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      295 2023-06-19 10:21:24.636659 emoji_converter-0.1.1/emoji_converter/__init__.py
--rw-r--r--   0        0        0     3188 2023-06-19 10:21:24.644659 emoji_converter-0.1.1/emoji_converter/converter.py
--rw-r--r--   0        0        0      557 2023-06-23 09:30:16.833657 emoji_converter-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 emoji_converter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       58 2023-06-19 10:21:24.628659 emoji_converter-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      586 2023-06-23 09:34:55.023525 emoji_converter-0.1.2/README.md
+-rw-r--r--   0        0        0      295 2023-06-19 10:21:24.636659 emoji_converter-0.1.2/emoji_converter/__init__.py
+-rw-r--r--   0        0        0     3188 2023-06-19 10:21:24.644659 emoji_converter-0.1.2/emoji_converter/converter.py
+-rw-r--r--   0        0        0      555 2023-06-23 09:36:41.112209 emoji_converter-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1487 1970-01-01 00:00:00.000000 emoji_converter-0.1.2/PKG-INFO
```

### Comparing `emoji_converter-0.1.1/emoji_converter/converter.py` & `emoji_converter-0.1.2/emoji_converter/converter.py`

 * *Files identical despite different names*

### Comparing `emoji_converter-0.1.1/pyproject.toml` & `emoji_converter-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "emoji-converter"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Python package for converting text to emoji and emoji to text."
 authors = ["Le Xuan Manh <lexuanmanh101199@gmail.com>"]
 license = "MIT License"
-#readme = "README.rst"
+readme = "README.md"
 keywords = ['emoji', 'emoji converter', 'text to emoji', 'emoji to text']
 repository = "https://github.com/lemanh99/emoji-converter"
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.6"
 emoji = "^2.5.1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

