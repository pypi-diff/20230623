# Comparing `tmp/xklb-2.1.7.tar.gz` & `tmp/xklb-2.1.8.tar.gz`

## Comparing `xklb-2.1.7.tar` & `xklb-2.1.8.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.1.7/.gitattributes
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 xklb-2.1.7/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.1.7/Windows.md
--rw-r--r--   0        0        0   490400 2020-02-02 00:00:00.000000 xklb-2.1.7/pdm.lock
--rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 xklb-2.1.7/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.1.7/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.1.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.1.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.1.7/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-2.1.7/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/__init__.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/books.py
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/consts.py
--rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/db.py
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/dl_config.py
--rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/dl_extract.py
--rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/fs_extract.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/gdl_extract.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/gui.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/history.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/hn_extract.py
--rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/lb.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/media.py
--rw-r--r--   0        0        0    25386 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/play_actions.py
--rw-r--r--   0        0        0    34705 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/player.py
--rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/playlists.py
--rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/praw_extract.py
--rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/search.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/subtitle.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/tabs_extract.py
--rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/tube_backend.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/tube_extract.py
--rw-r--r--   0        0        0    83349 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/usage.py
--rw-r--r--   0        0        0    41240 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7248 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/christen.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.1.7/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.1.7/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.1.7/LICENSE
--rw-r--r--   0        0        0    94113 2020-02-02 00:00:00.000000 xklb-2.1.7/README.md
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-2.1.7/pyproject.toml
--rw-r--r--   0        0        0    97739 2020-02-02 00:00:00.000000 xklb-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.1.8/.gitattributes
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xklb-2.1.8/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.1.8/Windows.md
+-rw-r--r--   0        0        0   490400 2020-02-02 00:00:00.000000 xklb-2.1.8/pdm.lock
+-rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 xklb-2.1.8/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.1.8/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.1.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.1.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.1.8/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-2.1.8/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/books.py
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/consts.py
+-rw-r--r--   0        0        0     8342 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/db.py
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/dl_config.py
+-rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/gui.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/history.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/hn_extract.py
+-rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/lb.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/media.py
+-rw-r--r--   0        0        0    25566 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/play_actions.py
+-rw-r--r--   0        0        0    36224 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/player.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/playlists.py
+-rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/subtitle.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/tube_extract.py
+-rw-r--r--   0        0        0    83354 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/usage.py
+-rw-r--r--   0        0        0    41329 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7248 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.1.8/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.1.8/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.1.8/LICENSE
+-rw-r--r--   0        0        0    94114 2020-02-02 00:00:00.000000 xklb-2.1.8/README.md
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-2.1.8/pyproject.toml
+-rw-r--r--   0        0        0    97740 2020-02-02 00:00:00.000000 xklb-2.1.8/PKG-INFO
```

### Comparing `xklb-2.1.7/TODO` & `xklb-2.1.8/TODO`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-- use socket-play as default playback -- accurately get playhead
+ncdu clone for sqlite
 
 - POIs CLI -- save your trip plans and see places to go with automated day trip itineraries, geopandas buffer
 
 - wt/lt/search join and use fts on both tables, threading ?
 
 - improve playlists subcommand
```

### Comparing `xklb-2.1.7/Windows.md` & `xklb-2.1.8/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/pdm.lock` & `xklb-2.1.8/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/readme.py` & `xklb-2.1.8/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-2.1.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-2.1.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/.github/workflows/push.yaml` & `xklb-2.1.8/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/av.py` & `xklb-2.1.8/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/books.py` & `xklb-2.1.8/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/consts.py` & `xklb-2.1.8/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/db.py` & `xklb-2.1.8/xklb/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,21 +182,23 @@
 
 def fts_quote(query: List[str]) -> List[str]:
     fts_words = [" NOT ", " AND ", " OR ", "*", ":", "NEAR("]
     return [s if any(r in s for r in fts_words) else '"' + s + '"' for s in query]
 
 
 def fts_search(args, table="media") -> str:
-    args.filter_bindings["query"] = " AND ".join(fts_quote(args.include))
+    fts_query = " AND ".join(fts_quote(args.include))
     if args.exclude:
