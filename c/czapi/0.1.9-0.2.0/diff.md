# Comparing `tmp/czapi-0.1.9.tar.gz` & `tmp/czapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\czapi-0.1.9.tar", last modified: Sat May 20 20:55:04 2023, max compression
+gzip compressed data, was "dist\czapi-0.2.0.tar", last modified: Fri Jun 23 03:57:09 2023, max compression
```

## Comparing `czapi-0.1.9.tar` & `czapi-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 20:55:04.000000 czapi-0.1.9/
--rw-rw-rw-   0        0        0     2381 2022-02-26 15:53:17.000000 czapi-0.1.9/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11558 2022-02-26 15:53:17.000000 czapi-0.1.9/LICENSE
--rw-rw-rw-   0        0        0      116 2022-02-26 15:53:17.000000 czapi-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0    34990 2023-05-20 20:55:04.000000 czapi-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0    34232 2023-05-20 20:53:19.000000 czapi-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi/
--rw-rw-rw-   0        0        0       23 2023-05-20 20:54:48.000000 czapi-0.1.9/czapi/__init__.py
--rw-rw-rw-   0        0        0     1418 2023-05-20 20:53:06.000000 czapi-0.1.9/czapi/_nbdev.py
--rw-rw-rw-   0        0        0      249 2023-05-20 20:53:06.000000 czapi-0.1.9/czapi/api.py
-drwxrwxrwx   0        0        0        0 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi/core/
--rw-rw-rw-   0        0        0        0 2023-03-10 03:45:51.000000 czapi-0.1.9/czapi/core/__init__.py
--rw-rw-rw-   0        0        0     1140 2023-05-20 20:53:06.000000 czapi-0.1.9/czapi/core/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi/core/scraping/
--rw-rw-rw-   0        0        0        0 2022-12-21 13:02:35.000000 czapi-0.1.9/czapi/core/scraping/__init__.py
--rw-rw-rw-   0        0        0    11369 2023-05-20 20:53:06.000000 czapi-0.1.9/czapi/core/scraping/base.py
--rw-rw-rw-   0        0        0     1641 2023-05-20 20:53:06.000000 czapi-0.1.9/czapi/core/testing.py
--rw-rw-rw-   0        0        0      633 2023-05-20 20:53:06.000000 czapi-0.1.9/czapi/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi.egg-info/
--rw-rw-rw-   0        0        0    34990 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-02-26 16:04:21.000000 czapi-0.1.9/czapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      612 2023-05-20 20:54:48.000000 czapi-0.1.9/settings.ini
--rw-rw-rw-   0        0        0       42 2023-05-20 20:55:04.000000 czapi-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     3158 2022-02-26 15:53:17.000000 czapi-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:57:09.000000 czapi-0.2.0/
+-rw-rw-rw-   0        0        0     2381 2022-02-26 15:53:17.000000 czapi-0.2.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11558 2022-02-26 15:53:17.000000 czapi-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      116 2022-02-26 15:53:17.000000 czapi-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    48870 2023-06-23 03:57:09.000000 czapi-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    48112 2023-06-23 02:40:42.000000 czapi-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 03:57:09.000000 czapi-0.2.0/czapi/
+-rw-rw-rw-   0        0        0       23 2023-06-23 02:40:22.000000 czapi-0.2.0/czapi/__init__.py
+-rw-rw-rw-   0        0        0     1457 2023-06-23 02:40:22.000000 czapi-0.2.0/czapi/_nbdev.py
+-rw-rw-rw-   0        0        0      249 2023-06-23 02:40:22.000000 czapi-0.2.0/czapi/api.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:57:09.000000 czapi-0.2.0/czapi/core/
+-rw-rw-rw-   0        0        0        0 2023-03-10 03:45:51.000000 czapi-0.2.0/czapi/core/__init__.py
+-rw-rw-rw-   0        0        0     1140 2023-06-23 02:40:22.000000 czapi-0.2.0/czapi/core/errors.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:57:09.000000 czapi-0.2.0/czapi/core/scraping/
+-rw-rw-rw-   0        0        0        0 2022-12-21 13:02:35.000000 czapi-0.2.0/czapi/core/scraping/__init__.py
+-rw-rw-rw-   0        0        0    11842 2023-06-23 02:40:22.000000 czapi-0.2.0/czapi/core/scraping/base.py
+-rw-rw-rw-   0        0        0     1641 2023-06-23 02:40:22.000000 czapi-0.2.0/czapi/core/testing.py
+-rw-rw-rw-   0        0        0      633 2023-06-23 02:40:22.000000 czapi-0.2.0/czapi/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:57:09.000000 czapi-0.2.0/czapi.egg-info/
+-rw-rw-rw-   0        0        0    48870 2023-06-23 03:57:08.000000 czapi-0.2.0/czapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-06-23 03:57:08.000000 czapi-0.2.0/czapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 03:57:08.000000 czapi-0.2.0/czapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-23 03:57:08.000000 czapi-0.2.0/czapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-02-26 16:04:21.000000 czapi-0.2.0/czapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-06-23 03:57:08.000000 czapi-0.2.0/czapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-23 03:57:08.000000 czapi-0.2.0/czapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      612 2023-06-23 02:35:21.000000 czapi-0.2.0/settings.ini
+-rw-rw-rw-   0        0        0       42 2023-06-23 03:57:09.000000 czapi-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     3158 2022-02-26 15:53:17.000000 czapi-0.2.0/setup.py
```

### Comparing `czapi-0.1.9/CONTRIBUTING.md` & `czapi-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `czapi-0.1.9/LICENSE` & `czapi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `czapi-0.1.9/PKG-INFO` & `czapi-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: czapi
-Version: 0.1.9
-Summary: CurlingZone scraper API.
-Home-page: https://github.com/calicorob/czapi/tree/master/
-Author: Robert Currie
-Author-email: robert.art.currie@gmail.com
-License: Apache Software License 2.0
-Keywords: curling,stats
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Welcome to czapi
 > A basic API for scraping curling boxscores off of the popular <a href='https://www.curlingzone.com'>CurlingZone</a> website. 
 
 
 ## Install
 
 ```
@@ -224,15 +202,15 @@
 ```python
 normalized_boxscore.guid
 ```
 
 
 
 
-    154352576001077780910640079893588160113
+    129690655252279755696295239689104705205
 
 
 
 czapi's `get_flat_boxscores_from` function takes a `cz_event_id` and `cz_draw_id` as an arguments and returns a (flat) nested list object of all the boxscore information on the linescore page. This nested list object can be ingested into a pandas DataFrame or pushed to a SQL database.
 
 ```python
 api.get_flat_boxscores_from(cz_event_id = 6400, cz_draw_id = 2)
@@ -246,85 +224,85 @@
       True,
       ['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'],
       '5',
       2,
       'Draw: 2',
       [True, True, False, True, True, True, True, False, False, False],
       [0, 0, 2, -2, -2, -2, -3, -2, -1, 0],
-      306528221620467227442052913955328486003),
+      296656328202528204780428618855733007061),
      ('Matthew Hall',
       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
       False,
       ['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'],
       '7',
       2,
       'Draw: 2',
       [False, False, True, False, False, False, False, True, True, True],
       [0, 0, -2, 2, 2, 2, 3, 2, 1, 0],
-      306528221620467227442052913955328486003),
+      296656328202528204780428618855733007061),
      ('Dayna Deruelle',
       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144346&profileid=26636#1',
       False,
       ['0', '0', '1', '0', '0', '0', '0', 'X'],
       '1',
       2,
       'Draw: 2',
       [False, False, True, False, True, True, True, True],
       [0, 0, -2, -1, -3, -4, -5, -9],
-      169959036371998794200683443427801286021),
+      105249071225393527432485074456849437076),
      ('Tyler Stewart',
       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
       True,
       ['0', '2', '0', '2', '1', '1', '4', 'X'],
       '10',
       2,
       'Draw: 2',
       [True, True, False, True, False, False, False, False],
       [0, 0, 2, 1, 3, 4, 5, 9],
-      169959036371998794200683443427801286021),
+      105249071225393527432485074456849437076),
      ('Mark Kean',
       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
       True,
       ['2', '0', '1', '0', '0', '0', '1', '3', 'X'],
       '7',
       2,
       'Draw: 2',
       [True, False, False, False, False, True, True, False, False],
       [0, 2, 2, 3, 3, 1, 0, 1, 4],
-      216723633949199876308042205365369844269),
+      17103980631020054974876512539607901632),
      ('Jason March',
       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
       False,
       ['0', '0', '0', '0', '2', '1', '0', '0', 'X'],
       '3',
       2,
       'Draw: 2',
       [False, True, True, True, True, False, False, True, True],
       [0, -2, -2, -3, -3, -1, 0, -1, -4],
-      216723633949199876308042205365369844269),
+      17103980631020054974876512539607901632),
      ('Richard Krell',
       'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144349&profileid=25962#1',
       True,
       ['2', '0', '1', '0', '2', '1', '1', 'X'],
       '7',
       2,
       'Draw: 2',
       [True, False, False, False, True, False, False, False],
       [0, 2, 2, 3, 2, 4, 5, 6],
-      142335171424399828625133635146510278418),
+      215489388707487834967933616755032135426),
      ('Rob Ainsley',
       'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
       False,
       ['0', '0', '0', '1', '0', '0', '0', 'X'],
       '1',
       2,
       'Draw: 2',
       [False, True, True, True, False, True, True, True],
       [0, -2, -2, -3, -2, -4, -5, -6],
-      142335171424399828625133635146510278418)]
+      215489388707487834967933616755032135426)]
 
 
 
 ## Event
 
 The `Event` object is a data structure which holds all of the `LinescorePage` objects which make up an entire event. 
 
@@ -449,503 +427,473 @@
        'href': 'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
        'score': ['2', '1', '0', '0', '1', '2', '1', '1', 'X'],
        'hammer': True,
        'finalscore': '8'}}]
 
 
 
-The `get_flat_boxscores` method can be used to return a list of (flat) nested list object of all the boxscore information on all the linescore pages.
-
-```python
-event.get_flat_boxscores()
-```
-
-
-
-
-    [[('Damien Villard',
-       'event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1',
-       True,
-       ['0', '0', '0', '0', 'X'],
-       '0',
-       1,
-       'Draw: 1',
-       [True, True, True, True, True],
-       [0, -1, -4, -6, -8],
-       227597408989477916004520082463493572762),
-      ('Matthew Hall',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
-       False,
-       ['1', '3', '2', '2', 'X'],
-       '8',
-       1,
-       'Draw: 1',
-       [False, False, False, False, False],
-       [0, 1, 4, 6, 8],
-       227597408989477916004520082463493572762),
-      ('Matthew Mepstead',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144356#1',
-       False,
-       ['0', '0', '1', '1', '0', '1', '0', '0', '0', '1', '0'],
-       '4',
-       1,
-       'Draw: 1',
-       [False, False, True, False, False, True, False, False, False, True, False],
-       [0, 0, -2, -1, 0, -1, 0, 0, 0, -1, 0],
-       230481195381514558834165699232540581342),
-      ('Tyler Stewart',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
-       True,
-       ['0', '2', '0', '0', '1', '0', '0', '0', '1', '0', '1'],
-       '5',
-       1,
-       'Draw: 1',
-       [True, True, False, True, True, False, True, True, True, False, True],
-       [0, 0, 2, 1, 0, 1, 0, 0, 0, 1, 0],
-       230481195381514558834165699232540581342),
-      ('Jason March',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
-       False,
-       ['0', '2', '0', '1', '0', '2', '2', '0', '2', 'X'],
-       '9',
-       1,
-       'Draw: 1',
-       [False, False, False, False, False, True, False, False, True, False],
-       [0, 0, 2, 2, 3, 2, 4, 6, 3, 5],
-       123876478142928441769100783560984935273),
-      ('Sam Steep',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144351&profileid=25978#1',
-       True,
-       ['0', '0', '0', '0', '1', '0', '0', '3', '0', 'X'],
-       '4',
-       1,
-       'Draw: 1',
-       [True, True, True, True, True, False, True, True, False, True],
-       [0, 0, -2, -2, -3, -2, -4, -6, -3, -5],
-       123876478142928441769100783560984935273)],
-     [('Wayne Tuck Jr.',
-       'event.php?view=Team&eventid=6400&teamid=144353&profileid=12486#1',
-       True,
-       ['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'],
-       '5',
-       2,
-       'Draw: 2',
-       [True, True, False, True, True, True, True, False, False, False],
-       [0, 0, 2, -2, -2, -2, -3, -2, -1, 0],
-       309985127892547751219643103116568617832),
-      ('Matthew Hall',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
-       False,
-       ['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'],
-       '7',
-       2,
-       'Draw: 2',
-       [False, False, True, False, False, False, False, True, True, True],
-       [0, 0, -2, 2, 2, 2, 3, 2, 1, 0],
-       309985127892547751219643103116568617832),
-      ('Dayna Deruelle',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144346&profileid=26636#1',
-       False,
-       ['0', '0', '1', '0', '0', '0', '0', 'X'],
-       '1',
-       2,
-       'Draw: 2',
-       [False, False, True, False, True, True, True, True],
-       [0, 0, -2, -1, -3, -4, -5, -9],
-       258827556868852829922619663221573707805),
-      ('Tyler Stewart',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
-       True,
-       ['0', '2', '0', '2', '1', '1', '4', 'X'],
-       '10',
-       2,
-       'Draw: 2',
-       [True, True, False, True, False, False, False, False],
-       [0, 0, 2, 1, 3, 4, 5, 9],
-       258827556868852829922619663221573707805),
-      ('Mark Kean',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
-       True,
-       ['2', '0', '1', '0', '0', '0', '1', '3', 'X'],
-       '7',
-       2,
-       'Draw: 2',
-       [True, False, False, False, False, True, True, False, False],
-       [0, 2, 2, 3, 3, 1, 0, 1, 4],
-       196156262752898539339442275025527127066),
-      ('Jason March',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
-       False,
-       ['0', '0', '0', '0', '2', '1', '0', '0', 'X'],
-       '3',
-       2,
-       'Draw: 2',
-       [False, True, True, True, True, False, False, True, True],
-       [0, -2, -2, -3, -3, -1, 0, -1, -4],
-       196156262752898539339442275025527127066),
-      ('Richard Krell',
-       'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144349&profileid=25962#1',
-       True,
-       ['2', '0', '1', '0', '2', '1', '1', 'X'],
-       '7',
-       2,
-       'Draw: 2',
-       [True, False, False, False, True, False, False, False],
-       [0, 2, 2, 3, 2, 4, 5, 6],
-       121058110285022966689701916848012130324),
-      ('Rob Ainsley',
-       'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
-       False,
-       ['0', '0', '0', '1', '0', '0', '0', 'X'],
-       '1',
-       2,
-       'Draw: 2',
-       [False, True, True, True, False, True, True, True],
-       [0, -2, -2, -3, -2, -4, -5, -6],
-       121058110285022966689701916848012130324)],
-     [('Matthew Hall',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
-       True,
-       ['0', '0', '2', '1', '2', '1', '0', '2', 'X'],
-       '8',
-       3,
-       'Draw: 3',
-       [True, True, True, False, False, False, False, True, False],
-       [0, 0, -1, 1, 2, 4, 5, 3, 5],
-       167908611678356344738885531672086035216),
-      ('Tyler Stewart',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
-       False,
-       ['0', '1', '0', '0', '0', '0', '2', '0', 'X'],
-       '3',
-       3,
-       'Draw: 3',
-       [False, False, False, True, True, True, True, False, True],
-       [0, 0, 1, -1, -2, -4, -5, -3, -5],
-       167908611678356344738885531672086035216),
-      ('Mark Kean',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
-       True,
-       ['0', '5', '0', '1', '1', '1', 'X'],
-       '8',
-       3,
-       'Draw: 3',
-       [True, True, False, True, False, False, False],
-       [0, -1, 4, 3, 4, 5, 6],
-       157383102330203138325358878297425755857),
-      ('Richard Krell',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144349&profileid=25962#1',
-       False,
-       ['1', '0', '1', '0', '0', '0', 'X'],
-       '2',
-       3,
-       'Draw: 3',
-       [False, False, True, False, True, True, True],
-       [0, 1, -4, -3, -4, -5, -6],
-       157383102330203138325358878297425755857),
-      ('Damien Villard',
-       'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144354&profileid=27373#1',
-       True,
-       ['2', '1', '0', '1', '0', '0', '1', '0', '0', '0'],
-       '5',
-       3,
-       'Draw: 3',
-       [True, False, False, True, False, True, True, False, True, True],
-       [0, 2, 3, 2, 3, 1, 1, 2, 1, 0],
-       197764335276159882538274022024920645468),
-      ('Sam Steep',
-       'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144351&profileid=25978#1',
-       False,
-       ['0', '0', '1', '0', '2', '0', '0', '1', '1', '1'],
-       '6',
-       3,
-       'Draw: 3',
-       [False, True, True, False, True, False, False, True, False, False],
-       [0, -2, -3, -2, -3, -1, -1, -2, -1, 0],
-       197764335276159882538274022024920645468),
-      ('Jason March',
-       'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144350#1',
-       True,
-       ['1', '1', '0', '0', '0', '0', '2', '1', '2', 'X'],
-       '7',
-       3,
-       'Draw: 3',
-       [True, False, False, True, True, True, True, False, False, False],
-       [0, 1, 2, 1, 0, 0, 0, 2, 3, 5],
-       19248089004956668591585521441771100702),
-      ('Matthew Mepstead',
-       'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144356#1',
-       False,
-       ['0', '0', '1', '1', '0', '0', '0', '0', '0', 'X'],
-       '2',
-       3,
-       'Draw: 3',
-       [False, True, True, False, False, False, False, True, True, True],
-       [0, -1, -2, -1, 0, 0, 0, -2, -3, -5],
-       19248089004956668591585521441771100702),
-      ('Wayne Tuck Jr.',
-       'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144353&profileid=12486#1',
-       False,
-       ['0', '0', '0', '2', '0', '0', '0', '0', 'X'],
-       '2',
-       3,
-       'Draw: 3',
-       [False, True, True, True, False, True, True, True, True],
-       [0, -2, -3, -3, -1, -2, -4, -5, -6],
-       152642289275163622503053683522534226102),
-      ('Rob Ainsley',
-       'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
-       True,
-       ['2', '1', '0', '0', '1', '2', '1', '1', 'X'],
-       '8',
-       3,
-       'Draw: 3',
-       [True, False, False, False, True, False, False, False, False],
-       [0, 2, 3, 3, 1, 2, 4, 5, 6],
-       152642289275163622503053683522534226102)],
-     [('Matthew Hall',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
-       True,
-       ['1', '0', '1', '0', '1', '0', '2', '0', '1', '0'],
-       '6',
-       4,
-       'Draw: 4',
-       [True, False, True, False, True, False, True, False, True, False],
-       [0, 1, -1, 0, -2, -1, -2, 0, -1, 0],
-       128520251865367755000080630810739466709),
-      ('Mark Kean',
-       'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961#1',
-       False,
-       ['0', '2', '0', '2', '0', '1', '0', '1', '0', '1'],
-       '7',
-       4,
-       'Draw: 4',
-       [False, True, False, True, False, True, False, True, False, True],
-       [0, -1, 1, 0, 2, 1, 2, 0, 1, 0],
-       128520251865367755000080630810739466709),
-      ('Sam Steep',
-       'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144351&profileid=25978#1',
-       False,
-       ['1', '0', '0', '2', '0', '1', '1', '0', '1', '1'],
-       '7',
-       4,
-       'Draw: 4',
-       [False, False, True, True, False, True, False, False, True, False],
-       [0, 1, 0, -2, 0, -2, -1, 0, -1, 0],
-       164045326452654642850026023480637847801),
-      ('Jason March',
-       'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144350#1',
-       True,
-       ['0', '1', '2', '0', '2', '0', '0', '1', '0', '0'],
-       '6',
-       4,
-       'Draw: 4',
-       [True, True, False, False, True, False, True, True, False, True],
-       [0, -1, 0, 2, 0, 2, 1, 0, 1, 0],
-       164045326452654642850026023480637847801),
-      ('Dayna Deruelle',
-       'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144346&profileid=26636#1',
-       False,
-       ['0', '2', '1', '1', '1', '0', '3', 'X'],
-       '8',
-       4,
-       'Draw: 4',
-       [False, True, False, False, False, False, True, False],
-       [0, -1, 1, 2, 3, 4, 3, 6],
-       76792983814886196713410396043046633915),
-      ('Rob Ainsley',
-       'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
-       True,
-       ['1', '0', '0', '0', '0', '1', '0', 'X'],
-       '2',
-       4,
-       'Draw: 4',
-       [True, False, True, True, True, True, False, True],
-       [0, 1, -1, -2, -3, -4, -3, -6],
-       76792983814886196713410396043046633915)],
-     [('Sam Steep',
-       'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978#1',
-       False,
-       ['0', '1', '0', '0', '0', '2', '0', '2', '0', '0'],
-       '5',
-       5,
-       'Draw: 5',
-       [False, False, False, True, True, True, False, True, False, False],
-       [0, 0, 1, 0, -1, -3, -1, -3, -1, -1],
-       38480930669174444566426826324563146081),
-      ('Richard Krell',
-       'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1',
-       True,
-       ['0', '0', '1', '1', '2', '0', '2', '0', '0', '1'],
-       '7',
-       5,
-       'Draw: 5',
-       [True, True, True, False, False, False, True, False, True, True],
-       [0, 0, -1, 0, 1, 3, 1, 3, 1, 1],
-       38480930669174444566426826324563146081),
-      ('Dayna Deruelle',
-       'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144346&profileid=26636#1',
-       False,
-       ['0', '0', '1', '0', '0', '0', '1', '0', '3', '1', '0'],
-       '6',
-       5,
-       'Draw: 5',
-       [False, True, True, False, True, True, True, False, True, False, False],
-       [0, -1, -1, 0, -1, -1, -3, -2, -4, -1, 0],
-       153896726080791122415283970396986089830),
-      ('Tyler Stewart',
-       'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144352&profileid=12477#1',
-       True,
-       ['1', '0', '0', '1', '0', '2', '0', '2', '0', '0', '1'],
-       '7',
-       5,
-       'Draw: 5',
-       [True, False, False, True, False, False, False, True, False, True, True],
-       [0, 1, 1, 0, 1, 1, 3, 2, 4, 1, 0],
-       153896726080791122415283970396986089830)],
-     [('Richard Krell',
-       'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1',
-       False,
-       ['0', '0', '1', '1', '0', '0', '1', '0', 'X'],
-       '3',
-       6,
-       'Draw: 6',
-       [False, False, True, False, False, True, True, False, True],
-       [0, 0, -2, -1, 0, -2, -5, -4, -5],
-       209637313717849892067917714730669554285),
-      ('Tyler Stewart',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
-       True,
-       ['0', '2', '0', '0', '2', '3', '0', '1', 'X'],
-       '8',
-       6,
-       'Draw: 6',
-       [True, True, False, True, True, False, False, True, False],
-       [0, 0, 2, 1, 0, 2, 5, 4, 5],
-       209637313717849892067917714730669554285)],
-     [('Tyler Stewart',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
-       False,
-       ['0', '0', '1', '1', '0', '3', '0', '0', '1', '0'],
-       '6',
-       7,
-       'Draw: 7',
-       [False, False, True, False, False, True, False, False, True, False],
-       [0, 0, -1, 0, 1, -2, 1, 1, 0, 1],
-       274892128276167031788079435153352244862),
-      ('Matthew Hall',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
-       True,
-       ['0', '1', '0', '0', '3', '0', '0', '1', '0', '2'],
-       '7',
-       7,
-       'Draw: 7',
-       [True, True, False, True, True, False, True, True, False, True],
-       [0, 0, 1, 0, -1, 2, -1, -1, 0, -1],
-       274892128276167031788079435153352244862)]]
-
-
+The `get_flat_boxscores` method can be used to return a list of tuples of all the boxscore information on all the linescore pages.
 
 ```python
-event.get_flat_boxscores()[0]
+event.get_flat_boxscores(flat=True)
 ```
 
 
 
 
     [('Damien Villard',
       'event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1',
       True,
       ['0', '0', '0', '0', 'X'],
       '0',
       1,
       'Draw: 1',
       [True, True, True, True, True],
       [0, -1, -4, -6, -8],
-      227597408989477916004520082463493572762),
+      209707243860236114112314247393927711356),
      ('Matthew Hall',
       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
       False,
       ['1', '3', '2', '2', 'X'],
       '8',
       1,
       'Draw: 1',
       [False, False, False, False, False],
       [0, 1, 4, 6, 8],
-      227597408989477916004520082463493572762),
+      209707243860236114112314247393927711356),
      ('Matthew Mepstead',
       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144356#1',
       False,
       ['0', '0', '1', '1', '0', '1', '0', '0', '0', '1', '0'],
       '4',
       1,
       'Draw: 1',
       [False, False, True, False, False, True, False, False, False, True, False],
       [0, 0, -2, -1, 0, -1, 0, 0, 0, -1, 0],
-      230481195381514558834165699232540581342),
+      38537103347544582345141893615297919005),
      ('Tyler Stewart',
       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
       True,
       ['0', '2', '0', '0', '1', '0', '0', '0', '1', '0', '1'],
       '5',
       1,
       'Draw: 1',
       [True, True, False, True, True, False, True, True, True, False, True],
       [0, 0, 2, 1, 0, 1, 0, 0, 0, 1, 0],
-      230481195381514558834165699232540581342),
+      38537103347544582345141893615297919005),
      ('Jason March',
       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
       False,
       ['0', '2', '0', '1', '0', '2', '2', '0', '2', 'X'],
       '9',
       1,
       'Draw: 1',
       [False, False, False, False, False, True, False, False, True, False],
       [0, 0, 2, 2, 3, 2, 4, 6, 3, 5],
-      123876478142928441769100783560984935273),
+      272348649831484335603593027216985821953),
      ('Sam Steep',
       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144351&profileid=25978#1',
       True,
       ['0', '0', '0', '0', '1', '0', '0', '3', '0', 'X'],
       '4',
       1,
       'Draw: 1',
       [True, True, True, True, True, False, True, True, False, True],
       [0, 0, -2, -2, -3, -2, -4, -6, -3, -5],
-      123876478142928441769100783560984935273)]
-
-
-
-```python
-event.get_flat_boxscores()[-1]
-```
-
-
-
-
-    [('Tyler Stewart',
+      272348649831484335603593027216985821953),
+     ('Wayne Tuck Jr.',
+      'event.php?view=Team&eventid=6400&teamid=144353&profileid=12486#1',
+      True,
+      ['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'],
+      '5',
+      2,
+      'Draw: 2',
+      [True, True, False, True, True, True, True, False, False, False],
+      [0, 0, 2, -2, -2, -2, -3, -2, -1, 0],
+      95112284881200216258215191883153462659),
+     ('Matthew Hall',
+      'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+      False,
+      ['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'],
+      '7',
+      2,
+      'Draw: 2',
+      [False, False, True, False, False, False, False, True, True, True],
+      [0, 0, -2, 2, 2, 2, 3, 2, 1, 0],
+      95112284881200216258215191883153462659),
+     ('Dayna Deruelle',
+      'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144346&profileid=26636#1',
+      False,
+      ['0', '0', '1', '0', '0', '0', '0', 'X'],
+      '1',
+      2,
+      'Draw: 2',
+      [False, False, True, False, True, True, True, True],
+      [0, 0, -2, -1, -3, -4, -5, -9],
+      59643628877953807377369574857821892232),
+     ('Tyler Stewart',
+      'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
+      True,
+      ['0', '2', '0', '2', '1', '1', '4', 'X'],
+      '10',
+      2,
+      'Draw: 2',
+      [True, True, False, True, False, False, False, False],
+      [0, 0, 2, 1, 3, 4, 5, 9],
+      59643628877953807377369574857821892232),
+     ('Mark Kean',
+      'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
+      True,
+      ['2', '0', '1', '0', '0', '0', '1', '3', 'X'],
+      '7',
+      2,
+      'Draw: 2',
+      [True, False, False, False, False, True, True, False, False],
+      [0, 2, 2, 3, 3, 1, 0, 1, 4],
+      122217858840490332010920244446431255640),
+     ('Jason March',
+      'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
+      False,
+      ['0', '0', '0', '0', '2', '1', '0', '0', 'X'],
+      '3',
+      2,
+      'Draw: 2',
+      [False, True, True, True, True, False, False, True, True],
+      [0, -2, -2, -3, -3, -1, 0, -1, -4],
+      122217858840490332010920244446431255640),
+     ('Richard Krell',
+      'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144349&profileid=25962#1',
+      True,
+      ['2', '0', '1', '0', '2', '1', '1', 'X'],
+      '7',
+      2,
+      'Draw: 2',
+      [True, False, False, False, True, False, False, False],
+      [0, 2, 2, 3, 2, 4, 5, 6],
+      335702133606077232579627915311442373664),
+     ('Rob Ainsley',
+      'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
+      False,
+      ['0', '0', '0', '1', '0', '0', '0', 'X'],
+      '1',
+      2,
+      'Draw: 2',
+      [False, True, True, True, False, True, True, True],
+      [0, -2, -2, -3, -2, -4, -5, -6],
+      335702133606077232579627915311442373664),
+     ('Matthew Hall',
+      'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+      True,
+      ['0', '0', '2', '1', '2', '1', '0', '2', 'X'],
+      '8',
+      3,
+      'Draw: 3',
+      [True, True, True, False, False, False, False, True, False],
+      [0, 0, -1, 1, 2, 4, 5, 3, 5],
+      53772503334370441085334378293107653659),
+     ('Tyler Stewart',
+      'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
+      False,
+      ['0', '1', '0', '0', '0', '0', '2', '0', 'X'],
+      '3',
+      3,
+      'Draw: 3',
+      [False, False, False, True, True, True, True, False, True],
+      [0, 0, 1, -1, -2, -4, -5, -3, -5],
+      53772503334370441085334378293107653659),
+     ('Mark Kean',
+      'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
+      True,
+      ['0', '5', '0', '1', '1', '1', 'X'],
+      '8',
+      3,
+      'Draw: 3',
+      [True, True, False, True, False, False, False],
+      [0, -1, 4, 3, 4, 5, 6],
+      310456475955908017873561887016699672637),
+     ('Richard Krell',
+      'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144349&profileid=25962#1',
+      False,
+      ['1', '0', '1', '0', '0', '0', 'X'],
+      '2',
+      3,
+      'Draw: 3',
+      [False, False, True, False, True, True, True],
+      [0, 1, -4, -3, -4, -5, -6],
+      310456475955908017873561887016699672637),
+     ('Damien Villard',
+      'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144354&profileid=27373#1',
+      True,
+      ['2', '1', '0', '1', '0', '0', '1', '0', '0', '0'],
+      '5',
+      3,
+      'Draw: 3',
+      [True, False, False, True, False, True, True, False, True, True],
+      [0, 2, 3, 2, 3, 1, 1, 2, 1, 0],
+      303047434632680540438656592556261333287),
+     ('Sam Steep',
+      'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144351&profileid=25978#1',
+      False,
+      ['0', '0', '1', '0', '2', '0', '0', '1', '1', '1'],
+      '6',
+      3,
+      'Draw: 3',
+      [False, True, True, False, True, False, False, True, False, False],
+      [0, -2, -3, -2, -3, -1, -1, -2, -1, 0],
+      303047434632680540438656592556261333287),
+     ('Jason March',
+      'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144350#1',
+      True,
+      ['1', '1', '0', '0', '0', '0', '2', '1', '2', 'X'],
+      '7',
+      3,
+      'Draw: 3',
+      [True, False, False, True, True, True, True, False, False, False],
+      [0, 1, 2, 1, 0, 0, 0, 2, 3, 5],
+      229699058183107339172217417532449914369),
+     ('Matthew Mepstead',
+      'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144356#1',
+      False,
+      ['0', '0', '1', '1', '0', '0', '0', '0', '0', 'X'],
+      '2',
+      3,
+      'Draw: 3',
+      [False, True, True, False, False, False, False, True, True, True],
+      [0, -1, -2, -1, 0, 0, 0, -2, -3, -5],
+      229699058183107339172217417532449914369),
+     ('Wayne Tuck Jr.',
+      'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144353&profileid=12486#1',
+      False,
+      ['0', '0', '0', '2', '0', '0', '0', '0', 'X'],
+      '2',
+      3,
+      'Draw: 3',
+      [False, True, True, True, False, True, True, True, True],
+      [0, -2, -3, -3, -1, -2, -4, -5, -6],
+      195399470224611539512163135746754073908),
+     ('Rob Ainsley',
+      'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
+      True,
+      ['2', '1', '0', '0', '1', '2', '1', '1', 'X'],
+      '8',
+      3,
+      'Draw: 3',
+      [True, False, False, False, True, False, False, False, False],
+      [0, 2, 3, 3, 1, 2, 4, 5, 6],
+      195399470224611539512163135746754073908),
+     ('Matthew Hall',
+      'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+      True,
+      ['1', '0', '1', '0', '1', '0', '2', '0', '1', '0'],
+      '6',
+      4,
+      'Draw: 4',
+      [True, False, True, False, True, False, True, False, True, False],
+      [0, 1, -1, 0, -2, -1, -2, 0, -1, 0],
+      63653233024470732271264476184228625543),
+     ('Mark Kean',
+      'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961#1',
+      False,
+      ['0', '2', '0', '2', '0', '1', '0', '1', '0', '1'],
+      '7',
+      4,
+      'Draw: 4',
+      [False, True, False, True, False, True, False, True, False, True],
+      [0, -1, 1, 0, 2, 1, 2, 0, 1, 0],
+      63653233024470732271264476184228625543),
+     ('Sam Steep',
+      'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144351&profileid=25978#1',
+      False,
+      ['1', '0', '0', '2', '0', '1', '1', '0', '1', '1'],
+      '7',
+      4,
+      'Draw: 4',
+      [False, False, True, True, False, True, False, False, True, False],
+      [0, 1, 0, -2, 0, -2, -1, 0, -1, 0],
+      279469483516704960424550934244064693031),
+     ('Jason March',
+      'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144350#1',
+      True,
+      ['0', '1', '2', '0', '2', '0', '0', '1', '0', '0'],
+      '6',
+      4,
+      'Draw: 4',
+      [True, True, False, False, True, False, True, True, False, True],
+      [0, -1, 0, 2, 0, 2, 1, 0, 1, 0],
+      279469483516704960424550934244064693031),
+     ('Dayna Deruelle',
+      'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144346&profileid=26636#1',
+      False,
+      ['0', '2', '1', '1', '1', '0', '3', 'X'],
+      '8',
+      4,
+      'Draw: 4',
+      [False, True, False, False, False, False, True, False],
+      [0, -1, 1, 2, 3, 4, 3, 6],
+      291113397726148010907174443006816563924),
+     ('Rob Ainsley',
+      'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
+      True,
+      ['1', '0', '0', '0', '0', '1', '0', 'X'],
+      '2',
+      4,
+      'Draw: 4',
+      [True, False, True, True, True, True, False, True],
+      [0, 1, -1, -2, -3, -4, -3, -6],
+      291113397726148010907174443006816563924),
+     ('Sam Steep',
+      'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978#1',
+      False,
+      ['0', '1', '0', '0', '0', '2', '0', '2', '0', '0'],
+      '5',
+      5,
+      'Draw: 5',
+      [False, False, False, True, True, True, False, True, False, False],
+      [0, 0, 1, 0, -1, -3, -1, -3, -1, -1],
+      95866945533461342246819997703085723055),
+     ('Richard Krell',
+      'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1',
+      True,
+      ['0', '0', '1', '1', '2', '0', '2', '0', '0', '1'],
+      '7',
+      5,
+      'Draw: 5',
+      [True, True, True, False, False, False, True, False, True, True],
+      [0, 0, -1, 0, 1, 3, 1, 3, 1, 1],
+      95866945533461342246819997703085723055),
+     ('Dayna Deruelle',
+      'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144346&profileid=26636#1',
+      False,
+      ['0', '0', '1', '0', '0', '0', '1', '0', '3', '1', '0'],
+      '6',
+      5,
+      'Draw: 5',
+      [False, True, True, False, True, True, True, False, True, False, False],
+      [0, -1, -1, 0, -1, -1, -3, -2, -4, -1, 0],
+      233581897033627594667237538445333000951),
+     ('Tyler Stewart',
+      'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144352&profileid=12477#1',
+      True,
+      ['1', '0', '0', '1', '0', '2', '0', '2', '0', '0', '1'],
+      '7',
+      5,
+      'Draw: 5',
+      [True, False, False, True, False, False, False, True, False, True, True],
+      [0, 1, 1, 0, 1, 1, 3, 2, 4, 1, 0],
+      233581897033627594667237538445333000951),
+     ('Richard Krell',
+      'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1',
+      False,
+      ['0', '0', '1', '1', '0', '0', '1', '0', 'X'],
+      '3',
+      6,
+      'Draw: 6',
+      [False, False, True, False, False, True, True, False, True],
+      [0, 0, -2, -1, 0, -2, -5, -4, -5],
+      61203104491141348409761697458039616615),
+     ('Tyler Stewart',
+      'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
+      True,
+      ['0', '2', '0', '0', '2', '3', '0', '1', 'X'],
+      '8',
+      6,
+      'Draw: 6',
+      [True, True, False, True, True, False, False, True, False],
+      [0, 0, 2, 1, 0, 2, 5, 4, 5],
+      61203104491141348409761697458039616615),
+     ('Tyler Stewart',
       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
       False,
       ['0', '0', '1', '1', '0', '3', '0', '0', '1', '0'],
       '6',
       7,
       'Draw: 7',
       [False, False, True, False, False, True, False, False, True, False],
       [0, 0, -1, 0, 1, -2, 1, 1, 0, 1],
-      274892128276167031788079435153352244862),
+      4915701019265174384644466584441738333),
      ('Matthew Hall',
       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
       True,
       ['0', '1', '0', '0', '3', '0', '0', '1', '0', '2'],
       '7',
       7,
       'Draw: 7',
       [True, True, False, True, True, False, True, True, False, True],
       [0, 0, 1, 0, -1, 2, -1, -1, 0, -1],
-      274892128276167031788079435153352244862)]
+      4915701019265174384644466584441738333)]
 
 
 
