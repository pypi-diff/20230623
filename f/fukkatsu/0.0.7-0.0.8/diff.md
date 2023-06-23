# Comparing `tmp/fukkatsu-0.0.7.tar.gz` & `tmp/fukkatsu-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fukkatsu-0.0.7.tar", last modified: Sun Jun 18 22:32:09 2023, max compression
+gzip compressed data, was "fukkatsu-0.0.8.tar", last modified: Fri Jun 23 00:15:05 2023, max compression
```

## Comparing `fukkatsu-0.0.7.tar` & `fukkatsu-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 22:32:09.152033 fukkatsu-0.0.7/
--rw-rw-rw-   0        0        0     1387 2023-06-18 20:59:20.000000 fukkatsu-0.0.7/CHANGELOG.md
--rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0    12171 2023-06-18 22:32:09.137523 fukkatsu-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    11530 2023-06-13 23:47:46.000000 fukkatsu-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 22:32:09.063719 fukkatsu-0.0.7/fukkatsu/
--rw-rw-rw-   0        0        0    10373 2023-06-18 22:31:09.000000 fukkatsu-0.0.7/fukkatsu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:32:09.104277 fukkatsu-0.0.7/fukkatsu/memory/
--rw-rw-rw-   0        0        0       75 2023-05-20 04:07:03.000000 fukkatsu-0.0.7/fukkatsu/memory/__init__.py
--rw-rw-rw-   0        0        0      663 2023-05-20 04:07:01.000000 fukkatsu-0.0.7/fukkatsu/memory/manage.py
--rw-rw-rw-   0        0        0       23 2023-05-20 04:07:01.000000 fukkatsu-0.0.7/fukkatsu/memory/short.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:32:09.120327 fukkatsu-0.0.7/fukkatsu/observer/
--rw-rw-rw-   0        0        0       40 2023-06-15 23:48:34.000000 fukkatsu-0.0.7/fukkatsu/observer/__init__.py
--rw-rw-rw-   0        0        0     1062 2023-06-18 20:00:23.000000 fukkatsu-0.0.7/fukkatsu/observer/tracker.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:32:09.137523 fukkatsu-0.0.7/fukkatsu/utils/
--rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.7/fukkatsu/utils/__init__.py
--rw-rw-rw-   0        0        0     4082 2023-06-12 22:53:43.000000 fukkatsu-0.0.7/fukkatsu/utils/helper.py
--rw-rw-rw-   0        0        0     3242 2023-06-18 22:31:09.000000 fukkatsu-0.0.7/fukkatsu/utils/medic.py
--rw-rw-rw-   0        0        0     2779 2023-06-14 23:23:55.000000 fukkatsu-0.0.7/fukkatsu/utils/prompt.py
-drwxrwxrwx   0        0        0        0 2023-06-18 22:32:09.094939 fukkatsu-0.0.7/fukkatsu.egg-info/
--rw-rw-rw-   0        0        0    12171 2023-06-18 22:32:08.000000 fukkatsu-0.0.7/fukkatsu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-06-18 22:32:08.000000 fukkatsu-0.0.7/fukkatsu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 22:32:08.000000 fukkatsu-0.0.7/fukkatsu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-18 22:32:08.000000 fukkatsu-0.0.7/fukkatsu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-18 22:32:08.000000 fukkatsu-0.0.7/fukkatsu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 22:32:09.152033 fukkatsu-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1086 2023-06-18 20:55:47.000000 fukkatsu-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:15:05.842525 fukkatsu-0.0.8/
+-rw-rw-rw-   0        0        0     1387 2023-06-18 20:59:20.000000 fukkatsu-0.0.8/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    34713 2023-06-23 00:15:05.826902 fukkatsu-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    34072 2023-06-22 18:47:10.000000 fukkatsu-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 00:15:05.733149 fukkatsu-0.0.8/fukkatsu/
+-rw-rw-rw-   0        0        0    14328 2023-06-23 00:04:08.000000 fukkatsu-0.0.8/fukkatsu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:15:05.780022 fukkatsu-0.0.8/fukkatsu/memory/
+-rw-rw-rw-   0        0        0       75 2023-05-20 04:07:03.000000 fukkatsu-0.0.8/fukkatsu/memory/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-05-20 04:07:01.000000 fukkatsu-0.0.8/fukkatsu/memory/manage.py
+-rw-rw-rw-   0        0        0       23 2023-05-20 04:07:01.000000 fukkatsu-0.0.8/fukkatsu/memory/short.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:15:05.795649 fukkatsu-0.0.8/fukkatsu/observer/
+-rw-rw-rw-   0        0        0       40 2023-06-15 23:48:34.000000 fukkatsu-0.0.8/fukkatsu/observer/__init__.py
+-rw-rw-rw-   0        0        0     1064 2023-06-21 22:36:45.000000 fukkatsu-0.0.8/fukkatsu/observer/tracker.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:15:05.811275 fukkatsu-0.0.8/fukkatsu/utils/
+-rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.8/fukkatsu/utils/__init__.py
+-rw-rw-rw-   0        0        0     4948 2023-06-21 01:01:09.000000 fukkatsu-0.0.8/fukkatsu/utils/helper.py
+-rw-rw-rw-   0        0        0     4300 2023-06-23 00:04:08.000000 fukkatsu-0.0.8/fukkatsu/utils/medic.py
+-rw-rw-rw-   0        0        0     3812 2023-06-21 00:15:16.000000 fukkatsu-0.0.8/fukkatsu/utils/prompt.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:15:05.764400 fukkatsu-0.0.8/fukkatsu.egg-info/
+-rw-rw-rw-   0        0        0    34713 2023-06-23 00:15:05.000000 fukkatsu-0.0.8/fukkatsu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-06-23 00:15:05.000000 fukkatsu-0.0.8/fukkatsu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 00:15:05.000000 fukkatsu-0.0.8/fukkatsu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-23 00:15:05.000000 fukkatsu-0.0.8/fukkatsu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 00:15:05.000000 fukkatsu-0.0.8/fukkatsu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 00:15:05.842525 fukkatsu-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2023-06-20 23:55:09.000000 fukkatsu-0.0.8/setup.py
```

### Comparing `fukkatsu-0.0.7/CHANGELOG.md` & `fukkatsu-0.0.8/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.7/LICENSE` & `fukkatsu-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.7/fukkatsu/__init__.py` & `fukkatsu-0.0.8/fukkatsu/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 import copy
 import functools
 import traceback
 
 from fukkatsu.memory import SHORT_TERM_MEMORY
 from fukkatsu.observer.tracker import track
 from fukkatsu.utils import (check_and_install_libraries, extract_imports,
                             extract_text_between_pipes,
                             insert_string_after_colon, remove_trace_lines,
-                            remove_wrapper_name, return_input_arguments,
-                            return_source_code)
-from fukkatsu.utils.medic import defibrillate, enhance, twin
+                            remove_wrapper_name, rename_function,
+                            return_input_arguments, return_source_code,
+                            sampler)
+from fukkatsu.utils.medic import defibrillate, enhance, stalker, twin
 
 
 def resurrect(
     lives: int = 1,
     additional_req: str = "",
     allow_installs: bool = False,
     active_twin: bool = False,
@@ -70,14 +71,18 @@
                         suggested_code = twin(
                             inputs=input_args,
                             target_function=suggested_code,
                             model=llm["secondary"],
                             temperature=temperature["secondary"],
                         )
                         track.warning(f"TWIN review complete:\n{suggested_code}")
+                        suggested_code = rename_function(suggested_code, func.__name__)
+                        track.warning(
+                            f"Twin Safeguard: Function name changed to {suggested_code}\n"
+                        )
                     suggested_code = extract_text_between_pipes(suggested_code)
                     track.warning(
                         f"Received INITIAL CLEANED suggestion:\n{suggested_code}\n"
                     )
 
                     import_block = extract_imports(suggested_code)
                     if allow_installs == True:
@@ -154,14 +159,21 @@
                                     target_function=suggested_code,
                                     model=llm["secondary"],
                                     temperature=temperature["secondary"],
                                 )
                                 track.warning(
                                     f"TWIN review complete:\n{suggested_code}"
                                 )