-        args.filter_bindings["query"] += " NOT " + " NOT ".join(fts_quote(args.exclude))
+        fts_query += " NOT " + " NOT ".join(fts_quote(args.exclude))
+    args.filter_bindings["query"] = fts_query
     table = "(" + args.db[table].search_sql(include_rank=True) + ")"
     return table
 
 
+
 def fts_flexible_search(args, table="media") -> str:
     args.filter_bindings["query"] = " OR ".join(fts_quote(args.include))
     if args.exclude:
         args.filter_bindings["query"] += " NOT " + " NOT ".join(fts_quote(args.exclude))
     table = "(" + args.db[table].search_sql(include_rank=True) + ")"
     return table
```

### Comparing `xklb-2.1.7/xklb/dl_config.py` & `xklb-2.1.8/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/dl_extract.py` & `xklb-2.1.8/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/fs_extract.py` & `xklb-2.1.8/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/gdl_backend.py` & `xklb-2.1.8/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/gdl_extract.py` & `xklb-2.1.8/xklb/gdl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/gui.py` & `xklb-2.1.8/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/history.py` & `xklb-2.1.8/xklb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/hn_extract.py` & `xklb-2.1.8/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/lb.py` & `xklb-2.1.8/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/media.py` & `xklb-2.1.8/xklb/media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/play_actions.py` & `xklb-2.1.8/xklb/play_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -260,15 +260,14 @@
 
     args.sock = None
     return args
 
 
 def construct_query(args) -> Tuple[str, dict]:
     m_columns = db.columns(args, "media")
-    h_columns = db.columns(args, "history")
 
     args.filter_sql = []
     args.filter_bindings = {}
 
     if args.duration:
         args.filter_sql.append(" and duration IS NOT NULL " + args.duration)
     if args.size:
@@ -301,33 +300,33 @@
         )
     if args.changed_before:
         args.filter_sql.append(
             f"and time_modified < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.changed_before)}')) as int)",
         )
     if args.played_within:
         args.filter_sql.append(
-            f"and time_played > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.played_within)}')) as int)",
+            f"and time_last_played > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.played_within)}')) as int)",
         )
     if args.played_before:
         args.filter_sql.append(
-            f"and time_played < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.played_before)}')) as int)",
+            f"and time_last_played < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.played_before)}')) as int)",
         )
     if args.deleted_within:
         args.filter_sql.append(
             f"and time_deleted > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.deleted_within)}')) as int)",
         )
     if args.deleted_before:
         args.filter_sql.append(
             f"and time_deleted < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.deleted_before)}')) as int)",
         )
 
     args.table = "media"
     if args.db["media"].detect_fts() and not args.no_fts:
         if args.include:
