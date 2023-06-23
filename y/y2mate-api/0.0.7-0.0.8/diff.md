# Comparing `tmp/y2mate-api-0.0.7.tar.gz` & `tmp/y2mate-api-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y2mate-api-0.0.7.tar", last modified: Thu Jun 22 15:49:55 2023, max compression
+gzip compressed data, was "y2mate-api-0.0.8.tar", last modified: Fri Jun 23 12:37:25 2023, max compression
```

## Comparing `y2mate-api-0.0.7.tar` & `y2mate-api-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 15:49:54.864275 y2mate-api-0.0.7/
--rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-0.0.7/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)    10898 2023-06-22 15:49:54.832275 y2mate-api-0.0.7/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     9803 2023-06-22 15:45:15.000000 y2mate-api-0.0.7/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-22 15:49:54.868275 y2mate-api-0.0.7/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1535 2023-06-17 16:53:45.000000 y2mate-api-0.0.7/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 15:49:54.428274 y2mate-api-0.0.7/tests/
--rw-rw----   0 root         (0) everybody  (9997)     1567 2023-06-21 13:35:40.000000 y2mate-api-0.0.7/tests/test_download.py
--rw-rw----   0 root         (0) everybody  (9997)     5577 2023-06-20 21:29:31.000000 y2mate-api-0.0.7/tests/test_queries.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 15:49:54.612275 y2mate-api-0.0.7/y2mate_api/
--rw-rw----   0 root         (0) everybody  (9997)      490 2023-06-22 13:44:12.000000 y2mate-api-0.0.7/y2mate_api/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-19 18:39:03.000000 y2mate-api-0.0.7/y2mate_api/__main__.py
--rw-rw----   0 root         (0) everybody  (9997)     5707 2023-06-22 15:05:00.000000 y2mate-api-0.0.7/y2mate_api/console.py
--rw-rw----   0 root         (0) everybody  (9997)    14654 2023-06-22 15:35:13.000000 y2mate-api-0.0.7/y2mate_api/downloader.py
--rw-rw----   0 root         (0) everybody  (9997)    14730 2023-06-22 12:43:52.000000 y2mate-api-0.0.7/y2mate_api/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-22 15:49:54.808275 y2mate-api-0.0.7/y2mate_api.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)    10898 2023-06-22 15:49:53.000000 y2mate-api-0.0.7/y2mate_api.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      389 2023-06-22 15:49:53.000000 y2mate-api-0.0.7/y2mate_api.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-22 15:49:53.000000 y2mate-api-0.0.7/y2mate_api.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       51 2023-06-22 15:49:53.000000 y2mate-api-0.0.7/y2mate_api.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       85 2023-06-22 15:49:53.000000 y2mate-api-0.0.7/y2mate_api.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-22 15:49:53.000000 y2mate-api-0.0.7/y2mate_api.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 12:37:25.734000 y2mate-api-0.0.8/
+-rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-0.0.8/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)    11042 2023-06-23 12:37:25.718000 y2mate-api-0.0.8/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     9947 2023-06-23 12:11:48.000000 y2mate-api-0.0.8/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-23 12:37:25.734000 y2mate-api-0.0.8/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1590 2023-06-23 12:31:47.000000 y2mate-api-0.0.8/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 12:37:25.262000 y2mate-api-0.0.8/tests/
+-rw-rw----   0 root         (0) everybody  (9997)     1567 2023-06-21 13:35:40.000000 y2mate-api-0.0.8/tests/test_download.py
+-rw-rw----   0 root         (0) everybody  (9997)     5577 2023-06-20 21:29:31.000000 y2mate-api-0.0.8/tests/test_queries.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 12:37:25.386000 y2mate-api-0.0.8/y2mate_api/
+-rw-rw----   0 root         (0) everybody  (9997)      490 2023-06-22 17:33:46.000000 y2mate-api-0.0.8/y2mate_api/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-19 18:39:03.000000 y2mate-api-0.0.8/y2mate_api/__main__.py
+-rw-rw----   0 root         (0) everybody  (9997)     5707 2023-06-22 15:05:00.000000 y2mate-api-0.0.8/y2mate_api/console.py
+-rw-rw----   0 root         (0) everybody  (9997)    14847 2023-06-23 12:01:05.000000 y2mate-api-0.0.8/y2mate_api/downloader.py
+-rw-rw----   0 root         (0) everybody  (9997)    14731 2023-06-22 17:22:06.000000 y2mate-api-0.0.8/y2mate_api/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 12:37:25.650000 y2mate-api-0.0.8/y2mate_api.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)    11042 2023-06-23 12:37:24.000000 y2mate-api-0.0.8/y2mate_api.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      389 2023-06-23 12:37:24.000000 y2mate-api-0.0.8/y2mate_api.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-23 12:37:24.000000 y2mate-api-0.0.8/y2mate_api.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       51 2023-06-23 12:37:24.000000 y2mate-api-0.0.8/y2mate_api.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       85 2023-06-23 12:37:24.000000 y2mate-api-0.0.8/y2mate_api.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-23 12:37:24.000000 y2mate-api-0.0.8/y2mate_api.egg-info/top_level.txt
```

### Comparing `y2mate-api-0.0.7/LICENSE` & `y2mate-api-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.7/PKG-INFO` & `y2mate-api-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.7
+Version: 0.0.8
 Summary: Download youtube videos and audios by title or link
 Home-page: https://github.com/Simatwa/y2mate-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/y2mate-api/issues/new