+                                suggested_code = rename_function(
+                                    suggested_code, func.__name__
+                                )
+                                track.warning(
+                                    f"Twin Safeguard: Function name changed to {suggested_code}\n"
+                                )
+
                             suggested_code = extract_text_between_pipes(suggested_code)
                             track.warning(
                                 f"Received attempt CLEANED suggestion:\n{suggested_code}\n"
                             )
 
                             import_block = extract_imports(suggested_code)
                             if allow_installs == True:
@@ -216,14 +228,19 @@
                 suggested_code = twin(
                     inputs=input_args,
                     target_function=suggested_code,
                     model=llm["secondary"],
                     temperature=temperature["secondary"],
                 )
                 track.warning(f"TWIN review complete:\n{suggested_code}")
+                suggested_code = rename_function(suggested_code, func.__name__)
+                track.warning(
+                    f"Twin Safeguard: Function name changed to {suggested_code}\n"
+                )
+                track.warning(f"TWIN review complete:\n{suggested_code}")
             suggested_code = extract_text_between_pipes(suggested_code)
             track.warning(f"Received CLEANED suggestion mutation: {suggested_code}\n")
 
             global_dict = globals()
             local_dict = locals()
 
             import_block = extract_imports(suggested_code)
@@ -245,7 +262,87 @@
             track.warning(f"Mutation successful, using {suggested_code}\n")
 
             return output
 
         return wrapper
 
     return _mutate