-            args.table = db.fts_flexible_search(args)
+            args.table = db.fts_search(args)
             m_columns = {**m_columns, "rank": int}
         elif args.exclude:
             db.construct_search_bindings(args, m_columns)
     else:
         db.construct_search_bindings(args, m_columns)
 
     if args.table == "media" and not any(
@@ -348,48 +347,55 @@
 
         where_not_deleted = (
             "where COALESCE(time_deleted,0) = 0"
             if "time_deleted" in m_columns and "time_deleted" not in " ".join(sys.argv)
             else ""
         )
         args.filter_sql.append(
-            f"and m.rowid in (select rowid from media {where_not_deleted} order by random() limit {limit})",
+            f"and m.id in (select id from media {where_not_deleted} order by random() limit {limit})",
         )
 
     cols = args.cols or ["path", "title", "duration", "size", "subtitle_count", "is_dir", "rank"]
     args.select = [c for c in cols if c in m_columns or c in ["*"]]
     if args.action == SC.read and "tags" in m_columns:
         args.select += "cast(length(tags) / 4.2 / 220 * 60 as INT) + 10 duration"
     args.select_sql = "\n        , ".join(args.select)
     args.limit_sql = "LIMIT " + str(args.limit) if args.limit else ""
     args.offset_sql = f"OFFSET {args.skip}" if args.skip and args.limit else ""
     query = f"""WITH m as (
-    SELECT rowid, * FROM {args.table}
-    WHERE 1=1
-        {player.filter_args_sql(args, m_columns)}
-    )
-    SELECT
-        {args.select_sql}
-        , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
-        , MIN(h.time_played) time_first_played
-        , MAX(h.time_played) time_last_played
-        , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
-    FROM m
-    LEFT JOIN history h on h.media_id = m.id
-    WHERE 1=1
-        {" ".join(args.filter_sql)}
-    GROUP BY m.id, m.path -- for time_played aggregates
-    ORDER BY 1=1
-        , {args.sort}
-    {args.limit_sql} {args.offset_sql}
+            SELECT
+                m.id
+                , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
+                , MIN(h.time_played) time_first_played
+                , MAX(h.time_played) time_last_played
+                , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
+                , *
+            FROM {args.table} m
+            LEFT JOIN history h on h.media_id = m.id
+            WHERE 1=1
+                {player.filter_args_sql(args, m_columns)}
+            GROUP BY m.id, m.path
+        )
+        SELECT
+            {args.select_sql}
+            , play_count
+            , time_first_played
+            , time_last_played
+            , playhead
+        FROM m
+        WHERE 1=1
+            {" ".join(args.filter_sql)}
+        ORDER BY 1=1
+            , {args.sort}
+        {args.limit_sql} {args.offset_sql}
     """
 
     args.filter_sql = [
-        s for s in args.filter_sql if "rowid" not in s
-    ]  # only use random rowid constraint in first query
+        s for s in args.filter_sql if "id" not in s
+    ]  # only use random id constraint in first query
 
     return query, args.filter_bindings
 
 
 def chromecast_play(args, m) -> None:
     if args.action in (SC.watch):
         catt_log = player.watch_chromecast(args, m, subtitles_file=safe_unpack(subtitle.get_subtitle_paths(m["path"])))
```

### Comparing `xklb-2.1.7/xklb/player.py` & `xklb-2.1.8/xklb/player.py`

 * *Files 4% similar despite different names*

```diff
@@ -396,26 +396,34 @@
         new_candidate = candidate[: -len(remove_chars)]
         log.debug(f"Matches for '{new_candidate}':")
 
         if candidate in ("" or new_candidate):
             return m
 
         candidate = new_candidate
-        query = f"""
+        query = f"""WITH m as (
+                SELECT
+                    SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
+                    , MIN(h.time_played) time_first_played
+                    , MAX(h.time_played) time_last_played
+                    , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
+                    , *
+                FROM media m
+                LEFT JOIN history h on h.media_id = m.id
+                GROUP BY m.id, m.path
+            )
             SELECT
                 {args.select_sql}
-                , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
-            FROM {'media' if args.play_in_order >= consts.SIMILAR_NO_FILTER_NO_FTS else args.table} m
-            LEFT JOIN history h on h.media_id = m.id
+                , play_count
+            FROM {'m' if args.play_in_order >= consts.SIMILAR_NO_FILTER_NO_FTS else args.table} AS m
             WHERE 1=1
                 and path like :candidate
                 {filter_args_sql(args, m_columns)}
                 {'' if args.play_in_order >= consts.SIMILAR_NO_FILTER else (" ".join(args.filter_sql) or '')}
                 {"and path not in ({})".format(",".join([f":ignore_path{i}" for i in range(len(ignore_paths))])) if len(ignore_paths) > 0 else ''}
