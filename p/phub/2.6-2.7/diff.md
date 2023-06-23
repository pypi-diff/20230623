# Comparing `tmp/phub-2.6.tar.gz` & `tmp/phub-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phub-2.6.tar", last modified: Thu Jun 22 17:50:44 2023, max compression
+gzip compressed data, was "phub-2.7.tar", last modified: Fri Jun 23 11:47:30 2023, max compression
```

## Comparing `phub-2.6.tar` & `phub-2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:50:44.156976 phub-2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-22 17:50:32.000000 phub-2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-22 17:50:44.156976 phub-2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-22 17:50:32.000000 phub-2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-22 17:50:32.000000 phub-2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-22 17:50:44.160976 phub-2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-22 17:50:32.000000 phub-2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:50:44.156976 phub-2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:50:44.156976 phub-2.6/src/phub/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-22 17:50:32.000000 phub-2.6/src/phub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-22 17:50:32.000000 phub-2.6/src/phub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17281 2023-06-22 17:50:32.000000 phub-2.6/src/phub/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-22 17:50:32.000000 phub-2.6/src/phub/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-22 17:50:32.000000 phub-2.6/src/phub/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-22 17:50:32.000000 phub-2.6/src/phub/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-22 17:50:32.000000 phub-2.6/src/phub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:50:44.156976 phub-2.6/src/phub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-22 17:50:44.000000 phub-2.6/src/phub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-22 17:50:44.000000 phub-2.6/src/phub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 17:50:44.000000 phub-2.6/src/phub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 17:50:44.000000 phub-2.6/src/phub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 17:50:44.000000 phub-2.6/src/phub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:30.808628 phub-2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 11:47:20.000000 phub-2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-23 11:47:30.808628 phub-2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-23 11:47:20.000000 phub-2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 11:47:20.000000 phub-2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-23 11:47:30.808628 phub-2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 11:47:20.000000 phub-2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:30.804628 phub-2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:30.804628 phub-2.7/src/phub/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-23 11:47:20.000000 phub-2.7/src/phub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-23 11:47:20.000000 phub-2.7/src/phub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-06-23 11:47:20.000000 phub-2.7/src/phub/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-23 11:47:20.000000 phub-2.7/src/phub/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-23 11:47:20.000000 phub-2.7/src/phub/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-23 11:47:20.000000 phub-2.7/src/phub/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-23 11:47:20.000000 phub-2.7/src/phub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:30.808628 phub-2.7/src/phub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-23 11:47:30.000000 phub-2.7/src/phub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-23 11:47:30.000000 phub-2.7/src/phub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:47:30.000000 phub-2.7/src/phub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 11:47:30.000000 phub-2.7/src/phub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 11:47:30.000000 phub-2.7/src/phub.egg-info/top_level.txt
```

### Comparing `phub-2.6/LICENSE` & `phub-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `phub-2.6/PKG-INFO` & `phub-2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 2.6
+Version: 2.7
 Summary: An API for PornHub
 Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
@@ -32,15 +32,27 @@
 ```
 
 - Or using this repository to get latest features:
 ```sh
 pip install --upgrade git+https://github.com/Egsagon/PHUB.git
 ```
 
-## Usage
+## CLI usage
+You can use phub like so form the terminal to start a small downloading script:
+(Assuming `py` represents your python executable, on linux use `python3`)
+```sh
+py -m phub --help
+```
+
+Example for downloading a video knowing its url, in the best available quality:
+```sh
+py -m phub --url https://... -q 'best'
+````
+
+## Package usage
 Example video download usage:
 ```python
 import phub
 
 client = phub.Client()
 video = client.get('enter video URL here')
