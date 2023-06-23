# Comparing `tmp/lmt-cli-0.0.1.tar.gz` & `tmp/lmt-cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmt-cli-0.0.1.tar", last modified: Thu Jun 22 16:10:29 2023, max compression
+gzip compressed data, was "lmt-cli-0.0.2.tar", last modified: Fri Jun 23 19:11:11 2023, max compression
```

## Comparing `lmt-cli-0.0.1.tar` & `lmt-cli-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-22 16:10:29.705788 lmt-cli-0.0.1/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-18 17:13:45.000000 lmt-cli-0.0.1/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7802 2023-06-22 16:10:29.705788 lmt-cli-0.0.1/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7159 2023-06-22 16:04:23.000000 lmt-cli-0.0.1/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-22 16:10:29.705788 lmt-cli-0.0.1/lmt/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 20:39:32.000000 lmt-cli-0.0.1/lmt/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    14911 2023-06-22 15:56:19.000000 lmt-cli-0.0.1/lmt/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4826 2023-06-22 13:13:31.000000 lmt-cli-0.0.1/lmt/gpt_integration.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-22 16:10:29.705788 lmt-cli-0.0.1/lmt_cli.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7802 2023-06-22 16:10:29.000000 lmt-cli-0.0.1/lmt_cli.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      264 2023-06-22 16:10:29.000000 lmt-cli-0.0.1/lmt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-22 16:10:29.000000 lmt-cli-0.0.1/lmt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       36 2023-06-22 16:10:29.000000 lmt-cli-0.0.1/lmt_cli.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       34 2023-06-22 16:10:29.000000 lmt-cli-0.0.1/lmt_cli.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        4 2023-06-22 16:10:29.000000 lmt-cli-0.0.1/lmt_cli.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-22 16:10:29.705788 lmt-cli-0.0.1/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1170 2023-06-22 16:10:02.000000 lmt-cli-0.0.1/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 19:11:11.734373 lmt-cli-0.0.2/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-18 17:13:45.000000 lmt-cli-0.0.2/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9055 2023-06-23 19:11:11.734373 lmt-cli-0.0.2/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     8412 2023-06-23 18:54:04.000000 lmt-cli-0.0.2/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 19:11:11.734373 lmt-cli-0.0.2/lmt/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 20:39:32.000000 lmt-cli-0.0.2/lmt/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7695 2023-06-23 19:02:32.000000 lmt-cli-0.0.2/lmt/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4828 2023-06-22 23:46:33.000000 lmt-cli-0.0.2/lmt/gpt_integration.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9224 2023-06-23 18:44:29.000000 lmt-cli-0.0.2/lmt/lib.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 19:11:11.734373 lmt-cli-0.0.2/lmt_cli.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9055 2023-06-23 19:11:11.000000 lmt-cli-0.0.2/lmt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      275 2023-06-23 19:11:11.000000 lmt-cli-0.0.2/lmt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-23 19:11:11.000000 lmt-cli-0.0.2/lmt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       36 2023-06-23 19:11:11.000000 lmt-cli-0.0.2/lmt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       34 2023-06-23 19:11:11.000000 lmt-cli-0.0.2/lmt_cli.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        4 2023-06-23 19:11:11.000000 lmt-cli-0.0.2/lmt_cli.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-23 19:11:11.734373 lmt-cli-0.0.2/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1170 2023-06-23 19:09:46.000000 lmt-cli-0.0.2/setup.py
```

### Comparing `lmt-cli-0.0.1/LICENSE` & `lmt-cli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.1/PKG-INFO` & `lmt-cli-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,8 @@
-Metadata-Version: 2.1
-Name: lmt-cli
-Version: 0.0.1
-Summary: The main CLI tool within the LLM-Toolbox, designed to enable seamless communication with ChatGPT from your terminal. You can customize your experience by creating templates and using them to generate messages.
-Home-page: https://github.com/sderev/lmt
-Author: Sébastien De Revière
-License: Apache Licence, Version 2.0
-Project-URL: Documentation, https://github.com/sderev/lmt
-Project-URL: Issues, http://github.com/sderev/lmt/issues
-Project-URL: Changelog, https://github.com/sderev/lmt/releases
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# `lmt`: The CLI Tool for ChatGPT
+# LMT: The CLI Tool for ChatGPT
 
 `lmt` is the primary tool of the [LLM-Toolbox](https://github.com/sderev/llm-toolbox) and a versatile command-line interface tool that allows you to interact directly with OpenAI's ChatGPT models. With `lmt`, you can bring the power of artificial intelligence to your terminal, utilizing.
 
 As a crucial component of the LLM-Toolbox, `lmt` exemplifies the toolbox's dedication to providing powerful, flexible tools that harness the capabilities of language models. It allows access to all available models of ChatGPT, including gpt-3.5-turbo, gpt-3.5-turbo-16k, gpt-4, and gpt-4-32k.
 
 Furthermore, `lmt` enables you to design and use your own templates, broadening its potential applications. The ability to read from `stdin` using pipes also allows for convenient integration with other command-line tools.
 
@@ -37,14 +23,15 @@
     1. [Basic Example](#basic-example)
     1. [Add a Persona](#add-a-persona)
     1. [Switching Models](#switching-models)
     1. [Switching Models](#switching-models)
     1. [Template Utilization](#template-utilization)
     1. [Emoji Integration](#emoji-integration)
     1. [Prompt Cost Estimation](#prompt-cost-estimation)
+    1. [Reading from stdin](#reading-from-stdin)
 1. [License](#license)
 1. [Upcoming Features](#upcoming-features)
 <!-- /TOC -->
 
 ## Features
 
 * **Access All ChatGPT Models**: `lmt` supports all available ChatGPT models (gpt-3.5-turbo, gpt-3.5-turbo-16k, gpt-4, gpt-4-32k), giving you the power to choose the most suitable one for your task.
@@ -140,18 +127,14 @@
 
   ```
   setx OPENAI_API_KEY your_key
   ```
 
 ## Usage
 
-Absolutely! Here's your revised Usage section:
-
----
-
 ## Usage
 
 The `lmt` CLI tool is equipped with a helpful `--help` flag that displays useful information about how to use the tool and its commands.
 
 **For a general overview of all commands, you can type**:
 
 ```bash
@@ -179,15 +162,16 @@
 ### Add a Persona
 
 You can also instruct the model to adopt a specific persona using the `--system` flag. This is useful when you want the model's responses to emulate a certain character or writing style.
 
 **Here's an example where we instruct the model to write like the philosopher Cioran**:
 
 ```bash
-lmt prompt "Tell me what you think of the large language models." --system "You are Cioran. You write like Cioran."
+lmt prompt "Tell me what you think of large language models." \
+        --system "You are Cioran. You write like Cioran."
 ```
 
 In this case, the model will generate a response based on its understanding of Cioran's writing style and perspective.
 
 ### Switching Models
 
 Sure, here's a reviewed and slightly enhanced version of your text:
@@ -219,15 +203,15 @@
 
 Templates, stored in `~/.config/lmt/templates` and written in YAML, can be effortlessly generated using the following command:
 
 ```bash
 lmt templates add
 ```
 
-For help regarding the `templates` subcommand, use:
+**For help regarding the `templates` subcommand, use**:
 
 ```bash
 lmt templates --help
 ```
 
 **Here's an example of invoking a template named "cioran"**:
 
@@ -239,14 +223,37 @@
 
 To infuse a touch of emotion into your requests, append the `--emoji` flag option.
 
 ### Prompt Cost Estimation
 
 For an estimation of your prompt's cost before sending, utilize the `--tokens` flag option.
 
+### Reading from stdin
+
+`lmt` facilitates reading inputs directly from `stdin`, allowing you to pipe in the content of a file as a prompt. This feature can be particularly useful when dealing with longer or more complex prompts, or when you want to streamline your workflow by incorporating `lmt` into a larger pipeline of commands.
+
+To use this feature, you simply need to pipe your content into the `lmt` command like this:
+
+```bash
+cat your_file.txt | lmt prompt
+```
+
+In this example, `lmt` would use the content of `your_file.txt` as the input for the `prompt` command.
+
+Also, remember that you can still use all other command line options with `stdin`. For instance, you might run:
+
+```bash
+cat your_file.py | lmt prompt \
+        --system "You explain code in the style of \
+        a fast-talkin' wise guy from a 1940's gangster movie" \
+        -m 4 --emoji
+```
+
+In this example, `lmt` takes the content of `your_file.py` as the input for the `prompt` command. With the `gpt-4` model selected via `-m 4`, the system is instructed to respond in the style of a fast-talking wiseguy from a 1940s gangster movie, as specified in the `--system` option. The `--emoji` flag indicates that the response may include emojis for added expressiveness.
+
 ## License
 
 `lmt` is licensed under Apache License version 2.0.
 
 ## Upcoming Features
 
 While `lmt` already boasts a wide array of features, development is ongoing. Expect more features and improvements in the future!
```

### Comparing `lmt-cli-0.0.1/README.md` & `lmt-cli-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,22 @@
-# `lmt`: The CLI Tool for ChatGPT
+Metadata-Version: 2.1
+Name: lmt-cli
+Version: 0.0.2
+Summary: The main CLI tool within the LLM-Toolbox, designed to enable seamless communication with ChatGPT from your terminal. You can customize your experience by creating templates and using them to generate messages.
+Home-page: https://github.com/sderev/lmt
+Author: Sébastien De Revière
+License: Apache Licence, Version 2.0
+Project-URL: Documentation, https://github.com/sderev/lmt
+Project-URL: Issues, http://github.com/sderev/lmt/issues
+Project-URL: Changelog, https://github.com/sderev/lmt/releases
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# LMT: The CLI Tool for ChatGPT
 
 `lmt` is the primary tool of the [LLM-Toolbox](https://github.com/sderev/llm-toolbox) and a versatile command-line interface tool that allows you to interact directly with OpenAI's ChatGPT models. With `lmt`, you can bring the power of artificial intelligence to your terminal, utilizing.
 
 As a crucial component of the LLM-Toolbox, `lmt` exemplifies the toolbox's dedication to providing powerful, flexible tools that harness the capabilities of language models. It allows access to all available models of ChatGPT, including gpt-3.5-turbo, gpt-3.5-turbo-16k, gpt-4, and gpt-4-32k.
 
 Furthermore, `lmt` enables you to design and use your own templates, broadening its potential applications. The ability to read from `stdin` using pipes also allows for convenient integration with other command-line tools.
 
@@ -23,14 +37,15 @@
     1. [Basic Example](#basic-example)
     1. [Add a Persona](#add-a-persona)
     1. [Switching Models](#switching-models)
     1. [Switching Models](#switching-models)
     1. [Template Utilization](#template-utilization)
     1. [Emoji Integration](#emoji-integration)
     1. [Prompt Cost Estimation](#prompt-cost-estimation)
+    1. [Reading from stdin](#reading-from-stdin)
 1. [License](#license)
 1. [Upcoming Features](#upcoming-features)
 <!-- /TOC -->
 
 ## Features
 
 * **Access All ChatGPT Models**: `lmt` supports all available ChatGPT models (gpt-3.5-turbo, gpt-3.5-turbo-16k, gpt-4, gpt-4-32k), giving you the power to choose the most suitable one for your task.
@@ -126,18 +141,14 @@
 
   ```
   setx OPENAI_API_KEY your_key
   ```
 
 ## Usage
 
-Absolutely! Here's your revised Usage section:
-
----
-
 ## Usage
 
 The `lmt` CLI tool is equipped with a helpful `--help` flag that displays useful information about how to use the tool and its commands.
 
 **For a general overview of all commands, you can type**:
 
 ```bash
@@ -165,15 +176,16 @@
 ### Add a Persona
 
 You can also instruct the model to adopt a specific persona using the `--system` flag. This is useful when you want the model's responses to emulate a certain character or writing style.
 
 **Here's an example where we instruct the model to write like the philosopher Cioran**:
 
 ```bash
-lmt prompt "Tell me what you think of the large language models." --system "You are Cioran. You write like Cioran."
+lmt prompt "Tell me what you think of large language models." \
+        --system "You are Cioran. You write like Cioran."
 ```
 
 In this case, the model will generate a response based on its understanding of Cioran's writing style and perspective.
 
 ### Switching Models
 
 Sure, here's a reviewed and slightly enhanced version of your text:
@@ -205,15 +217,15 @@
 
 Templates, stored in `~/.config/lmt/templates` and written in YAML, can be effortlessly generated using the following command:
 
 ```bash
 lmt templates add
 ```
 
-For help regarding the `templates` subcommand, use:
+**For help regarding the `templates` subcommand, use**:
 
 ```bash
 lmt templates --help
 ```
 
 **Here's an example of invoking a template named "cioran"**:
 
@@ -225,14 +237,37 @@
 
 To infuse a touch of emotion into your requests, append the `--emoji` flag option.
 
 ### Prompt Cost Estimation
 
 For an estimation of your prompt's cost before sending, utilize the `--tokens` flag option.
 
+### Reading from stdin
+
+`lmt` facilitates reading inputs directly from `stdin`, allowing you to pipe in the content of a file as a prompt. This feature can be particularly useful when dealing with longer or more complex prompts, or when you want to streamline your workflow by incorporating `lmt` into a larger pipeline of commands.
+
+To use this feature, you simply need to pipe your content into the `lmt` command like this:
+
+```bash
+cat your_file.txt | lmt prompt
+```
+
+In this example, `lmt` would use the content of `your_file.txt` as the input for the `prompt` command.
+
+Also, remember that you can still use all other command line options with `stdin`. For instance, you might run:
+
+```bash
+cat your_file.py | lmt prompt \
+        --system "You explain code in the style of \
+        a fast-talkin' wise guy from a 1940's gangster movie" \
+        -m 4 --emoji
+```
+
+In this example, `lmt` takes the content of `your_file.py` as the input for the `prompt` command. With the `gpt-4` model selected via `-m 4`, the system is instructed to respond in the style of a fast-talking wiseguy from a 1940s gangster movie, as specified in the `--system` option. The `--emoji` flag indicates that the response may include emojis for added expressiveness.
+
 ## License
 
 `lmt` is licensed under Apache License version 2.0.
 
 ## Upcoming Features
 
 While `lmt` already boasts a wide array of features, development is ongoing. Expect more features and improvements in the future!
```

### Comparing `lmt-cli-0.0.1/lmt/gpt_integration.py` & `lmt-cli-0.0.2/lmt/gpt_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,29 +17,29 @@
         },
     ]
 
 
 def chatgpt_request(
     prompt,
     model="gpt-3.5-turbo",
-    max_tokens=3900,
+    #max_tokens=3900,
     n=1,
     temperature=1,
     stop=None,
     stream=False,
     update_markdown_stream=None,
 ):
     start_time = time.monotonic_ns()
     openai.api_key = os.getenv("OPENAI_API_KEY")
 
     # Make the API request
     response = openai.ChatCompletion.create(
         messages=prompt,
         model=model,
-        max_tokens=max_tokens,
+        #max_tokens=max_tokens,
         n=n,
         temperature=temperature,
         stop=stop,
         stream=stream,
     )
 
     if stream:
```

### Comparing `lmt-cli-0.0.1/lmt_cli.egg-info/PKG-INFO` & `lmt-cli-0.0.2/lmt_cli.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: lmt-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: The main CLI tool within the LLM-Toolbox, designed to enable seamless communication with ChatGPT from your terminal. You can customize your experience by creating templates and using them to generate messages.
 Home-page: https://github.com/sderev/lmt
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/lmt
 Project-URL: Issues, http://github.com/sderev/lmt/issues
 Project-URL: Changelog, https://github.com/sderev/lmt/releases
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# `lmt`: The CLI Tool for ChatGPT
+# LMT: The CLI Tool for ChatGPT
 
 `lmt` is the primary tool of the [LLM-Toolbox](https://github.com/sderev/llm-toolbox) and a versatile command-line interface tool that allows you to interact directly with OpenAI's ChatGPT models. With `lmt`, you can bring the power of artificial intelligence to your terminal, utilizing.
 
 As a crucial component of the LLM-Toolbox, `lmt` exemplifies the toolbox's dedication to providing powerful, flexible tools that harness the capabilities of language models. It allows access to all available models of ChatGPT, including gpt-3.5-turbo, gpt-3.5-turbo-16k, gpt-4, and gpt-4-32k.
 
 Furthermore, `lmt` enables you to design and use your own templates, broadening its potential applications. The ability to read from `stdin` using pipes also allows for convenient integration with other command-line tools.
 
@@ -37,14 +37,15 @@
     1. [Basic Example](#basic-example)
     1. [Add a Persona](#add-a-persona)
     1. [Switching Models](#switching-models)
     1. [Switching Models](#switching-models)
     1. [Template Utilization](#template-utilization)
     1. [Emoji Integration](#emoji-integration)
     1. [Prompt Cost Estimation](#prompt-cost-estimation)
+    1. [Reading from stdin](#reading-from-stdin)
 1. [License](#license)
 1. [Upcoming Features](#upcoming-features)
 <!-- /TOC -->
 
 ## Features
 
 * **Access All ChatGPT Models**: `lmt` supports all available ChatGPT models (gpt-3.5-turbo, gpt-3.5-turbo-16k, gpt-4, gpt-4-32k), giving you the power to choose the most suitable one for your task.
@@ -140,18 +141,14 @@
 
   ```
   setx OPENAI_API_KEY your_key
   ```
 
 ## Usage
 
-Absolutely! Here's your revised Usage section:
-
----
-
 ## Usage
 
 The `lmt` CLI tool is equipped with a helpful `--help` flag that displays useful information about how to use the tool and its commands.
 
 **For a general overview of all commands, you can type**:
 
 ```bash
@@ -179,15 +176,16 @@
 ### Add a Persona
 
 You can also instruct the model to adopt a specific persona using the `--system` flag. This is useful when you want the model's responses to emulate a certain character or writing style.
 
 **Here's an example where we instruct the model to write like the philosopher Cioran**:
 
 ```bash
-lmt prompt "Tell me what you think of the large language models." --system "You are Cioran. You write like Cioran."
+lmt prompt "Tell me what you think of large language models." \
+        --system "You are Cioran. You write like Cioran."
 ```
 
 In this case, the model will generate a response based on its understanding of Cioran's writing style and perspective.
 
 ### Switching Models
 
 Sure, here's a reviewed and slightly enhanced version of your text:
@@ -219,15 +217,15 @@
 
 Templates, stored in `~/.config/lmt/templates` and written in YAML, can be effortlessly generated using the following command:
 
 ```bash
 lmt templates add
 ```
 
-For help regarding the `templates` subcommand, use:
+**For help regarding the `templates` subcommand, use**:
 
 ```bash
 lmt templates --help
 ```
 
 **Here's an example of invoking a template named "cioran"**:
 
@@ -239,14 +237,37 @@
 
 To infuse a touch of emotion into your requests, append the `--emoji` flag option.
 
 ### Prompt Cost Estimation
 
 For an estimation of your prompt's cost before sending, utilize the `--tokens` flag option.
 
+### Reading from stdin
+
+`lmt` facilitates reading inputs directly from `stdin`, allowing you to pipe in the content of a file as a prompt. This feature can be particularly useful when dealing with longer or more complex prompts, or when you want to streamline your workflow by incorporating `lmt` into a larger pipeline of commands.
+
+To use this feature, you simply need to pipe your content into the `lmt` command like this:
+
+```bash
+cat your_file.txt | lmt prompt
+```
+
+In this example, `lmt` would use the content of `your_file.txt` as the input for the `prompt` command.
+
+Also, remember that you can still use all other command line options with `stdin`. For instance, you might run:
+
+```bash
+cat your_file.py | lmt prompt \
+        --system "You explain code in the style of \
+        a fast-talkin' wise guy from a 1940's gangster movie" \
+        -m 4 --emoji
+```
+
+In this example, `lmt` takes the content of `your_file.py` as the input for the `prompt` command. With the `gpt-4` model selected via `-m 4`, the system is instructed to respond in the style of a fast-talking wiseguy from a 1940s gangster movie, as specified in the `--system` option. The `--emoji` flag indicates that the response may include emojis for added expressiveness.
+
 ## License
 
 `lmt` is licensed under Apache License version 2.0.
 
 ## Upcoming Features
 
 While `lmt` already boasts a wide array of features, development is ongoing. Expect more features and improvements in the future!
```

### Comparing `lmt-cli-0.0.1/setup.py` & `lmt-cli-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 
 def read_requirements():
     with open("requirements.txt") as file:
         return list(file)
```