-## About czapi
-czapi is a Python library for scraping curling linescores.
+The `get_flat_boxscores` method can also be used to return a list of `Boxscore` objects for convenience. 
+
+```python
+event.get_flat_boxscores(flat=False)
+```
+
+
+
+
+    [Boxscore(team_name='Damien Villard', href='event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1', hammer_start=True, score=['0', '0', '0', '0', 'X'], final_score='0', draw_num=1, draw='Draw: 1', hammer_progression=[True, True, True, True, True], relative_score=[0, -1, -4, -6, -8], guid=209707243860236114112314247393927711356),
+     Boxscore(team_name='Matthew Hall', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', hammer_start=False, score=['1', '3', '2', '2', 'X'], final_score='8', draw_num=1, draw='Draw: 1', hammer_progression=[False, False, False, False, False], relative_score=[0, 1, 4, 6, 8], guid=209707243860236114112314247393927711356),
+     Boxscore(team_name='Matthew Mepstead', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144356#1', hammer_start=False, score=['0', '0', '1', '1', '0', '1', '0', '0', '0', '1', '0'], final_score='4', draw_num=1, draw='Draw: 1', hammer_progression=[False, False, True, False, False, True, False, False, False, True, False], relative_score=[0, 0, -2, -1, 0, -1, 0, 0, 0, -1, 0], guid=38537103347544582345141893615297919005),
+     Boxscore(team_name='Tyler Stewart', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1', hammer_start=True, score=['0', '2', '0', '0', '1', '0', '0', '0', '1', '0', '1'], final_score='5', draw_num=1, draw='Draw: 1', hammer_progression=[True, True, False, True, True, False, True, True, True, False, True], relative_score=[0, 0, 2, 1, 0, 1, 0, 0, 0, 1, 0], guid=38537103347544582345141893615297919005),
+     Boxscore(team_name='Jason March', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1', hammer_start=False, score=['0', '2', '0', '1', '0', '2', '2', '0', '2', 'X'], final_score='9', draw_num=1, draw='Draw: 1', hammer_progression=[False, False, False, False, False, True, False, False, True, False], relative_score=[0, 0, 2, 2, 3, 2, 4, 6, 3, 5], guid=272348649831484335603593027216985821953),
+     Boxscore(team_name='Sam Steep', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144351&profileid=25978#1', hammer_start=True, score=['0', '0', '0', '0', '1', '0', '0', '3', '0', 'X'], final_score='4', draw_num=1, draw='Draw: 1', hammer_progression=[True, True, True, True, True, False, True, True, False, True], relative_score=[0, 0, -2, -2, -3, -2, -4, -6, -3, -5], guid=272348649831484335603593027216985821953),
+     Boxscore(team_name='Wayne Tuck Jr.', href='event.php?view=Team&eventid=6400&teamid=144353&profileid=12486#1', hammer_start=True, score=['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'], final_score='5', draw_num=2, draw='Draw: 2', hammer_progression=[True, True, False, True, True, True, True, False, False, False], relative_score=[0, 0, 2, -2, -2, -2, -3, -2, -1, 0], guid=95112284881200216258215191883153462659),
+     Boxscore(team_name='Matthew Hall', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', hammer_start=False, score=['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'], final_score='7', draw_num=2, draw='Draw: 2', hammer_progression=[False, False, True, False, False, False, False, True, True, True], relative_score=[0, 0, -2, 2, 2, 2, 3, 2, 1, 0], guid=95112284881200216258215191883153462659),
+     Boxscore(team_name='Dayna Deruelle', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144346&profileid=26636#1', hammer_start=False, score=['0', '0', '1', '0', '0', '0', '0', 'X'], final_score='1', draw_num=2, draw='Draw: 2', hammer_progression=[False, False, True, False, True, True, True, True], relative_score=[0, 0, -2, -1, -3, -4, -5, -9], guid=59643628877953807377369574857821892232),
+     Boxscore(team_name='Tyler Stewart', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1', hammer_start=True, score=['0', '2', '0', '2', '1', '1', '4', 'X'], final_score='10', draw_num=2, draw='Draw: 2', hammer_progression=[True, True, False, True, False, False, False, False], relative_score=[0, 0, 2, 1, 3, 4, 5, 9], guid=59643628877953807377369574857821892232),
+     Boxscore(team_name='Mark Kean', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1', hammer_start=True, score=['2', '0', '1', '0', '0', '0', '1', '3', 'X'], final_score='7', draw_num=2, draw='Draw: 2', hammer_progression=[True, False, False, False, False, True, True, False, False], relative_score=[0, 2, 2, 3, 3, 1, 0, 1, 4], guid=122217858840490332010920244446431255640),
+     Boxscore(team_name='Jason March', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1', hammer_start=False, score=['0', '0', '0', '0', '2', '1', '0', '0', 'X'], final_score='3', draw_num=2, draw='Draw: 2', hammer_progression=[False, True, True, True, True, False, False, True, True], relative_score=[0, -2, -2, -3, -3, -1, 0, -1, -4], guid=122217858840490332010920244446431255640),
+     Boxscore(team_name='Richard Krell', href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144349&profileid=25962#1', hammer_start=True, score=['2', '0', '1', '0', '2', '1', '1', 'X'], final_score='7', draw_num=2, draw='Draw: 2', hammer_progression=[True, False, False, False, True, False, False, False], relative_score=[0, 2, 2, 3, 2, 4, 5, 6], guid=335702133606077232579627915311442373664),
+     Boxscore(team_name='Rob Ainsley', href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1', hammer_start=False, score=['0', '0', '0', '1', '0', '0', '0', 'X'], final_score='1', draw_num=2, draw='Draw: 2', hammer_progression=[False, True, True, True, False, True, True, True], relative_score=[0, -2, -2, -3, -2, -4, -5, -6], guid=335702133606077232579627915311442373664),
+     Boxscore(team_name='Matthew Hall', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', hammer_start=True, score=['0', '0', '2', '1', '2', '1', '0', '2', 'X'], final_score='8', draw_num=3, draw='Draw: 3', hammer_progression=[True, True, True, False, False, False, False, True, False], relative_score=[0, 0, -1, 1, 2, 4, 5, 3, 5], guid=53772503334370441085334378293107653659),
+     Boxscore(team_name='Tyler Stewart', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1', hammer_start=False, score=['0', '1', '0', '0', '0', '0', '2', '0', 'X'], final_score='3', draw_num=3, draw='Draw: 3', hammer_progression=[False, False, False, True, True, True, True, False, True], relative_score=[0, 0, 1, -1, -2, -4, -5, -3, -5], guid=53772503334370441085334378293107653659),
+     Boxscore(team_name='Mark Kean', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1', hammer_start=True, score=['0', '5', '0', '1', '1', '1', 'X'], final_score='8', draw_num=3, draw='Draw: 3', hammer_progression=[True, True, False, True, False, False, False], relative_score=[0, -1, 4, 3, 4, 5, 6], guid=310456475955908017873561887016699672637),
+     Boxscore(team_name='Richard Krell', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144349&profileid=25962#1', hammer_start=False, score=['1', '0', '1', '0', '0', '0', 'X'], final_score='2', draw_num=3, draw='Draw: 3', hammer_progression=[False, False, True, False, True, True, True], relative_score=[0, 1, -4, -3, -4, -5, -6], guid=310456475955908017873561887016699672637),
+     Boxscore(team_name='Damien Villard', href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144354&profileid=27373#1', hammer_start=True, score=['2', '1', '0', '1', '0', '0', '1', '0', '0', '0'], final_score='5', draw_num=3, draw='Draw: 3', hammer_progression=[True, False, False, True, False, True, True, False, True, True], relative_score=[0, 2, 3, 2, 3, 1, 1, 2, 1, 0], guid=303047434632680540438656592556261333287),
+     Boxscore(team_name='Sam Steep', href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144351&profileid=25978#1', hammer_start=False, score=['0', '0', '1', '0', '2', '0', '0', '1', '1', '1'], final_score='6', draw_num=3, draw='Draw: 3', hammer_progression=[False, True, True, False, True, False, False, True, False, False], relative_score=[0, -2, -3, -2, -3, -1, -1, -2, -1, 0], guid=303047434632680540438656592556261333287),
+     Boxscore(team_name='Jason March', href='event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144350#1', hammer_start=True, score=['1', '1', '0', '0', '0', '0', '2', '1', '2', 'X'], final_score='7', draw_num=3, draw='Draw: 3', hammer_progression=[True, False, False, True, True, True, True, False, False, False], relative_score=[0, 1, 2, 1, 0, 0, 0, 2, 3, 5], guid=229699058183107339172217417532449914369),
+     Boxscore(team_name='Matthew Mepstead', href='event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144356#1', hammer_start=False, score=['0', '0', '1', '1', '0', '0', '0', '0', '0', 'X'], final_score='2', draw_num=3, draw='Draw: 3', hammer_progression=[False, True, True, False, False, False, False, True, True, True], relative_score=[0, -1, -2, -1, 0, 0, 0, -2, -3, -5], guid=229699058183107339172217417532449914369),
+     Boxscore(team_name='Wayne Tuck Jr.', href='event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144353&profileid=12486#1', hammer_start=False, score=['0', '0', '0', '2', '0', '0', '0', '0', 'X'], final_score='2', draw_num=3, draw='Draw: 3', hammer_progression=[False, True, True, True, False, True, True, True, True], relative_score=[0, -2, -3, -3, -1, -2, -4, -5, -6], guid=195399470224611539512163135746754073908),
+     Boxscore(team_name='Rob Ainsley', href='event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144345&profileid=15779#1', hammer_start=True, score=['2', '1', '0', '0', '1', '2', '1', '1', 'X'], final_score='8', draw_num=3, draw='Draw: 3', hammer_progression=[True, False, False, False, True, False, False, False, False], relative_score=[0, 2, 3, 3, 1, 2, 4, 5, 6], guid=195399470224611539512163135746754073908),
+     Boxscore(team_name='Matthew Hall', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', hammer_start=True, score=['1', '0', '1', '0', '1', '0', '2', '0', '1', '0'], final_score='6', draw_num=4, draw='Draw: 4', hammer_progression=[True, False, True, False, True, False, True, False, True, False], relative_score=[0, 1, -1, 0, -2, -1, -2, 0, -1, 0], guid=63653233024470732271264476184228625543),
+     Boxscore(team_name='Mark Kean', href='event.php?view=Team&eventid=6400&teamid=144348&profileid=25961#1', hammer_start=False, score=['0', '2', '0', '2', '0', '1', '0', '1', '0', '1'], final_score='7', draw_num=4, draw='Draw: 4', hammer_progression=[False, True, False, True, False, True, False, True, False, True], relative_score=[0, -1, 1, 0, 2, 1, 2, 0, 1, 0], guid=63653233024470732271264476184228625543),
+     Boxscore(team_name='Sam Steep', href='event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144351&profileid=25978#1', hammer_start=False, score=['1', '0', '0', '2', '0', '1', '1', '0', '1', '1'], final_score='7', draw_num=4, draw='Draw: 4', hammer_progression=[False, False, True, True, False, True, False, False, True, False], relative_score=[0, 1, 0, -2, 0, -2, -1, 0, -1, 0], guid=279469483516704960424550934244064693031),
+     Boxscore(team_name='Jason March', href='event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144350#1', hammer_start=True, score=['0', '1', '2', '0', '2', '0', '0', '1', '0', '0'], final_score='6', draw_num=4, draw='Draw: 4', hammer_progression=[True, True, False, False, True, False, True, True, False, True], relative_score=[0, -1, 0, 2, 0, 2, 1, 0, 1, 0], guid=279469483516704960424550934244064693031),
+     Boxscore(team_name='Dayna Deruelle', href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144346&profileid=26636#1', hammer_start=False, score=['0', '2', '1', '1', '1', '0', '3', 'X'], final_score='8', draw_num=4, draw='Draw: 4', hammer_progression=[False, True, False, False, False, False, True, False], relative_score=[0, -1, 1, 2, 3, 4, 3, 6], guid=291113397726148010907174443006816563924),
+     Boxscore(team_name='Rob Ainsley', href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1', hammer_start=True, score=['1', '0', '0', '0', '0', '1', '0', 'X'], final_score='2', draw_num=4, draw='Draw: 4', hammer_progression=[True, False, True, True, True, True, False, True], relative_score=[0, 1, -1, -2, -3, -4, -3, -6], guid=291113397726148010907174443006816563924),
+     Boxscore(team_name='Sam Steep', href='event.php?view=Team&eventid=6400&teamid=144351&profileid=25978#1', hammer_start=False, score=['0', '1', '0', '0', '0', '2', '0', '2', '0', '0'], final_score='5', draw_num=5, draw='Draw: 5', hammer_progression=[False, False, False, True, True, True, False, True, False, False], relative_score=[0, 0, 1, 0, -1, -3, -1, -3, -1, -1], guid=95866945533461342246819997703085723055),
+     Boxscore(team_name='Richard Krell', href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1', hammer_start=True, score=['0', '0', '1', '1', '2', '0', '2', '0', '0', '1'], final_score='7', draw_num=5, draw='Draw: 5', hammer_progression=[True, True, True, False, False, False, True, False, True, True], relative_score=[0, 0, -1, 0, 1, 3, 1, 3, 1, 1], guid=95866945533461342246819997703085723055),
+     Boxscore(team_name='Dayna Deruelle', href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144346&profileid=26636#1', hammer_start=False, score=['0', '0', '1', '0', '0', '0', '1', '0', '3', '1', '0'], final_score='6', draw_num=5, draw='Draw: 5', hammer_progression=[False, True, True, False, True, True, True, False, True, False, False], relative_score=[0, -1, -1, 0, -1, -1, -3, -2, -4, -1, 0], guid=233581897033627594667237538445333000951),
+     Boxscore(team_name='Tyler Stewart', href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144352&profileid=12477#1', hammer_start=True, score=['1', '0', '0', '1', '0', '2', '0', '2', '0', '0', '1'], final_score='7', draw_num=5, draw='Draw: 5', hammer_progression=[True, False, False, True, False, False, False, True, False, True, True], relative_score=[0, 1, 1, 0, 1, 1, 3, 2, 4, 1, 0], guid=233581897033627594667237538445333000951),
+     Boxscore(team_name='Richard Krell', href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1', hammer_start=False, score=['0', '0', '1', '1', '0', '0', '1', '0', 'X'], final_score='3', draw_num=6, draw='Draw: 6', hammer_progression=[False, False, True, False, False, True, True, False, True], relative_score=[0, 0, -2, -1, 0, -2, -5, -4, -5], guid=61203104491141348409761697458039616615),
+     Boxscore(team_name='Tyler Stewart', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1', hammer_start=True, score=['0', '2', '0', '0', '2', '3', '0', '1', 'X'], final_score='8', draw_num=6, draw='Draw: 6', hammer_progression=[True, True, False, True, True, False, False, True, False], relative_score=[0, 0, 2, 1, 0, 2, 5, 4, 5], guid=61203104491141348409761697458039616615),
+     Boxscore(team_name='Tyler Stewart', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1', hammer_start=False, score=['0', '0', '1', '1', '0', '3', '0', '0', '1', '0'], final_score='6', draw_num=7, draw='Draw: 7', hammer_progression=[False, False, True, False, False, True, False, False, True, False], relative_score=[0, 0, -1, 0, 1, -2, 1, 1, 0, 1], guid=4915701019265174384644466584441738333),
+     Boxscore(team_name='Matthew Hall', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', hammer_start=True, score=['0', '1', '0', '0', '3', '0', '0', '1', '0', '2'], final_score='7', draw_num=7, draw='Draw: 7', hammer_progression=[True, True, False, True, True, False, True, True, False, True], relative_score=[0, 0, 1, 0, -1, 2, -1, -1, 0, -1], guid=4915701019265174384644466584441738333)]
 
 
+
+```python
+event.get_flat_boxscores()[0]
+```
+
+
+
+
+    Boxscore(team_name='Damien Villard', href='event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1', hammer_start=True, score=['0', '0', '0', '0', 'X'], final_score='0', draw_num=1, draw='Draw: 1', hammer_progression=[True, True, True, True, True], relative_score=[0, -1, -4, -6, -8], guid=209707243860236114112314247393927711356)
+
+
+
+```python
+event.get_flat_boxscores()[-1]
+```
+
+
+
+
+    Boxscore(team_name='Matthew Hall', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', hammer_start=True, score=['0', '1', '0', '0', '3', '0', '0', '1', '0', '2'], final_score='7', draw_num=7, draw='Draw: 7', hammer_progression=[True, True, False, True, True, False, True, True, False, True], relative_score=[0, 0, 1, 0, -1, 2, -1, -1, 0, -1], guid=4915701019265174384644466584441738333)
+
+
+
+## About czapi
+czapi is a Python library for scraping curling linescores.
```

#### html2text {}

```diff
@@ -1,31 +1,21 @@
-Metadata-Version: 2.1 Name: czapi Version: 0.1.9 Summary: CurlingZone scraper
-API. Home-page: https://github.com/calicorob/czapi/tree/master/ Author: Robert
-Currie Author-email: robert.art.currie@gmail.com License: Apache Software
-License 2.0 Keywords: curling,stats Platform: UNKNOWN Classifier: Development
-Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
-Natural Language :: English Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: License :: OSI Approved :: Apache
-Software License Requires-Python: >=3.6 Description-Content-Type: text/markdown
-Provides-Extra: dev License-File: LICENSE # Welcome to czapi > A basic API for
-scraping curling boxscores off of the popular CurlingZone website. ## Install
-``` pip install czapi ``` ## How to use ```python import czapi.api as api ```
-## LinescorePage czapi is based around the `LinescorePage` object which
-represents a linescore page on the CurlingZone website. Click [here](https://
-curlingzone.com/event.php?view=Scores&eventid=7795#1) to see an example
-linescore page. Creating an instance of the `LinescorePage` class gives access
-to every boxscore on that linescore page. ```python linescore_page =
-api.LinescorePage(cz_event_id = 6400, cz_draw_id = 2) ``` The `cz_event_id` and
-`cz_draw_id` arguments are found in the CurlingZone URL. Here's an example: >
-https://curlingzone.com/
-event.php?**eventid=7795**&view=Scores&show**drawid=21**#1 The boxscores on the
-linescore page can be accessed through the `boxscores` property which returns a
-list of boxscores. ```python linescore_page.boxscores ``` [{'Wayne Tuck Jr.':
-{'draw': 'Draw: 2', 'draw_num': 2, 'href':
+# Welcome to czapi > A basic API for scraping curling boxscores off of the
+popular CurlingZone website. ## Install ``` pip install czapi ``` ## How to use
+```python import czapi.api as api ``` ## LinescorePage czapi is based around
+the `LinescorePage` object which represents a linescore page on the CurlingZone
+website. Click [here](https://curlingzone.com/
+event.php?view=Scores&eventid=7795#1) to see an example linescore page.
+Creating an instance of the `LinescorePage` class gives access to every
+boxscore on that linescore page. ```python linescore_page = api.LinescorePage
+(cz_event_id = 6400, cz_draw_id = 2) ``` The `cz_event_id` and `cz_draw_id`
+arguments are found in the CurlingZone URL. Here's an example: > https://
+curlingzone.com/event.php?**eventid=7795**&view=Scores&show**drawid=21**#1 The
+boxscores on the linescore page can be accessed through the `boxscores`
+property which returns a list of boxscores. ```python linescore_page.boxscores
+``` [{'Wayne Tuck Jr.': {'draw': 'Draw: 2', 'draw_num': 2, 'href':
 'event.php?view=Team&eventid=6400&teamid=144353&profileid=12486#1', 'score':
 ['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'], 'hammer': True,
 'finalscore': '5'}, 'Matthew Hall': {'draw': 'Draw: 2', 'draw_num': 2, 'href':
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', 'score':
 ['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'], 'hammer': False,
 'finalscore': '7'}}, {'Dayna Deruelle': {'draw': 'Draw: 2', 'draw_num': 2,
 'href':
@@ -101,53 +91,53 @@
 True, False, False, False, False, True, True, True], normalized_score=[0, 0, -
 2, 2, 2, 2, 3, 2, 1, 0]) For Matthew Hall, the `normalized_score` attribute can
 be interpreted as follows: * The score was tied in the first end (obviously). *
 The score was tied in the second end. * In the 3rd end, Matthew was down 2. *
 In the 4th end, Matthew was up 2 after taking 4. * And so on and so forth..
 You'll also notice the `NormalizedBoxscore` object has a guid property which
 identifies that two `NormalizedHalfBoxscore` belong to the same game. ```python
-normalized_boxscore.guid ``` 154352576001077780910640079893588160113 czapi's
+normalized_boxscore.guid ``` 129690655252279755696295239689104705205 czapi's
 `get_flat_boxscores_from` function takes a `cz_event_id` and `cz_draw_id` as an
 arguments and returns a (flat) nested list object of all the boxscore
 information on the linescore page. This nested list object can be ingested into
 a pandas DataFrame or pushed to a SQL database. ```python
 api.get_flat_boxscores_from(cz_event_id = 6400, cz_draw_id = 2) ``` [('Wayne
 Tuck Jr.', 'event.php?view=Team&eventid=6400&teamid=144353&profileid=12486#1',
 True, ['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'], '5', 2, 'Draw: 2',
 [True, True, False, True, True, True, True, False, False, False], [0, 0, 2, -2,
--2, -2, -3, -2, -1, 0], 306528221620467227442052913955328486003), ('Matthew
+-2, -2, -3, -2, -1, 0], 296656328202528204780428618855733007061), ('Matthew
 Hall', 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
 False, ['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'], '7', 2, 'Draw: 2',
 [False, False, True, False, False, False, False, True, True, True], [0, 0, -2,
-2, 2, 2, 3, 2, 1, 0], 306528221620467227442052913955328486003), ('Dayna
+2, 2, 2, 3, 2, 1, 0], 296656328202528204780428618855733007061), ('Dayna
 Deruelle',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144346&profileid=26636#1',
 False, ['0', '0', '1', '0', '0', '0', '0', 'X'], '1', 2, 'Draw: 2', [False,
 False, True, False, True, True, True, True], [0, 0, -2, -1, -3, -4, -5, -9],
-169959036371998794200683443427801286021), ('Tyler Stewart',
+105249071225393527432485074456849437076), ('Tyler Stewart',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
 True, ['0', '2', '0', '2', '1', '1', '4', 'X'], '10', 2, 'Draw: 2', [True,
 True, False, True, False, False, False, False], [0, 0, 2, 1, 3, 4, 5, 9],
-169959036371998794200683443427801286021), ('Mark Kean',
+105249071225393527432485074456849437076), ('Mark Kean',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
 True, ['2', '0', '1', '0', '0', '0', '1', '3', 'X'], '7', 2, 'Draw: 2', [True,
 False, False, False, False, True, True, False, False], [0, 2, 2, 3, 3, 1, 0, 1,
-4], 216723633949199876308042205365369844269), ('Jason March',
+4], 17103980631020054974876512539607901632), ('Jason March',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
 False, ['0', '0', '0', '0', '2', '1', '0', '0', 'X'], '3', 2, 'Draw: 2',
 [False, True, True, True, True, False, False, True, True], [0, -2, -2, -3, -3,
--1, 0, -1, -4], 216723633949199876308042205365369844269), ('Richard Krell',
+-1, 0, -1, -4], 17103980631020054974876512539607901632), ('Richard Krell',
 'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144349&profileid=25962#1',
 True, ['2', '0', '1', '0', '2', '1', '1', 'X'], '7', 2, 'Draw: 2', [True,
 False, False, False, True, False, False, False], [0, 2, 2, 3, 2, 4, 5, 6],
-142335171424399828625133635146510278418), ('Rob Ainsley',
+215489388707487834967933616755032135426), ('Rob Ainsley',
 'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
 False, ['0', '0', '0', '1', '0', '0', '0', 'X'], '1', 2, 'Draw: 2', [False,
 True, True, True, False, True, True, True], [0, -2, -2, -3, -2, -4, -5, -6],
-142335171424399828625133635146510278418)] ## Event The `Event` object is a data
+215489388707487834967933616755032135426)] ## Event The `Event` object is a data
 structure which holds all of the `LinescorePage` objects which make up an
 entire event. An `Event` instance is created by passing a `cz_event_id`.
 ```python event = api.Event(cz_event_id = 6400,delay=3,verbose=True) event ```
 Scraping draw 1. Scraping draw 2. Scraping draw 3. Scraping draw 4. Scraping
 draw 5. Scraping draw 6. Scraping draw 7. Event(cz_event_id=6400, delay=3,
 verbose=True) The created `Event` objects holds all the `LinescorePage` objects
 in it's `pages` property. ```python event.pages ``` [LinescorePage
@@ -187,205 +177,413 @@
 'href':
 'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144353&profileid=12486#1',
 'score': ['0', '0', '0', '2', '0', '0', '0', '0', 'X'], 'hammer': False,
 'finalscore': '2'}, 'Rob Ainsley': {'draw': 'Draw: 3', 'draw_num': 3, 'href':
 'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
 'score': ['2', '1', '0', '0', '1', '2', '1', '1', 'X'], 'hammer': True,
 'finalscore': '8'}}] The `get_flat_boxscores` method can be used to return a
-list of (flat) nested list object of all the boxscore information on all the
-linescore pages. ```python event.get_flat_boxscores() ``` [[('Damien Villard',
+list of tuples of all the boxscore information on all the linescore pages.
+```python event.get_flat_boxscores(flat=True) ``` [('Damien Villard',
 'event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1', True, ['0',
 '0', '0', '0', 'X'], '0', 1, 'Draw: 1', [True, True, True, True, True], [0, -1,
--4, -6, -8], 227597408989477916004520082463493572762), ('Matthew Hall',
+-4, -6, -8], 209707243860236114112314247393927711356), ('Matthew Hall',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', False,
 ['1', '3', '2', '2', 'X'], '8', 1, 'Draw: 1', [False, False, False, False,
-False], [0, 1, 4, 6, 8], 227597408989477916004520082463493572762), ('Matthew
+False], [0, 1, 4, 6, 8], 209707243860236114112314247393927711356), ('Matthew
 Mepstead',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144356#1',
 False, ['0', '0', '1', '1', '0', '1', '0', '0', '0', '1', '0'], '4', 1, 'Draw:
 1', [False, False, True, False, False, True, False, False, False, True, False],
-[0, 0, -2, -1, 0, -1, 0, 0, 0, -1, 0],
-230481195381514558834165699232540581342), ('Tyler Stewart',
+[0, 0, -2, -1, 0, -1, 0, 0, 0, -1, 0], 38537103347544582345141893615297919005),
+('Tyler Stewart',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
 True, ['0', '2', '0', '0', '1', '0', '0', '0', '1', '0', '1'], '5', 1, 'Draw:
 1', [True, True, False, True, True, False, True, True, True, False, True], [0,
-0, 2, 1, 0, 1, 0, 0, 0, 1, 0], 230481195381514558834165699232540581342),
-('Jason March',
+0, 2, 1, 0, 1, 0, 0, 0, 1, 0], 38537103347544582345141893615297919005), ('Jason
+March',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
 False, ['0', '2', '0', '1', '0', '2', '2', '0', '2', 'X'], '9', 1, 'Draw: 1',
 [False, False, False, False, False, True, False, False, True, False], [0, 0, 2,
-2, 3, 2, 4, 6, 3, 5], 123876478142928441769100783560984935273), ('Sam Steep',
+2, 3, 2, 4, 6, 3, 5], 272348649831484335603593027216985821953), ('Sam Steep',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144351&profileid=25978#1',
 True, ['0', '0', '0', '0', '1', '0', '0', '3', '0', 'X'], '4', 1, 'Draw: 1',
 [True, True, True, True, True, False, True, True, False, True], [0, 0, -2, -2,
--3, -2, -4, -6, -3, -5], 123876478142928441769100783560984935273)], [('Wayne
-Tuck Jr.', 'event.php?view=Team&eventid=6400&teamid=144353&profileid=12486#1',
-True, ['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'], '5', 2, 'Draw: 2',
-[True, True, False, True, True, True, True, False, False, False], [0, 0, 2, -2,
--2, -2, -3, -2, -1, 0], 309985127892547751219643103116568617832), ('Matthew
-Hall', 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
-False, ['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'], '7', 2, 'Draw: 2',
-[False, False, True, False, False, False, False, True, True, True], [0, 0, -2,
-2, 2, 2, 3, 2, 1, 0], 309985127892547751219643103116568617832), ('Dayna
-Deruelle',
+-3, -2, -4, -6, -3, -5], 272348649831484335603593027216985821953), ('Wayne Tuck
+Jr.', 'event.php?view=Team&eventid=6400&teamid=144353&profileid=12486#1', True,
+['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'], '5', 2, 'Draw: 2', [True,
+True, False, True, True, True, True, False, False, False], [0, 0, 2, -2, -2, -
+2, -3, -2, -1, 0], 95112284881200216258215191883153462659), ('Matthew Hall',
+'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', False,
+['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'], '7', 2, 'Draw: 2', [False,
+False, True, False, False, False, False, True, True, True], [0, 0, -2, 2, 2, 2,
+3, 2, 1, 0], 95112284881200216258215191883153462659), ('Dayna Deruelle',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144346&profileid=26636#1',
 False, ['0', '0', '1', '0', '0', '0', '0', 'X'], '1', 2, 'Draw: 2', [False,
 False, True, False, True, True, True, True], [0, 0, -2, -1, -3, -4, -5, -9],
-258827556868852829922619663221573707805), ('Tyler Stewart',
+59643628877953807377369574857821892232), ('Tyler Stewart',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
 True, ['0', '2', '0', '2', '1', '1', '4', 'X'], '10', 2, 'Draw: 2', [True,
 True, False, True, False, False, False, False], [0, 0, 2, 1, 3, 4, 5, 9],
-258827556868852829922619663221573707805), ('Mark Kean',
+59643628877953807377369574857821892232), ('Mark Kean',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
 True, ['2', '0', '1', '0', '0', '0', '1', '3', 'X'], '7', 2, 'Draw: 2', [True,
 False, False, False, False, True, True, False, False], [0, 2, 2, 3, 3, 1, 0, 1,
-4], 196156262752898539339442275025527127066), ('Jason March',
+4], 122217858840490332010920244446431255640), ('Jason March',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
 False, ['0', '0', '0', '0', '2', '1', '0', '0', 'X'], '3', 2, 'Draw: 2',
 [False, True, True, True, True, False, False, True, True], [0, -2, -2, -3, -3,
--1, 0, -1, -4], 196156262752898539339442275025527127066), ('Richard Krell',
+-1, 0, -1, -4], 122217858840490332010920244446431255640), ('Richard Krell',
 'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144349&profileid=25962#1',
 True, ['2', '0', '1', '0', '2', '1', '1', 'X'], '7', 2, 'Draw: 2', [True,
 False, False, False, True, False, False, False], [0, 2, 2, 3, 2, 4, 5, 6],
-121058110285022966689701916848012130324), ('Rob Ainsley',
+335702133606077232579627915311442373664), ('Rob Ainsley',
 'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
 False, ['0', '0', '0', '1', '0', '0', '0', 'X'], '1', 2, 'Draw: 2', [False,
 True, True, True, False, True, True, True], [0, -2, -2, -3, -2, -4, -5, -6],
-121058110285022966689701916848012130324)], [('Matthew Hall',
+335702133606077232579627915311442373664), ('Matthew Hall',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', True, ['0',
 '0', '2', '1', '2', '1', '0', '2', 'X'], '8', 3, 'Draw: 3', [True, True, True,
 False, False, False, False, True, False], [0, 0, -1, 1, 2, 4, 5, 3, 5],
-167908611678356344738885531672086035216), ('Tyler Stewart',
+53772503334370441085334378293107653659), ('Tyler Stewart',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1', False,
 ['0', '1', '0', '0', '0', '0', '2', '0', 'X'], '3', 3, 'Draw: 3', [False,
 False, False, True, True, True, True, False, True], [0, 0, 1, -1, -2, -4, -5, -
-3, -5], 167908611678356344738885531672086035216), ('Mark Kean',
+3, -5], 53772503334370441085334378293107653659), ('Mark Kean',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
 True, ['0', '5', '0', '1', '1', '1', 'X'], '8', 3, 'Draw: 3', [True, True,
 False, True, False, False, False], [0, -1, 4, 3, 4, 5, 6],
-157383102330203138325358878297425755857), ('Richard Krell',
+310456475955908017873561887016699672637), ('Richard Krell',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144349&profileid=25962#1',
 False, ['1', '0', '1', '0', '0', '0', 'X'], '2', 3, 'Draw: 3', [False, False,
 True, False, True, True, True], [0, 1, -4, -3, -4, -5, -6],
-157383102330203138325358878297425755857), ('Damien Villard',
+310456475955908017873561887016699672637), ('Damien Villard',
 'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144354&profileid=27373#1',
 True, ['2', '1', '0', '1', '0', '0', '1', '0', '0', '0'], '5', 3, 'Draw: 3',
 [True, False, False, True, False, True, True, False, True, True], [0, 2, 3, 2,
-3, 1, 1, 2, 1, 0], 197764335276159882538274022024920645468), ('Sam Steep',
+3, 1, 1, 2, 1, 0], 303047434632680540438656592556261333287), ('Sam Steep',
 'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144351&profileid=25978#1',
 False, ['0', '0', '1', '0', '2', '0', '0', '1', '1', '1'], '6', 3, 'Draw: 3',
 [False, True, True, False, True, False, False, True, False, False], [0, -2, -3,
--2, -3, -1, -1, -2, -1, 0], 197764335276159882538274022024920645468), ('Jason
+-2, -3, -1, -1, -2, -1, 0], 303047434632680540438656592556261333287), ('Jason
 March',
 'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144350#1',
 True, ['1', '1', '0', '0', '0', '0', '2', '1', '2', 'X'], '7', 3, 'Draw: 3',
 [True, False, False, True, True, True, True, False, False, False], [0, 1, 2, 1,
-0, 0, 0, 2, 3, 5], 19248089004956668591585521441771100702), ('Matthew
+0, 0, 0, 2, 3, 5], 229699058183107339172217417532449914369), ('Matthew
 Mepstead',
 'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144356#1',
 False, ['0', '0', '1', '1', '0', '0', '0', '0', '0', 'X'], '2', 3, 'Draw: 3',
 [False, True, True, False, False, False, False, True, True, True], [0, -1, -2,
--1, 0, 0, 0, -2, -3, -5], 19248089004956668591585521441771100702), ('Wayne Tuck
-Jr.',
+-1, 0, 0, 0, -2, -3, -5], 229699058183107339172217417532449914369), ('Wayne
+Tuck Jr.',
 'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144353&profileid=12486#1',
 False, ['0', '0', '0', '2', '0', '0', '0', '0', 'X'], '2', 3, 'Draw: 3',
 [False, True, True, True, False, True, True, True, True], [0, -2, -3, -3, -1, -
-2, -4, -5, -6], 152642289275163622503053683522534226102), ('Rob Ainsley',
+2, -4, -5, -6], 195399470224611539512163135746754073908), ('Rob Ainsley',
 'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
 True, ['2', '1', '0', '0', '1', '2', '1', '1', 'X'], '8', 3, 'Draw: 3', [True,
 False, False, False, True, False, False, False, False], [0, 2, 3, 3, 1, 2, 4,
-5, 6], 152642289275163622503053683522534226102)], [('Matthew Hall',
+5, 6], 195399470224611539512163135746754073908), ('Matthew Hall',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', True, ['1',
 '0', '1', '0', '1', '0', '2', '0', '1', '0'], '6', 4, 'Draw: 4', [True, False,
 True, False, True, False, True, False, True, False], [0, 1, -1, 0, -2, -1, -2,
-0, -1, 0], 128520251865367755000080630810739466709), ('Mark Kean',
+0, -1, 0], 63653233024470732271264476184228625543), ('Mark Kean',
 'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961#1', False,
 ['0', '2', '0', '2', '0', '1', '0', '1', '0', '1'], '7', 4, 'Draw: 4', [False,
 True, False, True, False, True, False, True, False, True], [0, -1, 1, 0, 2, 1,
-2, 0, 1, 0], 128520251865367755000080630810739466709), ('Sam Steep',
+2, 0, 1, 0], 63653233024470732271264476184228625543), ('Sam Steep',
 'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144351&profileid=25978#1',
 False, ['1', '0', '0', '2', '0', '1', '1', '0', '1', '1'], '7', 4, 'Draw: 4',
 [False, False, True, True, False, True, False, False, True, False], [0, 1, 0, -
-2, 0, -2, -1, 0, -1, 0], 164045326452654642850026023480637847801), ('Jason
+2, 0, -2, -1, 0, -1, 0], 279469483516704960424550934244064693031), ('Jason
 March',
 'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144350#1',
 True, ['0', '1', '2', '0', '2', '0', '0', '1', '0', '0'], '6', 4, 'Draw: 4',
 [True, True, False, False, True, False, True, True, False, True], [0, -1, 0, 2,
-0, 2, 1, 0, 1, 0], 164045326452654642850026023480637847801), ('Dayna Deruelle',
+0, 2, 1, 0, 1, 0], 279469483516704960424550934244064693031), ('Dayna Deruelle',
 'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144346&profileid=26636#1',
 False, ['0', '2', '1', '1', '1', '0', '3', 'X'], '8', 4, 'Draw: 4', [False,
 True, False, False, False, False, True, False], [0, -1, 1, 2, 3, 4, 3, 6],
-76792983814886196713410396043046633915), ('Rob Ainsley',
+291113397726148010907174443006816563924), ('Rob Ainsley',
 'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
 True, ['1', '0', '0', '0', '0', '1', '0', 'X'], '2', 4, 'Draw: 4', [True,
 False, True, True, True, True, False, True], [0, 1, -1, -2, -3, -4, -3, -6],
-76792983814886196713410396043046633915)], [('Sam Steep',
+291113397726148010907174443006816563924), ('Sam Steep',
 'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978#1', False,
 ['0', '1', '0', '0', '0', '2', '0', '2', '0', '0'], '5', 5, 'Draw: 5', [False,
 False, False, True, True, True, False, True, False, False], [0, 0, 1, 0, -1, -
-3, -1, -3, -1, -1], 38480930669174444566426826324563146081), ('Richard Krell',
+3, -1, -3, -1, -1], 95866945533461342246819997703085723055), ('Richard Krell',
 'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1', True, ['0',
 '0', '1', '1', '2', '0', '2', '0', '0', '1'], '7', 5, 'Draw: 5', [True, True,
 True, False, False, False, True, False, True, True], [0, 0, -1, 0, 1, 3, 1, 3,
-1, 1], 38480930669174444566426826324563146081), ('Dayna Deruelle',
+1, 1], 95866945533461342246819997703085723055), ('Dayna Deruelle',
 'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144346&profileid=26636#1',
 False, ['0', '0', '1', '0', '0', '0', '1', '0', '3', '1', '0'], '6', 5, 'Draw:
 5', [False, True, True, False, True, True, True, False, True, False, False],
 [0, -1, -1, 0, -1, -1, -3, -2, -4, -1, 0],
-153896726080791122415283970396986089830), ('Tyler Stewart',
+233581897033627594667237538445333000951), ('Tyler Stewart',
 'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144352&profileid=12477#1',
 True, ['1', '0', '0', '1', '0', '2', '0', '2', '0', '0', '1'], '7', 5, 'Draw:
 5', [True, False, False, True, False, False, False, True, False, True, True],
-[0, 1, 1, 0, 1, 1, 3, 2, 4, 1, 0], 153896726080791122415283970396986089830)], [
+[0, 1, 1, 0, 1, 1, 3, 2, 4, 1, 0], 233581897033627594667237538445333000951),
 ('Richard Krell',
 'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1', False,
 ['0', '0', '1', '1', '0', '0', '1', '0', 'X'], '3', 6, 'Draw: 6', [False,
 False, True, False, False, True, True, False, True], [0, 0, -2, -1, 0, -2, -5,
--4, -5], 209637313717849892067917714730669554285), ('Tyler Stewart',
+-4, -5], 61203104491141348409761697458039616615), ('Tyler Stewart',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1', True, ['0',
 '2', '0', '0', '2', '3', '0', '1', 'X'], '8', 6, 'Draw: 6', [True, True, False,
 True, True, False, False, True, False], [0, 0, 2, 1, 0, 2, 5, 4, 5],
-209637313717849892067917714730669554285)], [('Tyler Stewart',
+61203104491141348409761697458039616615), ('Tyler Stewart',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1', False,
 ['0', '0', '1', '1', '0', '3', '0', '0', '1', '0'], '6', 7, 'Draw: 7', [False,
 False, True, False, False, True, False, False, True, False], [0, 0, -1, 0, 1, -
-2, 1, 1, 0, 1], 274892128276167031788079435153352244862), ('Matthew Hall',
+2, 1, 1, 0, 1], 4915701019265174384644466584441738333), ('Matthew Hall',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', True, ['0',
 '1', '0', '0', '3', '0', '0', '1', '0', '2'], '7', 7, 'Draw: 7', [True, True,
 False, True, True, False, True, True, False, True], [0, 0, 1, 0, -1, 2, -1, -1,
-0, -1], 274892128276167031788079435153352244862)]] ```python
-event.get_flat_boxscores()[0] ``` [('Damien Villard',
-'event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1', True, ['0',
-'0', '0', '0', 'X'], '0', 1, 'Draw: 1', [True, True, True, True, True], [0, -1,
--4, -6, -8], 227597408989477916004520082463493572762), ('Matthew Hall',
-'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', False,
-['1', '3', '2', '2', 'X'], '8', 1, 'Draw: 1', [False, False, False, False,
-False], [0, 1, 4, 6, 8], 227597408989477916004520082463493572762), ('Matthew
+0, -1], 4915701019265174384644466584441738333)] The `get_flat_boxscores` method
+can also be used to return a list of `Boxscore` objects for convenience.
+```python event.get_flat_boxscores(flat=False) ``` [Boxscore(team_name='Damien
+Villard',
+href='event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1',
+hammer_start=True, score=['0', '0', '0', '0', 'X'], final_score='0',
+draw_num=1, draw='Draw: 1', hammer_progression=[True, True, True, True, True],
+relative_score=[0, -1, -4, -6, -8],
+guid=209707243860236114112314247393927711356), Boxscore(team_name='Matthew
+Hall', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+hammer_start=False, score=['1', '3', '2', '2', 'X'], final_score='8',
+draw_num=1, draw='Draw: 1', hammer_progression=[False, False, False, False,
+False], relative_score=[0, 1, 4, 6, 8],
+guid=209707243860236114112314247393927711356), Boxscore(team_name='Matthew
 Mepstead',
-'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144356#1',
-False, ['0', '0', '1', '1', '0', '1', '0', '0', '0', '1', '0'], '4', 1, 'Draw:
-1', [False, False, True, False, False, True, False, False, False, True, False],
-[0, 0, -2, -1, 0, -1, 0, 0, 0, -1, 0],
-230481195381514558834165699232540581342), ('Tyler Stewart',
-'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
-True, ['0', '2', '0', '0', '1', '0', '0', '0', '1', '0', '1'], '5', 1, 'Draw:
-1', [True, True, False, True, True, False, True, True, True, False, True], [0,
-0, 2, 1, 0, 1, 0, 0, 0, 1, 0], 230481195381514558834165699232540581342),
-('Jason March',
-'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
-False, ['0', '2', '0', '1', '0', '2', '2', '0', '2', 'X'], '9', 1, 'Draw: 1',
-[False, False, False, False, False, True, False, False, True, False], [0, 0, 2,
-2, 3, 2, 4, 6, 3, 5], 123876478142928441769100783560984935273), ('Sam Steep',
-'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144351&profileid=25978#1',
-True, ['0', '0', '0', '0', '1', '0', '0', '3', '0', 'X'], '4', 1, 'Draw: 1',
-[True, True, True, True, True, False, True, True, False, True], [0, 0, -2, -2,
--3, -2, -4, -6, -3, -5], 123876478142928441769100783560984935273)] ```python
-event.get_flat_boxscores()[-1] ``` [('Tyler Stewart',
-'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1', False,
-['0', '0', '1', '1', '0', '3', '0', '0', '1', '0'], '6', 7, 'Draw: 7', [False,
-False, True, False, False, True, False, False, True, False], [0, 0, -1, 0, 1, -
-2, 1, 1, 0, 1], 274892128276167031788079435153352244862), ('Matthew Hall',
-'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', True, ['0',
-'1', '0', '0', '3', '0', '0', '1', '0', '2'], '7', 7, 'Draw: 7', [True, True,
-False, True, True, False, True, True, False, True], [0, 0, 1, 0, -1, 2, -1, -1,
-0, -1], 274892128276167031788079435153352244862)] ## About czapi czapi is a
-Python library for scraping curling linescores.
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144356#1',
+hammer_start=False, score=['0', '0', '1', '1', '0', '1', '0', '0', '0', '1',
+'0'], final_score='4', draw_num=1, draw='Draw: 1', hammer_progression=[False,
+False, True, False, False, True, False, False, False, True, False],
+relative_score=[0, 0, -2, -1, 0, -1, 0, 0, 0, -1, 0],
+guid=38537103347544582345141893615297919005), Boxscore(team_name='Tyler
+Stewart',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
+hammer_start=True, score=['0', '2', '0', '0', '1', '0', '0', '0', '1', '0',
+'1'], final_score='5', draw_num=1, draw='Draw: 1', hammer_progression=[True,
+True, False, True, True, False, True, True, True, False, True], relative_score=
+[0, 0, 2, 1, 0, 1, 0, 0, 0, 1, 0],
+guid=38537103347544582345141893615297919005), Boxscore(team_name='Jason March',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
+hammer_start=False, score=['0', '2', '0', '1', '0', '2', '2', '0', '2', 'X'],
+final_score='9', draw_num=1, draw='Draw: 1', hammer_progression=[False, False,
+False, False, False, True, False, False, True, False], relative_score=[0, 0, 2,
+2, 3, 2, 4, 6, 3, 5], guid=272348649831484335603593027216985821953), Boxscore
+(team_name='Sam Steep',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144351&profileid=25978#1',
+hammer_start=True, score=['0', '0', '0', '0', '1', '0', '0', '3', '0', 'X'],
+final_score='4', draw_num=1, draw='Draw: 1', hammer_progression=[True, True,
+True, True, True, False, True, True, False, True], relative_score=[0, 0, -2, -
+2, -3, -2, -4, -6, -3, -5], guid=272348649831484335603593027216985821953),
+Boxscore(team_name='Wayne Tuck Jr.',
+href='event.php?view=Team&eventid=6400&teamid=144353&profileid=12486#1',
+hammer_start=True, score=['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'],
+final_score='5', draw_num=2, draw='Draw: 2', hammer_progression=[True, True,
+False, True, True, True, True, False, False, False], relative_score=[0, 0, 2, -
+2, -2, -2, -3, -2, -1, 0], guid=95112284881200216258215191883153462659),
+Boxscore(team_name='Matthew Hall',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+hammer_start=False, score=['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'],
+final_score='7', draw_num=2, draw='Draw: 2', hammer_progression=[False, False,
+True, False, False, False, False, True, True, True], relative_score=[0, 0, -2,
+2, 2, 2, 3, 2, 1, 0], guid=95112284881200216258215191883153462659), Boxscore
+(team_name='Dayna Deruelle',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144346&profileid=26636#1',
+hammer_start=False, score=['0', '0', '1', '0', '0', '0', '0', 'X'],
+final_score='1', draw_num=2, draw='Draw: 2', hammer_progression=[False, False,
+True, False, True, True, True, True], relative_score=[0, 0, -2, -1, -3, -4, -5,
+-9], guid=59643628877953807377369574857821892232), Boxscore(team_name='Tyler
+Stewart',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
+hammer_start=True, score=['0', '2', '0', '2', '1', '1', '4', 'X'],
+final_score='10', draw_num=2, draw='Draw: 2', hammer_progression=[True, True,
+False, True, False, False, False, False], relative_score=[0, 0, 2, 1, 3, 4, 5,
+9], guid=59643628877953807377369574857821892232), Boxscore(team_name='Mark
+Kean',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
+hammer_start=True, score=['2', '0', '1', '0', '0', '0', '1', '3', 'X'],
+final_score='7', draw_num=2, draw='Draw: 2', hammer_progression=[True, False,
+False, False, False, True, True, False, False], relative_score=[0, 2, 2, 3, 3,
+1, 0, 1, 4], guid=122217858840490332010920244446431255640), Boxscore
+(team_name='Jason March',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
+hammer_start=False, score=['0', '0', '0', '0', '2', '1', '0', '0', 'X'],
+final_score='3', draw_num=2, draw='Draw: 2', hammer_progression=[False, True,
+True, True, True, False, False, True, True], relative_score=[0, -2, -2, -3, -3,
+-1, 0, -1, -4], guid=122217858840490332010920244446431255640), Boxscore
+(team_name='Richard Krell',
+href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144349&profileid=25962#1',
+hammer_start=True, score=['2', '0', '1', '0', '2', '1', '1', 'X'],
+final_score='7', draw_num=2, draw='Draw: 2', hammer_progression=[True, False,
+False, False, True, False, False, False], relative_score=[0, 2, 2, 3, 2, 4, 5,
+6], guid=335702133606077232579627915311442373664), Boxscore(team_name='Rob
+Ainsley',
+href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
+hammer_start=False, score=['0', '0', '0', '1', '0', '0', '0', 'X'],
+final_score='1', draw_num=2, draw='Draw: 2', hammer_progression=[False, True,
+True, True, False, True, True, True], relative_score=[0, -2, -2, -3, -2, -4, -
+5, -6], guid=335702133606077232579627915311442373664), Boxscore
+(team_name='Matthew Hall',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+hammer_start=True, score=['0', '0', '2', '1', '2', '1', '0', '2', 'X'],
+final_score='8', draw_num=3, draw='Draw: 3', hammer_progression=[True, True,
+True, False, False, False, False, True, False], relative_score=[0, 0, -1, 1, 2,
+4, 5, 3, 5], guid=53772503334370441085334378293107653659), Boxscore
+(team_name='Tyler Stewart',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
+hammer_start=False, score=['0', '1', '0', '0', '0', '0', '2', '0', 'X'],
+final_score='3', draw_num=3, draw='Draw: 3', hammer_progression=[False, False,
+False, True, True, True, True, False, True], relative_score=[0, 0, 1, -1, -2, -
+4, -5, -3, -5], guid=53772503334370441085334378293107653659), Boxscore
+(team_name='Mark Kean',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
+hammer_start=True, score=['0', '5', '0', '1', '1', '1', 'X'], final_score='8',
+draw_num=3, draw='Draw: 3', hammer_progression=[True, True, False, True, False,
+False, False], relative_score=[0, -1, 4, 3, 4, 5, 6],
+guid=310456475955908017873561887016699672637), Boxscore(team_name='Richard
+Krell',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144349&profileid=25962#1',
+hammer_start=False, score=['1', '0', '1', '0', '0', '0', 'X'], final_score='2',
+draw_num=3, draw='Draw: 3', hammer_progression=[False, False, True, False,
+True, True, True], relative_score=[0, 1, -4, -3, -4, -5, -6],
+guid=310456475955908017873561887016699672637), Boxscore(team_name='Damien
+Villard',
+href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144354&profileid=27373#1',
+hammer_start=True, score=['2', '1', '0', '1', '0', '0', '1', '0', '0', '0'],
+final_score='5', draw_num=3, draw='Draw: 3', hammer_progression=[True, False,
+False, True, False, True, True, False, True, True], relative_score=[0, 2, 3, 2,
+3, 1, 1, 2, 1, 0], guid=303047434632680540438656592556261333287), Boxscore
+(team_name='Sam Steep',
+href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144351&profileid=25978#1',
+hammer_start=False, score=['0', '0', '1', '0', '2', '0', '0', '1', '1', '1'],
+final_score='6', draw_num=3, draw='Draw: 3', hammer_progression=[False, True,
+True, False, True, False, False, True, False, False], relative_score=[0, -2, -
+3, -2, -3, -1, -1, -2, -1, 0], guid=303047434632680540438656592556261333287),
+Boxscore(team_name='Jason March',
+href='event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144350#1',
+hammer_start=True, score=['1', '1', '0', '0', '0', '0', '2', '1', '2', 'X'],
+final_score='7', draw_num=3, draw='Draw: 3', hammer_progression=[True, False,
+False, True, True, True, True, False, False, False], relative_score=[0, 1, 2,
+1, 0, 0, 0, 2, 3, 5], guid=229699058183107339172217417532449914369), Boxscore
+(team_name='Matthew Mepstead',
+href='event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144356#1',
+hammer_start=False, score=['0', '0', '1', '1', '0', '0', '0', '0', '0', 'X'],
+final_score='2', draw_num=3, draw='Draw: 3', hammer_progression=[False, True,
+True, False, False, False, False, True, True, True], relative_score=[0, -1, -2,
+-1, 0, 0, 0, -2, -3, -5], guid=229699058183107339172217417532449914369),
+Boxscore(team_name='Wayne Tuck Jr.',
+href='event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144353&profileid=12486#1',
+hammer_start=False, score=['0', '0', '0', '2', '0', '0', '0', '0', 'X'],
+final_score='2', draw_num=3, draw='Draw: 3', hammer_progression=[False, True,
+True, True, False, True, True, True, True], relative_score=[0, -2, -3, -3, -1,
+-2, -4, -5, -6], guid=195399470224611539512163135746754073908), Boxscore
+(team_name='Rob Ainsley',
+href='event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
+hammer_start=True, score=['2', '1', '0', '0', '1', '2', '1', '1', 'X'],
+final_score='8', draw_num=3, draw='Draw: 3', hammer_progression=[True, False,
+False, False, True, False, False, False, False], relative_score=[0, 2, 3, 3, 1,
+2, 4, 5, 6], guid=195399470224611539512163135746754073908), Boxscore
+(team_name='Matthew Hall',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+hammer_start=True, score=['1', '0', '1', '0', '1', '0', '2', '0', '1', '0'],
+final_score='6', draw_num=4, draw='Draw: 4', hammer_progression=[True, False,
+True, False, True, False, True, False, True, False], relative_score=[0, 1, -1,
+0, -2, -1, -2, 0, -1, 0], guid=63653233024470732271264476184228625543),
+Boxscore(team_name='Mark Kean',
+href='event.php?view=Team&eventid=6400&teamid=144348&profileid=25961#1',
+hammer_start=False, score=['0', '2', '0', '2', '0', '1', '0', '1', '0', '1'],
+final_score='7', draw_num=4, draw='Draw: 4', hammer_progression=[False, True,
+False, True, False, True, False, True, False, True], relative_score=[0, -1, 1,
+0, 2, 1, 2, 0, 1, 0], guid=63653233024470732271264476184228625543), Boxscore
+(team_name='Sam Steep',
+href='event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144351&profileid=25978#1',
+hammer_start=False, score=['1', '0', '0', '2', '0', '1', '1', '0', '1', '1'],
+final_score='7', draw_num=4, draw='Draw: 4', hammer_progression=[False, False,
+True, True, False, True, False, False, True, False], relative_score=[0, 1, 0, -
+2, 0, -2, -1, 0, -1, 0], guid=279469483516704960424550934244064693031),
+Boxscore(team_name='Jason March',
+href='event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144350#1',
+hammer_start=True, score=['0', '1', '2', '0', '2', '0', '0', '1', '0', '0'],
+final_score='6', draw_num=4, draw='Draw: 4', hammer_progression=[True, True,
+False, False, True, False, True, True, False, True], relative_score=[0, -1, 0,
+2, 0, 2, 1, 0, 1, 0], guid=279469483516704960424550934244064693031), Boxscore
+(team_name='Dayna Deruelle',
+href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144346&profileid=26636#1',
+hammer_start=False, score=['0', '2', '1', '1', '1', '0', '3', 'X'],
+final_score='8', draw_num=4, draw='Draw: 4', hammer_progression=[False, True,
+False, False, False, False, True, False], relative_score=[0, -1, 1, 2, 3, 4, 3,
+6], guid=291113397726148010907174443006816563924), Boxscore(team_name='Rob
+Ainsley',
+href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
+hammer_start=True, score=['1', '0', '0', '0', '0', '1', '0', 'X'],
+final_score='2', draw_num=4, draw='Draw: 4', hammer_progression=[True, False,
+True, True, True, True, False, True], relative_score=[0, 1, -1, -2, -3, -4, -3,
+-6], guid=291113397726148010907174443006816563924), Boxscore(team_name='Sam
+Steep',
+href='event.php?view=Team&eventid=6400&teamid=144351&profileid=25978#1',
+hammer_start=False, score=['0', '1', '0', '0', '0', '2', '0', '2', '0', '0'],
+final_score='5', draw_num=5, draw='Draw: 5', hammer_progression=[False, False,
+False, True, True, True, False, True, False, False], relative_score=[0, 0, 1,
+0, -1, -3, -1, -3, -1, -1], guid=95866945533461342246819997703085723055),
+Boxscore(team_name='Richard Krell',
+href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1',
+hammer_start=True, score=['0', '0', '1', '1', '2', '0', '2', '0', '0', '1'],
+final_score='7', draw_num=5, draw='Draw: 5', hammer_progression=[True, True,
+True, False, False, False, True, False, True, True], relative_score=[0, 0, -1,
+0, 1, 3, 1, 3, 1, 1], guid=95866945533461342246819997703085723055), Boxscore
+(team_name='Dayna Deruelle',
+href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144346&profileid=26636#1',
+hammer_start=False, score=['0', '0', '1', '0', '0', '0', '1', '0', '3', '1',
+'0'], final_score='6', draw_num=5, draw='Draw: 5', hammer_progression=[False,
+True, True, False, True, True, True, False, True, False, False],
+relative_score=[0, -1, -1, 0, -1, -1, -3, -2, -4, -1, 0],
+guid=233581897033627594667237538445333000951), Boxscore(team_name='Tyler
+Stewart',
+href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144352&profileid=12477#1',
+hammer_start=True, score=['1', '0', '0', '1', '0', '2', '0', '2', '0', '0',
+'1'], final_score='7', draw_num=5, draw='Draw: 5', hammer_progression=[True,
+False, False, True, False, False, False, True, False, True, True],
+relative_score=[0, 1, 1, 0, 1, 1, 3, 2, 4, 1, 0],
+guid=233581897033627594667237538445333000951), Boxscore(team_name='Richard
+Krell',
+href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1',
+hammer_start=False, score=['0', '0', '1', '1', '0', '0', '1', '0', 'X'],
+final_score='3', draw_num=6, draw='Draw: 6', hammer_progression=[False, False,
+True, False, False, True, True, False, True], relative_score=[0, 0, -2, -1, 0,
+-2, -5, -4, -5], guid=61203104491141348409761697458039616615), Boxscore
+(team_name='Tyler Stewart',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
+hammer_start=True, score=['0', '2', '0', '0', '2', '3', '0', '1', 'X'],
+final_score='8', draw_num=6, draw='Draw: 6', hammer_progression=[True, True,
+False, True, True, False, False, True, False], relative_score=[0, 0, 2, 1, 0,
+2, 5, 4, 5], guid=61203104491141348409761697458039616615), Boxscore
+(team_name='Tyler Stewart',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
+hammer_start=False, score=['0', '0', '1', '1', '0', '3', '0', '0', '1', '0'],
+final_score='6', draw_num=7, draw='Draw: 7', hammer_progression=[False, False,
+True, False, False, True, False, False, True, False], relative_score=[0, 0, -1,
+0, 1, -2, 1, 1, 0, 1], guid=4915701019265174384644466584441738333), Boxscore
+(team_name='Matthew Hall',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+hammer_start=True, score=['0', '1', '0', '0', '3', '0', '0', '1', '0', '2'],
+final_score='7', draw_num=7, draw='Draw: 7', hammer_progression=[True, True,
+False, True, True, False, True, True, False, True], relative_score=[0, 0, 1, 0,
+-1, 2, -1, -1, 0, -1], guid=4915701019265174384644466584441738333)] ```python
+event.get_flat_boxscores()[0] ``` Boxscore(team_name='Damien Villard',
+href='event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1',
+hammer_start=True, score=['0', '0', '0', '0', 'X'], final_score='0',
+draw_num=1, draw='Draw: 1', hammer_progression=[True, True, True, True, True],
+relative_score=[0, -1, -4, -6, -8],
+guid=209707243860236114112314247393927711356) ```python
+event.get_flat_boxscores()[-1] ``` Boxscore(team_name='Matthew Hall',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+hammer_start=True, score=['0', '1', '0', '0', '3', '0', '0', '1', '0', '2'],
+final_score='7', draw_num=7, draw='Draw: 7', hammer_progression=[True, True,
+False, True, True, False, True, True, False, True], relative_score=[0, 0, 1, 0,
+-1, 2, -1, -1, 0, -1], guid=4915701019265174384644466584441738333) ## About
+czapi czapi is a Python library for scraping curling linescores.
```

### Comparing `czapi-0.1.9/czapi/_nbdev.py` & `czapi-0.2.0/czapi/_nbdev.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
          "NormalizedBoxscore": "00_base.ipynb",
          "Page": "00_base.ipynb",
          "LinescorePage": "00_base.ipynb",
          "BadLinescorePage": "00_base.ipynb",
          "GameData": "00_base.ipynb",
          "game_data_column_headers": "00_base.ipynb",
          "get_flat_boxscores_from": "00_base.ipynb",
+         "Boxscore": "00_base.ipynb",
          "Event": "00_base.ipynb",
          "DifferentScoreLengthError": "02_errors.ipynb",
          "InvalidScoreError": "02_errors.ipynb",
          "InvalidEventError": "02_errors.ipynb",
          "make_request_from": "03_utils.ipynb",
          "make_soup_from": "03_utils.ipynb",
          "TagBase": "04_testing.ipynb",
```

### Comparing `czapi-0.1.9/czapi/core/errors.py` & `czapi-0.2.0/czapi/core/errors.py`

 * *Files identical despite different names*

### Comparing `czapi-0.1.9/czapi/core/scraping/base.py` & `czapi-0.2.0/czapi/core/scraping/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/00_base.ipynb (unless otherwise specified).
 
-__all__ = ['LinescorePage', 'game_data_column_headers', 'get_flat_boxscores_from', 'Event']
+__all__ = ['LinescorePage', 'game_data_column_headers', 'get_flat_boxscores_from', 'Boxscore', 'Event']
 
 # Cell
 
 from bs4 import Tag
 from abc import ABC, abstractproperty, abstractmethod
 from dataclasses import dataclass
 from typing import Optional, List, Any, Tuple
@@ -332,14 +332,29 @@
 def get_flat_boxscores_from(cz_event_id:int,cz_draw_id:int)->GameData:
     """Returns a list of tuples of boxscore information on a linescore page."""
     linescore_page = LinescorePage(cz_event_id = cz_event_id,cz_draw_id = cz_draw_id)
     return _get_flat_boxscores_from(linescore_page = linescore_page)
 
 # Cell
 
+@dataclass
+class Boxscore:
+    team_name:str
+    href:str
+    hammer_start:bool
+    score:List[str]
+    final_score:str
+    draw_num: int
+    draw: str
+    hammer_progression: List[bool]
+    relative_score: List[int]
+    guid:int
+
+# Cell
+
 
 @dataclass
 class Event:
     cz_event_id : int
     delay : int =0
     verbose: bool = False
 
@@ -370,9 +385,12 @@
         return 'https://curlingzone.com/event.php?eventid=%s&view=Scores&showdrawid=1#1'%(self.cz_event_id)
 
     @property
     def draws(self)->int:
         return len(self.soup.find(name='select').find_all(name='option'))
 
 
-    def get_flat_boxscores(self)->List[GameData]:
-        return [_get_flat_boxscores_from(linescore_page = linescore_page) for linescore_page in self.pages]
+    def get_flat_boxscores(self,flat=False)->List[GameData]:
+        if flat:
+            return [boxscore for linescore_page in self.pages for boxscore in _get_flat_boxscores_from(linescore_page = linescore_page)]
+        return [Boxscore(*boxscore) for linescore_page in self.pages for boxscore in _get_flat_boxscores_from(linescore_page = linescore_page)]
+
```

### Comparing `czapi-0.1.9/czapi/core/testing.py` & `czapi-0.2.0/czapi/core/testing.py`

 * *Files identical despite different names*

### Comparing `czapi-0.1.9/czapi/core/utils.py` & `czapi-0.2.0/czapi/core/utils.py`

 * *Files identical despite different names*

### Comparing `czapi-0.1.9/czapi.egg-info/PKG-INFO` & `czapi-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czapi
-Version: 0.1.9
+Version: 0.2.0
 Summary: CurlingZone scraper API.
 Home-page: https://github.com/calicorob/czapi/tree/master/
 Author: Robert Currie
 Author-email: robert.art.currie@gmail.com
 License: Apache Software License 2.0
 Keywords: curling,stats
 Platform: UNKNOWN
@@ -224,15 +224,15 @@
 ```python
 normalized_boxscore.guid
 ```
 
 
 
 
-    154352576001077780910640079893588160113
+    129690655252279755696295239689104705205
 
 
 
 czapi's `get_flat_boxscores_from` function takes a `cz_event_id` and `cz_draw_id` as an arguments and returns a (flat) nested list object of all the boxscore information on the linescore page. This nested list object can be ingested into a pandas DataFrame or pushed to a SQL database.
 
 ```python
 api.get_flat_boxscores_from(cz_event_id = 6400, cz_draw_id = 2)
@@ -246,85 +246,85 @@
       True,
       ['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'],
       '5',
       2,
       'Draw: 2',
       [True, True, False, True, True, True, True, False, False, False],
       [0, 0, 2, -2, -2, -2, -3, -2, -1, 0],
-      306528221620467227442052913955328486003),
+      296656328202528204780428618855733007061),
      ('Matthew Hall',
       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
       False,
       ['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'],
       '7',
       2,
       'Draw: 2',
       [False, False, True, False, False, False, False, True, True, True],
       [0, 0, -2, 2, 2, 2, 3, 2, 1, 0],
-      306528221620467227442052913955328486003),
+      296656328202528204780428618855733007061),
      ('Dayna Deruelle',
       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144346&profileid=26636#1',
       False,
       ['0', '0', '1', '0', '0', '0', '0', 'X'],
       '1',
       2,
       'Draw: 2',
       [False, False, True, False, True, True, True, True],
       [0, 0, -2, -1, -3, -4, -5, -9],
-      169959036371998794200683443427801286021),
+      105249071225393527432485074456849437076),
      ('Tyler Stewart',
       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
       True,
       ['0', '2', '0', '2', '1', '1', '4', 'X'],
       '10',
       2,
       'Draw: 2',
       [True, True, False, True, False, False, False, False],
       [0, 0, 2, 1, 3, 4, 5, 9],
-      169959036371998794200683443427801286021),
+      105249071225393527432485074456849437076),
      ('Mark Kean',
       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
       True,
       ['2', '0', '1', '0', '0', '0', '1', '3', 'X'],
       '7',
       2,
       'Draw: 2',
       [True, False, False, False, False, True, True, False, False],
       [0, 2, 2, 3, 3, 1, 0, 1, 4],
-      216723633949199876308042205365369844269),
+      17103980631020054974876512539607901632),
      ('Jason March',
       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
       False,
       ['0', '0', '0', '0', '2', '1', '0', '0', 'X'],
       '3',
       2,
       'Draw: 2',
       [False, True, True, True, True, False, False, True, True],
       [0, -2, -2, -3, -3, -1, 0, -1, -4],
-      216723633949199876308042205365369844269),
+      17103980631020054974876512539607901632),
      ('Richard Krell',
       'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144349&profileid=25962#1',
       True,
       ['2', '0', '1', '0', '2', '1', '1', 'X'],
       '7',
       2,
       'Draw: 2',
       [True, False, False, False, True, False, False, False],
       [0, 2, 2, 3, 2, 4, 5, 6],
-      142335171424399828625133635146510278418),
+      215489388707487834967933616755032135426),
      ('Rob Ainsley',
       'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
       False,
       ['0', '0', '0', '1', '0', '0', '0', 'X'],
       '1',
       2,
       'Draw: 2',
       [False, True, True, True, False, True, True, True],
       [0, -2, -2, -3, -2, -4, -5, -6],
-      142335171424399828625133635146510278418)]
+      215489388707487834967933616755032135426)]
 
 
 
 ## Event
 
 The `Event` object is a data structure which holds all of the `LinescorePage` objects which make up an entire event. 
 
@@ -449,503 +449,475 @@
        'href': 'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
        'score': ['2', '1', '0', '0', '1', '2', '1', '1', 'X'],
        'hammer': True,
        'finalscore': '8'}}]
 
 
 
-The `get_flat_boxscores` method can be used to return a list of (flat) nested list object of all the boxscore information on all the linescore pages.
+The `get_flat_boxscores` method can be used to return a list of tuples of all the boxscore information on all the linescore pages.
 
 ```python
-event.get_flat_boxscores()
-```
-
-
-
-
-    [[('Damien Villard',
-       'event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1',
-       True,
-       ['0', '0', '0', '0', 'X'],
-       '0',
-       1,
-       'Draw: 1',
-       [True, True, True, True, True],
-       [0, -1, -4, -6, -8],
-       227597408989477916004520082463493572762),
-      ('Matthew Hall',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
-       False,
-       ['1', '3', '2', '2', 'X'],
-       '8',
-       1,
-       'Draw: 1',
-       [False, False, False, False, False],
-       [0, 1, 4, 6, 8],
-       227597408989477916004520082463493572762),
-      ('Matthew Mepstead',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144356#1',
-       False,
-       ['0', '0', '1', '1', '0', '1', '0', '0', '0', '1', '0'],
-       '4',
-       1,
-       'Draw: 1',
-       [False, False, True, False, False, True, False, False, False, True, False],
-       [0, 0, -2, -1, 0, -1, 0, 0, 0, -1, 0],
-       230481195381514558834165699232540581342),
-      ('Tyler Stewart',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
-       True,
-       ['0', '2', '0', '0', '1', '0', '0', '0', '1', '0', '1'],
-       '5',
-       1,
-       'Draw: 1',
-       [True, True, False, True, True, False, True, True, True, False, True],
-       [0, 0, 2, 1, 0, 1, 0, 0, 0, 1, 0],
-       230481195381514558834165699232540581342),
-      ('Jason March',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
-       False,
-       ['0', '2', '0', '1', '0', '2', '2', '0', '2', 'X'],
-       '9',
-       1,
-       'Draw: 1',
-       [False, False, False, False, False, True, False, False, True, False],
-       [0, 0, 2, 2, 3, 2, 4, 6, 3, 5],
-       123876478142928441769100783560984935273),
-      ('Sam Steep',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144351&profileid=25978#1',
-       True,
-       ['0', '0', '0', '0', '1', '0', '0', '3', '0', 'X'],
-       '4',
-       1,
-       'Draw: 1',
-       [True, True, True, True, True, False, True, True, False, True],
-       [0, 0, -2, -2, -3, -2, -4, -6, -3, -5],
-       123876478142928441769100783560984935273)],
-     [('Wayne Tuck Jr.',
-       'event.php?view=Team&eventid=6400&teamid=144353&profileid=12486#1',
-       True,
-       ['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'],
-       '5',
-       2,
-       'Draw: 2',
-       [True, True, False, True, True, True, True, False, False, False],
-       [0, 0, 2, -2, -2, -2, -3, -2, -1, 0],
-       309985127892547751219643103116568617832),
-      ('Matthew Hall',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
-       False,
-       ['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'],
-       '7',
-       2,
-       'Draw: 2',
-       [False, False, True, False, False, False, False, True, True, True],
-       [0, 0, -2, 2, 2, 2, 3, 2, 1, 0],
-       309985127892547751219643103116568617832),
-      ('Dayna Deruelle',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144346&profileid=26636#1',
-       False,
-       ['0', '0', '1', '0', '0', '0', '0', 'X'],
-       '1',
-       2,
-       'Draw: 2',
-       [False, False, True, False, True, True, True, True],
-       [0, 0, -2, -1, -3, -4, -5, -9],
-       258827556868852829922619663221573707805),
-      ('Tyler Stewart',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
-       True,
-       ['0', '2', '0', '2', '1', '1', '4', 'X'],
-       '10',
-       2,
-       'Draw: 2',
-       [True, True, False, True, False, False, False, False],
-       [0, 0, 2, 1, 3, 4, 5, 9],
-       258827556868852829922619663221573707805),
-      ('Mark Kean',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
-       True,
-       ['2', '0', '1', '0', '0', '0', '1', '3', 'X'],
-       '7',
-       2,
-       'Draw: 2',
-       [True, False, False, False, False, True, True, False, False],
-       [0, 2, 2, 3, 3, 1, 0, 1, 4],
-       196156262752898539339442275025527127066),
-      ('Jason March',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
-       False,
-       ['0', '0', '0', '0', '2', '1', '0', '0', 'X'],
-       '3',
-       2,
-       'Draw: 2',
-       [False, True, True, True, True, False, False, True, True],
-       [0, -2, -2, -3, -3, -1, 0, -1, -4],
-       196156262752898539339442275025527127066),
-      ('Richard Krell',
-       'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144349&profileid=25962#1',
-       True,
-       ['2', '0', '1', '0', '2', '1', '1', 'X'],
-       '7',
-       2,
-       'Draw: 2',
-       [True, False, False, False, True, False, False, False],
-       [0, 2, 2, 3, 2, 4, 5, 6],
-       121058110285022966689701916848012130324),
-      ('Rob Ainsley',
-       'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
-       False,
-       ['0', '0', '0', '1', '0', '0', '0', 'X'],
-       '1',
-       2,
-       'Draw: 2',
-       [False, True, True, True, False, True, True, True],
-       [0, -2, -2, -3, -2, -4, -5, -6],
-       121058110285022966689701916848012130324)],
-     [('Matthew Hall',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
-       True,
-       ['0', '0', '2', '1', '2', '1', '0', '2', 'X'],
-       '8',
-       3,
-       'Draw: 3',
-       [True, True, True, False, False, False, False, True, False],
-       [0, 0, -1, 1, 2, 4, 5, 3, 5],
-       167908611678356344738885531672086035216),
-      ('Tyler Stewart',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
-       False,
-       ['0', '1', '0', '0', '0', '0', '2', '0', 'X'],
-       '3',
-       3,
-       'Draw: 3',
-       [False, False, False, True, True, True, True, False, True],
-       [0, 0, 1, -1, -2, -4, -5, -3, -5],
-       167908611678356344738885531672086035216),
-      ('Mark Kean',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
-       True,
-       ['0', '5', '0', '1', '1', '1', 'X'],
-       '8',
-       3,
-       'Draw: 3',
-       [True, True, False, True, False, False, False],
-       [0, -1, 4, 3, 4, 5, 6],
-       157383102330203138325358878297425755857),
-      ('Richard Krell',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144349&profileid=25962#1',
-       False,
-       ['1', '0', '1', '0', '0', '0', 'X'],
-       '2',
-       3,
-       'Draw: 3',
-       [False, False, True, False, True, True, True],
-       [0, 1, -4, -3, -4, -5, -6],
-       157383102330203138325358878297425755857),
-      ('Damien Villard',
-       'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144354&profileid=27373#1',
-       True,
-       ['2', '1', '0', '1', '0', '0', '1', '0', '0', '0'],
-       '5',
-       3,
-       'Draw: 3',
-       [True, False, False, True, False, True, True, False, True, True],
-       [0, 2, 3, 2, 3, 1, 1, 2, 1, 0],
-       197764335276159882538274022024920645468),
-      ('Sam Steep',
-       'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144351&profileid=25978#1',
-       False,
-       ['0', '0', '1', '0', '2', '0', '0', '1', '1', '1'],
-       '6',
-       3,
-       'Draw: 3',
-       [False, True, True, False, True, False, False, True, False, False],
-       [0, -2, -3, -2, -3, -1, -1, -2, -1, 0],
-       197764335276159882538274022024920645468),
-      ('Jason March',
-       'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144350#1',
-       True,
-       ['1', '1', '0', '0', '0', '0', '2', '1', '2', 'X'],
-       '7',
-       3,
-       'Draw: 3',
-       [True, False, False, True, True, True, True, False, False, False],
-       [0, 1, 2, 1, 0, 0, 0, 2, 3, 5],
-       19248089004956668591585521441771100702),
-      ('Matthew Mepstead',
-       'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144356#1',
-       False,
-       ['0', '0', '1', '1', '0', '0', '0', '0', '0', 'X'],
-       '2',
-       3,
-       'Draw: 3',
-       [False, True, True, False, False, False, False, True, True, True],
-       [0, -1, -2, -1, 0, 0, 0, -2, -3, -5],
-       19248089004956668591585521441771100702),
-      ('Wayne Tuck Jr.',
-       'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144353&profileid=12486#1',
-       False,
-       ['0', '0', '0', '2', '0', '0', '0', '0', 'X'],
-       '2',
-       3,
-       'Draw: 3',
-       [False, True, True, True, False, True, True, True, True],
-       [0, -2, -3, -3, -1, -2, -4, -5, -6],
-       152642289275163622503053683522534226102),
-      ('Rob Ainsley',
-       'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
-       True,
-       ['2', '1', '0', '0', '1', '2', '1', '1', 'X'],
-       '8',
-       3,
-       'Draw: 3',
-       [True, False, False, False, True, False, False, False, False],
-       [0, 2, 3, 3, 1, 2, 4, 5, 6],
-       152642289275163622503053683522534226102)],
-     [('Matthew Hall',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
-       True,
-       ['1', '0', '1', '0', '1', '0', '2', '0', '1', '0'],
-       '6',
-       4,
-       'Draw: 4',
-       [True, False, True, False, True, False, True, False, True, False],
-       [0, 1, -1, 0, -2, -1, -2, 0, -1, 0],
-       128520251865367755000080630810739466709),
-      ('Mark Kean',
-       'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961#1',
-       False,
-       ['0', '2', '0', '2', '0', '1', '0', '1', '0', '1'],
-       '7',
-       4,
-       'Draw: 4',
-       [False, True, False, True, False, True, False, True, False, True],
-       [0, -1, 1, 0, 2, 1, 2, 0, 1, 0],
-       128520251865367755000080630810739466709),
-      ('Sam Steep',
-       'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144351&profileid=25978#1',
-       False,
-       ['1', '0', '0', '2', '0', '1', '1', '0', '1', '1'],
-       '7',
-       4,
-       'Draw: 4',
-       [False, False, True, True, False, True, False, False, True, False],
-       [0, 1, 0, -2, 0, -2, -1, 0, -1, 0],
-       164045326452654642850026023480637847801),
-      ('Jason March',
-       'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144350#1',
-       True,
-       ['0', '1', '2', '0', '2', '0', '0', '1', '0', '0'],
-       '6',
-       4,
-       'Draw: 4',
-       [True, True, False, False, True, False, True, True, False, True],
-       [0, -1, 0, 2, 0, 2, 1, 0, 1, 0],
-       164045326452654642850026023480637847801),
-      ('Dayna Deruelle',
-       'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144346&profileid=26636#1',
-       False,
-       ['0', '2', '1', '1', '1', '0', '3', 'X'],
-       '8',
-       4,
-       'Draw: 4',
-       [False, True, False, False, False, False, True, False],
-       [0, -1, 1, 2, 3, 4, 3, 6],
-       76792983814886196713410396043046633915),
-      ('Rob Ainsley',
-       'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
-       True,
-       ['1', '0', '0', '0', '0', '1', '0', 'X'],
-       '2',
-       4,
-       'Draw: 4',
-       [True, False, True, True, True, True, False, True],
-       [0, 1, -1, -2, -3, -4, -3, -6],
-       76792983814886196713410396043046633915)],
-     [('Sam Steep',
-       'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978#1',
-       False,
-       ['0', '1', '0', '0', '0', '2', '0', '2', '0', '0'],
-       '5',
-       5,
-       'Draw: 5',
-       [False, False, False, True, True, True, False, True, False, False],
-       [0, 0, 1, 0, -1, -3, -1, -3, -1, -1],
-       38480930669174444566426826324563146081),
-      ('Richard Krell',
-       'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1',
-       True,
-       ['0', '0', '1', '1', '2', '0', '2', '0', '0', '1'],
-       '7',
-       5,
-       'Draw: 5',
-       [True, True, True, False, False, False, True, False, True, True],
-       [0, 0, -1, 0, 1, 3, 1, 3, 1, 1],
-       38480930669174444566426826324563146081),
-      ('Dayna Deruelle',
-       'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144346&profileid=26636#1',
-       False,
-       ['0', '0', '1', '0', '0', '0', '1', '0', '3', '1', '0'],
-       '6',
-       5,
-       'Draw: 5',
-       [False, True, True, False, True, True, True, False, True, False, False],
-       [0, -1, -1, 0, -1, -1, -3, -2, -4, -1, 0],
-       153896726080791122415283970396986089830),
-      ('Tyler Stewart',
-       'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144352&profileid=12477#1',
-       True,
-       ['1', '0', '0', '1', '0', '2', '0', '2', '0', '0', '1'],
-       '7',
-       5,
-       'Draw: 5',
-       [True, False, False, True, False, False, False, True, False, True, True],
-       [0, 1, 1, 0, 1, 1, 3, 2, 4, 1, 0],
-       153896726080791122415283970396986089830)],
-     [('Richard Krell',
-       'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1',
-       False,
-       ['0', '0', '1', '1', '0', '0', '1', '0', 'X'],
-       '3',
-       6,
-       'Draw: 6',
-       [False, False, True, False, False, True, True, False, True],
-       [0, 0, -2, -1, 0, -2, -5, -4, -5],
-       209637313717849892067917714730669554285),
-      ('Tyler Stewart',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
-       True,
-       ['0', '2', '0', '0', '2', '3', '0', '1', 'X'],
-       '8',
-       6,
-       'Draw: 6',
-       [True, True, False, True, True, False, False, True, False],
-       [0, 0, 2, 1, 0, 2, 5, 4, 5],
-       209637313717849892067917714730669554285)],
-     [('Tyler Stewart',
-       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
-       False,
-       ['0', '0', '1', '1', '0', '3', '0', '0', '1', '0'],
-       '6',
-       7,
-       'Draw: 7',
-       [False, False, True, False, False, True, False, False, True, False],
-       [0, 0, -1, 0, 1, -2, 1, 1, 0, 1],
-       274892128276167031788079435153352244862),
-      ('Matthew Hall',
-       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
-       True,
-       ['0', '1', '0', '0', '3', '0', '0', '1', '0', '2'],
-       '7',
-       7,
-       'Draw: 7',
-       [True, True, False, True, True, False, True, True, False, True],
-       [0, 0, 1, 0, -1, 2, -1, -1, 0, -1],
-       274892128276167031788079435153352244862)]]
-
-
-
-```python
-event.get_flat_boxscores()[0]
+event.get_flat_boxscores(flat=True)
 ```
 
 
 
 
     [('Damien Villard',
       'event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1',
       True,
       ['0', '0', '0', '0', 'X'],
       '0',
       1,
       'Draw: 1',
       [True, True, True, True, True],
       [0, -1, -4, -6, -8],
-      227597408989477916004520082463493572762),
+      209707243860236114112314247393927711356),
      ('Matthew Hall',
       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
       False,
       ['1', '3', '2', '2', 'X'],
       '8',
       1,
       'Draw: 1',
       [False, False, False, False, False],
       [0, 1, 4, 6, 8],
-      227597408989477916004520082463493572762),
+      209707243860236114112314247393927711356),
      ('Matthew Mepstead',
       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144356#1',
       False,
       ['0', '0', '1', '1', '0', '1', '0', '0', '0', '1', '0'],
       '4',
       1,
       'Draw: 1',
       [False, False, True, False, False, True, False, False, False, True, False],
       [0, 0, -2, -1, 0, -1, 0, 0, 0, -1, 0],
-      230481195381514558834165699232540581342),
+      38537103347544582345141893615297919005),
      ('Tyler Stewart',
       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
       True,
       ['0', '2', '0', '0', '1', '0', '0', '0', '1', '0', '1'],
       '5',
       1,
       'Draw: 1',
       [True, True, False, True, True, False, True, True, True, False, True],
       [0, 0, 2, 1, 0, 1, 0, 0, 0, 1, 0],
-      230481195381514558834165699232540581342),
+      38537103347544582345141893615297919005),
      ('Jason March',
       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
       False,
       ['0', '2', '0', '1', '0', '2', '2', '0', '2', 'X'],
       '9',
       1,
       'Draw: 1',
       [False, False, False, False, False, True, False, False, True, False],
       [0, 0, 2, 2, 3, 2, 4, 6, 3, 5],
-      123876478142928441769100783560984935273),
+      272348649831484335603593027216985821953),
      ('Sam Steep',
       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144351&profileid=25978#1',
       True,
       ['0', '0', '0', '0', '1', '0', '0', '3', '0', 'X'],
       '4',
       1,
       'Draw: 1',
       [True, True, True, True, True, False, True, True, False, True],
       [0, 0, -2, -2, -3, -2, -4, -6, -3, -5],
-      123876478142928441769100783560984935273)]
-
-
-
-```python
-event.get_flat_boxscores()[-1]
-```
-
-
-
-
-    [('Tyler Stewart',
+      272348649831484335603593027216985821953),
+     ('Wayne Tuck Jr.',
+      'event.php?view=Team&eventid=6400&teamid=144353&profileid=12486#1',
+      True,
+      ['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'],
+      '5',
+      2,
+      'Draw: 2',
+      [True, True, False, True, True, True, True, False, False, False],
+      [0, 0, 2, -2, -2, -2, -3, -2, -1, 0],
+      95112284881200216258215191883153462659),
+     ('Matthew Hall',
+      'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+      False,
+      ['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'],
+      '7',
+      2,
+      'Draw: 2',
+      [False, False, True, False, False, False, False, True, True, True],
+      [0, 0, -2, 2, 2, 2, 3, 2, 1, 0],
+      95112284881200216258215191883153462659),
+     ('Dayna Deruelle',
+      'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144346&profileid=26636#1',
+      False,
+      ['0', '0', '1', '0', '0', '0', '0', 'X'],
+      '1',
+      2,
+      'Draw: 2',
+      [False, False, True, False, True, True, True, True],
+      [0, 0, -2, -1, -3, -4, -5, -9],
+      59643628877953807377369574857821892232),
+     ('Tyler Stewart',
+      'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
+      True,
+      ['0', '2', '0', '2', '1', '1', '4', 'X'],
+      '10',
+      2,
+      'Draw: 2',
+      [True, True, False, True, False, False, False, False],
+      [0, 0, 2, 1, 3, 4, 5, 9],
+      59643628877953807377369574857821892232),
+     ('Mark Kean',
+      'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
+      True,
+      ['2', '0', '1', '0', '0', '0', '1', '3', 'X'],
+      '7',
+      2,
+      'Draw: 2',
+      [True, False, False, False, False, True, True, False, False],
+      [0, 2, 2, 3, 3, 1, 0, 1, 4],
+      122217858840490332010920244446431255640),
+     ('Jason March',
+      'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
+      False,
+      ['0', '0', '0', '0', '2', '1', '0', '0', 'X'],
+      '3',
+      2,
+      'Draw: 2',
+      [False, True, True, True, True, False, False, True, True],
+      [0, -2, -2, -3, -3, -1, 0, -1, -4],
+      122217858840490332010920244446431255640),
+     ('Richard Krell',
+      'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144349&profileid=25962#1',
+      True,
+      ['2', '0', '1', '0', '2', '1', '1', 'X'],
+      '7',
+      2,
+      'Draw: 2',
+      [True, False, False, False, True, False, False, False],
+      [0, 2, 2, 3, 2, 4, 5, 6],
+      335702133606077232579627915311442373664),
+     ('Rob Ainsley',
+      'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
+      False,
+      ['0', '0', '0', '1', '0', '0', '0', 'X'],
+      '1',
+      2,
+      'Draw: 2',
+      [False, True, True, True, False, True, True, True],
+      [0, -2, -2, -3, -2, -4, -5, -6],
+      335702133606077232579627915311442373664),
+     ('Matthew Hall',
+      'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+      True,
+      ['0', '0', '2', '1', '2', '1', '0', '2', 'X'],
+      '8',
+      3,
+      'Draw: 3',
+      [True, True, True, False, False, False, False, True, False],
+      [0, 0, -1, 1, 2, 4, 5, 3, 5],
+      53772503334370441085334378293107653659),
+     ('Tyler Stewart',
+      'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
+      False,
+      ['0', '1', '0', '0', '0', '0', '2', '0', 'X'],
+      '3',
+      3,
+      'Draw: 3',
+      [False, False, False, True, True, True, True, False, True],
+      [0, 0, 1, -1, -2, -4, -5, -3, -5],
+      53772503334370441085334378293107653659),
+     ('Mark Kean',
+      'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
+      True,
+      ['0', '5', '0', '1', '1', '1', 'X'],
+      '8',
+      3,
+      'Draw: 3',
+      [True, True, False, True, False, False, False],
+      [0, -1, 4, 3, 4, 5, 6],
+      310456475955908017873561887016699672637),
+     ('Richard Krell',
+      'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144349&profileid=25962#1',
+      False,
+      ['1', '0', '1', '0', '0', '0', 'X'],
+      '2',
+      3,
+      'Draw: 3',
+      [False, False, True, False, True, True, True],
+      [0, 1, -4, -3, -4, -5, -6],
+      310456475955908017873561887016699672637),
+     ('Damien Villard',
+      'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144354&profileid=27373#1',
+      True,
+      ['2', '1', '0', '1', '0', '0', '1', '0', '0', '0'],
+      '5',
+      3,
+      'Draw: 3',
+      [True, False, False, True, False, True, True, False, True, True],
+      [0, 2, 3, 2, 3, 1, 1, 2, 1, 0],
+      303047434632680540438656592556261333287),
+     ('Sam Steep',
+      'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144351&profileid=25978#1',
+      False,
+      ['0', '0', '1', '0', '2', '0', '0', '1', '1', '1'],
+      '6',
+      3,
+      'Draw: 3',
+      [False, True, True, False, True, False, False, True, False, False],
+      [0, -2, -3, -2, -3, -1, -1, -2, -1, 0],
+      303047434632680540438656592556261333287),
+     ('Jason March',
+      'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144350#1',
+      True,
+      ['1', '1', '0', '0', '0', '0', '2', '1', '2', 'X'],
+      '7',
+      3,
+      'Draw: 3',
+      [True, False, False, True, True, True, True, False, False, False],
+      [0, 1, 2, 1, 0, 0, 0, 2, 3, 5],
+      229699058183107339172217417532449914369),
+     ('Matthew Mepstead',
+      'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144356#1',
+      False,
+      ['0', '0', '1', '1', '0', '0', '0', '0', '0', 'X'],
+      '2',
+      3,
+      'Draw: 3',
+      [False, True, True, False, False, False, False, True, True, True],
+      [0, -1, -2, -1, 0, 0, 0, -2, -3, -5],
+      229699058183107339172217417532449914369),
+     ('Wayne Tuck Jr.',
+      'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144353&profileid=12486#1',
+      False,
+      ['0', '0', '0', '2', '0', '0', '0', '0', 'X'],
+      '2',
+      3,
+      'Draw: 3',
+      [False, True, True, True, False, True, True, True, True],
+      [0, -2, -3, -3, -1, -2, -4, -5, -6],
+      195399470224611539512163135746754073908),
+     ('Rob Ainsley',
+      'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
+      True,
+      ['2', '1', '0', '0', '1', '2', '1', '1', 'X'],
+      '8',
+      3,
+      'Draw: 3',
+      [True, False, False, False, True, False, False, False, False],
+      [0, 2, 3, 3, 1, 2, 4, 5, 6],
+      195399470224611539512163135746754073908),
+     ('Matthew Hall',
+      'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+      True,
+      ['1', '0', '1', '0', '1', '0', '2', '0', '1', '0'],
+      '6',
+      4,
+      'Draw: 4',
+      [True, False, True, False, True, False, True, False, True, False],
+      [0, 1, -1, 0, -2, -1, -2, 0, -1, 0],
+      63653233024470732271264476184228625543),
+     ('Mark Kean',
+      'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961#1',
+      False,
+      ['0', '2', '0', '2', '0', '1', '0', '1', '0', '1'],
+      '7',
+      4,
+      'Draw: 4',
+      [False, True, False, True, False, True, False, True, False, True],
+      [0, -1, 1, 0, 2, 1, 2, 0, 1, 0],
+      63653233024470732271264476184228625543),
+     ('Sam Steep',
+      'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144351&profileid=25978#1',
+      False,
+      ['1', '0', '0', '2', '0', '1', '1', '0', '1', '1'],
+      '7',
+      4,
+      'Draw: 4',
+      [False, False, True, True, False, True, False, False, True, False],
+      [0, 1, 0, -2, 0, -2, -1, 0, -1, 0],
+      279469483516704960424550934244064693031),
+     ('Jason March',
+      'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144350#1',
+      True,
+      ['0', '1', '2', '0', '2', '0', '0', '1', '0', '0'],
+      '6',
+      4,
+      'Draw: 4',
+      [True, True, False, False, True, False, True, True, False, True],
+      [0, -1, 0, 2, 0, 2, 1, 0, 1, 0],
+      279469483516704960424550934244064693031),
+     ('Dayna Deruelle',
+      'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144346&profileid=26636#1',
+      False,
+      ['0', '2', '1', '1', '1', '0', '3', 'X'],
+      '8',
+      4,
+      'Draw: 4',
+      [False, True, False, False, False, False, True, False],
+      [0, -1, 1, 2, 3, 4, 3, 6],
+      291113397726148010907174443006816563924),
+     ('Rob Ainsley',
+      'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
+      True,
+      ['1', '0', '0', '0', '0', '1', '0', 'X'],
+      '2',
+      4,
+      'Draw: 4',
+      [True, False, True, True, True, True, False, True],
+      [0, 1, -1, -2, -3, -4, -3, -6],
+      291113397726148010907174443006816563924),
+     ('Sam Steep',
+      'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978#1',
+      False,
+      ['0', '1', '0', '0', '0', '2', '0', '2', '0', '0'],
+      '5',
+      5,
+      'Draw: 5',
+      [False, False, False, True, True, True, False, True, False, False],
+      [0, 0, 1, 0, -1, -3, -1, -3, -1, -1],
+      95866945533461342246819997703085723055),
+     ('Richard Krell',
+      'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1',
+      True,
+      ['0', '0', '1', '1', '2', '0', '2', '0', '0', '1'],
+      '7',
+      5,
+      'Draw: 5',
+      [True, True, True, False, False, False, True, False, True, True],
+      [0, 0, -1, 0, 1, 3, 1, 3, 1, 1],
+      95866945533461342246819997703085723055),
+     ('Dayna Deruelle',
+      'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144346&profileid=26636#1',
+      False,
+      ['0', '0', '1', '0', '0', '0', '1', '0', '3', '1', '0'],
+      '6',
+      5,
+      'Draw: 5',
+      [False, True, True, False, True, True, True, False, True, False, False],
+      [0, -1, -1, 0, -1, -1, -3, -2, -4, -1, 0],
+      233581897033627594667237538445333000951),
+     ('Tyler Stewart',
+      'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144352&profileid=12477#1',
+      True,
+      ['1', '0', '0', '1', '0', '2', '0', '2', '0', '0', '1'],
+      '7',
+      5,
+      'Draw: 5',
+      [True, False, False, True, False, False, False, True, False, True, True],
+      [0, 1, 1, 0, 1, 1, 3, 2, 4, 1, 0],
+      233581897033627594667237538445333000951),
+     ('Richard Krell',
+      'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1',
+      False,
+      ['0', '0', '1', '1', '0', '0', '1', '0', 'X'],
+      '3',
+      6,
+      'Draw: 6',
+      [False, False, True, False, False, True, True, False, True],
+      [0, 0, -2, -1, 0, -2, -5, -4, -5],
+      61203104491141348409761697458039616615),
+     ('Tyler Stewart',
+      'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
+      True,
+      ['0', '2', '0', '0', '2', '3', '0', '1', 'X'],
+      '8',
+      6,
+      'Draw: 6',
+      [True, True, False, True, True, False, False, True, False],
+      [0, 0, 2, 1, 0, 2, 5, 4, 5],
+      61203104491141348409761697458039616615),
+     ('Tyler Stewart',
       'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
       False,
       ['0', '0', '1', '1', '0', '3', '0', '0', '1', '0'],
       '6',
       7,
       'Draw: 7',
       [False, False, True, False, False, True, False, False, True, False],
       [0, 0, -1, 0, 1, -2, 1, 1, 0, 1],
-      274892128276167031788079435153352244862),
+      4915701019265174384644466584441738333),
      ('Matthew Hall',
       'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
       True,
       ['0', '1', '0', '0', '3', '0', '0', '1', '0', '2'],
       '7',
       7,
       'Draw: 7',
       [True, True, False, True, True, False, True, True, False, True],
       [0, 0, 1, 0, -1, 2, -1, -1, 0, -1],
-      274892128276167031788079435153352244862)]
+      4915701019265174384644466584441738333)]
+
+
+
+The `get_flat_boxscores` method can also be used to return a list of `Boxscore` objects for convenience. 
+
+```python
+event.get_flat_boxscores(flat=False)
+```
+
+
+
+
+    [Boxscore(team_name='Damien Villard', href='event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1', hammer_start=True, score=['0', '0', '0', '0', 'X'], final_score='0', draw_num=1, draw='Draw: 1', hammer_progression=[True, True, True, True, True], relative_score=[0, -1, -4, -6, -8], guid=209707243860236114112314247393927711356),
+     Boxscore(team_name='Matthew Hall', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', hammer_start=False, score=['1', '3', '2', '2', 'X'], final_score='8', draw_num=1, draw='Draw: 1', hammer_progression=[False, False, False, False, False], relative_score=[0, 1, 4, 6, 8], guid=209707243860236114112314247393927711356),
+     Boxscore(team_name='Matthew Mepstead', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144356#1', hammer_start=False, score=['0', '0', '1', '1', '0', '1', '0', '0', '0', '1', '0'], final_score='4', draw_num=1, draw='Draw: 1', hammer_progression=[False, False, True, False, False, True, False, False, False, True, False], relative_score=[0, 0, -2, -1, 0, -1, 0, 0, 0, -1, 0], guid=38537103347544582345141893615297919005),
+     Boxscore(team_name='Tyler Stewart', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1', hammer_start=True, score=['0', '2', '0', '0', '1', '0', '0', '0', '1', '0', '1'], final_score='5', draw_num=1, draw='Draw: 1', hammer_progression=[True, True, False, True, True, False, True, True, True, False, True], relative_score=[0, 0, 2, 1, 0, 1, 0, 0, 0, 1, 0], guid=38537103347544582345141893615297919005),
+     Boxscore(team_name='Jason March', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1', hammer_start=False, score=['0', '2', '0', '1', '0', '2', '2', '0', '2', 'X'], final_score='9', draw_num=1, draw='Draw: 1', hammer_progression=[False, False, False, False, False, True, False, False, True, False], relative_score=[0, 0, 2, 2, 3, 2, 4, 6, 3, 5], guid=272348649831484335603593027216985821953),
+     Boxscore(team_name='Sam Steep', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144351&profileid=25978#1', hammer_start=True, score=['0', '0', '0', '0', '1', '0', '0', '3', '0', 'X'], final_score='4', draw_num=1, draw='Draw: 1', hammer_progression=[True, True, True, True, True, False, True, True, False, True], relative_score=[0, 0, -2, -2, -3, -2, -4, -6, -3, -5], guid=272348649831484335603593027216985821953),
+     Boxscore(team_name='Wayne Tuck Jr.', href='event.php?view=Team&eventid=6400&teamid=144353&profileid=12486#1', hammer_start=True, score=['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'], final_score='5', draw_num=2, draw='Draw: 2', hammer_progression=[True, True, False, True, True, True, True, False, False, False], relative_score=[0, 0, 2, -2, -2, -2, -3, -2, -1, 0], guid=95112284881200216258215191883153462659),
+     Boxscore(team_name='Matthew Hall', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', hammer_start=False, score=['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'], final_score='7', draw_num=2, draw='Draw: 2', hammer_progression=[False, False, True, False, False, False, False, True, True, True], relative_score=[0, 0, -2, 2, 2, 2, 3, 2, 1, 0], guid=95112284881200216258215191883153462659),
+     Boxscore(team_name='Dayna Deruelle', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144346&profileid=26636#1', hammer_start=False, score=['0', '0', '1', '0', '0', '0', '0', 'X'], final_score='1', draw_num=2, draw='Draw: 2', hammer_progression=[False, False, True, False, True, True, True, True], relative_score=[0, 0, -2, -1, -3, -4, -5, -9], guid=59643628877953807377369574857821892232),
+     Boxscore(team_name='Tyler Stewart', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1', hammer_start=True, score=['0', '2', '0', '2', '1', '1', '4', 'X'], final_score='10', draw_num=2, draw='Draw: 2', hammer_progression=[True, True, False, True, False, False, False, False], relative_score=[0, 0, 2, 1, 3, 4, 5, 9], guid=59643628877953807377369574857821892232),
+     Boxscore(team_name='Mark Kean', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1', hammer_start=True, score=['2', '0', '1', '0', '0', '0', '1', '3', 'X'], final_score='7', draw_num=2, draw='Draw: 2', hammer_progression=[True, False, False, False, False, True, True, False, False], relative_score=[0, 2, 2, 3, 3, 1, 0, 1, 4], guid=122217858840490332010920244446431255640),
+     Boxscore(team_name='Jason March', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1', hammer_start=False, score=['0', '0', '0', '0', '2', '1', '0', '0', 'X'], final_score='3', draw_num=2, draw='Draw: 2', hammer_progression=[False, True, True, True, True, False, False, True, True], relative_score=[0, -2, -2, -3, -3, -1, 0, -1, -4], guid=122217858840490332010920244446431255640),
+     Boxscore(team_name='Richard Krell', href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144349&profileid=25962#1', hammer_start=True, score=['2', '0', '1', '0', '2', '1', '1', 'X'], final_score='7', draw_num=2, draw='Draw: 2', hammer_progression=[True, False, False, False, True, False, False, False], relative_score=[0, 2, 2, 3, 2, 4, 5, 6], guid=335702133606077232579627915311442373664),
+     Boxscore(team_name='Rob Ainsley', href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1', hammer_start=False, score=['0', '0', '0', '1', '0', '0', '0', 'X'], final_score='1', draw_num=2, draw='Draw: 2', hammer_progression=[False, True, True, True, False, True, True, True], relative_score=[0, -2, -2, -3, -2, -4, -5, -6], guid=335702133606077232579627915311442373664),
+     Boxscore(team_name='Matthew Hall', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', hammer_start=True, score=['0', '0', '2', '1', '2', '1', '0', '2', 'X'], final_score='8', draw_num=3, draw='Draw: 3', hammer_progression=[True, True, True, False, False, False, False, True, False], relative_score=[0, 0, -1, 1, 2, 4, 5, 3, 5], guid=53772503334370441085334378293107653659),
+     Boxscore(team_name='Tyler Stewart', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1', hammer_start=False, score=['0', '1', '0', '0', '0', '0', '2', '0', 'X'], final_score='3', draw_num=3, draw='Draw: 3', hammer_progression=[False, False, False, True, True, True, True, False, True], relative_score=[0, 0, 1, -1, -2, -4, -5, -3, -5], guid=53772503334370441085334378293107653659),
+     Boxscore(team_name='Mark Kean', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1', hammer_start=True, score=['0', '5', '0', '1', '1', '1', 'X'], final_score='8', draw_num=3, draw='Draw: 3', hammer_progression=[True, True, False, True, False, False, False], relative_score=[0, -1, 4, 3, 4, 5, 6], guid=310456475955908017873561887016699672637),
+     Boxscore(team_name='Richard Krell', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144349&profileid=25962#1', hammer_start=False, score=['1', '0', '1', '0', '0', '0', 'X'], final_score='2', draw_num=3, draw='Draw: 3', hammer_progression=[False, False, True, False, True, True, True], relative_score=[0, 1, -4, -3, -4, -5, -6], guid=310456475955908017873561887016699672637),
+     Boxscore(team_name='Damien Villard', href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144354&profileid=27373#1', hammer_start=True, score=['2', '1', '0', '1', '0', '0', '1', '0', '0', '0'], final_score='5', draw_num=3, draw='Draw: 3', hammer_progression=[True, False, False, True, False, True, True, False, True, True], relative_score=[0, 2, 3, 2, 3, 1, 1, 2, 1, 0], guid=303047434632680540438656592556261333287),
+     Boxscore(team_name='Sam Steep', href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144351&profileid=25978#1', hammer_start=False, score=['0', '0', '1', '0', '2', '0', '0', '1', '1', '1'], final_score='6', draw_num=3, draw='Draw: 3', hammer_progression=[False, True, True, False, True, False, False, True, False, False], relative_score=[0, -2, -3, -2, -3, -1, -1, -2, -1, 0], guid=303047434632680540438656592556261333287),
+     Boxscore(team_name='Jason March', href='event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144350#1', hammer_start=True, score=['1', '1', '0', '0', '0', '0', '2', '1', '2', 'X'], final_score='7', draw_num=3, draw='Draw: 3', hammer_progression=[True, False, False, True, True, True, True, False, False, False], relative_score=[0, 1, 2, 1, 0, 0, 0, 2, 3, 5], guid=229699058183107339172217417532449914369),
+     Boxscore(team_name='Matthew Mepstead', href='event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144356#1', hammer_start=False, score=['0', '0', '1', '1', '0', '0', '0', '0', '0', 'X'], final_score='2', draw_num=3, draw='Draw: 3', hammer_progression=[False, True, True, False, False, False, False, True, True, True], relative_score=[0, -1, -2, -1, 0, 0, 0, -2, -3, -5], guid=229699058183107339172217417532449914369),
+     Boxscore(team_name='Wayne Tuck Jr.', href='event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144353&profileid=12486#1', hammer_start=False, score=['0', '0', '0', '2', '0', '0', '0', '0', 'X'], final_score='2', draw_num=3, draw='Draw: 3', hammer_progression=[False, True, True, True, False, True, True, True, True], relative_score=[0, -2, -3, -3, -1, -2, -4, -5, -6], guid=195399470224611539512163135746754073908),
+     Boxscore(team_name='Rob Ainsley', href='event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144345&profileid=15779#1', hammer_start=True, score=['2', '1', '0', '0', '1', '2', '1', '1', 'X'], final_score='8', draw_num=3, draw='Draw: 3', hammer_progression=[True, False, False, False, True, False, False, False, False], relative_score=[0, 2, 3, 3, 1, 2, 4, 5, 6], guid=195399470224611539512163135746754073908),
+     Boxscore(team_name='Matthew Hall', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', hammer_start=True, score=['1', '0', '1', '0', '1', '0', '2', '0', '1', '0'], final_score='6', draw_num=4, draw='Draw: 4', hammer_progression=[True, False, True, False, True, False, True, False, True, False], relative_score=[0, 1, -1, 0, -2, -1, -2, 0, -1, 0], guid=63653233024470732271264476184228625543),
+     Boxscore(team_name='Mark Kean', href='event.php?view=Team&eventid=6400&teamid=144348&profileid=25961#1', hammer_start=False, score=['0', '2', '0', '2', '0', '1', '0', '1', '0', '1'], final_score='7', draw_num=4, draw='Draw: 4', hammer_progression=[False, True, False, True, False, True, False, True, False, True], relative_score=[0, -1, 1, 0, 2, 1, 2, 0, 1, 0], guid=63653233024470732271264476184228625543),
+     Boxscore(team_name='Sam Steep', href='event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144351&profileid=25978#1', hammer_start=False, score=['1', '0', '0', '2', '0', '1', '1', '0', '1', '1'], final_score='7', draw_num=4, draw='Draw: 4', hammer_progression=[False, False, True, True, False, True, False, False, True, False], relative_score=[0, 1, 0, -2, 0, -2, -1, 0, -1, 0], guid=279469483516704960424550934244064693031),
+     Boxscore(team_name='Jason March', href='event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144350#1', hammer_start=True, score=['0', '1', '2', '0', '2', '0', '0', '1', '0', '0'], final_score='6', draw_num=4, draw='Draw: 4', hammer_progression=[True, True, False, False, True, False, True, True, False, True], relative_score=[0, -1, 0, 2, 0, 2, 1, 0, 1, 0], guid=279469483516704960424550934244064693031),
+     Boxscore(team_name='Dayna Deruelle', href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144346&profileid=26636#1', hammer_start=False, score=['0', '2', '1', '1', '1', '0', '3', 'X'], final_score='8', draw_num=4, draw='Draw: 4', hammer_progression=[False, True, False, False, False, False, True, False], relative_score=[0, -1, 1, 2, 3, 4, 3, 6], guid=291113397726148010907174443006816563924),
+     Boxscore(team_name='Rob Ainsley', href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1', hammer_start=True, score=['1', '0', '0', '0', '0', '1', '0', 'X'], final_score='2', draw_num=4, draw='Draw: 4', hammer_progression=[True, False, True, True, True, True, False, True], relative_score=[0, 1, -1, -2, -3, -4, -3, -6], guid=291113397726148010907174443006816563924),
+     Boxscore(team_name='Sam Steep', href='event.php?view=Team&eventid=6400&teamid=144351&profileid=25978#1', hammer_start=False, score=['0', '1', '0', '0', '0', '2', '0', '2', '0', '0'], final_score='5', draw_num=5, draw='Draw: 5', hammer_progression=[False, False, False, True, True, True, False, True, False, False], relative_score=[0, 0, 1, 0, -1, -3, -1, -3, -1, -1], guid=95866945533461342246819997703085723055),
+     Boxscore(team_name='Richard Krell', href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1', hammer_start=True, score=['0', '0', '1', '1', '2', '0', '2', '0', '0', '1'], final_score='7', draw_num=5, draw='Draw: 5', hammer_progression=[True, True, True, False, False, False, True, False, True, True], relative_score=[0, 0, -1, 0, 1, 3, 1, 3, 1, 1], guid=95866945533461342246819997703085723055),
+     Boxscore(team_name='Dayna Deruelle', href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144346&profileid=26636#1', hammer_start=False, score=['0', '0', '1', '0', '0', '0', '1', '0', '3', '1', '0'], final_score='6', draw_num=5, draw='Draw: 5', hammer_progression=[False, True, True, False, True, True, True, False, True, False, False], relative_score=[0, -1, -1, 0, -1, -1, -3, -2, -4, -1, 0], guid=233581897033627594667237538445333000951),
+     Boxscore(team_name='Tyler Stewart', href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144352&profileid=12477#1', hammer_start=True, score=['1', '0', '0', '1', '0', '2', '0', '2', '0', '0', '1'], final_score='7', draw_num=5, draw='Draw: 5', hammer_progression=[True, False, False, True, False, False, False, True, False, True, True], relative_score=[0, 1, 1, 0, 1, 1, 3, 2, 4, 1, 0], guid=233581897033627594667237538445333000951),
+     Boxscore(team_name='Richard Krell', href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1', hammer_start=False, score=['0', '0', '1', '1', '0', '0', '1', '0', 'X'], final_score='3', draw_num=6, draw='Draw: 6', hammer_progression=[False, False, True, False, False, True, True, False, True], relative_score=[0, 0, -2, -1, 0, -2, -5, -4, -5], guid=61203104491141348409761697458039616615),
+     Boxscore(team_name='Tyler Stewart', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1', hammer_start=True, score=['0', '2', '0', '0', '2', '3', '0', '1', 'X'], final_score='8', draw_num=6, draw='Draw: 6', hammer_progression=[True, True, False, True, True, False, False, True, False], relative_score=[0, 0, 2, 1, 0, 2, 5, 4, 5], guid=61203104491141348409761697458039616615),
+     Boxscore(team_name='Tyler Stewart', href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1', hammer_start=False, score=['0', '0', '1', '1', '0', '3', '0', '0', '1', '0'], final_score='6', draw_num=7, draw='Draw: 7', hammer_progression=[False, False, True, False, False, True, False, False, True, False], relative_score=[0, 0, -1, 0, 1, -2, 1, 1, 0, 1], guid=4915701019265174384644466584441738333),
+     Boxscore(team_name='Matthew Hall', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', hammer_start=True, score=['0', '1', '0', '0', '3', '0', '0', '1', '0', '2'], final_score='7', draw_num=7, draw='Draw: 7', hammer_progression=[True, True, False, True, True, False, True, True, False, True], relative_score=[0, 0, 1, 0, -1, 2, -1, -1, 0, -1], guid=4915701019265174384644466584441738333)]
+
+
+
+```python
+event.get_flat_boxscores()[0]
+```
+
+
+
+
+    Boxscore(team_name='Damien Villard', href='event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1', hammer_start=True, score=['0', '0', '0', '0', 'X'], final_score='0', draw_num=1, draw='Draw: 1', hammer_progression=[True, True, True, True, True], relative_score=[0, -1, -4, -6, -8], guid=209707243860236114112314247393927711356)
+
+
+
+```python
+event.get_flat_boxscores()[-1]
+```
+
+
+
+
+    Boxscore(team_name='Matthew Hall', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', hammer_start=True, score=['0', '1', '0', '0', '3', '0', '0', '1', '0', '2'], final_score='7', draw_num=7, draw='Draw: 7', hammer_progression=[True, True, False, True, True, False, True, True, False, True], relative_score=[0, 0, 1, 0, -1, 2, -1, -1, 0, -1], guid=4915701019265174384644466584441738333)
 
 
 
 ## About czapi
 czapi is a Python library for scraping curling linescores.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: czapi Version: 0.1.9 Summary: CurlingZone scraper
+Metadata-Version: 2.1 Name: czapi Version: 0.2.0 Summary: CurlingZone scraper
 API. Home-page: https://github.com/calicorob/czapi/tree/master/ Author: Robert
 Currie Author-email: robert.art.currie@gmail.com License: Apache Software
 License 2.0 Keywords: curling,stats Platform: UNKNOWN Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: License :: OSI Approved :: Apache
@@ -101,53 +101,53 @@
 True, False, False, False, False, True, True, True], normalized_score=[0, 0, -
 2, 2, 2, 2, 3, 2, 1, 0]) For Matthew Hall, the `normalized_score` attribute can
 be interpreted as follows: * The score was tied in the first end (obviously). *
 The score was tied in the second end. * In the 3rd end, Matthew was down 2. *
 In the 4th end, Matthew was up 2 after taking 4. * And so on and so forth..
 You'll also notice the `NormalizedBoxscore` object has a guid property which
 identifies that two `NormalizedHalfBoxscore` belong to the same game. ```python
-normalized_boxscore.guid ``` 154352576001077780910640079893588160113 czapi's
+normalized_boxscore.guid ``` 129690655252279755696295239689104705205 czapi's
 `get_flat_boxscores_from` function takes a `cz_event_id` and `cz_draw_id` as an
 arguments and returns a (flat) nested list object of all the boxscore
 information on the linescore page. This nested list object can be ingested into
 a pandas DataFrame or pushed to a SQL database. ```python
 api.get_flat_boxscores_from(cz_event_id = 6400, cz_draw_id = 2) ``` [('Wayne
 Tuck Jr.', 'event.php?view=Team&eventid=6400&teamid=144353&profileid=12486#1',
 True, ['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'], '5', 2, 'Draw: 2',
 [True, True, False, True, True, True, True, False, False, False], [0, 0, 2, -2,
--2, -2, -3, -2, -1, 0], 306528221620467227442052913955328486003), ('Matthew
+-2, -2, -3, -2, -1, 0], 296656328202528204780428618855733007061), ('Matthew
 Hall', 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
 False, ['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'], '7', 2, 'Draw: 2',
 [False, False, True, False, False, False, False, True, True, True], [0, 0, -2,
-2, 2, 2, 3, 2, 1, 0], 306528221620467227442052913955328486003), ('Dayna
+2, 2, 2, 3, 2, 1, 0], 296656328202528204780428618855733007061), ('Dayna
 Deruelle',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144346&profileid=26636#1',
 False, ['0', '0', '1', '0', '0', '0', '0', 'X'], '1', 2, 'Draw: 2', [False,
 False, True, False, True, True, True, True], [0, 0, -2, -1, -3, -4, -5, -9],
-169959036371998794200683443427801286021), ('Tyler Stewart',
+105249071225393527432485074456849437076), ('Tyler Stewart',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
 True, ['0', '2', '0', '2', '1', '1', '4', 'X'], '10', 2, 'Draw: 2', [True,
 True, False, True, False, False, False, False], [0, 0, 2, 1, 3, 4, 5, 9],
-169959036371998794200683443427801286021), ('Mark Kean',
+105249071225393527432485074456849437076), ('Mark Kean',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
 True, ['2', '0', '1', '0', '0', '0', '1', '3', 'X'], '7', 2, 'Draw: 2', [True,
 False, False, False, False, True, True, False, False], [0, 2, 2, 3, 3, 1, 0, 1,
-4], 216723633949199876308042205365369844269), ('Jason March',
+4], 17103980631020054974876512539607901632), ('Jason March',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
 False, ['0', '0', '0', '0', '2', '1', '0', '0', 'X'], '3', 2, 'Draw: 2',
 [False, True, True, True, True, False, False, True, True], [0, -2, -2, -3, -3,
--1, 0, -1, -4], 216723633949199876308042205365369844269), ('Richard Krell',
+-1, 0, -1, -4], 17103980631020054974876512539607901632), ('Richard Krell',
 'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144349&profileid=25962#1',
 True, ['2', '0', '1', '0', '2', '1', '1', 'X'], '7', 2, 'Draw: 2', [True,
 False, False, False, True, False, False, False], [0, 2, 2, 3, 2, 4, 5, 6],
-142335171424399828625133635146510278418), ('Rob Ainsley',
+215489388707487834967933616755032135426), ('Rob Ainsley',
 'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
 False, ['0', '0', '0', '1', '0', '0', '0', 'X'], '1', 2, 'Draw: 2', [False,
 True, True, True, False, True, True, True], [0, -2, -2, -3, -2, -4, -5, -6],
-142335171424399828625133635146510278418)] ## Event The `Event` object is a data
+215489388707487834967933616755032135426)] ## Event The `Event` object is a data
 structure which holds all of the `LinescorePage` objects which make up an
 entire event. An `Event` instance is created by passing a `cz_event_id`.
 ```python event = api.Event(cz_event_id = 6400,delay=3,verbose=True) event ```
 Scraping draw 1. Scraping draw 2. Scraping draw 3. Scraping draw 4. Scraping
 draw 5. Scraping draw 6. Scraping draw 7. Event(cz_event_id=6400, delay=3,
 verbose=True) The created `Event` objects holds all the `LinescorePage` objects
 in it's `pages` property. ```python event.pages ``` [LinescorePage
@@ -187,205 +187,413 @@
 'href':
 'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144353&profileid=12486#1',
 'score': ['0', '0', '0', '2', '0', '0', '0', '0', 'X'], 'hammer': False,
 'finalscore': '2'}, 'Rob Ainsley': {'draw': 'Draw: 3', 'draw_num': 3, 'href':
 'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
 'score': ['2', '1', '0', '0', '1', '2', '1', '1', 'X'], 'hammer': True,
 'finalscore': '8'}}] The `get_flat_boxscores` method can be used to return a
-list of (flat) nested list object of all the boxscore information on all the
-linescore pages. ```python event.get_flat_boxscores() ``` [[('Damien Villard',
+list of tuples of all the boxscore information on all the linescore pages.
+```python event.get_flat_boxscores(flat=True) ``` [('Damien Villard',
 'event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1', True, ['0',
 '0', '0', '0', 'X'], '0', 1, 'Draw: 1', [True, True, True, True, True], [0, -1,
--4, -6, -8], 227597408989477916004520082463493572762), ('Matthew Hall',
+-4, -6, -8], 209707243860236114112314247393927711356), ('Matthew Hall',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', False,
 ['1', '3', '2', '2', 'X'], '8', 1, 'Draw: 1', [False, False, False, False,
-False], [0, 1, 4, 6, 8], 227597408989477916004520082463493572762), ('Matthew
+False], [0, 1, 4, 6, 8], 209707243860236114112314247393927711356), ('Matthew
 Mepstead',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144356#1',
 False, ['0', '0', '1', '1', '0', '1', '0', '0', '0', '1', '0'], '4', 1, 'Draw:
 1', [False, False, True, False, False, True, False, False, False, True, False],
-[0, 0, -2, -1, 0, -1, 0, 0, 0, -1, 0],
-230481195381514558834165699232540581342), ('Tyler Stewart',
+[0, 0, -2, -1, 0, -1, 0, 0, 0, -1, 0], 38537103347544582345141893615297919005),
+('Tyler Stewart',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
 True, ['0', '2', '0', '0', '1', '0', '0', '0', '1', '0', '1'], '5', 1, 'Draw:
 1', [True, True, False, True, True, False, True, True, True, False, True], [0,
-0, 2, 1, 0, 1, 0, 0, 0, 1, 0], 230481195381514558834165699232540581342),
-('Jason March',
+0, 2, 1, 0, 1, 0, 0, 0, 1, 0], 38537103347544582345141893615297919005), ('Jason
+March',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
 False, ['0', '2', '0', '1', '0', '2', '2', '0', '2', 'X'], '9', 1, 'Draw: 1',
 [False, False, False, False, False, True, False, False, True, False], [0, 0, 2,
-2, 3, 2, 4, 6, 3, 5], 123876478142928441769100783560984935273), ('Sam Steep',
+2, 3, 2, 4, 6, 3, 5], 272348649831484335603593027216985821953), ('Sam Steep',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144351&profileid=25978#1',
 True, ['0', '0', '0', '0', '1', '0', '0', '3', '0', 'X'], '4', 1, 'Draw: 1',
 [True, True, True, True, True, False, True, True, False, True], [0, 0, -2, -2,
--3, -2, -4, -6, -3, -5], 123876478142928441769100783560984935273)], [('Wayne
-Tuck Jr.', 'event.php?view=Team&eventid=6400&teamid=144353&profileid=12486#1',
-True, ['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'], '5', 2, 'Draw: 2',
-[True, True, False, True, True, True, True, False, False, False], [0, 0, 2, -2,
--2, -2, -3, -2, -1, 0], 309985127892547751219643103116568617832), ('Matthew
-Hall', 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
-False, ['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'], '7', 2, 'Draw: 2',
-[False, False, True, False, False, False, False, True, True, True], [0, 0, -2,
-2, 2, 2, 3, 2, 1, 0], 309985127892547751219643103116568617832), ('Dayna
-Deruelle',
+-3, -2, -4, -6, -3, -5], 272348649831484335603593027216985821953), ('Wayne Tuck
+Jr.', 'event.php?view=Team&eventid=6400&teamid=144353&profileid=12486#1', True,
+['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'], '5', 2, 'Draw: 2', [True,
+True, False, True, True, True, True, False, False, False], [0, 0, 2, -2, -2, -
+2, -3, -2, -1, 0], 95112284881200216258215191883153462659), ('Matthew Hall',
+'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', False,
+['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'], '7', 2, 'Draw: 2', [False,
+False, True, False, False, False, False, True, True, True], [0, 0, -2, 2, 2, 2,
+3, 2, 1, 0], 95112284881200216258215191883153462659), ('Dayna Deruelle',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144346&profileid=26636#1',
 False, ['0', '0', '1', '0', '0', '0', '0', 'X'], '1', 2, 'Draw: 2', [False,
 False, True, False, True, True, True, True], [0, 0, -2, -1, -3, -4, -5, -9],
-258827556868852829922619663221573707805), ('Tyler Stewart',
+59643628877953807377369574857821892232), ('Tyler Stewart',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
 True, ['0', '2', '0', '2', '1', '1', '4', 'X'], '10', 2, 'Draw: 2', [True,
 True, False, True, False, False, False, False], [0, 0, 2, 1, 3, 4, 5, 9],
-258827556868852829922619663221573707805), ('Mark Kean',
+59643628877953807377369574857821892232), ('Mark Kean',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
 True, ['2', '0', '1', '0', '0', '0', '1', '3', 'X'], '7', 2, 'Draw: 2', [True,
 False, False, False, False, True, True, False, False], [0, 2, 2, 3, 3, 1, 0, 1,
-4], 196156262752898539339442275025527127066), ('Jason March',
+4], 122217858840490332010920244446431255640), ('Jason March',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
 False, ['0', '0', '0', '0', '2', '1', '0', '0', 'X'], '3', 2, 'Draw: 2',
 [False, True, True, True, True, False, False, True, True], [0, -2, -2, -3, -3,
--1, 0, -1, -4], 196156262752898539339442275025527127066), ('Richard Krell',
+-1, 0, -1, -4], 122217858840490332010920244446431255640), ('Richard Krell',
 'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144349&profileid=25962#1',
 True, ['2', '0', '1', '0', '2', '1', '1', 'X'], '7', 2, 'Draw: 2', [True,
 False, False, False, True, False, False, False], [0, 2, 2, 3, 2, 4, 5, 6],
-121058110285022966689701916848012130324), ('Rob Ainsley',
+335702133606077232579627915311442373664), ('Rob Ainsley',
 'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
 False, ['0', '0', '0', '1', '0', '0', '0', 'X'], '1', 2, 'Draw: 2', [False,
 True, True, True, False, True, True, True], [0, -2, -2, -3, -2, -4, -5, -6],
-121058110285022966689701916848012130324)], [('Matthew Hall',
+335702133606077232579627915311442373664), ('Matthew Hall',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', True, ['0',
 '0', '2', '1', '2', '1', '0', '2', 'X'], '8', 3, 'Draw: 3', [True, True, True,
 False, False, False, False, True, False], [0, 0, -1, 1, 2, 4, 5, 3, 5],
-167908611678356344738885531672086035216), ('Tyler Stewart',
+53772503334370441085334378293107653659), ('Tyler Stewart',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1', False,
 ['0', '1', '0', '0', '0', '0', '2', '0', 'X'], '3', 3, 'Draw: 3', [False,
 False, False, True, True, True, True, False, True], [0, 0, 1, -1, -2, -4, -5, -
-3, -5], 167908611678356344738885531672086035216), ('Mark Kean',
+3, -5], 53772503334370441085334378293107653659), ('Mark Kean',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
 True, ['0', '5', '0', '1', '1', '1', 'X'], '8', 3, 'Draw: 3', [True, True,
 False, True, False, False, False], [0, -1, 4, 3, 4, 5, 6],
-157383102330203138325358878297425755857), ('Richard Krell',
+310456475955908017873561887016699672637), ('Richard Krell',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144349&profileid=25962#1',
 False, ['1', '0', '1', '0', '0', '0', 'X'], '2', 3, 'Draw: 3', [False, False,
 True, False, True, True, True], [0, 1, -4, -3, -4, -5, -6],
-157383102330203138325358878297425755857), ('Damien Villard',
+310456475955908017873561887016699672637), ('Damien Villard',
 'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144354&profileid=27373#1',
 True, ['2', '1', '0', '1', '0', '0', '1', '0', '0', '0'], '5', 3, 'Draw: 3',
 [True, False, False, True, False, True, True, False, True, True], [0, 2, 3, 2,
-3, 1, 1, 2, 1, 0], 197764335276159882538274022024920645468), ('Sam Steep',
+3, 1, 1, 2, 1, 0], 303047434632680540438656592556261333287), ('Sam Steep',
 'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144351&profileid=25978#1',
 False, ['0', '0', '1', '0', '2', '0', '0', '1', '1', '1'], '6', 3, 'Draw: 3',
 [False, True, True, False, True, False, False, True, False, False], [0, -2, -3,
--2, -3, -1, -1, -2, -1, 0], 197764335276159882538274022024920645468), ('Jason
+-2, -3, -1, -1, -2, -1, 0], 303047434632680540438656592556261333287), ('Jason
 March',
 'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144350#1',
 True, ['1', '1', '0', '0', '0', '0', '2', '1', '2', 'X'], '7', 3, 'Draw: 3',
 [True, False, False, True, True, True, True, False, False, False], [0, 1, 2, 1,
-0, 0, 0, 2, 3, 5], 19248089004956668591585521441771100702), ('Matthew
+0, 0, 0, 2, 3, 5], 229699058183107339172217417532449914369), ('Matthew
 Mepstead',
 'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144356#1',
 False, ['0', '0', '1', '1', '0', '0', '0', '0', '0', 'X'], '2', 3, 'Draw: 3',
 [False, True, True, False, False, False, False, True, True, True], [0, -1, -2,
--1, 0, 0, 0, -2, -3, -5], 19248089004956668591585521441771100702), ('Wayne Tuck
-Jr.',
+-1, 0, 0, 0, -2, -3, -5], 229699058183107339172217417532449914369), ('Wayne
+Tuck Jr.',
 'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144353&profileid=12486#1',
 False, ['0', '0', '0', '2', '0', '0', '0', '0', 'X'], '2', 3, 'Draw: 3',
 [False, True, True, True, False, True, True, True, True], [0, -2, -3, -3, -1, -
-2, -4, -5, -6], 152642289275163622503053683522534226102), ('Rob Ainsley',
+2, -4, -5, -6], 195399470224611539512163135746754073908), ('Rob Ainsley',
 'event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
 True, ['2', '1', '0', '0', '1', '2', '1', '1', 'X'], '8', 3, 'Draw: 3', [True,
 False, False, False, True, False, False, False, False], [0, 2, 3, 3, 1, 2, 4,
-5, 6], 152642289275163622503053683522534226102)], [('Matthew Hall',
+5, 6], 195399470224611539512163135746754073908), ('Matthew Hall',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', True, ['1',
 '0', '1', '0', '1', '0', '2', '0', '1', '0'], '6', 4, 'Draw: 4', [True, False,
 True, False, True, False, True, False, True, False], [0, 1, -1, 0, -2, -1, -2,
-0, -1, 0], 128520251865367755000080630810739466709), ('Mark Kean',
+0, -1, 0], 63653233024470732271264476184228625543), ('Mark Kean',
 'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961#1', False,
 ['0', '2', '0', '2', '0', '1', '0', '1', '0', '1'], '7', 4, 'Draw: 4', [False,
 True, False, True, False, True, False, True, False, True], [0, -1, 1, 0, 2, 1,
-2, 0, 1, 0], 128520251865367755000080630810739466709), ('Sam Steep',
+2, 0, 1, 0], 63653233024470732271264476184228625543), ('Sam Steep',
 'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144351&profileid=25978#1',
 False, ['1', '0', '0', '2', '0', '1', '1', '0', '1', '1'], '7', 4, 'Draw: 4',
 [False, False, True, True, False, True, False, False, True, False], [0, 1, 0, -
-2, 0, -2, -1, 0, -1, 0], 164045326452654642850026023480637847801), ('Jason
+2, 0, -2, -1, 0, -1, 0], 279469483516704960424550934244064693031), ('Jason
 March',
 'event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144350#1',
 True, ['0', '1', '2', '0', '2', '0', '0', '1', '0', '0'], '6', 4, 'Draw: 4',
 [True, True, False, False, True, False, True, True, False, True], [0, -1, 0, 2,
-0, 2, 1, 0, 1, 0], 164045326452654642850026023480637847801), ('Dayna Deruelle',
+0, 2, 1, 0, 1, 0], 279469483516704960424550934244064693031), ('Dayna Deruelle',
 'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144346&profileid=26636#1',
 False, ['0', '2', '1', '1', '1', '0', '3', 'X'], '8', 4, 'Draw: 4', [False,
 True, False, False, False, False, True, False], [0, -1, 1, 2, 3, 4, 3, 6],
-76792983814886196713410396043046633915), ('Rob Ainsley',
+291113397726148010907174443006816563924), ('Rob Ainsley',
 'event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
 True, ['1', '0', '0', '0', '0', '1', '0', 'X'], '2', 4, 'Draw: 4', [True,
 False, True, True, True, True, False, True], [0, 1, -1, -2, -3, -4, -3, -6],
-76792983814886196713410396043046633915)], [('Sam Steep',
+291113397726148010907174443006816563924), ('Sam Steep',
 'event.php?view=Team&eventid=6400&teamid=144351&profileid=25978#1', False,
 ['0', '1', '0', '0', '0', '2', '0', '2', '0', '0'], '5', 5, 'Draw: 5', [False,
 False, False, True, True, True, False, True, False, False], [0, 0, 1, 0, -1, -
-3, -1, -3, -1, -1], 38480930669174444566426826324563146081), ('Richard Krell',
+3, -1, -3, -1, -1], 95866945533461342246819997703085723055), ('Richard Krell',
 'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1', True, ['0',
 '0', '1', '1', '2', '0', '2', '0', '0', '1'], '7', 5, 'Draw: 5', [True, True,
 True, False, False, False, True, False, True, True], [0, 0, -1, 0, 1, 3, 1, 3,
-1, 1], 38480930669174444566426826324563146081), ('Dayna Deruelle',
+1, 1], 95866945533461342246819997703085723055), ('Dayna Deruelle',
 'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144346&profileid=26636#1',
 False, ['0', '0', '1', '0', '0', '0', '1', '0', '3', '1', '0'], '6', 5, 'Draw:
 5', [False, True, True, False, True, True, True, False, True, False, False],
 [0, -1, -1, 0, -1, -1, -3, -2, -4, -1, 0],
-153896726080791122415283970396986089830), ('Tyler Stewart',
+233581897033627594667237538445333000951), ('Tyler Stewart',
 'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144352&profileid=12477#1',
 True, ['1', '0', '0', '1', '0', '2', '0', '2', '0', '0', '1'], '7', 5, 'Draw:
 5', [True, False, False, True, False, False, False, True, False, True, True],
-[0, 1, 1, 0, 1, 1, 3, 2, 4, 1, 0], 153896726080791122415283970396986089830)], [
+[0, 1, 1, 0, 1, 1, 3, 2, 4, 1, 0], 233581897033627594667237538445333000951),
 ('Richard Krell',
 'event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1', False,
 ['0', '0', '1', '1', '0', '0', '1', '0', 'X'], '3', 6, 'Draw: 6', [False,
 False, True, False, False, True, True, False, True], [0, 0, -2, -1, 0, -2, -5,
--4, -5], 209637313717849892067917714730669554285), ('Tyler Stewart',
+-4, -5], 61203104491141348409761697458039616615), ('Tyler Stewart',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1', True, ['0',
 '2', '0', '0', '2', '3', '0', '1', 'X'], '8', 6, 'Draw: 6', [True, True, False,
 True, True, False, False, True, False], [0, 0, 2, 1, 0, 2, 5, 4, 5],
-209637313717849892067917714730669554285)], [('Tyler Stewart',
+61203104491141348409761697458039616615), ('Tyler Stewart',
 'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1', False,
 ['0', '0', '1', '1', '0', '3', '0', '0', '1', '0'], '6', 7, 'Draw: 7', [False,
 False, True, False, False, True, False, False, True, False], [0, 0, -1, 0, 1, -
-2, 1, 1, 0, 1], 274892128276167031788079435153352244862), ('Matthew Hall',
+2, 1, 1, 0, 1], 4915701019265174384644466584441738333), ('Matthew Hall',
 'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', True, ['0',
 '1', '0', '0', '3', '0', '0', '1', '0', '2'], '7', 7, 'Draw: 7', [True, True,
 False, True, True, False, True, True, False, True], [0, 0, 1, 0, -1, 2, -1, -1,
-0, -1], 274892128276167031788079435153352244862)]] ```python
-event.get_flat_boxscores()[0] ``` [('Damien Villard',
-'event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1', True, ['0',
-'0', '0', '0', 'X'], '0', 1, 'Draw: 1', [True, True, True, True, True], [0, -1,
--4, -6, -8], 227597408989477916004520082463493572762), ('Matthew Hall',
-'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', False,
-['1', '3', '2', '2', 'X'], '8', 1, 'Draw: 1', [False, False, False, False,
-False], [0, 1, 4, 6, 8], 227597408989477916004520082463493572762), ('Matthew
+0, -1], 4915701019265174384644466584441738333)] The `get_flat_boxscores` method
+can also be used to return a list of `Boxscore` objects for convenience.
+```python event.get_flat_boxscores(flat=False) ``` [Boxscore(team_name='Damien
+Villard',
+href='event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1',
+hammer_start=True, score=['0', '0', '0', '0', 'X'], final_score='0',
+draw_num=1, draw='Draw: 1', hammer_progression=[True, True, True, True, True],
+relative_score=[0, -1, -4, -6, -8],
+guid=209707243860236114112314247393927711356), Boxscore(team_name='Matthew
+Hall', href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+hammer_start=False, score=['1', '3', '2', '2', 'X'], final_score='8',
+draw_num=1, draw='Draw: 1', hammer_progression=[False, False, False, False,
+False], relative_score=[0, 1, 4, 6, 8],
+guid=209707243860236114112314247393927711356), Boxscore(team_name='Matthew
 Mepstead',
-'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144356#1',
-False, ['0', '0', '1', '1', '0', '1', '0', '0', '0', '1', '0'], '4', 1, 'Draw:
-1', [False, False, True, False, False, True, False, False, False, True, False],
-[0, 0, -2, -1, 0, -1, 0, 0, 0, -1, 0],
-230481195381514558834165699232540581342), ('Tyler Stewart',
-'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
-True, ['0', '2', '0', '0', '1', '0', '0', '0', '1', '0', '1'], '5', 1, 'Draw:
-1', [True, True, False, True, True, False, True, True, True, False, True], [0,
-0, 2, 1, 0, 1, 0, 0, 0, 1, 0], 230481195381514558834165699232540581342),
-('Jason March',
-'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
-False, ['0', '2', '0', '1', '0', '2', '2', '0', '2', 'X'], '9', 1, 'Draw: 1',
-[False, False, False, False, False, True, False, False, True, False], [0, 0, 2,
-2, 3, 2, 4, 6, 3, 5], 123876478142928441769100783560984935273), ('Sam Steep',
-'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144351&profileid=25978#1',
-True, ['0', '0', '0', '0', '1', '0', '0', '3', '0', 'X'], '4', 1, 'Draw: 1',
-[True, True, True, True, True, False, True, True, False, True], [0, 0, -2, -2,
--3, -2, -4, -6, -3, -5], 123876478142928441769100783560984935273)] ```python
-event.get_flat_boxscores()[-1] ``` [('Tyler Stewart',
-'event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1', False,
-['0', '0', '1', '1', '0', '3', '0', '0', '1', '0'], '6', 7, 'Draw: 7', [False,
-False, True, False, False, True, False, False, True, False], [0, 0, -1, 0, 1, -
-2, 1, 1, 0, 1], 274892128276167031788079435153352244862), ('Matthew Hall',
-'event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1', True, ['0',
-'1', '0', '0', '3', '0', '0', '1', '0', '2'], '7', 7, 'Draw: 7', [True, True,
-False, True, True, False, True, True, False, True], [0, 0, 1, 0, -1, 2, -1, -1,
-0, -1], 274892128276167031788079435153352244862)] ## About czapi czapi is a
-Python library for scraping curling linescores.
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144356#1',
+hammer_start=False, score=['0', '0', '1', '1', '0', '1', '0', '0', '0', '1',
+'0'], final_score='4', draw_num=1, draw='Draw: 1', hammer_progression=[False,
+False, True, False, False, True, False, False, False, True, False],
+relative_score=[0, 0, -2, -1, 0, -1, 0, 0, 0, -1, 0],
+guid=38537103347544582345141893615297919005), Boxscore(team_name='Tyler
+Stewart',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
+hammer_start=True, score=['0', '2', '0', '0', '1', '0', '0', '0', '1', '0',
+'1'], final_score='5', draw_num=1, draw='Draw: 1', hammer_progression=[True,
+True, False, True, True, False, True, True, True, False, True], relative_score=
+[0, 0, 2, 1, 0, 1, 0, 0, 0, 1, 0],
+guid=38537103347544582345141893615297919005), Boxscore(team_name='Jason March',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
+hammer_start=False, score=['0', '2', '0', '1', '0', '2', '2', '0', '2', 'X'],
+final_score='9', draw_num=1, draw='Draw: 1', hammer_progression=[False, False,
+False, False, False, True, False, False, True, False], relative_score=[0, 0, 2,
+2, 3, 2, 4, 6, 3, 5], guid=272348649831484335603593027216985821953), Boxscore
+(team_name='Sam Steep',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144351&profileid=25978#1',
+hammer_start=True, score=['0', '0', '0', '0', '1', '0', '0', '3', '0', 'X'],
+final_score='4', draw_num=1, draw='Draw: 1', hammer_progression=[True, True,
+True, True, True, False, True, True, False, True], relative_score=[0, 0, -2, -
+2, -3, -2, -4, -6, -3, -5], guid=272348649831484335603593027216985821953),
+Boxscore(team_name='Wayne Tuck Jr.',
+href='event.php?view=Team&eventid=6400&teamid=144353&profileid=12486#1',
+hammer_start=True, score=['0', '2', '0', '0', '0', '0', '1', '1', '1', '0'],
+final_score='5', draw_num=2, draw='Draw: 2', hammer_progression=[True, True,
+False, True, True, True, True, False, False, False], relative_score=[0, 0, 2, -
+2, -2, -2, -3, -2, -1, 0], guid=95112284881200216258215191883153462659),
+Boxscore(team_name='Matthew Hall',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+hammer_start=False, score=['0', '0', '4', '0', '0', '1', '0', '0', '0', '2'],
+final_score='7', draw_num=2, draw='Draw: 2', hammer_progression=[False, False,
+True, False, False, False, False, True, True, True], relative_score=[0, 0, -2,
+2, 2, 2, 3, 2, 1, 0], guid=95112284881200216258215191883153462659), Boxscore
+(team_name='Dayna Deruelle',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144346&profileid=26636#1',
+hammer_start=False, score=['0', '0', '1', '0', '0', '0', '0', 'X'],
+final_score='1', draw_num=2, draw='Draw: 2', hammer_progression=[False, False,
+True, False, True, True, True, True], relative_score=[0, 0, -2, -1, -3, -4, -5,
+-9], guid=59643628877953807377369574857821892232), Boxscore(team_name='Tyler
+Stewart',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435&eventid=6400&teamid=144352&profileid=12477#1',
+hammer_start=True, score=['0', '2', '0', '2', '1', '1', '4', 'X'],
+final_score='10', draw_num=2, draw='Draw: 2', hammer_progression=[True, True,
+False, True, False, False, False, False], relative_score=[0, 0, 2, 1, 3, 4, 5,
+9], guid=59643628877953807377369574857821892232), Boxscore(team_name='Mark
+Kean',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
+hammer_start=True, score=['2', '0', '1', '0', '0', '0', '1', '3', 'X'],
+final_score='7', draw_num=2, draw='Draw: 2', hammer_progression=[True, False,
+False, False, False, True, True, False, False], relative_score=[0, 2, 2, 3, 3,
+1, 0, 1, 4], guid=122217858840490332010920244446431255640), Boxscore
+(team_name='Jason March',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144350#1',
+hammer_start=False, score=['0', '0', '0', '0', '2', '1', '0', '0', 'X'],
+final_score='3', draw_num=2, draw='Draw: 2', hammer_progression=[False, True,
+True, True, True, False, False, True, True], relative_score=[0, -2, -2, -3, -3,
+-1, 0, -1, -4], guid=122217858840490332010920244446431255640), Boxscore
+(team_name='Richard Krell',
+href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144349&profileid=25962#1',
+hammer_start=True, score=['2', '0', '1', '0', '2', '1', '1', 'X'],
+final_score='7', draw_num=2, draw='Draw: 2', hammer_progression=[True, False,
+False, False, True, False, False, False], relative_score=[0, 2, 2, 3, 2, 4, 5,
+6], guid=335702133606077232579627915311442373664), Boxscore(team_name='Rob
+Ainsley',
+href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
+hammer_start=False, score=['0', '0', '0', '1', '0', '0', '0', 'X'],
+final_score='1', draw_num=2, draw='Draw: 2', hammer_progression=[False, True,
+True, True, False, True, True, True], relative_score=[0, -2, -2, -3, -2, -4, -
+5, -6], guid=335702133606077232579627915311442373664), Boxscore
+(team_name='Matthew Hall',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+hammer_start=True, score=['0', '0', '2', '1', '2', '1', '0', '2', 'X'],
+final_score='8', draw_num=3, draw='Draw: 3', hammer_progression=[True, True,
+True, False, False, False, False, True, False], relative_score=[0, 0, -1, 1, 2,
+4, 5, 3, 5], guid=53772503334370441085334378293107653659), Boxscore
+(team_name='Tyler Stewart',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
+hammer_start=False, score=['0', '1', '0', '0', '0', '0', '2', '0', 'X'],
+final_score='3', draw_num=3, draw='Draw: 3', hammer_progression=[False, False,
+False, True, True, True, True, False, True], relative_score=[0, 0, 1, -1, -2, -
+4, -5, -3, -5], guid=53772503334370441085334378293107653659), Boxscore
+(team_name='Mark Kean',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144348&profileid=25961#1',
+hammer_start=True, score=['0', '5', '0', '1', '1', '1', 'X'], final_score='8',
+draw_num=3, draw='Draw: 3', hammer_progression=[True, True, False, True, False,
+False, False], relative_score=[0, -1, 4, 3, 4, 5, 6],
+guid=310456475955908017873561887016699672637), Boxscore(team_name='Richard
+Krell',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477&eventid=6400&teamid=144349&profileid=25962#1',
+hammer_start=False, score=['1', '0', '1', '0', '0', '0', 'X'], final_score='2',
+draw_num=3, draw='Draw: 3', hammer_progression=[False, False, True, False,
+True, True, True], relative_score=[0, 1, -4, -3, -4, -5, -6],
+guid=310456475955908017873561887016699672637), Boxscore(team_name='Damien
+Villard',
+href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144354&profileid=27373#1',
+hammer_start=True, score=['2', '1', '0', '1', '0', '0', '1', '0', '0', '0'],
+final_score='5', draw_num=3, draw='Draw: 3', hammer_progression=[True, False,
+False, True, False, True, True, False, True, True], relative_score=[0, 2, 3, 2,
+3, 1, 1, 2, 1, 0], guid=303047434632680540438656592556261333287), Boxscore
+(team_name='Sam Steep',
+href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144351&profileid=25978#1',
+hammer_start=False, score=['0', '0', '1', '0', '2', '0', '0', '1', '1', '1'],
+final_score='6', draw_num=3, draw='Draw: 3', hammer_progression=[False, True,
+True, False, True, False, False, True, False, False], relative_score=[0, -2, -
+3, -2, -3, -1, -1, -2, -1, 0], guid=303047434632680540438656592556261333287),
+Boxscore(team_name='Jason March',
+href='event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144350#1',
+hammer_start=True, score=['1', '1', '0', '0', '0', '0', '2', '1', '2', 'X'],
+final_score='7', draw_num=3, draw='Draw: 3', hammer_progression=[True, False,
+False, True, True, True, True, False, False, False], relative_score=[0, 1, 2,
+1, 0, 0, 0, 2, 3, 5], guid=229699058183107339172217417532449914369), Boxscore
+(team_name='Matthew Mepstead',
+href='event.php?view=Team&eventid=6400&teamid=144351&profileid=25978&eventid=6400&teamid=144356#1',
+hammer_start=False, score=['0', '0', '1', '1', '0', '0', '0', '0', '0', 'X'],
+final_score='2', draw_num=3, draw='Draw: 3', hammer_progression=[False, True,
+True, False, False, False, False, True, True, True], relative_score=[0, -1, -2,
+-1, 0, 0, 0, -2, -3, -5], guid=229699058183107339172217417532449914369),
+Boxscore(team_name='Wayne Tuck Jr.',
+href='event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144353&profileid=12486#1',
+hammer_start=False, score=['0', '0', '0', '2', '0', '0', '0', '0', 'X'],
+final_score='2', draw_num=3, draw='Draw: 3', hammer_progression=[False, True,
+True, True, False, True, True, True, True], relative_score=[0, -2, -3, -3, -1,
+-2, -4, -5, -6], guid=195399470224611539512163135746754073908), Boxscore
+(team_name='Rob Ainsley',
+href='event.php?view=Team&eventid=6400&teamid=144356&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
+hammer_start=True, score=['2', '1', '0', '0', '1', '2', '1', '1', 'X'],
+final_score='8', draw_num=3, draw='Draw: 3', hammer_progression=[True, False,
+False, False, True, False, False, False, False], relative_score=[0, 2, 3, 3, 1,
+2, 4, 5, 6], guid=195399470224611539512163135746754073908), Boxscore
+(team_name='Matthew Hall',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+hammer_start=True, score=['1', '0', '1', '0', '1', '0', '2', '0', '1', '0'],
+final_score='6', draw_num=4, draw='Draw: 4', hammer_progression=[True, False,
+True, False, True, False, True, False, True, False], relative_score=[0, 1, -1,
+0, -2, -1, -2, 0, -1, 0], guid=63653233024470732271264476184228625543),
+Boxscore(team_name='Mark Kean',
+href='event.php?view=Team&eventid=6400&teamid=144348&profileid=25961#1',
+hammer_start=False, score=['0', '2', '0', '2', '0', '1', '0', '1', '0', '1'],
+final_score='7', draw_num=4, draw='Draw: 4', hammer_progression=[False, True,
+False, True, False, True, False, True, False, True], relative_score=[0, -1, 1,
+0, 2, 1, 2, 0, 1, 0], guid=63653233024470732271264476184228625543), Boxscore
+(team_name='Sam Steep',
+href='event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144351&profileid=25978#1',
+hammer_start=False, score=['1', '0', '0', '2', '0', '1', '1', '0', '1', '1'],
+final_score='7', draw_num=4, draw='Draw: 4', hammer_progression=[False, False,
+True, True, False, True, False, False, True, False], relative_score=[0, 1, 0, -
+2, 0, -2, -1, 0, -1, 0], guid=279469483516704960424550934244064693031),
+Boxscore(team_name='Jason March',
+href='event.php?view=Team&eventid=6400&teamid=144348&profileid=25961&eventid=6400&teamid=144350#1',
+hammer_start=True, score=['0', '1', '2', '0', '2', '0', '0', '1', '0', '0'],
+final_score='6', draw_num=4, draw='Draw: 4', hammer_progression=[True, True,
+False, False, True, False, True, True, False, True], relative_score=[0, -1, 0,
+2, 0, 2, 1, 0, 1, 0], guid=279469483516704960424550934244064693031), Boxscore
+(team_name='Dayna Deruelle',
+href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144346&profileid=26636#1',
+hammer_start=False, score=['0', '2', '1', '1', '1', '0', '3', 'X'],
+final_score='8', draw_num=4, draw='Draw: 4', hammer_progression=[False, True,
+False, False, False, False, True, False], relative_score=[0, -1, 1, 2, 3, 4, 3,
+6], guid=291113397726148010907174443006816563924), Boxscore(team_name='Rob
+Ainsley',
+href='event.php?view=Team&eventid=6400&teamid=144350&profileid=0&eventid=6400&teamid=144345&profileid=15779#1',
+hammer_start=True, score=['1', '0', '0', '0', '0', '1', '0', 'X'],
+final_score='2', draw_num=4, draw='Draw: 4', hammer_progression=[True, False,
+True, True, True, True, False, True], relative_score=[0, 1, -1, -2, -3, -4, -3,
+-6], guid=291113397726148010907174443006816563924), Boxscore(team_name='Sam
+Steep',
+href='event.php?view=Team&eventid=6400&teamid=144351&profileid=25978#1',
+hammer_start=False, score=['0', '1', '0', '0', '0', '2', '0', '2', '0', '0'],
+final_score='5', draw_num=5, draw='Draw: 5', hammer_progression=[False, False,
+False, True, True, True, False, True, False, False], relative_score=[0, 0, 1,
+0, -1, -3, -1, -3, -1, -1], guid=95866945533461342246819997703085723055),
+Boxscore(team_name='Richard Krell',
+href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1',
+hammer_start=True, score=['0', '0', '1', '1', '2', '0', '2', '0', '0', '1'],
+final_score='7', draw_num=5, draw='Draw: 5', hammer_progression=[True, True,
+True, False, False, False, True, False, True, True], relative_score=[0, 0, -1,
+0, 1, 3, 1, 3, 1, 1], guid=95866945533461342246819997703085723055), Boxscore
+(team_name='Dayna Deruelle',
+href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144346&profileid=26636#1',
+hammer_start=False, score=['0', '0', '1', '0', '0', '0', '1', '0', '3', '1',
+'0'], final_score='6', draw_num=5, draw='Draw: 5', hammer_progression=[False,
+True, True, False, True, True, True, False, True, False, False],
+relative_score=[0, -1, -1, 0, -1, -1, -3, -2, -4, -1, 0],
+guid=233581897033627594667237538445333000951), Boxscore(team_name='Tyler
+Stewart',
+href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962&eventid=6400&teamid=144352&profileid=12477#1',
+hammer_start=True, score=['1', '0', '0', '1', '0', '2', '0', '2', '0', '0',
+'1'], final_score='7', draw_num=5, draw='Draw: 5', hammer_progression=[True,
+False, False, True, False, False, False, True, False, True, True],
+relative_score=[0, 1, 1, 0, 1, 1, 3, 2, 4, 1, 0],
+guid=233581897033627594667237538445333000951), Boxscore(team_name='Richard
+Krell',
+href='event.php?view=Team&eventid=6400&teamid=144349&profileid=25962#1',
+hammer_start=False, score=['0', '0', '1', '1', '0', '0', '1', '0', 'X'],
+final_score='3', draw_num=6, draw='Draw: 6', hammer_progression=[False, False,
+True, False, False, True, True, False, True], relative_score=[0, 0, -2, -1, 0,
+-2, -5, -4, -5], guid=61203104491141348409761697458039616615), Boxscore
+(team_name='Tyler Stewart',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
+hammer_start=True, score=['0', '2', '0', '0', '2', '3', '0', '1', 'X'],
+final_score='8', draw_num=6, draw='Draw: 6', hammer_progression=[True, True,
+False, True, True, False, False, True, False], relative_score=[0, 0, 2, 1, 0,
+2, 5, 4, 5], guid=61203104491141348409761697458039616615), Boxscore
+(team_name='Tyler Stewart',
+href='event.php?view=Team&eventid=6400&teamid=144352&profileid=12477#1',
+hammer_start=False, score=['0', '0', '1', '1', '0', '3', '0', '0', '1', '0'],
+final_score='6', draw_num=7, draw='Draw: 7', hammer_progression=[False, False,
+True, False, False, True, False, False, True, False], relative_score=[0, 0, -1,
+0, 1, -2, 1, 1, 0, 1], guid=4915701019265174384644466584441738333), Boxscore
+(team_name='Matthew Hall',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+hammer_start=True, score=['0', '1', '0', '0', '3', '0', '0', '1', '0', '2'],
+final_score='7', draw_num=7, draw='Draw: 7', hammer_progression=[True, True,
+False, True, True, False, True, True, False, True], relative_score=[0, 0, 1, 0,
+-1, 2, -1, -1, 0, -1], guid=4915701019265174384644466584441738333)] ```python
+event.get_flat_boxscores()[0] ``` Boxscore(team_name='Damien Villard',
+href='event.php?view=Team&eventid=6400&teamid=144354&profileid=27373#1',
+hammer_start=True, score=['0', '0', '0', '0', 'X'], final_score='0',
+draw_num=1, draw='Draw: 1', hammer_progression=[True, True, True, True, True],
+relative_score=[0, -1, -4, -6, -8],
+guid=209707243860236114112314247393927711356) ```python
+event.get_flat_boxscores()[-1] ``` Boxscore(team_name='Matthew Hall',
+href='event.php?view=Team&eventid=6400&teamid=144347&profileid=12435#1',
+hammer_start=True, score=['0', '1', '0', '0', '3', '0', '0', '1', '0', '2'],
+final_score='7', draw_num=7, draw='Draw: 7', hammer_progression=[True, True,
+False, True, True, False, True, True, False, True], relative_score=[0, 0, 1, 0,
+-1, 2, -1, -1, 0, -1], guid=4915701019265174384644466584441738333) ## About
+czapi czapi is a Python library for scraping curling linescores.
```

### Comparing `czapi-0.1.9/settings.ini` & `czapi-0.2.0/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = calicorob
 description = CurlingZone scraper API.
 keywords = curling, stats
 author = Robert Currie
 author_email = robert.art.currie@gmail.com
 copyright = Robert Currie
 branch = master
-version = 0.1.9
+version = 0.2.0
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 2
 requirements = bs4 requests
```

### Comparing `czapi-0.1.9/setup.py` & `czapi-0.2.0/setup.py`

 * *Files identical despite different names*

