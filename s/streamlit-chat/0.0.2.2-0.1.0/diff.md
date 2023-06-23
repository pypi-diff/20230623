# Comparing `tmp/streamlit-chat-0.0.2.2.tar.gz` & `tmp/streamlit-chat-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chat-0.0.2.2.tar", last modified: Thu Mar  9 12:28:54 2023, max compression
+gzip compressed data, was "dist/streamlit-chat-0.1.0.tar", last modified: Fri Jun 23 14:55:31 2023, max compression
```

## Comparing `streamlit-chat-0.0.2.2.tar` & `streamlit-chat-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,80 @@
-drwxrwxrwx   0 yashp     (1000) yashp     (1000)        0 2023-03-09 12:28:54.112888 streamlit-chat-0.0.2.2/
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)     1064 2021-12-18 06:15:24.000000 streamlit-chat-0.0.2.2/LICENSE
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)       50 2021-12-27 01:53:00.000000 streamlit-chat-0.0.2.2/MANIFEST.in
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)     1197 2023-03-09 12:28:54.105840 streamlit-chat-0.0.2.2/PKG-INFO
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)      698 2023-03-09 11:33:59.000000 streamlit-chat-0.0.2.2/README.md
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)       38 2023-03-09 12:28:54.114923 streamlit-chat-0.0.2.2/setup.cfg
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)      919 2023-03-09 12:28:03.000000 streamlit-chat-0.0.2.2/setup.py
-drwxrwxrwx   0 yashp     (1000) yashp     (1000)        0 2023-03-09 12:28:52.798503 streamlit-chat-0.0.2.2/streamlit_chat/
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)     3343 2023-03-09 12:19:08.000000 streamlit-chat-0.0.2.2/streamlit_chat/__init__.py
-drwxrwxrwx   0 yashp     (1000) yashp     (1000)        0 2023-03-09 12:28:52.551566 streamlit-chat-0.0.2.2/streamlit_chat/frontend/
-drwxrwxrwx   0 yashp     (1000) yashp     (1000)        0 2023-03-09 12:28:53.376669 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)      859 2023-03-09 12:04:15.000000 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/asset-manifest.json
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)   197459 2023-03-09 12:00:56.000000 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/bootstrap.min.css
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)   646432 2023-03-09 12:00:56.000000 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/bootstrap.min.css.map
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)     2101 2023-03-09 12:04:15.000000 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/index.html
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)      564 2023-03-09 12:04:15.000000 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/precache-manifest.9ba864910e4b9dd4b3cd9c536c2918f1.js
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)     1183 2023-03-09 12:04:15.000000 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/service-worker.js
-drwxrwxrwx   0 yashp     (1000) yashp     (1000)        0 2023-03-09 12:28:52.600642 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/static/
-drwxrwxrwx   0 yashp     (1000) yashp     (1000)        0 2023-03-09 12:28:54.035445 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/static/js/
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)   490293 2023-03-09 12:04:15.000000 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/static/js/2.995d757f.chunk.js
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)     1653 2023-03-09 12:04:15.000000 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/static/js/2.995d757f.chunk.js.LICENSE.txt
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)  1704701 2023-03-09 12:04:15.000000 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/static/js/2.995d757f.chunk.js.map
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)     1799 2023-03-09 12:04:15.000000 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/static/js/main.5efa2225.chunk.js
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)     3946 2023-03-09 12:04:15.000000 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/static/js/main.5efa2225.chunk.js.map
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)     1598 2023-03-09 12:04:15.000000 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)     8317 2023-03-09 12:04:15.000000 streamlit-chat-0.0.2.2/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxrwxrwx   0 yashp     (1000) yashp     (1000)        0 2023-03-09 12:28:52.999563 streamlit-chat-0.0.2.2/streamlit_chat.egg-info/
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)     1197 2023-03-09 12:28:51.000000 streamlit-chat-0.0.2.2/streamlit_chat.egg-info/PKG-INFO
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)     1037 2023-03-09 12:28:52.000000 streamlit-chat-0.0.2.2/streamlit_chat.egg-info/SOURCES.txt
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)        1 2023-03-09 12:28:51.000000 streamlit-chat-0.0.2.2/streamlit_chat.egg-info/dependency_links.txt
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)       16 2023-03-09 12:28:51.000000 streamlit-chat-0.0.2.2/streamlit_chat.egg-info/requires.txt
--rwxrwxrwx   0 yashp     (1000) yashp     (1000)       15 2023-03-09 12:28:51.000000 streamlit-chat-0.0.2.2/streamlit_chat.egg-info/top_level.txt
+drwxrwxrwx   0 yashp     (1000) yashp     (1000)        0 2023-06-23 14:55:31.000000 streamlit-chat-0.1.0/
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     1064 2021-12-18 06:15:24.000000 streamlit-chat-0.1.0/LICENSE
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)       49 2023-06-23 14:37:23.000000 streamlit-chat-0.1.0/MANIFEST.in
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     1722 2023-06-23 14:55:31.000000 streamlit-chat-0.1.0/PKG-INFO
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     1225 2023-06-23 12:49:11.000000 streamlit-chat-0.1.0/README.md
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)       38 2023-06-23 14:55:31.000000 streamlit-chat-0.1.0/setup.cfg
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)      917 2023-06-23 14:54:58.000000 streamlit-chat-0.1.0/setup.py
+drwxrwxrwx   0 yashp     (1000) yashp     (1000)        0 2023-06-23 14:55:26.000000 streamlit-chat-0.1.0/streamlit_chat/
+drwxrwxrwx   0 yashp     (1000) yashp     (1000)        0 2023-06-23 14:55:26.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/
+drwxrwxrwx   0 yashp     (1000) yashp     (1000)        0 2023-06-23 14:55:26.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/
+drwxrwxrwx   0 yashp     (1000) yashp     (1000)        0 2023-06-23 14:55:31.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    29147 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/index-11ac706c.css
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)  1179411 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/index-e3f228e0.js
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    28076 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_AMS-Regular-0cdd387c.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    33516 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_AMS-Regular-30da91e8.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    63632 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_AMS-Regular-68534840.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    12368 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Caligraphic-Bold-07d8e303.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     7716 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Caligraphic-Bold-1ae6bd74.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     6912 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Caligraphic-Bold-de7701e4.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     7656 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Caligraphic-Regular-3398dd02.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     6908 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Caligraphic-Regular-5d53e70a.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    12344 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Caligraphic-Regular-ed0b7437.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    11348 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Fraktur-Bold-74444efd.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    19584 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Fraktur-Bold-9163df9c.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    13296 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Fraktur-Bold-9be7ceb8.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    19572 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Fraktur-Regular-1e6f9579.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    11316 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Fraktur-Regular-51814d27.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    13208 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Fraktur-Regular-5e28753b.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    25324 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Main-Bold-0f60d1b8.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    51336 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Main-Bold-138ac28d.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    29912 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Main-Bold-c76c5d69.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    32968 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Main-BoldItalic-70ee1f64.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    16780 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Main-BoldItalic-99cd42a3.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    19412 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Main-BoldItalic-a6f7ec0d.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    33580 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Main-Italic-0d85ae7c.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    16988 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Main-Italic-97479ca6.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    19676 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Main-Italic-f1d6ef86.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    26272 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Main-Regular-c2342cd8.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    30772 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Main-Regular-c6368d87.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    53580 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Main-Regular-d0332f52.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    18668 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Math-BoldItalic-850c0af5.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    16400 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Math-BoldItalic-dc47344d.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    31196 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Math-BoldItalic-f9377ab0.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    31308 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Math-Italic-08ce98e5.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    16440 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Math-Italic-7af58c5e.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    18748 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Math-Italic-8a8d2445.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    24504 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_SansSerif-Bold-1ece03f7.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    12216 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_SansSerif-Bold-e99ae511.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    14408 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_SansSerif-Bold-ece03cfd.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    12028 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_SansSerif-Italic-00b26ac8.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    22364 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_SansSerif-Italic-3931dd81.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    14112 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_SansSerif-Italic-91ee6750.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    12316 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_SansSerif-Regular-11e4dc8a.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    10344 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_SansSerif-Regular-68e8c73e.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    19436 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_SansSerif-Regular-f36ea897.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     9644 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Script-Regular-036d4e95.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    16648 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Script-Regular-1c67f068.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    10588 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Script-Regular-d96cdf2b.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     5468 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Size1-Regular-6b47c401.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    12228 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Size1-Regular-95b6d2f1.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     6496 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Size1-Regular-c943cc98.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     6188 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Size2-Regular-2014c523.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    11508 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Size2-Regular-a6b2099f.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     5208 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Size2-Regular-d04c5421.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     7588 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Size3-Regular-500e04d5.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     4420 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Size3-Regular-6ab6b62e.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     5980 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Size4-Regular-99f9c675.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     4928 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Size4-Regular-a4af7d41.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    10364 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Size4-Regular-c647367d.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    13568 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Typewriter-Regular-71d517d6.woff2
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    16028 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Typewriter-Regular-e14fed02.woff
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)    27556 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/assets/KaTeX_Typewriter-Regular-f01f3e87.ttf
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)      404 2023-06-23 14:32:36.000000 streamlit-chat-0.1.0/streamlit_chat/frontend/dist/index.html
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     3136 2023-06-23 14:32:42.000000 streamlit-chat-0.1.0/streamlit_chat/__init__.py
+drwxrwxrwx   0 yashp     (1000) yashp     (1000)        0 2023-06-23 14:55:26.000000 streamlit-chat-0.1.0/streamlit_chat.egg-info/
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)        1 2023-06-23 14:55:24.000000 streamlit-chat-0.1.0/streamlit_chat.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     1722 2023-06-23 14:55:24.000000 streamlit-chat-0.1.0/streamlit_chat.egg-info/PKG-INFO
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)       16 2023-06-23 14:55:24.000000 streamlit-chat-0.1.0/streamlit_chat.egg-info/requires.txt
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)     4583 2023-06-23 14:55:26.000000 streamlit-chat-0.1.0/streamlit_chat.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yashp     (1000) yashp     (1000)       15 2023-06-23 14:55:24.000000 streamlit-chat-0.1.0/streamlit_chat.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `streamlit-chat-0.0.2.2/LICENSE` & `streamlit-chat-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-chat-0.0.2.2/PKG-INFO` & `streamlit-chat-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,41 @@
 Metadata-Version: 2.1
 Name: streamlit-chat
-Version: 0.0.2.2
+Version: 0.1.0
 Summary: A streamlit component, to make chatbots
 Home-page: https://github.com/AI-Yash/st-chat
 Author: Yash Pravin Pawar, Yash Vardhan Kapil
 Author-email: yashpawarp@gmail.com
 License: UNKNOWN
 Keywords: chat streamlit streamlit-component
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# st-chat
+<!-- # Welcome to MkDocs
+
+For full documentation visit [mkdocs.org](https://www.mkdocs.org).
+
+## Commands
+
+* `mkdocs new [dir-name]` - Create a new project.
+* `mkdocs serve` - Start the live-reloading docs server.
+* `mkdocs build` - Build the documentation site.
+* `mkdocs -h` - Print help message and exit.
+
+## Project layout
+
+    mkdocs.yml    # The configuration file.
+    docs/
+        index.md  # The documentation homepage.
+        ...       # Other markdown pages, images and other files. -->
+# Welcome to Streamlit Chat [st-chat]
 
 Streamlit Component, for a Chat-bot UI, [example app](https://share.streamlit.io/ai-yash/st-chat/main/examples/chatbot.py)
 
 authors - [@yashppawar](https://github.com/yashppawar) & [@YashVardhan-AI](https://github.com/yashvardhan-ai)
 
 ## Installation
 
@@ -32,12 +49,12 @@
 import streamlit as st
 from streamlit_chat import message
 
 message("My message") 
 message("Hello bot!", is_user=True)  # align's the message to the right
 ```
    