-            GROUP BY m.id
             ORDER BY play_count, path
             LIMIT 1000
             """
 
         ignore_path_params = {f"ignore_path{i}": value for i, value in enumerate(ignore_paths)}
         bindings = {"candidate": candidate + "%", **ignore_path_params}
         if args.play_in_order >= consts.SIMILAR_NO_FILTER:
@@ -449,25 +457,33 @@
     m = media.get(args, m["path"])
     words = set(
         utils.conform(utils.extract_words(m.get(k)) for k in m if k in db.config["media"]["search_columns"]),
     )
     args.include = sorted(words, key=len, reverse=True)[:100]
     args.table = db.fts_flexible_search(args)
 
-    query = f"""
+    query = f"""WITH m as (
+            SELECT
+                SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
+                , MIN(h.time_played) time_first_played
+                , MAX(h.time_played) time_last_played
+                , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
+                , *
+            FROM media m
+            LEFT JOIN history h on h.media_id = m.id
+            GROUP BY m.id, m.path
+        )
         SELECT
             {args.select_sql}, rank
-            , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
+            , play_count
         FROM {args.table} m
-        LEFT JOIN history h on h.media_id = m.id
         WHERE 1=1
             and path != :path
             {filter_args_sql(args, m_columns)}
             {'' if args.related >= consts.RELATED_NO_FILTER else (" ".join(args.filter_sql) or '')}
-        GROUP BY m.id
         ORDER BY play_count
             , m.path like "http%"
             , {'rank' if 'sort' in args.defaults else f'ntile(1000) over (order by rank), {args.sort}'}
             , path
         {"LIMIT " + str(args.limit - 1) if args.limit else ""} {args.offset_sql}
         """
     bindings = {"path": m["path"]}
@@ -493,25 +509,33 @@
     else:
         filter_paths = (
             "AND ("
             + " OR ".join([f"(path LIKE :subpath{i} and path not like :subpath{i} || '/%')" for i in range(len(dirs))])
             + ")"
         )
 
-    query = f"""
+    query = f"""WITH m as (
+            SELECT
+                SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
+                , MIN(h.time_played) time_first_played
+                , MAX(h.time_played) time_last_played
+                , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
+                , *
+            FROM media m
+            LEFT JOIN history h on h.media_id = m.id
+            GROUP BY m.id, m.path
+        )
         SELECT
             {args.select_sql}
-            , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
+            , play_count
         FROM {args.table} m
-        LEFT JOIN history h on h.media_id = m.id
         WHERE 1=1
             {filter_args_sql(args, m_columns)}
             {filter_paths}
             {'' if args.related >= consts.DIRS_NO_FILTER else (" ".join(args.filter_sql) or '')}
-        GROUP BY m.id
         ORDER BY play_count
             , m.path LIKE "http%"
             {'' if 'sort' in args.defaults else ', ' + args.sort}
             , path
         {"LIMIT 10000" if 'limit' in args.defaults else str(args.limit)} {args.offset_sql}
     """
     subpath_params = {f"subpath{i}": value + "%" for i, value in enumerate(dirs)}
@@ -847,25 +871,34 @@
         time_period = f"strftime('%Y', datetime({time_column}, 'unixepoch', '-3 months')) || '-Q' || ((strftime('%m', datetime({time_column}, 'unixepoch', '-3 months')) - 1) / 3 + 1)"
     elif freq == "yearly":
         time_period = f"strftime('%Y', datetime({time_column}, 'unixepoch'))"
     else:
         msg = f"Invalid value for 'freq': {freq}"
         raise ValueError(msg)
 
-    query = f"""
-    SELECT
-        {time_period} AS time_period
-        , SUM(duration) AS duration_sum
-        , AVG(duration) AS duration_avg
-        , SUM(size) AS size_sum
-        , AVG(size) AS size_avg
-    FROM media m
-    LEFT JOIN history h on h.media_id = m.id
-    WHERE coalesce(time_period, 0)>0 and {time_column}>0 {where}
-    GROUP BY time_period
+    query = f"""WITH m as (
+            SELECT
+                SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
+                , MIN(h.time_played) time_first_played
+                , MAX(h.time_played) time_last_played
+                , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
+                , *
+            FROM media m
+            LEFT JOIN history h on h.media_id = m.id
+            GROUP BY m.id, m.path
+        )
+        SELECT
+            {time_period} AS time_period
+            , SUM(duration) AS duration_sum
+            , AVG(duration) AS duration_avg
+            , SUM(size) AS size_sum
+            , AVG(size) AS size_avg
+        FROM m
+        WHERE coalesce(time_period, 0)>0 and {time_column}>0 {where}
+        GROUP BY time_period
     """
     return list(args.db.query(query))
 
 
 def cadence_adjusted_duration(args, duration):
     try:
         historical_daily = statistics.mean((d["duration_sum"] or 0) for d in historical_usage(args))
