# Comparing `tmp/audiobook-tags-1.1.1.tar.gz` & `tmp/audiobook-tags-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiobook-tags-1.1.1.tar", last modified: Tue Jun 20 04:22:59 2023, max compression
+gzip compressed data, was "audiobook-tags-1.2.0.tar", last modified: Fri Jun 23 03:50:24 2023, max compression
```

## Comparing `audiobook-tags-1.1.1.tar` & `audiobook-tags-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:22:59.373826 audiobook-tags-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-20 04:22:48.000000 audiobook-tags-1.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-20 04:22:48.000000 audiobook-tags-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-20 04:22:59.373826 audiobook-tags-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-20 04:22:48.000000 audiobook-tags-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 04:22:59.373826 audiobook-tags-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-20 04:22:48.000000 audiobook-tags-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:22:59.369826 audiobook-tags-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:22:59.373826 audiobook-tags-1.1.1/src/audiobook_tags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-20 04:22:59.000000 audiobook-tags-1.1.1/src/audiobook_tags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-20 04:22:59.000000 audiobook-tags-1.1.1/src/audiobook_tags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:22:59.000000 audiobook-tags-1.1.1/src/audiobook_tags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 04:22:59.000000 audiobook-tags-1.1.1/src/audiobook_tags.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 04:22:59.000000 audiobook-tags-1.1.1/src/audiobook_tags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:22:59.000000 audiobook-tags-1.1.1/src/audiobook_tags.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:50:24.186730 audiobook-tags-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-23 03:50:09.000000 audiobook-tags-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 03:50:09.000000 audiobook-tags-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-23 03:50:24.186730 audiobook-tags-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-23 03:50:09.000000 audiobook-tags-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 03:50:24.186730 audiobook-tags-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-23 03:50:09.000000 audiobook-tags-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:50:24.186730 audiobook-tags-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:50:24.186730 audiobook-tags-1.2.0/src/audiobook_tags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-23 03:50:24.000000 audiobook-tags-1.2.0/src/audiobook_tags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-23 03:50:24.000000 audiobook-tags-1.2.0/src/audiobook_tags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 03:50:24.000000 audiobook-tags-1.2.0/src/audiobook_tags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 03:50:24.000000 audiobook-tags-1.2.0/src/audiobook_tags.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-23 03:50:24.000000 audiobook-tags-1.2.0/src/audiobook_tags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 03:50:24.000000 audiobook-tags-1.2.0/src/audiobook_tags.egg-info/top_level.txt
```

### Comparing `audiobook-tags-1.1.1/LICENSE.txt` & `audiobook-tags-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `audiobook-tags-1.1.1/PKG-INFO` & `audiobook-tags-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiobook-tags
-Version: 1.1.1
+Version: 1.2.0
 Summary: Fix mp3 tags to use in iTunes/iPhone audiobooks
 Home-page: https://andgineer.github.io/audiobook-tags/
 Author: Andrey Sorokin
 Author-email: andrey@sorokin.engineer
 Keywords: audiobook mp3-tags
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,44 +21,48 @@
 - Fixes sort order.
 - Supports messed encoding like cyrillic Win1251.
 
 Details in [my blog's article](https://sorokin.engineer/posts/en/itunes_audiobook_from_mp3.html).
 
 ## Installation
 
-You should have Python 3.6+ installed.
+You should have Python installed.
 
-    pip install audiobook-tags
+    python -m pip install audiobook-tags
 
 ## Usage
     audiobook-tags [-h] [--encoding ENCODING] [--extension EXTENSION] [--set-tag [SET_TAG ...]] [--track-num TRACK_NUM] [--title-prefix TITLE_PREFIX] [--dry] [folder]
 
     Fixes mp3 tags for iOS audiobooks.
 
     positional arguments:
       folder                Folder to process. By default current folder.
 
     options:
       -h, --help            show this help message and exit
-      --mask MASK, -m MASK  Files mask. By default .mp3
+      --suffix SUFFIX, -s SUFFIX
+                            Files suffix. By default mp3
       --encoding ENCODING, -e ENCODING
                             mp3 tags encoding. "none" if you do not need mp3 tags encoding fix. By default "cp1251".
       --tag [SET_TAG ...], -t [SET_TAG ...]
                             Change mp3 tag to specified string. Format "tag-name/tag-value".
       --num TRACK_NUM, -n TRACK_NUM
-                            Sort files and set mp3 tag `track_num`: TRACK_NUM=`name` - sort by names; TRACK_NUM=`tag-<TAG>` - sort by mp3 tag with name <TAG>.
+                            Sort files and set mp3 tag `track_num`:
+                              --num="name" - sort by names;
+                              --num="tag-<TAG>" - sort by mp3 tag with name <TAG>.
+                                For example to sort by title tag use --num="tag-title".
       --prefix TITLE_PREFIX, -p TITLE_PREFIX
                             Add prefix to title tags. By default `{track:04} - ` if `--num` and no prefix if not.
       --dry, -d             Dry run without changing files.
 
 ## Example:
 
     audiobook-tags --tag="album_artist/Юрий Заборовский (Ардис)" --num="name" --prefix=""
 
-- converts all `.mp3` files in current folder and subfolders
+- converts all `mp3` files in current folder and subfolders
 - fix encoding supposing that original encoding was `Windows 1251`
 - change tag album artist.
 - set `track_num` mp3 tag to file number as ordered by file name.
   But do not add the track number to the title (`--prefix="""`).
 
 # Development
 
@@ -70,7 +74,9 @@
   brew install libmagic
 
 ### Python dependencies
 
 Note the dot before `./activate.sh`:
 
   . ./activate.sh
+
+We use [eyeD3](https://eyed3.readthedocs.io/en/latest/) to work with mp3 tags.
```

### Comparing `audiobook-tags-1.1.1/README.md` & `audiobook-tags-1.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,44 +6,48 @@
 - Fixes sort order.
 - Supports messed encoding like cyrillic Win1251.
 
 Details in [my blog's article](https://sorokin.engineer/posts/en/itunes_audiobook_from_mp3.html).
 
 ## Installation
 
-You should have Python 3.6+ installed.
+You should have Python installed.
 
-    pip install audiobook-tags
+    python -m pip install audiobook-tags
 
 ## Usage
     audiobook-tags [-h] [--encoding ENCODING] [--extension EXTENSION] [--set-tag [SET_TAG ...]] [--track-num TRACK_NUM] [--title-prefix TITLE_PREFIX] [--dry] [folder]
 
     Fixes mp3 tags for iOS audiobooks.
 
     positional arguments:
       folder                Folder to process. By default current folder.
 
     options:
       -h, --help            show this help message and exit
-      --mask MASK, -m MASK  Files mask. By default .mp3
+      --suffix SUFFIX, -s SUFFIX
+                            Files suffix. By default mp3
       --encoding ENCODING, -e ENCODING
                             mp3 tags encoding. "none" if you do not need mp3 tags encoding fix. By default "cp1251".
       --tag [SET_TAG ...], -t [SET_TAG ...]
                             Change mp3 tag to specified string. Format "tag-name/tag-value".
       --num TRACK_NUM, -n TRACK_NUM
-                            Sort files and set mp3 tag `track_num`: TRACK_NUM=`name` - sort by names; TRACK_NUM=`tag-<TAG>` - sort by mp3 tag with name <TAG>.
+                            Sort files and set mp3 tag `track_num`:
+                              --num="name" - sort by names;
+                              --num="tag-<TAG>" - sort by mp3 tag with name <TAG>.
+                                For example to sort by title tag use --num="tag-title".
       --prefix TITLE_PREFIX, -p TITLE_PREFIX
                             Add prefix to title tags. By default `{track:04} - ` if `--num` and no prefix if not.
       --dry, -d             Dry run without changing files.
 
 ## Example:
 
     audiobook-tags --tag="album_artist/Юрий Заборовский (Ардис)" --num="name" --prefix=""
 
-- converts all `.mp3` files in current folder and subfolders
+- converts all `mp3` files in current folder and subfolders
 - fix encoding supposing that original encoding was `Windows 1251`
 - change tag album artist.
 - set `track_num` mp3 tag to file number as ordered by file name.
   But do not add the track number to the title (`--prefix="""`).
 
 # Development
 
@@ -55,7 +59,9 @@
   brew install libmagic
 
 ### Python dependencies
 
 Note the dot before `./activate.sh`:
 
   . ./activate.sh
+
+We use [eyeD3](https://eyed3.readthedocs.io/en/latest/) to work with mp3 tags.
```

