# Comparing `tmp/rubbrband-0.2.5.tar.gz` & `tmp/rubbrband-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubbrband-0.2.5.tar", last modified: Mon Jun 19 21:08:30 2023, max compression
+gzip compressed data, was "rubbrband-0.2.6.tar", last modified: Fri Jun 23 04:42:24 2023, max compression
```

## Comparing `rubbrband-0.2.5.tar` & `rubbrband-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-19 21:08:30.611046 rubbrband-0.2.5/
--rw-r--r--   0 llewyn     (501) staff       (20)    11357 2023-03-07 10:22:28.000000 rubbrband-0.2.5/LICENSE
--rw-r--r--   0 llewyn     (501) staff       (20)       48 2023-02-24 08:26:52.000000 rubbrband-0.2.5/MANIFEST.in
--rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-06-19 21:08:30.611101 rubbrband-0.2.5/PKG-INFO
--rw-r--r--   0 llewyn     (501) staff       (20)       54 2023-06-07 21:39:04.000000 rubbrband-0.2.5/README.md
--rw-r--r--   0 llewyn     (501) staff       (20)      103 2023-06-19 21:07:21.000000 rubbrband-0.2.5/pyproject.toml
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-19 21:08:30.610217 rubbrband-0.2.5/rubbrband/
--rw-r--r--   0 llewyn     (501) staff       (20)       61 2023-06-07 21:45:01.000000 rubbrband-0.2.5/rubbrband/__init__.py
--rw-r--r--   0 llewyn     (501) staff       (20)     1358 2023-06-19 20:39:18.000000 rubbrband-0.2.5/rubbrband/main.py
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-19 21:08:30.610941 rubbrband-0.2.5/rubbrband.egg-info/
--rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-06-19 21:08:30.000000 rubbrband-0.2.5/rubbrband.egg-info/PKG-INFO
--rw-r--r--   0 llewyn     (501) staff       (20)      267 2023-06-19 21:08:30.000000 rubbrband-0.2.5/rubbrband.egg-info/SOURCES.txt
--rw-r--r--   0 llewyn     (501) staff       (20)        1 2023-06-19 21:08:30.000000 rubbrband-0.2.5/rubbrband.egg-info/dependency_links.txt
--rw-r--r--   0 llewyn     (501) staff       (20)       16 2023-06-19 21:08:30.000000 rubbrband-0.2.5/rubbrband.egg-info/requires.txt
--rw-r--r--   0 llewyn     (501) staff       (20)       10 2023-06-19 21:08:30.000000 rubbrband-0.2.5/rubbrband.egg-info/top_level.txt
--rw-r--r--   0 llewyn     (501) staff       (20)      259 2023-06-19 21:08:30.611308 rubbrband-0.2.5/setup.cfg
--rw-r--r--   0 llewyn     (501) staff       (20)      182 2023-06-19 21:07:10.000000 rubbrband-0.2.5/setup.py
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-23 04:42:24.686425 rubbrband-0.2.6/
+-rw-r--r--   0 llewyn     (501) staff       (20)    11357 2023-03-07 10:22:28.000000 rubbrband-0.2.6/LICENSE
+-rw-r--r--   0 llewyn     (501) staff       (20)       48 2023-02-24 08:26:52.000000 rubbrband-0.2.6/MANIFEST.in
+-rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-06-23 04:42:24.686481 rubbrband-0.2.6/PKG-INFO
+-rw-r--r--   0 llewyn     (501) staff       (20)       54 2023-06-07 21:39:04.000000 rubbrband-0.2.6/README.md
+-rw-r--r--   0 llewyn     (501) staff       (20)      103 2023-06-19 21:09:40.000000 rubbrband-0.2.6/pyproject.toml
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-23 04:42:24.685709 rubbrband-0.2.6/rubbrband/
+-rw-r--r--   0 llewyn     (501) staff       (20)       61 2023-06-07 21:45:01.000000 rubbrband-0.2.6/rubbrband/__init__.py
+-rw-r--r--   0 llewyn     (501) staff       (20)     1473 2023-06-23 04:41:52.000000 rubbrband-0.2.6/rubbrband/main.py
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-23 04:42:24.686318 rubbrband-0.2.6/rubbrband.egg-info/
+-rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-06-23 04:42:24.000000 rubbrband-0.2.6/rubbrband.egg-info/PKG-INFO
+-rw-r--r--   0 llewyn     (501) staff       (20)      267 2023-06-23 04:42:24.000000 rubbrband-0.2.6/rubbrband.egg-info/SOURCES.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)        1 2023-06-23 04:42:24.000000 rubbrband-0.2.6/rubbrband.egg-info/dependency_links.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)       16 2023-06-23 04:42:24.000000 rubbrband-0.2.6/rubbrband.egg-info/requires.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)       10 2023-06-23 04:42:24.000000 rubbrband-0.2.6/rubbrband.egg-info/top_level.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)      259 2023-06-23 04:42:24.686703 rubbrband-0.2.6/setup.cfg
+-rw-r--r--   0 llewyn     (501) staff       (20)      182 2023-06-19 21:09:40.000000 rubbrband-0.2.6/setup.py
```

### Comparing `rubbrband-0.2.5/LICENSE` & `rubbrband-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rubbrband-0.2.5/rubbrband/main.py` & `rubbrband-0.2.6/rubbrband/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,11 +48,14 @@
         return False
 
     response = response["url"]
 
     files = {"file": (name, image)}
     http_response = requests.post(response["url"], data=response["fields"], files=files)
 
-    if http_response.status_code == 204:
-        print(f"Successfully uploaded {name}")
-    else:
-        print(f"Upload failed: {http_response.text}")
+    image_url = f"https://rubbrband-image-bucket.s3.amazonaws.com/{api_key}/{name}"
+    block_req = requests.post(
+        f"https://block.rubbrband.com/process_img?api_key={api_key}&image_url={image_url}",
+        json={"metadata": metadata},
+    )
+
+    return True
```