@@ -22,20 +22,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# y2mate-api
+<h1 align="center">y2mate-api</h1>
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.7&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.8&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -59,21 +59,20 @@
 ```
 
 2. Locally
 
 ```sh
 git clone https://github.com/Simatwa/y2mate-api.git
 cd y2mate-api
-python setup.py build
-python setup.py install
+pip install .
 ```
 
 # Usage 
 
-`$ y2mate <youtube-link or video id or keyword>`
+`$ y2mate -f <mp3/mp4> <youtube-link or video id or keyword>`
 
 <details>
 <summary>
 Developer docs
 </summary>
 1.Generate download links and other metadata
 
@@ -189,18 +188,18 @@
 	
 For more info run `$ y2mate -h`
 
 </summary>
 
 ```
 usage: y2mate [-h] [-v] [-f mp3|mp4]
-              [-q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
+              [-q 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
               [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]]
               [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-              [-t TIMEOUT] [-i PATH] [-o FORMAT]
+              [-t TIMEOUT] [-c CHUNK] [-i PATH] [-o FORMAT]
               [-thr THREAD] [--disable-bar] [--ask]
               [--unique] [--quiet] [--history] [--clear]
               [query ...]
 
 Download youtube videos and audios by title or link
 
 positional arguments:
@@ -209,39 +208,41 @@
 
 options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and
                         exit
   -f mp3|mp4, --format mp3|mp4
                         Specify media type - audio/video
-  -q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps, --quality 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
-                        Media quality -720p
+  -q 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps, --quality 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps
+                        Media quality - auto
   -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3
                         Other media formats incase of
                         multiple options - mp4/mp3
   -k [KEYWORD ...], --keyword [KEYWORD ...]
                         Media should contain this keywords -
                         None
   -a [AUTHOR ...], --author [AUTHOR ...]
                         Media author i.e YouTube channel
                         name - None
   -l LIMIT, --limit LIMIT
                         Total videos to be downloaded - 1
   -d PATH, --dir PATH   Directory for saving the contents -
-                        /storage/emulated/0/git/Smartwa/y2ma
-                        te-api
+                        /data/data/com.termux/files/home
   -t TIMEOUT, --timeout TIMEOUT
                         Http request timeout in seconds - 30
+  -c CHUNK, --chunk CHUNK
+                        Chunk-size for downloading files in
+                        KB - 256
   -i PATH, --input PATH
                         Path to text file containing query
                         per line - None
   -o FORMAT, --output FORMAT
                         Format for generating filename
                         %(key)s : [title,vid,fquality,ftype]
-                        - None
+                        or 'pretty' - None
   -thr THREAD, --thread THREAD
                         Download [x] amount of videos/audios
                         at once - 1
   --disable-bar         Disable download progress bar -
                         False
   --ask                 Confirm before downloading file -
                         False
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.7 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.8 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
 Audience :: Customer Service Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE # y2mate-api
+text/markdown License-File: LICENSE
+                           ****** y2mate-api ******
  [Github] [License] [PyPi] [Black] [Passing] [coverage] [Progress] [Downloads]
 > Download youtube videos and audios by **title/id/url** # Installation -
 Either of the following ways will get you ready. 1. Pip a. From source ```sh
 pip install git+https://github.com/Simatwa/y2mate-api.git ``` b. From pypi
 ```sh pip install y2mate-api ``` 2. Locally ```sh git clone https://github.com/
-Simatwa/y2mate-api.git cd y2mate-api python setup.py build python setup.py
-install ``` # Usage `$ y2mate `   Developer docs  1.Generate download links and
-other metadata - Video ```py from y2mate_api import Handler api = Handler
-("Quantum computing in detail") for video_metadata in api.run(): print
-(video_metadata) """Output { "size": "13.9 MB", "f": "mp4", "q": "720p",
-"q_text": "720p (.mp4)
+Simatwa/y2mate-api.git cd y2mate-api pip install . ``` # Usage `$ y2mate -f
+p4> `   Developer docs  1.Generate download links and other metadata - Video
+```py from y2mate_api import Handler api = Handler("Quantum computing in
+detail") for video_metadata in api.run(): print(video_metadata) """Output
+{ "size": "13.9 MB", "f": "mp4", "q": "720p", "q_text": "720p (.mp4)
 ">m-HD", "k": "joQdX4S3z8ShOJWn6qaA9sL4Al7j4vBwhNgqkwx0U/
 tQ99R4mbX1dYceffBBnNn7", "status": "ok", "mess": "", "c_status": "CONVERTED",
 "vid": "X8MZWCGgIb8", "title": "Quantum Computing In 5 Minutes | Quantum
 Computing Explained | Quantum Computer |Simplilearn", "ftype": "mp4",
 "fquality": "720", "dlink": "https://rr2---sn-gjo-w43s.googlevideo.com/
 videoplayback?expire=1686946638&ei=7m6MZK-
 2NdKQgAepgJGIBg&ip=212.119.40.85&id=o-
@@ -66,35 +66,38 @@
 yields third_query object - `Handler.run` * progress_bar : Stdout media-name &
 Display progress bar - `Handler.save` * third_dict : Response of
 `third_query.run()` * dir : Directory for saving the contents * progress_bar :
 Display download progress bar * quiet : Not to stdout anything * naming_format
 : Format for generating media filename using the `third_query` response keys *
 chunk_size : Size of chunks in KB for downloads    For more info run `$ y2mate
 -h`  ``` usage: y2mate [-h] [-v] [-f mp3|mp4] [-
-q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
+q
+4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
 [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]] [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-[-t TIMEOUT] [-i PATH] [-o FORMAT] [-thr THREAD] [--disable-bar] [--ask] [--
-unique] [--quiet] [--history] [--clear] [query ...] Download youtube videos and
-audios by title or link positional arguments: query Youtube video title, link
-or id - None options: -h, --help show this help message and exit -v, --version
-show program's version number and exit -f mp3|mp4, --format mp3|mp4 Specify
-media type - audio/video -
-q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps,
+[-t TIMEOUT] [-c CHUNK] [-i PATH] [-o FORMAT] [-thr THREAD] [--disable-bar] [--
+ask] [--unique] [--quiet] [--history] [--clear] [query ...] Download youtube
+videos and audios by title or link positional arguments: query Youtube video
+title, link or id - None options: -h, --help show this help message and exit -
+v, --version show program's version number and exit -f mp3|mp4, --format
+mp3|mp4 Specify media type - audio/video -
+q
+4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps,
 --quality
-4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
-Media quality -720p -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3 Other media
+4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps
+Media quality - auto -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3 Other media
 formats incase of multiple options - mp4/mp3 -k [KEYWORD ...], --keyword
 [KEYWORD ...] Media should contain this keywords - None -a [AUTHOR ...], --
 author [AUTHOR ...] Media author i.e YouTube channel name - None -l LIMIT, --
 limit LIMIT Total videos to be downloaded - 1 -d PATH, --dir PATH Directory for
-saving the contents - /storage/emulated/0/git/Smartwa/y2ma te-api -t TIMEOUT, -
--timeout TIMEOUT Http request timeout in seconds - 30 -i PATH, --input PATH
-Path to text file containing query per line - None -o FORMAT, --output FORMAT
-Format for generating filename %(key)s : [title,vid,fquality,ftype] - None -thr
-THREAD, --thread THREAD Download [x] amount of videos/audios at once - 1 --
+saving the contents - /data/data/com.termux/files/home -t TIMEOUT, --timeout
+TIMEOUT Http request timeout in seconds - 30 -c CHUNK, --chunk CHUNK Chunk-size
+for downloading files in KB - 256 -i PATH, --input PATH Path to text file
+containing query per line - None -o FORMAT, --output FORMAT Format for
+generating filename %(key)s : [title,vid,fquality,ftype] or 'pretty' - None -
+thr THREAD, --thread THREAD Download [x] amount of videos/audios at once - 1 --
 disable-bar Disable download progress bar - False --ask Confirm before
 downloading file - False --unique Auto-skip any media that you once dowloaded -
 False --quiet Not to stdout anything other than logs - False --history Stdout
 all media metadata ever downloaded - False --clear Clear all download histories
 - False This script has no official relation with y2mate.com ```  - Review
 [CHANGELOG](https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md)
 for latest updates. ## Disclaimer This repository is intended for educational
```

### Comparing `y2mate-api-0.0.7/README.md` & `y2mate-api-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# y2mate-api
+<h1 align="center">y2mate-api</h1>
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.7&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.8&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -31,21 +31,20 @@
 ```
 
 2. Locally
 
 ```sh
 git clone https://github.com/Simatwa/y2mate-api.git
 cd y2mate-api
-python setup.py build
-python setup.py install
+pip install .
 ```
 
 # Usage 
 
-`$ y2mate <youtube-link or video id or keyword>`
+`$ y2mate -f <mp3/mp4> <youtube-link or video id or keyword>`
 
 <details>
 <summary>
 Developer docs
 </summary>
 1.Generate download links and other metadata
 
@@ -161,18 +160,18 @@
 	
 For more info run `$ y2mate -h`
 
 </summary>
 
 ```
 usage: y2mate [-h] [-v] [-f mp3|mp4]
-              [-q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
+              [-q 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
               [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]]
               [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-              [-t TIMEOUT] [-i PATH] [-o FORMAT]
+              [-t TIMEOUT] [-c CHUNK] [-i PATH] [-o FORMAT]
               [-thr THREAD] [--disable-bar] [--ask]
               [--unique] [--quiet] [--history] [--clear]
               [query ...]
 
 Download youtube videos and audios by title or link
 
 positional arguments:
@@ -181,39 +180,41 @@
 
 options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and
                         exit
   -f mp3|mp4, --format mp3|mp4
                         Specify media type - audio/video
-  -q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps, --quality 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
-                        Media quality -720p
+  -q 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps, --quality 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps
+                        Media quality - auto
   -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3
                         Other media formats incase of
                         multiple options - mp4/mp3
   -k [KEYWORD ...], --keyword [KEYWORD ...]
                         Media should contain this keywords -
                         None
   -a [AUTHOR ...], --author [AUTHOR ...]
                         Media author i.e YouTube channel
                         name - None
   -l LIMIT, --limit LIMIT
                         Total videos to be downloaded - 1
   -d PATH, --dir PATH   Directory for saving the contents -
-                        /storage/emulated/0/git/Smartwa/y2ma
-                        te-api
+                        /data/data/com.termux/files/home
   -t TIMEOUT, --timeout TIMEOUT
                         Http request timeout in seconds - 30
+  -c CHUNK, --chunk CHUNK
+                        Chunk-size for downloading files in
+                        KB - 256
   -i PATH, --input PATH
                         Path to text file containing query
                         per line - None
   -o FORMAT, --output FORMAT
                         Format for generating filename
                         %(key)s : [title,vid,fquality,ftype]
-                        - None
+                        or 'pretty' - None
   -thr THREAD, --thread THREAD
                         Download [x] amount of videos/audios
                         at once - 1
   --disable-bar         Disable download progress bar -
                         False
   --ask                 Confirm before downloading file -
                         False
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-# y2mate-api
+                           ****** y2mate-api ******
  [Github] [License] [PyPi] [Black] [Passing] [coverage] [Progress] [Downloads]
 > Download youtube videos and audios by **title/id/url** # Installation -
 Either of the following ways will get you ready. 1. Pip a. From source ```sh
 pip install git+https://github.com/Simatwa/y2mate-api.git ``` b. From pypi
 ```sh pip install y2mate-api ``` 2. Locally ```sh git clone https://github.com/
-Simatwa/y2mate-api.git cd y2mate-api python setup.py build python setup.py
-install ``` # Usage `$ y2mate `   Developer docs  1.Generate download links and
-other metadata - Video ```py from y2mate_api import Handler api = Handler
-("Quantum computing in detail") for video_metadata in api.run(): print
-(video_metadata) """Output { "size": "13.9 MB", "f": "mp4", "q": "720p",
-"q_text": "720p (.mp4)
+Simatwa/y2mate-api.git cd y2mate-api pip install . ``` # Usage `$ y2mate -f
+p4> `   Developer docs  1.Generate download links and other metadata - Video
+```py from y2mate_api import Handler api = Handler("Quantum computing in
+detail") for video_metadata in api.run(): print(video_metadata) """Output
+{ "size": "13.9 MB", "f": "mp4", "q": "720p", "q_text": "720p (.mp4)
 ">m-HD", "k": "joQdX4S3z8ShOJWn6qaA9sL4Al7j4vBwhNgqkwx0U/
 tQ99R4mbX1dYceffBBnNn7", "status": "ok", "mess": "", "c_status": "CONVERTED",
 "vid": "X8MZWCGgIb8", "title": "Quantum Computing In 5 Minutes | Quantum
 Computing Explained | Quantum Computer |Simplilearn", "ftype": "mp4",
 "fquality": "720", "dlink": "https://rr2---sn-gjo-w43s.googlevideo.com/
 videoplayback?expire=1686946638&ei=7m6MZK-
 2NdKQgAepgJGIBg&ip=212.119.40.85&id=o-
@@ -52,35 +51,38 @@
 yields third_query object - `Handler.run` * progress_bar : Stdout media-name &
 Display progress bar - `Handler.save` * third_dict : Response of
 `third_query.run()` * dir : Directory for saving the contents * progress_bar :
 Display download progress bar * quiet : Not to stdout anything * naming_format
 : Format for generating media filename using the `third_query` response keys *
 chunk_size : Size of chunks in KB for downloads    For more info run `$ y2mate
 -h`  ``` usage: y2mate [-h] [-v] [-f mp3|mp4] [-
-q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
+q
+4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
 [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]] [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-[-t TIMEOUT] [-i PATH] [-o FORMAT] [-thr THREAD] [--disable-bar] [--ask] [--
-unique] [--quiet] [--history] [--clear] [query ...] Download youtube videos and
-audios by title or link positional arguments: query Youtube video title, link
-or id - None options: -h, --help show this help message and exit -v, --version
-show program's version number and exit -f mp3|mp4, --format mp3|mp4 Specify
-media type - audio/video -
-q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps,
+[-t TIMEOUT] [-c CHUNK] [-i PATH] [-o FORMAT] [-thr THREAD] [--disable-bar] [--
+ask] [--unique] [--quiet] [--history] [--clear] [query ...] Download youtube
+videos and audios by title or link positional arguments: query Youtube video
+title, link or id - None options: -h, --help show this help message and exit -
+v, --version show program's version number and exit -f mp3|mp4, --format
+mp3|mp4 Specify media type - audio/video -
+q
+4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps,
 --quality
-4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
-Media quality -720p -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3 Other media
+4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps
+Media quality - auto -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3 Other media
 formats incase of multiple options - mp4/mp3 -k [KEYWORD ...], --keyword
 [KEYWORD ...] Media should contain this keywords - None -a [AUTHOR ...], --
 author [AUTHOR ...] Media author i.e YouTube channel name - None -l LIMIT, --
 limit LIMIT Total videos to be downloaded - 1 -d PATH, --dir PATH Directory for
-saving the contents - /storage/emulated/0/git/Smartwa/y2ma te-api -t TIMEOUT, -
--timeout TIMEOUT Http request timeout in seconds - 30 -i PATH, --input PATH
-Path to text file containing query per line - None -o FORMAT, --output FORMAT
-Format for generating filename %(key)s : [title,vid,fquality,ftype] - None -thr
-THREAD, --thread THREAD Download [x] amount of videos/audios at once - 1 --
+saving the contents - /data/data/com.termux/files/home -t TIMEOUT, --timeout
+TIMEOUT Http request timeout in seconds - 30 -c CHUNK, --chunk CHUNK Chunk-size
+for downloading files in KB - 256 -i PATH, --input PATH Path to text file
+containing query per line - None -o FORMAT, --output FORMAT Format for
+generating filename %(key)s : [title,vid,fquality,ftype] or 'pretty' - None -
+thr THREAD, --thread THREAD Download [x] amount of videos/audios at once - 1 --
 disable-bar Disable download progress bar - False --ask Confirm before
 downloading file - False --unique Auto-skip any media that you once dowloaded -
 False --quiet Not to stdout anything other than logs - False --history Stdout
 all media metadata ever downloaded - False --clear Clear all download histories
 - False This script has no official relation with y2mate.com ```  - Review
 [CHANGELOG](https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md)
 for latest updates. ## Disclaimer This repository is intended for educational
```

### Comparing `y2mate-api-0.0.7/setup.py` & `y2mate-api-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from setuptools import setup
-from y2mate_api import __version__, __author__, __repo__, __info__
+
+version = "0.0.8"
+info = "Download youtube videos and audios by title or link"
+author = "Smartwa"
+repo = "https://github.com/Simatwa/y2mate-api"
 
 setup(
     name="y2mate-api",
     packages=["y2mate_api"],
-    version=__version__,
+    version=version,
     license="MIT",
-    author=__author__,
-    maintainer=__author__,
+    author=author,
+    maintainer=author,
     author_email="smartwacaleb@gmail.com",
-    description=__info__,
-    url=__repo__,
-    project_urls={"Bug Report": f"{__repo__}/issues/new"},
+    description=info,
+    url=repo,
+    project_urls={"Bug Report": f"{repo}/issues/new"},
     install_requires=[
         "argparse>=1.1",
         "requests>=2.0.2",
         "tqdm==4.65.0",
         "colorama==0.4.6",
         "appdirs==1.4.4",
         "getch==1.0",
```

### Comparing `y2mate-api-0.0.7/tests/test_download.py` & `y2mate-api-0.0.8/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.7/tests/test_queries.py` & `y2mate-api-0.0.8/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.7/y2mate_api/console.py` & `y2mate-api-0.0.8/y2mate_api/console.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.7/y2mate_api/downloader.py` & `y2mate-api-0.0.8/y2mate_api/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,15 +250,27 @@
         fnm = (
             f"{naming_format}" % third_dict
             if naming_format
             else f"{third_dict['title']} {third_dict['vid']}_{third_dict['fquality']}.{third_dict['ftype']}"
         )
 
         def sanitize(nm):
-            trash = ["\\", "/", ":", "*", "?", '"', "<", "|", ">","y2mate.com","y2mate com"]
+            trash = [
+                "\\",
+                "/",
+                ":",
+                "*",
+                "?",
+                '"',
+                "<",
+                "|",
+                ">",
+                "y2mate.com",
+                "y2mate com",
+            ]
             for val in trash:
                 nm = nm.replace(val, "")
             return nm.strip()
 
         return sanitize(fnm)
 
     def auto_save(
```

### Comparing `y2mate-api-0.0.7/y2mate_api/main.py` & `y2mate-api-0.0.8/y2mate_api/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,15 +430,15 @@
                 resp_data = hunted[0]
                 resp_data.update(resp.json())
                 return resp_data
 
             else:
                 logging.debug(f"{resp.headers.get('content-type')} - {resp.content}")
                 logging.error(
-                    f"Third query failed - [{resp.status_code} : {resp.reason}"
+                    f"Third query failed - [{resp.status_code} : {resp.reason}]"
                 )
                 return {}
         else:
             logging.error(
                 f"Zero media hunted with params : {{quality : {quality}, format : {format}  }}"
             )
             return {}
```

### Comparing `y2mate-api-0.0.7/y2mate_api.egg-info/PKG-INFO` & `y2mate-api-0.0.8/y2mate_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.7
+Version: 0.0.8
 Summary: Download youtube videos and audios by title or link
 Home-page: https://github.com/Simatwa/y2mate-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/y2mate-api/issues/new
@@ -22,20 +22,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# y2mate-api
+<h1 align="center">y2mate-api</h1>
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.7&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.8&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -59,21 +59,20 @@
 ```
 
 2. Locally
 
 ```sh
 git clone https://github.com/Simatwa/y2mate-api.git
 cd y2mate-api
-python setup.py build
-python setup.py install
+pip install .
 ```
 
 # Usage 
 
-`$ y2mate <youtube-link or video id or keyword>`
+`$ y2mate -f <mp3/mp4> <youtube-link or video id or keyword>`
 
 <details>
 <summary>
 Developer docs
 </summary>
 1.Generate download links and other metadata
 
@@ -189,18 +188,18 @@
 	
 For more info run `$ y2mate -h`
 
 </summary>
 
 ```
 usage: y2mate [-h] [-v] [-f mp3|mp4]
-              [-q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
+              [-q 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
               [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]]
               [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-              [-t TIMEOUT] [-i PATH] [-o FORMAT]
+              [-t TIMEOUT] [-c CHUNK] [-i PATH] [-o FORMAT]
               [-thr THREAD] [--disable-bar] [--ask]
               [--unique] [--quiet] [--history] [--clear]
               [query ...]
 
 Download youtube videos and audios by title or link
 
 positional arguments:
@@ -209,39 +208,41 @@
 
 options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and
                         exit
   -f mp3|mp4, --format mp3|mp4
                         Specify media type - audio/video
-  -q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps, --quality 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
-                        Media quality -720p
+  -q 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps, --quality 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps
+                        Media quality - auto
   -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3
                         Other media formats incase of
                         multiple options - mp4/mp3
   -k [KEYWORD ...], --keyword [KEYWORD ...]
                         Media should contain this keywords -
                         None
   -a [AUTHOR ...], --author [AUTHOR ...]
                         Media author i.e YouTube channel
                         name - None
   -l LIMIT, --limit LIMIT
                         Total videos to be downloaded - 1
   -d PATH, --dir PATH   Directory for saving the contents -
-                        /storage/emulated/0/git/Smartwa/y2ma
-                        te-api
+                        /data/data/com.termux/files/home
   -t TIMEOUT, --timeout TIMEOUT
                         Http request timeout in seconds - 30
+  -c CHUNK, --chunk CHUNK
+                        Chunk-size for downloading files in
+                        KB - 256
   -i PATH, --input PATH
                         Path to text file containing query
                         per line - None
   -o FORMAT, --output FORMAT
                         Format for generating filename
                         %(key)s : [title,vid,fquality,ftype]
-                        - None
+                        or 'pretty' - None
   -thr THREAD, --thread THREAD
                         Download [x] amount of videos/audios
                         at once - 1
   --disable-bar         Disable download progress bar -
                         False
   --ask                 Confirm before downloading file -
                         False
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.7 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.8 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
 Audience :: Customer Service Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE # y2mate-api
+text/markdown License-File: LICENSE
+                           ****** y2mate-api ******
  [Github] [License] [PyPi] [Black] [Passing] [coverage] [Progress] [Downloads]
 > Download youtube videos and audios by **title/id/url** # Installation -
 Either of the following ways will get you ready. 1. Pip a. From source ```sh
 pip install git+https://github.com/Simatwa/y2mate-api.git ``` b. From pypi
 ```sh pip install y2mate-api ``` 2. Locally ```sh git clone https://github.com/
-Simatwa/y2mate-api.git cd y2mate-api python setup.py build python setup.py
-install ``` # Usage `$ y2mate `   Developer docs  1.Generate download links and
-other metadata - Video ```py from y2mate_api import Handler api = Handler
-("Quantum computing in detail") for video_metadata in api.run(): print
-(video_metadata) """Output { "size": "13.9 MB", "f": "mp4", "q": "720p",
-"q_text": "720p (.mp4)
+Simatwa/y2mate-api.git cd y2mate-api pip install . ``` # Usage `$ y2mate -f
+p4> `   Developer docs  1.Generate download links and other metadata - Video
+```py from y2mate_api import Handler api = Handler("Quantum computing in
+detail") for video_metadata in api.run(): print(video_metadata) """Output
+{ "size": "13.9 MB", "f": "mp4", "q": "720p", "q_text": "720p (.mp4)
 ">m-HD", "k": "joQdX4S3z8ShOJWn6qaA9sL4Al7j4vBwhNgqkwx0U/
 tQ99R4mbX1dYceffBBnNn7", "status": "ok", "mess": "", "c_status": "CONVERTED",
 "vid": "X8MZWCGgIb8", "title": "Quantum Computing In 5 Minutes | Quantum
 Computing Explained | Quantum Computer |Simplilearn", "ftype": "mp4",
 "fquality": "720", "dlink": "https://rr2---sn-gjo-w43s.googlevideo.com/
 videoplayback?expire=1686946638&ei=7m6MZK-
 2NdKQgAepgJGIBg&ip=212.119.40.85&id=o-
@@ -66,35 +66,38 @@
 yields third_query object - `Handler.run` * progress_bar : Stdout media-name &
 Display progress bar - `Handler.save` * third_dict : Response of
 `third_query.run()` * dir : Directory for saving the contents * progress_bar :
 Display download progress bar * quiet : Not to stdout anything * naming_format
 : Format for generating media filename using the `third_query` response keys *
 chunk_size : Size of chunks in KB for downloads    For more info run `$ y2mate
 -h`  ``` usage: y2mate [-h] [-v] [-f mp3|mp4] [-
-q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
+q
+4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
 [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]] [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-[-t TIMEOUT] [-i PATH] [-o FORMAT] [-thr THREAD] [--disable-bar] [--ask] [--
-unique] [--quiet] [--history] [--clear] [query ...] Download youtube videos and
-audios by title or link positional arguments: query Youtube video title, link
-or id - None options: -h, --help show this help message and exit -v, --version
-show program's version number and exit -f mp3|mp4, --format mp3|mp4 Specify
-media type - audio/video -
-q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps,
+[-t TIMEOUT] [-c CHUNK] [-i PATH] [-o FORMAT] [-thr THREAD] [--disable-bar] [--
+ask] [--unique] [--quiet] [--history] [--clear] [query ...] Download youtube
+videos and audios by title or link positional arguments: query Youtube video
+title, link or id - None options: -h, --help show this help message and exit -
+v, --version show program's version number and exit -f mp3|mp4, --format
+mp3|mp4 Specify media type - audio/video -
+q
+4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps,
 --quality
-4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
-Media quality -720p -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3 Other media
+4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps
+Media quality - auto -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3 Other media
 formats incase of multiple options - mp4/mp3 -k [KEYWORD ...], --keyword
 [KEYWORD ...] Media should contain this keywords - None -a [AUTHOR ...], --
 author [AUTHOR ...] Media author i.e YouTube channel name - None -l LIMIT, --
 limit LIMIT Total videos to be downloaded - 1 -d PATH, --dir PATH Directory for
-saving the contents - /storage/emulated/0/git/Smartwa/y2ma te-api -t TIMEOUT, -
--timeout TIMEOUT Http request timeout in seconds - 30 -i PATH, --input PATH
-Path to text file containing query per line - None -o FORMAT, --output FORMAT
-Format for generating filename %(key)s : [title,vid,fquality,ftype] - None -thr
-THREAD, --thread THREAD Download [x] amount of videos/audios at once - 1 --
+saving the contents - /data/data/com.termux/files/home -t TIMEOUT, --timeout
+TIMEOUT Http request timeout in seconds - 30 -c CHUNK, --chunk CHUNK Chunk-size
+for downloading files in KB - 256 -i PATH, --input PATH Path to text file
+containing query per line - None -o FORMAT, --output FORMAT Format for
+generating filename %(key)s : [title,vid,fquality,ftype] or 'pretty' - None -
+thr THREAD, --thread THREAD Download [x] amount of videos/audios at once - 1 --
 disable-bar Disable download progress bar - False --ask Confirm before
 downloading file - False --unique Auto-skip any media that you once dowloaded -
 False --quiet Not to stdout anything other than logs - False --history Stdout
 all media metadata ever downloaded - False --clear Clear all download histories
 - False This script has no official relation with y2mate.com ```  - Review
 [CHANGELOG](https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md)
 for latest updates. ## Disclaimer This repository is intended for educational
```