```

### Comparing `xklb-2.1.7/xklb/playlists.py` & `xklb-2.1.8/xklb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/praw_extract.py` & `xklb-2.1.8/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/search.py` & `xklb-2.1.8/xklb/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,17 +119,17 @@
         db.construct_search_bindings(args, c_columns)
 
     cols = args.cols or ["path", "text", "time", "rank", "title"]
     args.select = [c for c in cols if c in {**c_columns, **m_columns, **{"*": "Any"}}]
     args.select_sql = "\n        , ".join(args.select)
     args.limit_sql = "LIMIT " + str(args.limit) if args.limit else ""
     query = f"""WITH c as (
-    SELECT rowid, * FROM {table}
-    WHERE 1=1
-        {player.filter_args_sql(args, c_columns)}
+        SELECT id, * FROM {table}
+        WHERE 1=1
+            {player.filter_args_sql(args, c_columns)}
     )
     SELECT
         {args.select_sql}
     FROM c
     JOIN media m on m.id = c.media_id
     WHERE 1=1
         {" ".join(args.filter_sql)}
```

### Comparing `xklb-2.1.7/xklb/subtitle.py` & `xklb-2.1.8/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/tabs_actions.py` & `xklb-2.1.8/xklb/tabs_actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,41 +91,41 @@
     LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
     OFFSET = f"OFFSET {args.skip}" if args.skip else ""
 
     query = f"""WITH m as (
             SELECT
                 path
                 , frequency
-                , COALESCE(MAX(time_played), 0) time_played
+                , COALESCE(MAX(h.time_played), 0) time_last_played
                 , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                 , time_deleted
                 , hostname
                 , category
             FROM media
             LEFT JOIN history h on h.media_id = media.id
             GROUP BY media.id
         )
         SELECT path
         , frequency
         , CASE
-            WHEN frequency = 'daily' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+1 Day' )) as int)
-            WHEN frequency = 'weekly' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+7 Days' )) as int)
-            WHEN frequency = 'monthly' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+1 Month' )) as int)
-            WHEN frequency = 'quarterly' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+3 Months' )) as int)
-            WHEN frequency = 'yearly' THEN cast(STRFTIME('%s', datetime( time_played, 'unixepoch', '+1 Year' )) as int)
+            WHEN frequency = 'daily' THEN cast(STRFTIME('%s', datetime( time_last_played, 'unixepoch', '+1 Day' )) as int)
+            WHEN frequency = 'weekly' THEN cast(STRFTIME('%s', datetime( time_last_played, 'unixepoch', '+7 Days' )) as int)
+            WHEN frequency = 'monthly' THEN cast(STRFTIME('%s', datetime( time_last_played, 'unixepoch', '+1 Month' )) as int)
+            WHEN frequency = 'quarterly' THEN cast(STRFTIME('%s', datetime( time_last_played, 'unixepoch', '+3 Months' )) as int)
+            WHEN frequency = 'yearly' THEN cast(STRFTIME('%s', datetime( time_last_played, 'unixepoch', '+1 Year' )) as int)
         END time_valid
         {', ' + ', '.join(args.cols) if args.cols else ''}
     FROM m
     WHERE 1=1
         and COALESCE(time_deleted,0) = 0
         {" ".join(args.filter_sql)}
         {"and time_valid < cast(STRFTIME('%s', datetime()) as int)" if not args.print else ''}
     ORDER BY 1=1
         {', ' + args.sort if args.sort else ''}