-### Screenshot
+## Screenshot
 
 ![chatbot-og](https://user-images.githubusercontent.com/90775147/210397700-5ab9e00d-a61b-4bc9-a34a-b5bd4454b084.png)
```

### Comparing `streamlit-chat-0.0.2.2/setup.py` & `streamlit-chat-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setuptools.setup(
     name="streamlit-chat",
-    version="0.0.2.2",
+    version="0.1.0",
     author="Yash Pravin Pawar, Yash Vardhan Kapil",
     author_email="yashpawarp@gmail.com",
     description="A streamlit component, to make chatbots",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-Yash/st-chat",
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     keywords="chat streamlit streamlit-component",
-    python_requires=">=3.8",
+    python_requires=">=3.6",
     install_requires=[
         # By definition, a Custom Component depends on Streamlit.
         # If your component has other Python dependencies, list
         # them here.
         "streamlit >= 0.63",
     ],
 )
```

### Comparing `streamlit-chat-0.0.2.2/streamlit_chat.egg-info/PKG-INFO` & `streamlit-chat-0.1.0/streamlit_chat.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,41 @@
 Metadata-Version: 2.1
 Name: streamlit-chat
-Version: 0.0.2.2
+Version: 0.1.0
 Summary: A streamlit component, to make chatbots
 Home-page: https://github.com/AI-Yash/st-chat
 Author: Yash Pravin Pawar, Yash Vardhan Kapil
 Author-email: yashpawarp@gmail.com
 License: UNKNOWN
 Keywords: chat streamlit streamlit-component
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# st-chat
+<!-- # Welcome to MkDocs
+
+For full documentation visit [mkdocs.org](https://www.mkdocs.org).
+
+## Commands
+
+* `mkdocs new [dir-name]` - Create a new project.
+* `mkdocs serve` - Start the live-reloading docs server.
+* `mkdocs build` - Build the documentation site.
+* `mkdocs -h` - Print help message and exit.
+
+## Project layout
+
+    mkdocs.yml    # The configuration file.
+    docs/
+        index.md  # The documentation homepage.
+        ...       # Other markdown pages, images and other files. -->
+# Welcome to Streamlit Chat [st-chat]
 
 Streamlit Component, for a Chat-bot UI, [example app](https://share.streamlit.io/ai-yash/st-chat/main/examples/chatbot.py)
 
 authors - [@yashppawar](https://github.com/yashppawar) & [@YashVardhan-AI](https://github.com/yashvardhan-ai)
 
 ## Installation
 
@@ -32,12 +49,12 @@
 import streamlit as st
 from streamlit_chat import message
 
 message("My message") 
 message("Hello bot!", is_user=True)  # align's the message to the right
 ```
    
-### Screenshot
+## Screenshot
 
 ![chatbot-og](https://user-images.githubusercontent.com/90775147/210397700-5ab9e00d-a61b-4bc9-a34a-b5bd4454b084.png)
```