+
+
+def stalk(
+    likelihood: float = 1,
+    additional_req: str = "",
+    allow_installs: bool = False,
+    active_twin: bool = False,
+    llm: dict = {"primary": "gpt-3.5-turbo", "secondary": "gpt-3.5-turbo"},
+    temperature: dict = {"primary": 0.1, "secondary": 0.1},
+):
+    def _stalk(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+
+            if sampler(likelihood) == False:
+                track.warning(
+                    "Continue without reviewing function, using original function\n"
+                )
+                return func(*args, **kwargs)
+
+            input_args = return_input_arguments(func, *args, **kwargs)
+            source = return_source_code(func)
+            source = remove_wrapper_name(source)
+
+            track.warning(f"Input arguments: {input_args}\n")
+            track.warning(f"\nSource Code: \n {source}\n")
+
+            track.warning("Stalking function\n")
+            suggested_code = stalker(
+                inputs=input_args,
+                function=source,
+                model=llm["primary"],
+                temperature=temperature["primary"],
+                additional_req=additional_req,
+            )
+            track.warning(f"Received RAW suggestion from Stalker:\n{suggested_code}\n")
+
+            if active_twin == True:
+                track.warning("Requesting TWIN review:\n")
+                suggested_code = twin(
+                    inputs=input_args,
+                    target_function=suggested_code,
+                    model=llm["secondary"],
+                    temperature=temperature["secondary"],
+                )
+                track.warning(f"TWIN review complete:\n{suggested_code}")
+                suggested_code = rename_function(suggested_code, func.__name__)
+                track.warning(
+                    f"Twin Safeguard: Function name changed to {suggested_code}\n"
+                )
+
+            suggested_code = extract_text_between_pipes(suggested_code)
+            track.warning(f"Received CLEANED suggestion review: {suggested_code}\n")
+
+            global_dict = globals()
+            local_dict = locals()
+
+            import_block = extract_imports(suggested_code)
+            if allow_installs == True:
+                check_and_install_libraries(import_statements=import_block)
+
+            suggested_code = insert_string_after_colon(suggested_code, import_block)
+            track.warning(f"Import block added to suggested code:\n {suggested_code}\n")
+
+            compiled_code = compile(suggested_code, "<string>", "exec")
+
+            exec(compiled_code, global_dict, local_dict)
+            new_function = local_dict[func.__name__]
+
+            locals()[func.__name__] = new_function
+
+            output = new_function(*args, **kwargs)
+
+            track.warning(f"Review successful, using {suggested_code}\n")
+
+            return output
+
+        return wrapper
+
+    return _stalk
```

### Comparing `fukkatsu-0.0.7/fukkatsu/memory/manage.py` & `fukkatsu-0.0.8/fukkatsu/memory/manage.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.7/fukkatsu/observer/tracker.py` & `fukkatsu-0.0.8/fukkatsu/observer/tracker.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def format(self, record):
         level = record.levelname
         message = super().format(record)
 
         if level == "INFO":
             message = COLORS["GREEN"] + message + COLORS["DEFAULT"]
         elif level == "WARNING" or level == "DEBUG":
-            message = COLORS["BLACK"] + message + COLORS["DEFAULT"]
+            message = COLORS["DEFAULT"] + message + COLORS["DEFAULT"]
         elif level == "ERROR" or level == "CRITICAL":
             message = COLORS["RED"] + message + COLORS["DEFAULT"]
 
         return message
 
 
 formatter = ColoredFormatter("%(asctime)s - %(message)s")
```

### Comparing `fukkatsu-0.0.7/fukkatsu/utils/helper.py` & `fukkatsu-0.0.8/fukkatsu/utils/helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import ast
 import importlib
 import inspect
 import logging
+import random
 import re
 import subprocess
 import sys
 
+from fukkatsu.observer.tracker import track
+
 
 def remove_trace_lines(trace_error: str) -> str:
     pattern = r"\b\w*line\s\d+\w*\b"
     output_str = re.sub(pattern, "", trace_error)
     return output_str
 
 
@@ -114,17 +117,40 @@
 
         try:
             importlib.import_module(statement)
         except ImportError:
             missing_libraries.append(statement)
 
     if missing_libraries:
-        logging.warning(f"Missing libraries: {', '.join(missing_libraries)}\n")
+        track.warning(f"Missing libraries: {', '.join(missing_libraries)}\n")
         install_libraries(missing_libraries)
 
 
-def install_libraries(libraries: str) -> None:
+def install_libraries(libraries: list) -> None:
     for library in libraries:
-        logging.warning(f"Installing library {library}\n")
+        track.warning(f"Installing library {library}\n")
         subprocess.check_call([sys.executable, "-m", "pip", "install", library])
 
-    logging.warning(f"Libraries installed successfully\n")
+    track.warning(f"Libraries installed successfully\n")
+
+
+def sampler(likelihood: float) -> bool:
+    "Function that returns True or False depending on the likelihood provided. A higher likelihood indicates a bigger chances of returning True."
+    random_number = random.random()
+    track.warning(f"Random number: {random_number}, Likelihood: {likelihood}")
+
+    if random_number < likelihood:
+        return True
+    else:
+        return False
+
+
+def rename_function(function_string: str, new_name: str) -> str:
+    pattern = r"def\s+([a-zA-Z_]\w*)\s*\("
+    match = re.search(pattern, function_string)
+
+    if match:
+        renamed_function = re.sub(pattern, f"def {new_name}(", function_string)
+        return renamed_function
+    else:
+        track.warning(f"Could not rename function {function_string}")
+        return function_string
```

### Comparing `fukkatsu-0.0.7/fukkatsu/utils/medic.py` & `fukkatsu-0.0.8/fukkatsu/utils/medic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 
 import openai
 
 from fukkatsu.observer.tracker import track
 from fukkatsu.utils.prompt import (ADDITIONAL, CONTEXT, CONTEXT_MUTATE,
-                                   CONTEXT_TWIN, OUTPUT_CONSTRAINTS,
+                                   CONTEXT_STALKER, CONTEXT_TWIN,
+                                   OUTPUT_CONSTRAINTS,
                                    OUTPUT_CONSTRAINTS_MUTATE,
                                    OUTPUT_CONSTRAINTS_TWIN)
 
 try:
     openai.api_key = os.environ.get("OPENAI_API_KEY")
     print("OPENAI_API_KEY found in environment variables.")
 except:
@@ -99,7 +100,42 @@
         stop=None,
         temperature=temperature,
     )
 
     mutated_function = response["choices"][0]["message"]["content"].strip()
 
     return mutated_function