-        {', time_played, time_valid, path' if args.print else ''}
+        {', time_last_played, time_valid, path' if args.print else ''}
         , play_count
         , frequency = 'daily' desc
         , frequency = 'weekly' desc
         , frequency = 'monthly' desc
         , frequency = 'quarterly' desc
         , frequency = 'yearly' desc
         , ROW_NUMBER() OVER ( PARTITION BY
```

### Comparing `xklb-2.1.7/xklb/tabs_extract.py` & `xklb-2.1.8/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/tube_backend.py` & `xklb-2.1.8/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/tube_extract.py` & `xklb-2.1.8/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/usage.py` & `xklb-2.1.8/xklb/usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,15 @@
 
     Constrain media to file size (in megabytes):
         library {action} --size 20
         library {action} -S 6  # 6 MB ±10 percent (ie. between 5 and 7 MB)
         library {action} -S-6  # less than 6 MB
         library {action} -S+6  # more than 6 MB
 
-    Constrain media by time_created / time_played / time_deleted / time_modified:
+    Constrain media by time_created / time_last_played / time_deleted / time_modified:
         library {action} --created-within '3 days'
         library {action} --created-before '3 years'
 
     Constrain media by throughput:
         Bitrate information is not explicitly saved.
         You can use file size and duration as a proxy for throughput:
         library {action} -w 'size/duration<50000'
```

### Comparing `xklb-2.1.7/xklb/utils.py` & `xklb-2.1.8/xklb/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1082,14 +1082,17 @@
                 files.append(entry.path)
                 if len(files) == limit:
                     break
     return sorted(files)
 
 
 def cluster_paths(paths, n_clusters=None):
+    if len(paths) < 2:
+        return paths
+
     from sklearn.cluster import KMeans
     from sklearn.feature_extraction.text import TfidfVectorizer
 
     sentence_strings = (path_to_sentence(s) for s in paths)
 
     try:
         vectorizer = TfidfVectorizer(min_df=2, strip_accents="unicode", stop_words="english")
@@ -1197,14 +1200,16 @@
         result.append(metadata)
     log.info("common_prefix %s", t.elapsed())
 
     return result
 
 
 def cluster_dicts(args, media):
+    if len(media) < 2:
+        return media
     media_keyed = {d["path"]: d for d in media}
     groups = cluster_paths([d["path"] for d in media])
     groups = sorted(groups, key=lambda d: (-len(d["grouped_paths"]), -len(d["common_prefix"])))
     if hasattr(args, "sort") and "duration" in args.sort:
         sorted_paths = flatten(
             sorted(d["grouped_paths"], key=lambda p: media_keyed[p]["duration"], reverse="duration desc" in args.sort)
             for d in groups
```

### Comparing `xklb-2.1.7/xklb/scripts/bigdirs.py` & `xklb-2.1.8/xklb/scripts/bigdirs.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,30 +110,29 @@
             d.pop(path)
 
     return [{**v, "path": k} for k, v in d.items()]
 
 
 def get_table(args) -> List[dict]:
     m_columns = db.columns(args, "media")
-    h_columns = db.columns(args, "history")
     args.filter_sql = []
     args.filter_bindings = {}
 
     if args.size:
         args.filter_sql.append(" and size IS NOT NULL " + args.size)
     db.construct_search_bindings(args, m_columns)
 
     media = list(
         args.db.query(
             f"""
         SELECT
             path
             , size
             {', time_deleted' if 'time_deleted' in m_columns else ''}
-            {', time_played' if 'time_played' in h_columns else ''}
+            , time_played
         FROM media m
         LEFT JOIN history h on h.media_id = m.id
         WHERE 1=1
             {'and time_downloaded > 0' if 'time_downloaded' in m_columns else ''}
             {" ".join(args.filter_sql)}
         GROUP BY m.id
         ORDER BY path
@@ -161,15 +160,15 @@
     if args.depth:
         folders = folder_depth(args, folders)
     if args.folder_size:
         args.folder_size = utils.parse_human_to_lambda(utils.human_to_bytes, args.folder_size)
         folders = [d for d in folders if args.folder_size(d["size"])]
 
     reverse = False
-    if " desc" in args.sort_by:
+    if args.sort_by and " desc" in args.sort_by:
         args.sort_by = args.sort_by.replace(" desc", "")
         reverse = True
 
     return sorted(folders, key=sort_by(args), reverse=reverse)
 
 
 def bigdirs() -> None:
```

### Comparing `xklb-2.1.7/xklb/scripts/block.py` & `xklb-2.1.8/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/christen.py` & `xklb-2.1.8/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/cluster_sort.py` & `xklb-2.1.8/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/copy_play_counts.py` & `xklb-2.1.8/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/dedupe.py` & `xklb-2.1.8/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/dedupe_db.py` & `xklb-2.1.8/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/download_status.py` & `xklb-2.1.8/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/history.py` & `xklb-2.1.8/xklb/scripts/history.py`

 * *Files 10% similar despite different names*

```diff
@@ -106,54 +106,70 @@
 
     m_columns = args.db["media"].columns_dict
 
     if args.facet.startswith("watching"):
         print("Partially watched:")
         tbl = player.historical_usage(args, args.frequency, "time_played", "and coalesce(play_count, 0)=0")
         print_history(tbl)
-        query = f"""SELECT
+        query = f"""WITH m as (
+                SELECT
+                    SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
+                    , MIN(h.time_played) time_first_played
+                    , MAX(h.time_played) time_last_played
+                    , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
+                    , *
+                FROM media m
+                LEFT JOIN history h on h.media_id = m.id
+                GROUP BY m.id, m.path
+            )
+            SELECT
                 path
                 {', title' if 'title' in m_columns else ''}
                 {', duration' if 'duration' in m_columns else ''}
                 {', subtitle_count' if 'subtitle_count' in m_columns else ''}
-                , MAX(h.time_played) time_played
-                , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
-                , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
-            FROM media m
-            LEFT JOIN history h on h.media_id = m.id
+                , time_last_played
+            FROM m
             WHERE coalesce(time_deleted, 0) = 0
                 and coalesce(playhead, 0) > 60
                 and coalesce(play_count, 0) = 0
-            GROUP BY m.id
-            ORDER BY time_played desc, playhead desc
+            ORDER BY time_last_played desc, playhead desc
             LIMIT {args.limit or 5}
         """
         tbl = list(args.db.query(query))
-        print_recent(tbl, "time_played")
+        print_recent(tbl, "time_last_played")
 
     elif args.facet.startswith("watched"):
         print("Finished watching:")
         tbl = player.historical_usage(args, args.frequency, "time_played", "and coalesce(play_count, 0)>0")
         print_history(tbl)
-        query = f"""SELECT
+        query = f"""WITH m as (
+                SELECT
+                    SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
+                    , MIN(h.time_played) time_first_played
+                    , MAX(h.time_played) time_last_played
+                    , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
+                    , *
+                FROM media m
+                LEFT JOIN history h on h.media_id = m.id
+                GROUP BY m.id, m.path
+            )
+            SELECT
                 path
                 {', title' if 'title' in m_columns else ''}
                 {', duration' if 'duration' in m_columns else ''}
                 {', subtitle_count' if 'subtitle_count' in m_columns else ''}
-                , MAX(h.time_played) time_played
-                , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
-            FROM media m
-            LEFT JOIN history h on h.media_id = m.id
+                , time_last_played
+                , play_count
+            FROM m
             WHERE coalesce(play_count, 0)>0
-            GROUP BY m.id
-            ORDER BY time_played desc, path
+            ORDER BY time_last_played desc, path
             LIMIT {args.limit or 5}
         """
         tbl = list(args.db.query(query))
-        print_recent(tbl, "time_played")
+        print_recent(tbl, "time_last_played")
 
     else:
         print(f"{args.facet.title()} media:")
         tbl = player.historical_usage(args, args.frequency, f"time_{args.facet}")
         print_history(tbl)
         tbl = recent_media(args, f"time_{args.facet}")
         print_recent(tbl, f"time_{args.facet}")
```

### Comparing `xklb-2.1.7/xklb/scripts/merge_dbs.py` & `xklb-2.1.8/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/merge_online_local.py` & `xklb-2.1.8/xklb/scripts/merge_online_local.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,39 +23,39 @@
     query = """
     WITH m1 as (
         SELECT
             *
         FROM
             media
         WHERE 1=1
-            and id is not null
-            and id != ""
+            and extractor_id is not null
+            and extractor_id != ""
             and time_deleted = 0
             and playlist_id in (
                 SELECT id from playlists
                 WHERE extractor_key
                     NOT IN ('Local', 'NBCStations', 'TedTalk', 'ThisAmericanLife', 'InfoQ', 'NFB', 'KickStarter')
             )
     )
     SELECT
         m2.path keep_path
         , m1.path duplicate_path
         , m1.title
     FROM m1, (
         SELECT
-            rowid,
+            media.id,
             *
         FROM
             media
         WHERE 1=1
             and time_deleted = 0
-            and id is null
+            and extractor_id is null
             and title is null
     ) m2
-    JOIN media_fts on m2.rowid = media_fts.rowid
+    JOIN media_fts on m2.id = media_fts.id
     JOIN playlists p2 on p2.id = m2.playlist_id
     WHERE p2.extractor_key = 'Local'
         AND media_fts.path MATCH '"'||m1.extractor_id||'"'
         AND m2.PATH LIKE '%['||m1.extractor_id||']%'
     ORDER BY 1=1
         , length(m2.path)-length(REPLACE(m2.path, '/', '')) desc
         , length(m2.path)-length(REPLACE(m2.path, '.', ''))
```

### Comparing `xklb-2.1.7/xklb/scripts/move_list.py` & `xklb-2.1.8/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/optimize_db.py` & `xklb-2.1.8/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/playback_control.py` & `xklb-2.1.8/xklb/scripts/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/playlists.py` & `xklb-2.1.8/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/redownload.py` & `xklb-2.1.8/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/relmv.py` & `xklb-2.1.8/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/scatter.py` & `xklb-2.1.8/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/streaming_tab_loader.py` & `xklb-2.1.8/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/mining/data.py` & `xklb-2.1.8/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/mining/extract_links.py` & `xklb-2.1.8/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.1.8/xklb/scripts/mining/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/mining/nouns.py` & `xklb-2.1.8/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/mining/pushshift.py` & `xklb-2.1.8/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.1.8/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/xklb/assets/kotobago.png` & `xklb-2.1.8/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/.gitignore` & `xklb-2.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/LICENSE` & `xklb-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/README.md` & `xklb-2.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 
       lb extract-links         Extract links from lists of web pages
 
       lb mpv-watchlater        Import timestamps from mpv watchlater to history table
 
       lb cluster-sort          Lines -> sorted by sentence similarity groups (stdin)
       lb nouns                 Unstructured text -> compound nouns (stdin)
-    
+
 
 </details>
 
 ## Examples
 
 ### Watch online media on your PC
 
@@ -751,15 +751,15 @@
 
     Constrain media to file size (in megabytes):
         library watch --size 20
         library watch -S 6  # 6 MB ±10 percent (ie. between 5 and 7 MB)
         library watch -S-6  # less than 6 MB
         library watch -S+6  # more than 6 MB
 
-    Constrain media by time_created / time_played / time_deleted / time_modified:
+    Constrain media by time_created / time_last_played / time_deleted / time_modified:
         library watch --created-within '3 days'
         library watch --created-before '3 years'
 
     Constrain media by throughput:
         Bitrate information is not explicitly saved.
         You can use file size and duration as a proxy for throughput:
         library watch -w 'size/duration<50000'
```

### Comparing `xklb-2.1.7/pyproject.toml` & `xklb-2.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.1.7/PKG-INFO` & `xklb-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 2.1.7
+Version: 2.1.8
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -292,15 +292,15 @@
 
       lb extract-links         Extract links from lists of web pages
 
       lb mpv-watchlater        Import timestamps from mpv watchlater to history table
 
       lb cluster-sort          Lines -> sorted by sentence similarity groups (stdin)
       lb nouns                 Unstructured text -> compound nouns (stdin)
-    
+
 
 </details>
 
 ## Examples
 
 ### Watch online media on your PC
 
@@ -836,15 +836,15 @@
 
     Constrain media to file size (in megabytes):
         library watch --size 20
         library watch -S 6  # 6 MB ±10 percent (ie. between 5 and 7 MB)
         library watch -S-6  # less than 6 MB
         library watch -S+6  # more than 6 MB
 
-    Constrain media by time_created / time_played / time_deleted / time_modified:
+    Constrain media by time_created / time_last_played / time_deleted / time_modified:
         library watch --created-within '3 days'
         library watch --created-before '3 years'
 
     Constrain media by throughput:
         Bitrate information is not explicitly saved.
         You can use file size and duration as a proxy for throughput:
         library watch -w 'size/duration<50000'
```