```

### Comparing `phub-2.6/README.md` & `phub-2.7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -12,15 +12,27 @@
 ```
 
 - Or using this repository to get latest features:
 ```sh
 pip install --upgrade git+https://github.com/Egsagon/PHUB.git
 ```
 
-## Usage
+## CLI usage
+You can use phub like so form the terminal to start a small downloading script:
+(Assuming `py` represents your python executable, on linux use `python3`)
+```sh
+py -m phub --help
+```
+
+Example for downloading a video knowing its url, in the best available quality:
+```sh
+py -m phub --url https://... -q 'best'
+````
+
+## Package usage
 Example video download usage:
 ```python
 import phub
 
 client = phub.Client()
 video = client.get('enter video URL here')
```

### Comparing `phub-2.6/setup.cfg` & `phub-2.7/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phub
-version = 2.6
+version = 2.7
 description = An API for PornHub
 author = Egsagon
 author_email = egsagon12@gmail.com
 url = https://github.com/Egsagon/PHUB/
 license = GPLv3
 license_file = LICENSE
 long_description = file: README.md
@@ -17,14 +17,16 @@
 	Intended Audience :: Education
 
 [options]
 packages = 
 	phub
 install_requires = 
 	requests>=2
+	tqdm>=4
+	click>=8
 python_requires = >=3.11
 package_dir = 
 	=src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `phub-2.6/src/phub/__init__.py` & `phub-2.7/src/phub/__init__.py`

 * *Files identical despite different names*

### Comparing `phub-2.6/src/phub/__main__.py` & `phub-2.7/src/phub/__main__.py`

 * *Files identical despite different names*

### Comparing `phub-2.6/src/phub/classes.py` & `phub-2.7/src/phub/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import json
 from functools import cached_property
 from datetime import datetime, timedelta
 
 from phub import utils
 from phub import consts
 from phub import parser
-from phub.utils import log
+from phub.utils import log, download_presets as dlp
 
 # Errors
 class UserNotFoundError(Exception): pass
 
 
 @dataclass
 class User:
@@ -241,25 +241,23 @@
         segments = [url_base + segment for segment in utils.extract_urls(raw.text)]
         log('video', f'Parsed {len(segments)} video segments', level = 3)
         return segments
 
     def download(self,
                  path: str,
                  quality: utils.Quality,
-                 quiet: bool = False,
-                 callback: Callable = None,
+                 callback: Callable = dlp.bar(),
                  max_retries: int = 5) -> str:
         '''
         #### Download the video locally. ####
         -------------------------------------
         
         Arguments:
         - `path`               -- Directory or file to write to.
         - `quality`            -- Desired video quality.
-        - `quiet`   (=`False`) -- Whether to enable logs to view download progress.
         - `callback` (=`None`) -- Function to call to update download progress.
         - `max_retries` (=`5`) -- Maximum retries per segment request.
         
         NOTE 1 - If `path` is a directory, will create a new file in that directory
                  with the name of the video.
         NOTE 2 - Slow download. To use threaded downloads, call `get_M3U` instead.
         NOTE 3 - Glitchy logs.
@@ -270,18 +268,14 @@
         log('video', f'Downloading {self} at', path, level = 5)
         
         # Append name if path is directory
         if os.path.isdir(path):
             path += ('' if path.endswith('/') else '/') + utils.pathify(self.title) + '.mp4'
             log('video', f'Changing path to', path, level = 2)
         
-        # Exceptionally allow debugging
-        is_logging = utils.DEBUG
-        if not quiet: utils.DEBUG = True
-        
         log(' D L ', 'Starting video download for', self)
         
         segments = self.get_M3U(quality, process = True)
         
         # Start downloading
         with open(path, 'wb') as output:
             
@@ -295,18 +289,16 @@
                     if not res.ok:                        
                         log(' D L ', f'Segment download failed, retrying ({i}/{max_retries})', level = 1)
                         continue
                     
                     output.write(res.content)
                     break
         
+        # Stop
         log(' D L ', 'Successfully downloaded video at', path)
-        
-        # Reset logging to previous
-        utils.DEBUG = is_logging
         return path
     
     # ======== Properties ======== #
     
     @cached_property
     def title(self) -> str:
         '''