### Comparing `audiobook-tags-1.1.1/setup.py` & `audiobook-tags-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `audiobook-tags-1.1.1/src/audiobook_tags.egg-info/PKG-INFO` & `audiobook-tags-1.2.0/src/audiobook_tags.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiobook-tags
-Version: 1.1.1
+Version: 1.2.0
 Summary: Fix mp3 tags to use in iTunes/iPhone audiobooks
 Home-page: https://andgineer.github.io/audiobook-tags/
 Author: Andrey Sorokin
 Author-email: andrey@sorokin.engineer
 Keywords: audiobook mp3-tags
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,44 +21,48 @@
 - Fixes sort order.
 - Supports messed encoding like cyrillic Win1251.
 
 Details in [my blog's article](https://sorokin.engineer/posts/en/itunes_audiobook_from_mp3.html).
 
 ## Installation
 
-You should have Python 3.6+ installed.
+You should have Python installed.
 
-    pip install audiobook-tags
+    python -m pip install audiobook-tags
 
 ## Usage
     audiobook-tags [-h] [--encoding ENCODING] [--extension EXTENSION] [--set-tag [SET_TAG ...]] [--track-num TRACK_NUM] [--title-prefix TITLE_PREFIX] [--dry] [folder]
 
     Fixes mp3 tags for iOS audiobooks.
 
     positional arguments:
       folder                Folder to process. By default current folder.
 
     options:
       -h, --help            show this help message and exit
-      --mask MASK, -m MASK  Files mask. By default .mp3
+      --suffix SUFFIX, -s SUFFIX
+                            Files suffix. By default mp3
       --encoding ENCODING, -e ENCODING
                             mp3 tags encoding. "none" if you do not need mp3 tags encoding fix. By default "cp1251".
       --tag [SET_TAG ...], -t [SET_TAG ...]
                             Change mp3 tag to specified string. Format "tag-name/tag-value".
       --num TRACK_NUM, -n TRACK_NUM
-                            Sort files and set mp3 tag `track_num`: TRACK_NUM=`name` - sort by names; TRACK_NUM=`tag-<TAG>` - sort by mp3 tag with name <TAG>.
+                            Sort files and set mp3 tag `track_num`:
+                              --num="name" - sort by names;
+                              --num="tag-<TAG>" - sort by mp3 tag with name <TAG>.
+                                For example to sort by title tag use --num="tag-title".
       --prefix TITLE_PREFIX, -p TITLE_PREFIX
                             Add prefix to title tags. By default `{track:04} - ` if `--num` and no prefix if not.
       --dry, -d             Dry run without changing files.
 
 ## Example:
 
     audiobook-tags --tag="album_artist/Юрий Заборовский (Ардис)" --num="name" --prefix=""
 
-- converts all `.mp3` files in current folder and subfolders
+- converts all `mp3` files in current folder and subfolders
 - fix encoding supposing that original encoding was `Windows 1251`
 - change tag album artist.
 - set `track_num` mp3 tag to file number as ordered by file name.
   But do not add the track number to the title (`--prefix="""`).
 
 # Development
 
@@ -70,7 +74,9 @@
   brew install libmagic
 
 ### Python dependencies
 
 Note the dot before `./activate.sh`:
 
   . ./activate.sh
+
+We use [eyeD3](https://eyed3.readthedocs.io/en/latest/) to work with mp3 tags.
```

