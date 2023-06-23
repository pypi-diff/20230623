# Comparing `tmp/openai_function_call-0.0.3.tar.gz` & `tmp/openai_function_call-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function_call-0.0.3.tar", max compression
+gzip compressed data, was "openai_function_call-0.0.4.tar", max compression
```

## Comparing `openai_function_call-0.0.3.tar` & `openai_function_call-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2023-06-17 12:35:29.432156 openai_function_call-0.0.3/LICENSE
--rw-r--r--   0        0        0     3242 2023-06-23 03:49:25.348705 openai_function_call-0.0.3/README.md
--rw-r--r--   0        0        0     4155 2023-06-23 03:49:25.348966 openai_function_call-0.0.3/openai_function_call/__init__.py
--rw-r--r--   0        0        0      445 2023-06-23 03:54:17.314715 openai_function_call-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3850 1970-01-01 00:00:00.000000 openai_function_call-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-23 05:04:41.352474 openai_function_call-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3346 2023-06-23 05:04:41.352474 openai_function_call-0.0.4/README.md
+-rw-r--r--   0        0        0     4155 2023-06-23 05:04:41.352474 openai_function_call-0.0.4/openai_function_call/__init__.py
+-rw-r--r--   0        0        0      445 2023-06-23 05:04:41.352474 openai_function_call-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3954 1970-01-01 00:00:00.000000 openai_function_call-0.0.4/PKG-INFO
```

### Comparing `openai_function_call-0.0.3/LICENSE` & `openai_function_call-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.0.3/README.md` & `openai_function_call-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,46 @@
-# OpenAI Function Call and Pydantic Integration Module
+# Pydantic is all you need: An OpenAI Function Call Pydantic Integration Module
 
-This Python module provides a powerful and efficient approach to output parsing when interacting with OpenAI's Function Call API. It leverages the data validation capabilities of the Pydantic library to handle output parsing in a more structured and reliable manner. This README will guide you through the installation, usage, and contribution processes of this module.
+We try to provides a powerful and efficient approach to output parsing when interacting with OpenAI's Function Call API. One that is framework agnostic and minimizes any dependencies. It leverages the data validation capabilities of the Pydantic library to handle output parsing in a more structured and reliable manner.
 If you have any feedback, leave an issue or hit me up on [twitter](https://twitter.com/jxnlco). 
 
+This repo also contains a range of examples I've used in experimetnation and in production and I welcome new contributions for different types of schemas.
 
 ## Installation
 
+```python
+pip install openai_function_call
+```
+
+## Contributing
+
 To get started, clone the repository
 
 ```bash
 git clone https://github.com/jxnl/openai_function_call.git
 ```
 
 Next, install the necessary Python packages from the requirements.txt file:
 
 ```bash
 pip install -r requirements.txt
 ```
 
-## Contributing
-
-Your contributions are welcome! If you have great examples or find neat patterns, clone the repo and add another example. 
-The goal is to find great patterns and cool examples to highlight.
-
-If you encounter any issues or want to provide feedback, you can create an issue in this repository. You can also reach out to me on Twitter at @jxnlco.
-
 ### Poetry
 
 We also use poetry if you'd like
 
 ```bash
 poetry build
 ```
 
-Note that there's no separate pip install command for this module. Simply copy and paste the module's code into your application.
+Your contributions are welcome! If you have great examples or find neat patterns, clone the repo and add another example.
+Check out the issues for any ideas if you want to learn. The goal is to find great patterns and cool examples to highlight.
+
+If you encounter any issues or want to provide feedback, you can create an issue in this repository. You can also reach out to me on Twitter at @jxnlco.
 
 ## Usage
 
 This module simplifies the interaction with the OpenAI API, enabling a more structured and predictable conversation with the AI. Below are examples showcasing the use of function calls and schemas with OpenAI and Pydantic.
 
 ### Example 1: Function Calls
```

### Comparing `openai_function_call-0.0.3/openai_function_call/__init__.py` & `openai_function_call-0.0.4/openai_function_call/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.0.3/PKG-INFO` & `openai_function_call-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 Metadata-Version: 2.1
 Name: openai-function-call
-Version: 0.0.3
+Version: 0.0.4
 Summary: Helper functions that allow us to improve openai's function_call ergonomics
 License: MIT
 Author: Jason
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Description-Content-Type: text/markdown
 
-# OpenAI Function Call and Pydantic Integration Module
+# Pydantic is all you need: An OpenAI Function Call Pydantic Integration Module
 
-This Python module provides a powerful and efficient approach to output parsing when interacting with OpenAI's Function Call API. It leverages the data validation capabilities of the Pydantic library to handle output parsing in a more structured and reliable manner. This README will guide you through the installation, usage, and contribution processes of this module.
+We try to provides a powerful and efficient approach to output parsing when interacting with OpenAI's Function Call API. One that is framework agnostic and minimizes any dependencies. It leverages the data validation capabilities of the Pydantic library to handle output parsing in a more structured and reliable manner.
 If you have any feedback, leave an issue or hit me up on [twitter](https://twitter.com/jxnlco). 
 
+This repo also contains a range of examples I've used in experimetnation and in production and I welcome new contributions for different types of schemas.
 
 ## Installation
 
+```python
+pip install openai_function_call
+```
+
+## Contributing
+
 To get started, clone the repository
 
 ```bash
 git clone https://github.com/jxnl/openai_function_call.git
 ```
 
 Next, install the necessary Python packages from the requirements.txt file:
 
 ```bash
 pip install -r requirements.txt
 ```
 
-## Contributing
-
-Your contributions are welcome! If you have great examples or find neat patterns, clone the repo and add another example. 
-The goal is to find great patterns and cool examples to highlight.
-
-If you encounter any issues or want to provide feedback, you can create an issue in this repository. You can also reach out to me on Twitter at @jxnlco.
-
 ### Poetry
 
 We also use poetry if you'd like
 
 ```bash
 poetry build
 ```
 
-Note that there's no separate pip install command for this module. Simply copy and paste the module's code into your application.
+Your contributions are welcome! If you have great examples or find neat patterns, clone the repo and add another example.
+Check out the issues for any ideas if you want to learn. The goal is to find great patterns and cool examples to highlight.
+
+If you encounter any issues or want to provide feedback, you can create an issue in this repository. You can also reach out to me on Twitter at @jxnlco.
 
 ## Usage
 
 This module simplifies the interaction with the OpenAI API, enabling a more structured and predictable conversation with the AI. Below are examples showcasing the use of function calls and schemas with OpenAI and Pydantic.
 
 ### Example 1: Function Calls
```

