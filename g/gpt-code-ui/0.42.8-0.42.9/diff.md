# Comparing `tmp/gpt_code_ui-0.42.8.tar.gz` & `tmp/gpt_code_ui-0.42.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_code_ui-0.42.8.tar", last modified: Thu May 18 12:35:14 2023, max compression
+gzip compressed data, was "gpt_code_ui-0.42.9.tar", last modified: Thu May 18 13:07:15 2023, max compression
```

## Comparing `gpt_code_ui-0.42.8.tar` & `gpt_code_ui-0.42.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-18 12:35:14.589937 gpt_code_ui-0.42.8/
--rw-r--r--   0 rick       (501) staff       (20)     1067 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.8/LICENSE
--rw-r--r--   0 rick       (501) staff       (20)       78 2023-05-18 12:35:14.589810 gpt_code_ui-0.42.8/PKG-INFO
--rw-r--r--   0 rick       (501) staff       (20)      902 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.8/README.md
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-18 12:35:14.584154 gpt_code_ui-0.42.8/gpt_code_ui/
--rw-r--r--   0 rick       (501) staff       (20)        0 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.8/gpt_code_ui/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-18 12:35:14.585367 gpt_code_ui-0.42.8/gpt_code_ui/kernel_program/
--rw-r--r--   0 rick       (501) staff       (20)        0 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.8/gpt_code_ui/kernel_program/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)      396 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.8/gpt_code_ui/kernel_program/config.py
--rw-r--r--   0 rick       (501) staff       (20)     6801 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.8/gpt_code_ui/kernel_program/kernel_manager.py
--rw-r--r--   0 rick       (501) staff       (20)      100 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.8/gpt_code_ui/kernel_program/launch_kernel.py
--rw-r--r--   0 rick       (501) staff       (20)     4011 2023-05-18 12:09:52.000000 gpt_code_ui-0.42.8/gpt_code_ui/kernel_program/main.py
--rw-r--r--   0 rick       (501) staff       (20)      943 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.8/gpt_code_ui/kernel_program/utils.py
--rw-r--r--   0 rick       (501) staff       (20)     3092 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.8/gpt_code_ui/main.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-18 12:35:14.585574 gpt_code_ui-0.42.8/gpt_code_ui/webapp/
--rw-r--r--   0 rick       (501) staff       (20)        0 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.8/gpt_code_ui/webapp/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     5496 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.8/gpt_code_ui/webapp/main.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-18 12:35:14.585703 gpt_code_ui-0.42.8/gpt_code_ui/webapp/static/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-18 12:35:14.589638 gpt_code_ui-0.42.8/gpt_code_ui/webapp/static/assets/
--rw-r--r--   0 rick       (501) staff       (20)      312 2023-05-18 12:35:14.000000 gpt_code_ui-0.42.8/gpt_code_ui/webapp/static/assets/assistant.svg
--rw-r--r--   0 rick       (501) staff       (20)     2701 2023-05-18 12:35:14.000000 gpt_code_ui-0.42.8/gpt_code_ui/webapp/static/assets/index-6b3678eb.css
--rw-r--r--   0 rick       (501) staff       (20)  1122082 2023-05-18 12:11:31.000000 gpt_code_ui-0.42.8/gpt_code_ui/webapp/static/assets/index-6feeddde.js
--rw-r--r--   0 rick       (501) staff       (20)  1122082 2023-05-18 12:35:14.000000 gpt_code_ui-0.42.8/gpt_code_ui/webapp/static/assets/index-75555e19.js
--rw-r--r--   0 rick       (501) staff       (20)  1122082 2023-05-18 12:29:59.000000 gpt_code_ui-0.42.8/gpt_code_ui/webapp/static/assets/index-c59a18f4.js
--rw-r--r--   0 rick       (501) staff       (20)     2790 2023-05-18 12:11:31.000000 gpt_code_ui-0.42.8/gpt_code_ui/webapp/static/assets/index-f84b874e.css
--rw-r--r--   0 rick       (501) staff       (20)      463 2023-05-18 12:35:14.000000 gpt_code_ui-0.42.8/gpt_code_ui/webapp/static/index.html
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-18 12:35:14.584771 gpt_code_ui-0.42.8/gpt_code_ui.egg-info/
--rw-r--r--   0 rick       (501) staff       (20)       78 2023-05-18 12:35:14.000000 gpt_code_ui-0.42.8/gpt_code_ui.egg-info/PKG-INFO
--rw-r--r--   0 rick       (501) staff       (20)      917 2023-05-18 12:35:14.000000 gpt_code_ui-0.42.8/gpt_code_ui.egg-info/SOURCES.txt
--rw-r--r--   0 rick       (501) staff       (20)        1 2023-05-18 12:35:14.000000 gpt_code_ui-0.42.8/gpt_code_ui.egg-info/dependency_links.txt
--rw-r--r--   0 rick       (501) staff       (20)       50 2023-05-18 12:35:14.000000 gpt_code_ui-0.42.8/gpt_code_ui.egg-info/entry_points.txt
--rw-r--r--   0 rick       (501) staff       (20)       94 2023-05-18 12:35:14.000000 gpt_code_ui-0.42.8/gpt_code_ui.egg-info/requires.txt
--rw-r--r--   0 rick       (501) staff       (20)       12 2023-05-18 12:35:14.000000 gpt_code_ui-0.42.8/gpt_code_ui.egg-info/top_level.txt
--rw-r--r--   0 rick       (501) staff       (20)       38 2023-05-18 12:35:14.589969 gpt_code_ui-0.42.8/setup.cfg
--rw-r--r--   0 rick       (501) staff       (20)      506 2023-05-18 12:34:28.000000 gpt_code_ui-0.42.8/setup.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-18 13:07:15.049851 gpt_code_ui-0.42.9/
+-rw-r--r--   0 rick       (501) staff       (20)     1067 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.9/LICENSE
+-rw-r--r--   0 rick       (501) staff       (20)       78 2023-05-18 13:07:15.049715 gpt_code_ui-0.42.9/PKG-INFO
+-rw-r--r--   0 rick       (501) staff       (20)      888 2023-05-18 13:06:42.000000 gpt_code_ui-0.42.9/README.md
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-18 13:07:15.034344 gpt_code_ui-0.42.9/gpt_code_ui/
+-rw-r--r--   0 rick       (501) staff       (20)        0 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.9/gpt_code_ui/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-18 13:07:15.036666 gpt_code_ui-0.42.9/gpt_code_ui/kernel_program/
+-rw-r--r--   0 rick       (501) staff       (20)        0 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.9/gpt_code_ui/kernel_program/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)      396 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.9/gpt_code_ui/kernel_program/config.py
+-rw-r--r--   0 rick       (501) staff       (20)     6801 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.9/gpt_code_ui/kernel_program/kernel_manager.py
+-rw-r--r--   0 rick       (501) staff       (20)      100 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.9/gpt_code_ui/kernel_program/launch_kernel.py
+-rw-r--r--   0 rick       (501) staff       (20)     4011 2023-05-18 12:09:52.000000 gpt_code_ui-0.42.9/gpt_code_ui/kernel_program/main.py
+-rw-r--r--   0 rick       (501) staff       (20)      943 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.9/gpt_code_ui/kernel_program/utils.py
+-rw-r--r--   0 rick       (501) staff       (20)     3098 2023-05-18 13:06:03.000000 gpt_code_ui-0.42.9/gpt_code_ui/main.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-18 13:07:15.036938 gpt_code_ui-0.42.9/gpt_code_ui/webapp/
+-rw-r--r--   0 rick       (501) staff       (20)        0 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.9/gpt_code_ui/webapp/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     5496 2023-05-18 12:09:33.000000 gpt_code_ui-0.42.9/gpt_code_ui/webapp/main.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-18 13:07:15.037107 gpt_code_ui-0.42.9/gpt_code_ui/webapp/static/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-18 13:07:15.049309 gpt_code_ui-0.42.9/gpt_code_ui/webapp/static/assets/
+-rw-r--r--   0 rick       (501) staff       (20)      312 2023-05-18 13:07:14.000000 gpt_code_ui-0.42.9/gpt_code_ui/webapp/static/assets/assistant.svg
+-rw-r--r--   0 rick       (501) staff       (20)  1122085 2023-05-18 13:07:14.000000 gpt_code_ui-0.42.9/gpt_code_ui/webapp/static/assets/index-2b326644.js
+-rw-r--r--   0 rick       (501) staff       (20)     2701 2023-05-18 13:07:14.000000 gpt_code_ui-0.42.9/gpt_code_ui/webapp/static/assets/index-6b3678eb.css
+-rw-r--r--   0 rick       (501) staff       (20)  1122082 2023-05-18 12:11:31.000000 gpt_code_ui-0.42.9/gpt_code_ui/webapp/static/assets/index-6feeddde.js
+-rw-r--r--   0 rick       (501) staff       (20)  1122082 2023-05-18 12:35:14.000000 gpt_code_ui-0.42.9/gpt_code_ui/webapp/static/assets/index-75555e19.js
+-rw-r--r--   0 rick       (501) staff       (20)  1122082 2023-05-18 12:29:59.000000 gpt_code_ui-0.42.9/gpt_code_ui/webapp/static/assets/index-c59a18f4.js
+-rw-r--r--   0 rick       (501) staff       (20)     2790 2023-05-18 12:11:31.000000 gpt_code_ui-0.42.9/gpt_code_ui/webapp/static/assets/index-f84b874e.css
+-rw-r--r--   0 rick       (501) staff       (20)      463 2023-05-18 13:07:14.000000 gpt_code_ui-0.42.9/gpt_code_ui/webapp/static/index.html
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-18 13:07:15.035372 gpt_code_ui-0.42.9/gpt_code_ui.egg-info/
+-rw-r--r--   0 rick       (501) staff       (20)       78 2023-05-18 13:07:15.000000 gpt_code_ui-0.42.9/gpt_code_ui.egg-info/PKG-INFO
+-rw-r--r--   0 rick       (501) staff       (20)      968 2023-05-18 13:07:15.000000 gpt_code_ui-0.42.9/gpt_code_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 rick       (501) staff       (20)        1 2023-05-18 13:07:15.000000 gpt_code_ui-0.42.9/gpt_code_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 rick       (501) staff       (20)       50 2023-05-18 13:07:15.000000 gpt_code_ui-0.42.9/gpt_code_ui.egg-info/entry_points.txt
+-rw-r--r--   0 rick       (501) staff       (20)       94 2023-05-18 13:07:15.000000 gpt_code_ui-0.42.9/gpt_code_ui.egg-info/requires.txt
+-rw-r--r--   0 rick       (501) staff       (20)       12 2023-05-18 13:07:15.000000 gpt_code_ui-0.42.9/gpt_code_ui.egg-info/top_level.txt
+-rw-r--r--   0 rick       (501) staff       (20)       38 2023-05-18 13:07:15.049891 gpt_code_ui-0.42.9/setup.cfg
+-rw-r--r--   0 rick       (501) staff       (20)      506 2023-05-18 13:06:09.000000 gpt_code_ui-0.42.9/setup.py
```

### Comparing `gpt_code_ui-0.42.8/LICENSE` & `gpt_code_ui-0.42.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.8/README.md` & `gpt_code_ui-0.42.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 - Model switching (GPT-3.5 and GPT-4)
 
 ## More information
 Read the [blog post](https://ricklamers.io/posts/gpt-code) to find out more.
 
 ## Misc.
 ### Using .env for OpenAI key
-You can put a .env in the root of the repository directory to load the `OPENAI_API_KEY` environment variable.
+You can put a .env in the working directory to load the `OPENAI_API_KEY` environment variable.
```

### Comparing `gpt_code_ui-0.42.8/gpt_code_ui/kernel_program/kernel_manager.py` & `gpt_code_ui-0.42.9/gpt_code_ui/kernel_program/kernel_manager.py`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.8/gpt_code_ui/kernel_program/main.py` & `gpt_code_ui-0.42.9/gpt_code_ui/kernel_program/main.py`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.8/gpt_code_ui/kernel_program/utils.py` & `gpt_code_ui-0.42.9/gpt_code_ui/kernel_program/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.8/gpt_code_ui/main.py` & `gpt_code_ui-0.42.9/gpt_code_ui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         print("")
         print("You can inspect detailed logs in app.log.")
         print("")
         print("Find your OpenAI API key at https://platform.openai.com/account/api-keys")
         print("")
         print_color("I'm looking for exciting MLE opportunities! Find out more https://ricklamers.io/about", color="green")
         print_color("")
-        print_color("Contribute to GPT-Code at https://github.com/ricklamers/gpt-code")   
+        print_color("Contribute to GPT-Code UI at https://github.com/ricklamers/gpt-code-ui")   
 
 def main():
     setup_logging()
 
     webapp_process = Process(target=run_webapp)
     kernel_program_process = Process(target=run_kernel_program)
```

### Comparing `gpt_code_ui-0.42.8/gpt_code_ui/webapp/main.py` & `gpt_code_ui-0.42.9/gpt_code_ui/webapp/main.py`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.8/gpt_code_ui/webapp/static/assets/index-6b3678eb.css` & `gpt_code_ui-0.42.9/gpt_code_ui/webapp/static/assets/index-6b3678eb.css`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.8/gpt_code_ui/webapp/static/assets/index-6feeddde.js` & `gpt_code_ui-0.42.9/gpt_code_ui/webapp/static/assets/index-6feeddde.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.8/gpt_code_ui/webapp/static/assets/index-75555e19.js` & `gpt_code_ui-0.42.9/gpt_code_ui/webapp/static/assets/index-75555e19.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.8/gpt_code_ui/webapp/static/assets/index-c59a18f4.js` & `gpt_code_ui-0.42.9/gpt_code_ui/webapp/static/assets/index-c59a18f4.js`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.8/gpt_code_ui/webapp/static/assets/index-f84b874e.css` & `gpt_code_ui-0.42.9/gpt_code_ui/webapp/static/assets/index-f84b874e.css`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.8/gpt_code_ui.egg-info/SOURCES.txt` & `gpt_code_ui-0.42.9/gpt_code_ui.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,12 +15,13 @@
 gpt_code_ui/kernel_program/launch_kernel.py
 gpt_code_ui/kernel_program/main.py
 gpt_code_ui/kernel_program/utils.py
 gpt_code_ui/webapp/__init__.py
 gpt_code_ui/webapp/main.py
 gpt_code_ui/webapp/static/index.html
 gpt_code_ui/webapp/static/assets/assistant.svg
+gpt_code_ui/webapp/static/assets/index-2b326644.js
 gpt_code_ui/webapp/static/assets/index-6b3678eb.css
 gpt_code_ui/webapp/static/assets/index-6feeddde.js
 gpt_code_ui/webapp/static/assets/index-75555e19.js
 gpt_code_ui/webapp/static/assets/index-c59a18f4.js
 gpt_code_ui/webapp/static/assets/index-f84b874e.css
```