+
+
+def stalker(
+    inputs: str,
+    function: str,
+    model: str,
+    temperature: float,
+    additional_req: str = "",
+) -> str:
+    if additional_req == "":
+        set_prompt = (
+            f"{CONTEXT_STALKER}\n\n{function}\n\nThe function received the following inputs:\n\n"
+            f"{inputs}\n\n{OUTPUT_CONSTRAINTS}\n"
+        )
+    else:
+        set_prompt = (
+            f"{CONTEXT}\n\n{function}\n\nThe function received the following inputs:\n\n"
+            f"{inputs}\n\n{OUTPUT_CONSTRAINTS}\n"
+            f"{ADDITIONAL}{additional_req}"
+        )
+    track.warning(f"API REQUEST to {model}")
+    response = openai.ChatCompletion.create(
+        model=model,
+        messages=[
+            {"role": "system", "content": set_prompt},
+        ],
+        max_tokens=1024,
+        n=1,
+        stop=None,
+        temperature=temperature,
+    )
+
+    corrected_function = response["choices"][0]["message"]["content"].strip()
+
+    return corrected_function
```

### Comparing `fukkatsu-0.0.7/setup.py` & `fukkatsu-0.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     author="Maximilian Mekiska",
     author_email="maxmekiska@gmail.com",
     url="https://github.com/maxmekiska/fukkatsu",
     description="A python library for runtime LLM supported code corrections.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="fukkatsu",
-    version="0.0.7",
+    version="0.0.8",
     packages=find_packages(include=["fukkatsu", "fukkatsu.*"]),
     install_requires=[
         "setuptools >= 41.0.0",
         "openai >= 0.27.5, <= 0.28",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
```