```

### Comparing `phub-2.6/src/phub/consts.py` & `phub-2.7/src/phub/consts.py`

 * *Files identical despite different names*

### Comparing `phub-2.6/src/phub/core.py` & `phub-2.7/src/phub/core.py`

 * *Files identical despite different names*

### Comparing `phub-2.6/src/phub/parser.py` & `phub-2.7/src/phub/parser.py`

 * *Files identical despite different names*

### Comparing `phub-2.6/src/phub/utils.py` & `phub-2.7/src/phub/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 '''
 ### Utilities for the PHUB package. ###
 '''
 
 import sys
 from string import ascii_letters
 
+import tqdm
 from datetime import datetime
 from typing import Callable, Self
 
 from phub import consts
 
 # Debug settings
 DEBUG = False
@@ -168,14 +169,76 @@
         DEBUG_RESET = True
     
     elif r and DEBUG_RESET: print(f'\r{raw}', end = '', file = DEBUG_FILE)
     elif not r and DEBUG_RESET: print(f'\n{raw}', file = DEBUG_FILE)
     else: print(raw, file = DEBUG_FILE)
 
 
+class download_presets:
+    '''
+    Callback presets for displaying download progress.
+    '''
+    
+    @staticmethod
+    def progress(color: bool = True) -> Callable:
+        '''
+        Print current process on one line.
+        '''
+        
+        tem = 'Downloading: {percent}% [{cur}/{total}]'
+        if color:
+            tem = 'Downloading: \033[92m{percent}%\033[0m [\033[93m{cur}\033[0m/\033[93m{total}\033[0m]'
+        
+        def wrapper(cur: int, total: int) -> None:
+            percent = round( (cur / total) * 100 )
+        
+            print(tem.format(percent = percent, cur = cur, total = total),
+                  end = '\n' if percent >= 100 else '')
+        
+        return wrapper
+    
+    @staticmethod
+    def bar(*args, **kwargs) -> Callable:
+        '''
+        Display current progress a a bar.
+        '''
+        
+        bar = tqdm.tqdm(*args, **kwargs)
+        
+        def wrapper(current: int, total: int) -> None:
+            
+            bar.total = total
+            bar.update(1)
+            if current == total: bar.close()
+        
+        return wrapper
+    
+    @staticmethod
+    def std(file = sys.stdout) -> Callable:
+        '''
+        Output progress as percentage to a file.
+        '''
+        
+        def wrapper(cur: int, total: int) -> None:
+            print(round( (cur / total) * 100 ), file = file)
+            
+        return wrapper
+    
+    @staticmethod
+    def percent(callback: Callable) -> Callable:
+        '''
+        Link a function to the percentage output of the progress.
+        '''
+        
+        def wrapper(cur: int, total: int) -> None:
+            callback(round( (cur / total) * 100 ))
+        
+        return wrapper
+
+
 class Quality:
     '''
     Represents a custom quality, e.g.:
     
     ```python
     # Using constants
     Quality.BEST
```

### Comparing `phub-2.6/src/phub.egg-info/PKG-INFO` & `phub-2.7/src/phub.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 2.6
+Version: 2.7
 Summary: An API for PornHub
 Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
@@ -32,15 +32,27 @@
 ```
 
 - Or using this repository to get latest features:
 ```sh
 pip install --upgrade git+https://github.com/Egsagon/PHUB.git
 ```
 
-## Usage
+## CLI usage
+You can use phub like so form the terminal to start a small downloading script:
+(Assuming `py` represents your python executable, on linux use `python3`)
+```sh
+py -m phub --help
+```
+
+Example for downloading a video knowing its url, in the best available quality:
+```sh
+py -m phub --url https://... -q 'best'
+````
+
+## Package usage
 Example video download usage:
 ```python
 import phub
 
 client = phub.Client()
 video = client.get('enter video URL here')
```

