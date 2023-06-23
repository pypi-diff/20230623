# Comparing `tmp/pyadlml-0.0.7.9a0.tar.gz` & `tmp/pyadlml-0.0.8.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyadlml-0.0.7.9a0.tar", last modified: Mon Nov 14 13:29:39 2022, max compression
+gzip compressed data, was "pyadlml-0.0.8.0a0.tar", last modified: Fri Jun 23 08:38:04 2023, max compression
```

## Comparing `pyadlml-0.0.7.9a0.tar` & `pyadlml-0.0.8.0a0.tar`

### file list

```diff
@@ -1,150 +1,170 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.980399 pyadlml-0.0.7.9a0/
--rw-r--r--   0 chris     (1000) chris     (1000)        8 2020-10-29 09:58:19.000000 pyadlml-0.0.7.9a0/MANIFEST.in
--rw-rw-r--   0 chris     (1000) chris     (1000)     8272 2022-11-14 13:29:39.980399 pyadlml-0.0.7.9a0/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     6164 2022-10-26 18:21:17.000000 pyadlml-0.0.7.9a0/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.964399 pyadlml-0.0.7.9a0/pyadlml/
--rw-r--r--   0 chris     (1000) chris     (1000)      774 2022-10-26 19:47:31.000000 pyadlml-0.0.7.9a0/pyadlml/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2735 2021-08-16 09:39:57.000000 pyadlml-0.0.7.9a0/pyadlml/benchmark.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      743 2022-10-21 09:41:03.000000 pyadlml-0.0.7.9a0/pyadlml/constants.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.964399 pyadlml-0.0.7.9a0/pyadlml/dataset/
--rw-r--r--   0 chris     (1000) chris     (1000)      827 2022-10-26 19:48:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.968399 pyadlml-0.0.7.9a0/pyadlml/dataset/_core/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-01-16 14:29:28.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_core/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3723 2022-11-10 08:12:28.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_core/_dataset.py
--rw-r--r--   0 chris     (1000) chris     (1000)    17657 2022-11-13 10:03:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_core/activities.py
--rw-r--r--   0 chris     (1000) chris     (1000)    29737 2022-11-10 08:15:15.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_core/devices.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7431 2022-10-28 13:22:22.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_core/obj.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.968399 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-10-19 16:38:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3551 2022-11-14 11:15:15.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/activity_assistant.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5714 2022-10-28 21:53:36.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/amsterdam.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7335 2022-11-11 12:45:06.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/aras.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6857 2022-03-26 11:45:38.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/casas_aruba.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4278 2022-10-18 20:14:29.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/homeassistant.py
--rw-r--r--   0 chris     (1000) chris     (1000)     9878 2022-11-13 10:04:34.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/kasteren_2010.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7216 2022-02-27 20:26:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/mitlab.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1888 2022-02-27 15:21:23.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/tuebingen_2019.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5604 2022-02-27 20:26:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/uci_adl_binary.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.968399 pyadlml-0.0.7.9a0/pyadlml/dataset/_representations/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-10-29 10:44:22.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_representations/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1755 2022-03-26 11:45:38.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_representations/changepoint.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2389 2022-03-26 11:45:38.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_representations/lastfired.py
--rw-r--r--   0 chris     (1000) chris     (1000)    16185 2022-03-26 11:45:38.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/_representations/raw.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.968399 pyadlml-0.0.7.9a0/pyadlml/dataset/bokeh/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-06-08 12:41:16.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/bokeh/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    26262 2022-02-26 17:55:45.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/bokeh/activities.py
--rw-r--r--   0 chris     (1000) chris     (1000)    13816 2022-11-04 08:18:29.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/io.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.968399 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-07-29 16:09:37.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    16891 2022-11-11 10:22:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/act_and_devs.py
--rw-r--r--   0 chris     (1000) chris     (1000)    20932 2022-07-19 11:48:50.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/activities.py
--rw-r--r--   0 chris     (1000) chris     (1000)    32382 2022-11-11 10:22:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/devices.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4498 2020-12-25 12:52:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/discrete.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3460 2020-09-02 22:18:42.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/image.py
--rw-r--r--   0 chris     (1000) chris     (1000)    40971 2022-11-11 09:54:13.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.968399 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-10-29 10:44:42.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     8582 2022-02-27 15:41:43.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/activities.py
--rw-r--r--   0 chris     (1000) chris     (1000)    34211 2022-11-14 13:19:31.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/acts_and_devs.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/dashboard/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2022-11-13 22:17:20.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/dashboard/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7895 2022-11-13 09:30:23.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/dashboard/callbacks.py
--rw-r--r--   0 chris     (1000) chris     (1000)    39517 2022-11-13 09:38:08.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/dashboard/dashboard.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    36938 2022-11-11 19:28:09.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/dashboard/layout.py
--rw-r--r--   0 chris     (1000) chris     (1000)     8661 2022-03-26 11:45:39.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/devices.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5782 2022-11-12 16:55:09.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/dataset/stats/
--rw-r--r--   0 chris     (1000) chris     (1000)      880 2021-08-19 19:01:44.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/stats/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    14163 2022-11-13 09:16:51.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/stats/activities.py
--rw-r--r--   0 chris     (1000) chris     (1000)    18770 2022-11-10 08:13:02.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/stats/acts_and_devs.py
--rw-r--r--   0 chris     (1000) chris     (1000)    20860 2022-11-10 08:13:32.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/stats/devices.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2529 2020-12-24 16:41:19.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/stats/discrete.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2481 2022-03-26 11:45:38.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/stats/util.py
--rw-r--r--   0 chris     (1000) chris     (1000)    28389 2022-11-13 10:24:28.000000 pyadlml-0.0.7.9a0/pyadlml/dataset/util.py
--rw-r--r--   0 chris     (1000) chris     (1000)    10134 2022-02-27 15:13:21.000000 pyadlml-0.0.7.9a0/pyadlml/feature_extraction.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1786 2020-09-02 22:18:54.000000 pyadlml-0.0.7.9a0/pyadlml/feature_selection.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7825 2021-06-29 14:23:16.000000 pyadlml-0.0.7.9a0/pyadlml/metrics.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/model/
--rw-r--r--   0 chris     (1000) chris     (1000)       95 2021-07-03 07:55:55.000000 pyadlml-0.0.7.9a0/pyadlml/model/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    14720 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/_model.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/model/hbhmm/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/hbhmm/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    11921 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/hbhmm/hmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)     8911 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/hbhmm/pchmm.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/model/hmm/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/hmm/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    12315 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/hmm/_model_categorical.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6056 2022-02-26 12:12:51.000000 pyadlml-0.0.7.9a0/pyadlml/model/hmm/bhmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3859 2022-02-26 12:12:51.000000 pyadlml-0.0.7.9a0/pyadlml/model/hmm/bhmm_hp.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6736 2022-02-26 12:12:51.000000 pyadlml-0.0.7.9a0/pyadlml/model/hmm/bhsmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6074 2022-02-26 12:12:51.000000 pyadlml-0.0.7.9a0/pyadlml/model/hmm/hmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)     9413 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/hmm/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/model/rnn/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-07-03 07:24:43.000000 pyadlml-0.0.7.9a0/pyadlml/model/rnn/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3398 2021-08-23 09:10:35.000000 pyadlml-0.0.7.9a0/pyadlml/model/rnn/rnn.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/model/transformer/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-08-16 15:10:00.000000 pyadlml-0.0.7.9a0/pyadlml/model/transformer/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1684 2021-08-16 15:10:29.000000 pyadlml-0.0.7.9a0/pyadlml/model/transformer/layers.py
--rw-r--r--   0 chris     (1000) chris     (1000)      705 2020-05-21 17:07:26.000000 pyadlml-0.0.7.9a0/pyadlml/model/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/model/vrnn/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2021-02-05 21:01:34.000000 pyadlml-0.0.7.9a0/pyadlml/model/vrnn/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)      183 2021-02-05 22:06:01.000000 pyadlml-0.0.7.9a0/pyadlml/model/vrnn/classifying_vrnn.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4513 2021-03-12 12:10:19.000000 pyadlml-0.0.7.9a0/pyadlml/model/vrnn/vrnn.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.972399 pyadlml-0.0.7.9a0/pyadlml/model_selection/
--rw-r--r--   0 chris     (1000) chris     (1000)      113 2021-08-16 12:17:10.000000 pyadlml-0.0.7.9a0/pyadlml/model_selection/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    31628 2022-11-10 08:15:51.000000 pyadlml-0.0.7.9a0/pyadlml/model_selection/_search.py
--rw-r--r--   0 chris     (1000) chris     (1000)    19896 2021-08-29 15:00:49.000000 pyadlml-0.0.7.9a0/pyadlml/model_selection/_split.py
--rw-r--r--   0 chris     (1000) chris     (1000)    33208 2022-11-10 08:14:54.000000 pyadlml-0.0.7.9a0/pyadlml/pipeline.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.976399 pyadlml-0.0.7.9a0/pyadlml/plot/
--rw-r--r--   0 chris     (1000) chris     (1000)     1784 2022-02-26 21:27:23.000000 pyadlml-0.0.7.9a0/pyadlml/plot/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5984 2022-02-26 12:12:51.000000 pyadlml-0.0.7.9a0/pyadlml/plot/_benchmark.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3935 2020-05-21 17:04:42.000000 pyadlml-0.0.7.9a0/pyadlml/plot/explanation.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2695 2020-05-21 17:04:42.000000 pyadlml-0.0.7.9a0/pyadlml/plot/feature_importance.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6752 2020-05-28 14:58:05.000000 pyadlml-0.0.7.9a0/pyadlml/plot/interpretation.py
--rw-r--r--   0 chris     (1000) chris     (1000)    25582 2022-03-26 11:45:39.000000 pyadlml-0.0.7.9a0/pyadlml/preprocessing.py
--rw-r--r--   0 chris     (1000) chris     (1000)      849 2021-10-28 15:24:21.000000 pyadlml-0.0.7.9a0/pyadlml/stats.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1306 2020-12-24 20:43:33.000000 pyadlml-0.0.7.9a0/pyadlml/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.964399 pyadlml-0.0.7.9a0/pyadlml.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)     8272 2022-11-14 13:29:39.000000 pyadlml-0.0.7.9a0/pyadlml.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     4001 2022-11-14 13:29:39.000000 pyadlml-0.0.7.9a0/pyadlml.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2022-11-14 13:29:39.000000 pyadlml-0.0.7.9a0/pyadlml.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      264 2022-11-14 13:29:39.000000 pyadlml-0.0.7.9a0/pyadlml.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       24 2022-11-14 13:29:39.000000 pyadlml-0.0.7.9a0/pyadlml.egg-info/top_level.txt
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.976399 pyadlml-0.0.7.9a0/scripts/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 17:02:55.000000 pyadlml-0.0.7.9a0/scripts/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1703 2022-02-21 21:37:20.000000 pyadlml-0.0.7.9a0/scripts/generate_dataset_info.py
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2022-11-14 13:29:39.980399 pyadlml-0.0.7.9a0/setup.cfg
--rw-r--r--   0 chris     (1000) chris     (1000)     1664 2022-11-14 13:23:30.000000 pyadlml-0.0.7.9a0/setup.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.976399 pyadlml-0.0.7.9a0/testing/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.976399 pyadlml-0.0.7.9a0/testing/models/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.976399 pyadlml-0.0.7.9a0/testing/models/hmm/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hmm/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5253 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hmm/testing_hass_forwardhmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)    10706 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hmm/testing_hass_pchmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)    12916 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hmm/testing_homeassistant.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7011 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hmm/testing_kasteren.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6855 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hmm/testing_kasteren_pom.py
--rw-r--r--   0 chris     (1000) chris     (1000)     8518 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hmm/testing_pendigits.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2022-11-14 13:29:39.980399 pyadlml-0.0.7.9a0/testing/models/hsmm/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hsmm/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6932 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hsmm/testing_kasteren_hsmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)    10437 2020-05-21 08:54:05.000000 pyadlml-0.0.7.9a0/testing/models/hsmm/testing_pyhsmm.py
--rw-r--r--   0 chris     (1000) chris     (1000)    11793 2022-02-26 12:12:51.000000 pyadlml-0.0.7.9a0/testing/models/hsmm/testing_ssm.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3045 2021-08-22 19:43:50.000000 pyadlml-0.0.7.9a0/testing/test_crossval.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2052 2021-04-27 13:28:35.000000 pyadlml-0.0.7.9a0/testing/test_dataset_amsterdam.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2091 2021-04-28 07:06:03.000000 pyadlml-0.0.7.9a0/testing/test_dataset_aras.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6888 2021-08-14 20:00:22.000000 pyadlml-0.0.7.9a0/testing/test_dataset_base.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1589 2021-04-27 13:36:49.000000 pyadlml-0.0.7.9a0/testing/test_dataset_casas_aruba.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5925 2021-08-14 20:00:22.000000 pyadlml-0.0.7.9a0/testing/test_dataset_dirty.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7272 2021-08-14 20:00:22.000000 pyadlml-0.0.7.9a0/testing/test_dataset_empty_partial.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2816 2021-04-27 13:38:30.000000 pyadlml-0.0.7.9a0/testing/test_dataset_mitlab.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1606 2021-04-28 07:23:55.000000 pyadlml-0.0.7.9a0/testing/test_dataset_tuebingen2019.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2889 2021-04-28 07:23:16.000000 pyadlml-0.0.7.9a0/testing/test_dataset_uci_adl_binary.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1381 2021-03-13 11:57:30.000000 pyadlml-0.0.7.9a0/testing/test_feature_extraction.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1571 2021-04-23 20:32:20.000000 pyadlml-0.0.7.9a0/testing/test_gridsearch.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1890 2021-01-14 11:07:32.000000 pyadlml-0.0.7.9a0/testing/test_imports.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4008 2021-04-23 20:32:20.000000 pyadlml-0.0.7.9a0/testing/test_pipeline.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2730 2021-06-29 09:26:25.000000 pyadlml-0.0.7.9a0/testing/test_preprocessing.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3281 2021-10-28 08:54:13.000000 pyadlml-0.0.7.9a0/testing/test_utils.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.201040 pyadlml-0.0.8.0a0/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        8 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/MANIFEST.in
+-rw-rw-r--   0 chris     (1001) chris     (1001)    11573 2023-06-23 08:38:04.201040 pyadlml-0.0.8.0a0/PKG-INFO
+-rw-rw-r--   0 chris     (1001) chris     (1001)     8905 2023-06-23 08:18:44.000000 pyadlml-0.0.8.0a0/README.md
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.193040 pyadlml-0.0.8.0a0/pyadlml/
+-rw-rw-r--   0 chris     (1001) chris     (1001)      666 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     2754 2023-05-31 20:45:41.000000 pyadlml-0.0.8.0a0/pyadlml/benchmark.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1657 2023-06-22 07:01:01.000000 pyadlml-0.0.8.0a0/pyadlml/constants.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.193040 pyadlml-0.0.8.0a0/pyadlml/dataset/
+-rw-rw-r--   0 chris     (1001) chris     (1001)      857 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/__init__.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.193040 pyadlml-0.0.8.0a0/pyadlml/dataset/_core/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_core/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    23202 2023-06-06 13:13:08.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_core/activities.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     6494 2023-06-19 15:53:02.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_core/acts_and_devs.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    36000 2023-06-22 14:52:40.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_core/devices.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.193040 pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     6522 2023-06-22 11:33:54.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/activity_assistant.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     5418 2023-06-22 11:28:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/amsterdam.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     7291 2023-06-22 11:30:15.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/aras.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    27463 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/casas_houses.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     4437 2023-06-22 11:31:08.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/homeassistant.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    11883 2023-06-22 11:32:07.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/kasteren_2010.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     8146 2023-06-22 11:32:35.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/mitlab.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     2318 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/tuebingen_2019.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     7664 2023-06-22 14:52:22.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/uci_adl_binary.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.193040 pyadlml-0.0.8.0a0/pyadlml/dataset/_representations/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_representations/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     2098 2023-06-22 11:50:16.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_representations/changepoint.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1683 2023-06-22 14:46:21.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_representations/lastfired.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     9783 2023-06-22 17:51:23.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/_representations/state.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)      338 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/act_assist.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.193040 pyadlml-0.0.8.0a0/pyadlml/dataset/cleaning/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/cleaning/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    13477 2023-06-08 05:43:28.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/cleaning/misc.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1424 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/cleaning/util.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.193040 pyadlml-0.0.8.0a0/pyadlml/dataset/io/
+-rw-rw-r--   0 chris     (1001) chris     (1001)      257 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/io/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     2982 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/io/downloader.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     8893 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/io/io.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     4266 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/io/local.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     5961 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/io/remote.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.197040 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/__init__.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.197040 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/_bokeh/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/_bokeh/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    26224 2023-05-31 20:45:41.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/_bokeh/activities.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/_bokeh/util.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.197040 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/matplotlib/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/matplotlib/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    17067 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/matplotlib/act_and_devs.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    20216 2023-05-31 20:45:41.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/matplotlib/activities.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    32444 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/matplotlib/devices.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     6681 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/matplotlib/discrete.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     3460 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/matplotlib/image.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    43533 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/matplotlib/util.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.197040 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/plotly/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/plotly/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    15429 2023-06-22 07:00:57.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/plotly/activities.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    40108 2023-06-22 07:00:57.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/plotly/acts_and_devs.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.197040 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/plotly/dashboard/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/plotly/dashboard/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    19572 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/plotly/dashboard/callbacks.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    36962 2023-05-21 18:24:36.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/plotly/dashboard/dashboard.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    44648 2023-06-08 13:50:38.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/plotly/dashboard/layout.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    14992 2023-06-22 07:00:57.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/plotly/devices.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    16017 2023-06-22 07:00:57.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/plotly/discrete.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    11337 2023-06-22 07:00:57.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/plotly/util.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)      898 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/plot/util.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.197040 pyadlml-0.0.8.0a0/pyadlml/dataset/stats/
+-rw-rw-r--   0 chris     (1001) chris     (1001)      880 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/stats/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    14684 2023-06-06 13:13:08.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/stats/activities.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    24923 2023-06-22 14:52:27.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/stats/acts_and_devs.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    30726 2023-06-22 14:52:34.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/stats/devices.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     2609 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/stats/discrete.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     2490 2023-06-22 14:52:13.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/stats/util.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    10979 2023-06-06 13:13:08.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/torch.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    32350 2023-06-22 14:52:20.000000 pyadlml-0.0.8.0a0/pyadlml/dataset/util.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    10976 2023-06-22 14:52:09.000000 pyadlml-0.0.8.0a0/pyadlml/feature_extraction.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1806 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/feature_selection.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    10421 2023-06-08 12:06:41.000000 pyadlml-0.0.8.0a0/pyadlml/metrics.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.197040 pyadlml-0.0.8.0a0/pyadlml/ml_viz/
+-rw-rw-r--   0 chris     (1001) chris     (1001)     4561 2023-06-06 13:13:08.000000 pyadlml-0.0.8.0a0/pyadlml/ml_viz/__init__.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.197040 pyadlml-0.0.8.0a0/pyadlml/model/
+-rw-rw-r--   0 chris     (1001) chris     (1001)    10220 2023-04-24 11:53:21.000000 pyadlml-0.0.8.0a0/pyadlml/model/WaveNet.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)      167 2023-04-24 11:53:21.000000 pyadlml-0.0.8.0a0/pyadlml/model/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    14720 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/_model.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    15507 2023-05-09 20:46:40.000000 pyadlml-0.0.8.0a0/pyadlml/model/dummy.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.197040 pyadlml-0.0.8.0a0/pyadlml/model/hbhmm/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/hbhmm/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    11921 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/hbhmm/hmm.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     8911 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/hbhmm/pchmm.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.197040 pyadlml-0.0.8.0a0/pyadlml/model/hmm/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/hmm/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    12315 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/hmm/_model_categorical.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     6056 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/hmm/bhmm.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     3859 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/hmm/bhmm_hp.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     6736 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/hmm/bhsmm.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     6074 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/hmm/hmm.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     9413 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/hmm/util.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1178 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/mlp.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.197040 pyadlml-0.0.8.0a0/pyadlml/model/nn/
+-rw-rw-r--   0 chris     (1001) chris     (1001)       19 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/nn/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     6068 2023-04-24 11:53:21.000000 pyadlml-0.0.8.0a0/pyadlml/model/nn/util.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.197040 pyadlml-0.0.8.0a0/pyadlml/model/rnn/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/rnn/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     3426 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/rnn/rnn.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.197040 pyadlml-0.0.8.0a0/pyadlml/model/tpp/
+-rw-rw-r--   0 chris     (1001) chris     (1001)       28 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/tpp/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1004 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/tpp/util.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.197040 pyadlml-0.0.8.0a0/pyadlml/model/transformer/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/transformer/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    13472 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/transformer/vanilla.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)      705 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/util.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.201040 pyadlml-0.0.8.0a0/pyadlml/model/vrnn/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/vrnn/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)      183 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/vrnn/classifying_vrnn.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     4513 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model/vrnn/vrnn.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.201040 pyadlml-0.0.8.0a0/pyadlml/model_selection/
+-rw-rw-r--   0 chris     (1001) chris     (1001)       90 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model_selection/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    31440 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/model_selection/_search.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    29250 2023-06-22 07:00:57.000000 pyadlml-0.0.8.0a0/pyadlml/model_selection/_split.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    36991 2023-06-06 13:13:08.000000 pyadlml-0.0.8.0a0/pyadlml/pipeline.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.201040 pyadlml-0.0.8.0a0/pyadlml/plot/
+-rw-rw-r--   0 chris     (1001) chris     (1001)     2225 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/plot/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     5984 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/plot/_benchmark.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     3935 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/plot/explanation.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     2695 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/plot/feature_importance.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     6752 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/pyadlml/plot/interpretation.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.201040 pyadlml-0.0.8.0a0/pyadlml/preprocessing/
+-rw-rw-r--   0 chris     (1001) chris     (1001)      436 2023-06-16 07:55:39.000000 pyadlml-0.0.8.0a0/pyadlml/preprocessing/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    34833 2023-06-22 15:09:06.000000 pyadlml-0.0.8.0a0/pyadlml/preprocessing/preprocessing.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    40386 2023-06-23 08:08:32.000000 pyadlml-0.0.8.0a0/pyadlml/preprocessing/windows.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)      999 2023-04-26 21:06:39.000000 pyadlml-0.0.8.0a0/pyadlml/stats.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.201040 pyadlml-0.0.8.0a0/pyadlml/training/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-05-15 07:49:50.000000 pyadlml-0.0.8.0a0/pyadlml/training/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    17301 2023-06-16 07:55:39.000000 pyadlml-0.0.8.0a0/pyadlml/training/trainable.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1780 2023-06-06 13:13:08.000000 pyadlml-0.0.8.0a0/pyadlml/util.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.193040 pyadlml-0.0.8.0a0/pyadlml.egg-info/
+-rw-rw-r--   0 chris     (1001) chris     (1001)    11573 2023-06-23 08:38:04.000000 pyadlml-0.0.8.0a0/pyadlml.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1001) chris     (1001)     4275 2023-06-23 08:38:04.000000 pyadlml-0.0.8.0a0/pyadlml.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1001) chris     (1001)        1 2023-06-23 08:38:04.000000 pyadlml-0.0.8.0a0/pyadlml.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1001) chris     (1001)      270 2023-06-23 08:38:04.000000 pyadlml-0.0.8.0a0/pyadlml.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1001) chris     (1001)       30 2023-06-23 08:38:04.000000 pyadlml-0.0.8.0a0/pyadlml.egg-info/top_level.txt
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.201040 pyadlml-0.0.8.0a0/scripts/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/scripts/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)       38 2023-06-23 08:38:04.201040 pyadlml-0.0.8.0a0/setup.cfg
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1700 2023-06-23 08:37:32.000000 pyadlml-0.0.8.0a0/setup.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.201040 pyadlml-0.0.8.0a0/testing/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/testing/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1828 2023-04-29 07:01:01.000000 pyadlml-0.0.8.0a0/testing/test_imports.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     2742 2023-06-06 13:13:08.000000 pyadlml-0.0.8.0a0/testing/test_metrics.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     4293 2023-06-16 07:55:39.000000 pyadlml-0.0.8.0a0/testing/test_pipeline.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     4579 2023-04-29 07:30:30.000000 pyadlml-0.0.8.0a0/testing/test_stats.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     4544 2023-06-06 13:13:08.000000 pyadlml-0.0.8.0a0/testing/test_utils.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.201040 pyadlml-0.0.8.0a0/tools/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/tools/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    17307 2023-06-22 07:00:57.000000 pyadlml-0.0.8.0a0/tools/clean_device_signals.py
+drwxrwxr-x   0 chris     (1001) chris     (1001)        0 2023-06-23 08:38:04.201040 pyadlml-0.0.8.0a0/tools/configs/
+-rw-rw-r--   0 chris     (1001) chris     (1001)        0 2023-04-24 11:53:21.000000 pyadlml-0.0.8.0a0/tools/configs/__init__.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1476 2023-06-06 13:13:08.000000 pyadlml-0.0.8.0a0/tools/configs/models.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)      794 2023-06-16 07:55:39.000000 pyadlml-0.0.8.0a0/tools/configs/pipes.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    14329 2023-06-22 07:00:57.000000 pyadlml-0.0.8.0a0/tools/correct_activities.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     2090 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/tools/dashboard.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1949 2023-04-18 19:30:30.000000 pyadlml-0.0.8.0a0/tools/generate_dataset_info.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     3315 2023-06-16 07:55:39.000000 pyadlml-0.0.8.0a0/tools/hparam_sweep.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    36334 2023-06-22 14:52:07.000000 pyadlml-0.0.8.0a0/tools/label_data.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     1668 2023-06-16 07:55:39.000000 pyadlml-0.0.8.0a0/tools/train.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)    22561 2023-06-19 13:05:34.000000 pyadlml-0.0.8.0a0/tools/train_debug.py
+-rw-rw-r--   0 chris     (1001) chris     (1001)     8199 2023-06-16 07:55:39.000000 pyadlml-0.0.8.0a0/tools/train_debug_sktime.py
```

### Comparing `pyadlml-0.0.7.9a0/README.md` & `pyadlml-0.0.8.0a0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -2,153 +2,222 @@
 > Contains data preprocessing and visualization methods for ADL datasets.
 
 ![PyPI version](https://img.shields.io/pypi/v/pyadlml?style=flat-square)
 ![Download Stats](https://img.shields.io/pypi/dd/pyadlml?style=flat-square)
 ![Read the Docs (version)](https://img.shields.io/readthedocs/pyadlml/latest?style=flat-square)
 ![License](https://img.shields.io/pypi/l/pyadlml?style=flat-square)
 <p align="center"><img width=95% src="https://github.com/tcsvn/pyadlml/blob/master/media/pyadlml_banner.png"></p>
-Activities of Daily living (ADLs) e.g cooking, working, sleeping and device readings are recorded by Smart 
-Home inhabitants. 
+Activities of Daily living (ADLs) such as eating, working, sleeping and Smart Home device readings are recorded by inhabitants. Predicting resident activities based on the device event-stream allows for a range of applications, including automation, action recommendation and abnormal activity detection in the context of assisted living for elderly inhabitants. Pyadlml offers an easy way to fetch, visualize and preprocess common datasets.
 
-The objective is to predict inhabitants activities using the device readings.
-Pyadlml offers an easy way to fetch, visualize and preprocess common datasets. Furthermore 
-a pipeline and TODO
 
 ## !! Disclaimer !!
-Package is still an alpha-version and in active development. 
-Consequently, things are going to change and break and may not work at all. 
-Nevertheless, feel free to take a look the package and use what is already finished.
+Package is still an alpha-version and under active development. 
+As of now do not expect anything to work! APIs are going to change, 
+stuff breaks and the documentation may lack behind. Nevertheless, feel 
+free to take a look. The safest point to start is probably the API reference.
 
-## Last Stable Release
+## Last (stable) Release
 ```sh 
 $ pip install pyadlml
 ```
 ## Latest Development Changes
 ```sh
 $ git clone https://github.com/tcsvn/pyadlml
 $ cd pyadlml
 $ pip install .
 ```
 
 ## Usage example
 
-```python
-from pyadlml.dataset import fetch_amsterdam
 
+### Simple
+
+```python
 # Fetch dataset
+from pyadlml.dataset import fetch_amsterdam
 data = fetch_amsterdam()
+df_devs, df_acts = data['devices'], data['activities']
 
-# Plot an inhabitants activity density distribution over one day
-from pyadlml.plot import density
-
-density(data.df_activities)
-
-# Plot a cross-correlogram to visualize temporal dependency of events
-from pyadlml.plot import plot_device_cross_correlogram
 
-plot_device_cross_correlogram(data.df_devices)
+# Plot the residents activity density over one day
+from pyadlml.plot import plot_activity_density
+fig = plot_activity_density(df_acts)
+fig.show()
 
-# Create a vector of smart home device states and discretize the event data in 20 second bins
-from pyadlml.preprocessing import StateVectorEncoder, LabelEncoder
 
-sve = StateVectorEncoder(encoding='raw', dt='20s')
-raw = sve.fit_transform(data.df_devices)
+# Create a vector representing the state of all Smart Home devices
+# at a certain time and discretize the events into 20 second bins
+from pyadlml.preprocessing import Event2Vec, LabelMatcher
+e2v = Event2Vec(encode='state', dt='20s')
+states = e2v.fit_transform(df_devs)
 
-# Label the datapoints with the corresponding activity
-lbls = LabelEncoder().fit_transform(data.df_activities, raw)
+# Label each datum with the corresponding activity.
+# When an event matches no activity set the activity to "other"
+lbls = LabelMatcher(other=True).fit_transform(df_acts, states)
 
-X = raw.values
-y = lbls.values
+# Extract numpy arrays without timestamps (1st column)
+X, y = states.values[:,1:], lbls.values[:,1:]
 
-# Proceed with machine learning techniques you already know
+# Proceed with machine learning stuff 
 from sklearn.tree import DecisionTreeClassifier
-
 clf = DecisionTreeClassifier()
 clf.fit(X, y)
+clf.score(X, y)
+...
+```
+
+### Less simple
+
+
+```python
+from pyadlml.dataset import fetch_amsterdam
+from pyadlml.constants import VALUE
+from pyadlml.pipeline import Pipeline
+from pyadlml.preprocessing import IndexEncoder, LabelMatcher, DropTimeIndex, \
+                                  EventWindows, DropColumn
+from pyadlml.model_selection import train_test_split
+from pyadlml.model import DilatedModel
+from pyadlml.dataset.torch import TorchDataset
+from torch.utils.data import DataLoader
+from torch.optim import Adam 
+from torch.nn import functional as F
+
+# Featch data and split into train/val/test based on time rather than #events
+data = fetch_amsterdam()
+X_train, X_val, X_test, y_train, y_val, y_test = train_test_split(
+    data['devices'], data['activities'], \
+    split=(0.6, 0.2, 0.2), temporal=True,
+)
+
+# Formulate all preprocessing steps using a sklearn styled pipeline 
+pipe = Pipeline([
+    ('enc', IndexEncoder()),            # Encode devices strings with indices
+    ('drop_obs', DropColumn(VALUE)),    # Disregard device observations
+    ('lbl', LabelMatcher(other=True)),  # Generate labels y  
+    ('drop_time', DropTimeIndex()),     # Remove timestamps for x and y
+    ('windows', EventWindows(           # Create sequences S with a sliding window
+                  rep='many-to-one',    # Only one label y_i per sequence S_i
+                  window_size=16,       # Each sequence contains 16 events 
+                  stride=2)),           # A sequence is created every 2 events
+    ('passthrough', 'passthrough')      # Do not use a classifier in the pipeline
+])
+
+# Create a dataset to sample from
+dataset = TorchDataset(X_train, y_train, pipe) 
+train_loader = DataLoader(dataset, batch_size=32, shuffle=True)
+model = DilatedModel(
+    n_features=14,       # Number of devices
+    n_classes=8          # Number of activities
+)
+optimizer = Adam(model.parameters(), lr=3e-4)
+
+# Minimal loop to overfit the data
+for s in range(10000):
+    for (Xb, yb) in train_loader:
+        optimizer.zero_grad()
+        logits = model(Xb)
+        loss = F.cross_entropy(logits, yb)
+        loss.backward()
+        optimizer.step()
+
 ...
 ```
 
-_For more examples and how to use, please refer to the [documentation](https://pyadlml.readthedocs.io/en/latest/)
-or the [notebooks](https://github.com/tcsvn/pyadlml/notebooks/README.md)._
+
+
+_For more examples and how to use, please refer to the [documentation](https://pyadlml.readthedocs.io/en/latest/)._
+
 ## Features
-  - 12 Datasets
-  - Many visualizations depicting devices, activities and their interaction
-  - Different device representations:
-      - Raw
-      - Changepoint
-      - Lastfired
-  - Timeseries transformations:
-    - Sequential
-    - Timeslice/grid
-    - Event based
-  - Feature extraction based on the time devices produce events 
-  - Full fledged pipeline to create production ready models
-  - Cross validation and Grid-search adapted to the task of predicting ADLs
-  - Importing data from [Home Assistant](todo) or [Activity Assistant](todo)
-  - Ready-to-use models providing a friction less start:
-    - Hidden Markov Model
-    - Recurrent Neural Net
-    - 
+  - Access to 14 Datasets 
+  - Importing data from [Home Assistant](https://www.home-assistant.io/) or [Activity Assistant](https://github.com/tcsvn/activity-assistant)
+  - Tools for data cleaning
+    - Relabel activities and devices
+    - Merge overlapping activities
+    - Find and replace specific patterns in device signals
+    - Interactive dashboard for data exploration
+  - Various statistics and visualizations for devices, activities and their interaction
+  - Preprocessing methods
+    - Device encoder (index, state, changepoint, last_fired, ...)
+    - Feature extraction (inter-event-times, intensity, time2vec, ...)
+    - Sliding windows (event, temporal, explicit or (fuzzytime))
+    - Many more ... 
+  - Cross validation iterators and pipeline adapted for ADLs
+    - LeaveKDayOutSplit, TimeSeriesSplit
+    - Conditional transformer: YTransformer, XorYTransformer, ...
+  - Online metrics to compare models regardless of resample frequency
+    - Accuracy, TPR, PPV, ConfMat, Calibration
+  - Ready to use models (TODO)
+    - RNNs
+    - WaveNet
+    - Transformer
+  - Translate datasets to sktime formats
  
 ### Supported Datasets
   - [x] Amsterdam [1]
   - [x] Aras [2]
   - [x] Casas Aruba (2011) [3]
+  - [X] Casas Cairo [4]
+  - [X] Casas Milan (2009) [4]
+  - [X] Casas Tulum [4]
+  - [X] Casas Kyoto (2010) [4]
   - [x] Kasteren House A,B,C [5]
   - [x] MITLab [6]
-  - [x] Tuebingen 2019 [7]
   - [x] UCI Adl Binary [8]
-  - [ ] Casas Milan (2009) [4]
-  - [ ] Casas Cairo [4]
-  - [ ] Casas Tokyo [4]
   - [ ] Chinokeeh [9]
+  - [ ] Orange [TODO]
 
-## Educational examples, benchmarks and replications
-The project includes a leaderboard of current models to the best of knowledge. 
-In addition, a lot of models are compared on a cleaned version of all the available datasets. 
-Furthermore, there is a useful list of references that is still 
-growing on papers to read. 
-For all this check out the [notebooks]().
+## Examples, benchmarks and replications
+The project includes (TODO) a ranked model leaderboard evaluated on the cleaned dataset versions.
+Additionaly, here is a useful list of awesome references (todo include link) to papers
+and repos related to ADLs and machine learning.
 
 
 ## Contributing 
 1. Fork it (<https://github.com/tcsvn/pyadlml/fork>)
 2. Create your feature branch (`git checkout -b feature/fooBar`)
 3. Commit your changes (`git commit -am 'Add some fooBar'`)
 4. Push to the branch (`git push origin feature/fooBar`)
 5. Create a new Pull Request
 
 ## Related projects
-  - [Activity-assistant](https://github.com/tcsvn/activity-assistant) - Recording, predicting ADLs within Home assistant.
-  - [Sci-kit learn](https://github.com/sklearn) - The main inspiration and some borrowed source of code.
+  - [Activity Assistant](https://github.com/tcsvn/activity-assistant) - Recording, predicting ADLs within Home assistant.
+  - [Sci-kit learn](https://github.com/sklearn) - The main inspiration and some borrowed source code.
   
 ## Support 
 [![Buy me a coffee][buy-me-a-coffee-shield]][buy-me-a-coffee]
   
 ## How to cite
 If you are using pyadlml for publications consider citing the package
 ```
-@software{activity-assistant,
+@software{pyadlml,
   author = {Christian Meier},
-  title = {Pyadlml - Machine Learning for Activities of Daily Living},    
+  title = {PyADLMl - Machine Learning library for Activities of Daily Living},    
   url = {https://github.com/tcsvn/pyadlml},
-  version = {0.0.7-alpha},
-  date = {2021-08-15}
+  version = {0.0.22-alpha},
+  date = {2023-01-03}
 }
 ```
 
 ## Sources
+
+#### Dataset
+
+
 [1]: T.L.M. van Kasteren; A. K. Noulas; G. Englebienne and B.J.A. Kroese, Tenth International Conference on Ubiquitous Computing 2008  
 [2]: H. Alemdar, H. Ertan, O.D. Incel, C. Ersoy, ARAS Human Activity Datasets in Multiple Homes with Multiple Residents, Pervasive Health, Venice, May 2013.  
 [3,4]: WSU CASAS smart home project: D. Cook. Learning setting-generalized activity models for smart spaces. IEEE Intelligent Systems, 2011.  
 [5]: Transferring Knowledge of Activity Recognition across Sensor networks. Eighth International Conference on Pervasive Computing. Helsinki, Finland, 2010.  
 [6]: E. Munguia Tapia. Activity Recognition in the Home Setting Using Simple and Ubiquitous sensors. S.M Thesis  
 [7]: Activity Recognition in Smart Home Environments using Hidden Markov Models. Bachelor Thesis. Uni Tuebingen.   
 [8]: Ordonez, F.J.; de Toledo, P.; Sanchis, A. Activity Recognition Using Hybrid Generative/Discriminative Models on Home Environments Using Binary Sensors. Sensors 2013, 13, 5460-5477.  
 [9]: D. Cook and M. Schmitter-Edgecombe, Assessing the quality of activities in a smart environment. Methods of information in Medicine, 2009
-  
+
+#### Software
+
+TODO add software used in TPPs 
+
 ## License
 MIT  © [tcsvn](http://deadlink)
 
 
 [buy-me-a-coffee-shield]: https://img.shields.io/static/v1.svg?label=%20&message=Buy%20me%20a%20coffee&color=6f4e37&logo=buy%20me%20a%20coffee&logoColor=white
 [buy-me-a-coffee]: https://www.buymeacoffee.com/tscvn
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/benchmark.py` & `pyadlml-0.0.8.0a0/pyadlml/benchmark.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pyadlml.model_selection import train_test_split, KFold, GridSearchCV
 from pyadlml.pipeline import Pipeline
-from pyadlml.preprocessing import LabelEncoder, CVSubset
+from pyadlml.preprocessing import LabelMatcher, CrossValSplitter
 
 
 def evaluate(data, param_grid, pipeline_steps, n_jobs=6):
     """ High level evaluation method that builds a pipeline from gs_steps does a train
         test split with leave one day out. Then the best parameters are found using
         grid-search. The best model is initialized with best_model_steps and gets
         assigned the best_model_steps
@@ -27,15 +27,15 @@
         the best model
 
     """
     print('splitting data in train and test set...')
     X_train, X_test, y_train, y_test, y_pre_vals = train_test_split(
         data.df_devices,
         data.df_activities,
-        return_pre_vals=True,
+        return_init_states=True,
         split='leave_one_day_out')
 
 
     print('Grid Search to determine best parameters...')
     ts = KFold()
     pipe = Pipeline(pipeline_steps).train()
     gscv = GridSearchCV(
@@ -51,15 +51,15 @@
     gscv = gscv.fit(X_train, y_train)
 
     print('Retrain model with best parameters...')
 
     best_model_steps = []
     # remove the CSV splitter for the best model
     for name, step in pipeline_steps:
-        if isinstance(step, CVSubset):
+        if isinstance(step, CrossValSplitter):
             continue
         best_model_steps.append((name, step))
 
     best_model = Pipeline(best_model_steps).set_params(**gscv.best_params_)
     best_model.fit(X_train, y_train)
 
     print('test best model...')
@@ -70,15 +70,15 @@
 
     print('computing confusion matrix...')
     from sklearn.metrics import confusion_matrix, ConfusionMatrixDisplay
     cm = confusion_matrix(y_true, y_pred)
 
     classes = []
     for step in pipe:
-        if isinstance(step, LabelEncoder):
+        if isinstance(step, LabelMatcher):
             classes = step.wr.classes_
             break
 
     if classes == []:
         raise ValueError("No labelencoder found in Pipeline.")
 
     print('generating classification report:')
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/__init__.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 from pyadlml.dataset._datasets.amsterdam import fetch_amsterdam
 from pyadlml.dataset._datasets.aras import fetch_aras
-from pyadlml.dataset._datasets.casas_aruba import fetch_casas_aruba
 from pyadlml.dataset._datasets.mitlab import fetch_mitlab
 from pyadlml.dataset._datasets.tuebingen_2019 import fetch_tuebingen_2019
 from pyadlml.dataset._datasets.uci_adl_binary import fetch_uci_adl_binary
 from pyadlml.dataset._datasets.kasteren_2010 import fetch_kasteren_2010
+from pyadlml.dataset._datasets.casas_houses import fetch_casas
 
 from pyadlml.dataset._datasets.homeassistant import (
     load_homeassistant, load_homeassistant_devices
 )
 
 from pyadlml.dataset._datasets.activity_assistant import load as load_act_assist
+from pyadlml.dataset import io
 
-from pyadlml.dataset.io import (
-    set_data_home,
-    get_data_home,
-    clear_data_home,
-    load,
-    dump,
-)
-
-from pyadlml.dataset import matplotlib, plotly, io, util
+# TODO refactor, importing stuff from pyadlml.dataset must not require 
+#                torch as a dependency to be installed. 
+#from pyadlml.dataset.misc import TorchDataset
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/_core/activities.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/_core/activities.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,78 @@
-from pyadlml.constants import START_TIME, ACTIVITY, END_TIME
+from pathlib import Path
+from pyadlml.constants import OTHER, START_TIME, ACTIVITY, END_TIME
 import pandas as pd
 import numpy as np
 
 """
     df_activities:
         - per definition no activity can be performed in parallel
 
         start_time | end_time   | activity
         ---------------------------------
         timestamp   | timestamp | act_name
 
 
 """
 INT_EPS = pd.Timedelta('1ms')
+COLS = [START_TIME, END_TIME, ACTIVITY]
+
+
+def get_index_matching_rows(df_act, rows, tolerance='1ms'):
+    """
+
+    Note
+    ----
+    Attention, since rows are read from strings or whatever the format assumed is dayfirst
+               i.e. 01.08.2009 equalst the first of august.
+
+    """
+    if isinstance(rows, list):
+        df = pd.DataFrame(rows, columns=COLS)
+        df[START_TIME] = pd.to_datetime(
+            df[START_TIME], errors='coerce', dayfirst=True)
+        df[END_TIME] = pd.to_datetime(
+            df[END_TIME], errors='coerce', dayfirst=True)
+    else:
+        print('went here')
+        df = rows
+
+    assert isinstance(df, pd.DataFrame)
+
+    tol = pd.Timedelta(tolerance)
+    idxs = []
+    for idx, row in df.iterrows():
+        mask_st = (row[START_TIME]-tol < df_act[START_TIME])\
+            & (df_act[START_TIME] < row[START_TIME]+tol)
+        mask_et = (row[END_TIME]-tol < df_act[END_TIME])\
+            & (df_act[END_TIME] < row[END_TIME]+tol)
+        mask_act = (df_act[ACTIVITY] == row[ACTIVITY])
+        res = df_act[mask_st & mask_et & mask_act].index.values
+        assert len(res) <= 1
+        if len(res) == 1:
+            idxs.append(*res)
+        if len(res) == 0:
+            print('Warning!!!. Activity corrections are not applied!')
+    return idxs
 
 
 def is_activity_df(df):
     """
         :param: df
         start_time | end_time   | activity
         ----------------------------------
         timestamp   | timestamp | act_name
     """
-    return START_TIME in df.columns \
-        and END_TIME in df.columns \
-        and ACTIVITY in df.columns \
-        and len(df.columns) == 3
+    try:
+        return START_TIME in df.columns \
+            and END_TIME in df.columns \
+            and ACTIVITY in df.columns \
+            and len(df.columns) == 3
+    except:
+        return False
 
 
 def check_activity_df(df):
     """
     check if the activitiy dataframe is valid by checking if
         - the dataframe has the correct dimensions and labels
         - activities are non overlapping
@@ -52,55 +95,67 @@
     """ checks if any activity is overlapping another
     Parameters
     ----------
     df : pd.DataFrame
 
     """
     assert df.shape[1] == 3, "Activity dataframes must have 3 columns."
-    epsilon = pd.Timedelta('0ms')
-    mask = (df[END_TIME].shift()-df[START_TIME]) >= epsilon
+
+    df = df.sort_values(by=START_TIME).reset_index(drop=True)
+    mask = (df[END_TIME].shift() - df[START_TIME]) >= pd.Timedelta('0ms')
     overlapping = df[mask]
     return not overlapping.empty
 
 
-def _create_activity_df():
+def _get_overlapping_activities(df):
+    df = df.sort_values(by=START_TIME).reset_index(drop=True)
+    mask = (df[END_TIME].shift()-df[START_TIME]) >= pd.Timedelta('0ms')
+    overlapping = df[mask]
+    return overlapping
+
+
+def create_empty_activity_df():
     """
     returns: empty pd Dataframe 
     """
     df = pd.DataFrame(columns=[START_TIME, END_TIME, ACTIVITY])
     df[START_TIME] = pd.to_datetime(df[START_TIME])
     df[END_TIME] = pd.to_datetime(df[END_TIME])
     return df
 
 
 def add_other_activity(acts, min_diff=pd.Timedelta('5s')):
-    """ adds a dummy Idle activity for gaps between activities greater than min_diff
+    """ adds a dummy "other" activity for gaps between activities greater than min_diff
     Parameters
     ----------
     acts: pd.DataFrame
         the activity data with columns: start_time, end_time, activity
     Returns
     ----------
     pd.DataFrame
         activity data with columns: start_time, end_time, activity
     """
     acts = acts.copy().reset_index(drop=True)
+    eps = pd.Timedelta('10ns')
+    assert 2*eps < min_diff
 
     def func(series, df):
         """
         """
+        if series.name in [209, 211]:
+            print()
         # check if at end of the series
         if series.name == len(df)-1:
             return series
         else:
             next_entry = df.loc[series.name+1, :]
             return pd.Series({
-                START_TIME: series.end_time + pd.Timedelta('1ms'),
-                END_TIME: next_entry.start_time - pd.Timedelta('1ms'),
-                ACTIVITY: 'idle'
+                START_TIME: series.end_time + eps,
+                END_TIME: next_entry.start_time - eps,
+                ACTIVITY: OTHER
             })
 
     acts['diff'] = acts[START_TIME].shift(-1) - acts[END_TIME]
     tmp = acts[acts['diff'] > min_diff].copy()
     tmp = tmp.apply(func, axis=1, df=acts)
     res = pd.concat([acts.iloc[:, :-1], tmp]).sort_values(by=START_TIME)
     return res.reset_index(drop=True)
@@ -115,15 +170,15 @@
     ----------
     ov: pd.DataFrame
         single df with one row
     row: pd.Series
         one row 
     """
     assert strat in ['inplace']
-    df = _create_activity_df()
+    df = create_empty_activity_df()
 
     if strat == 'inplace':
         df.loc[0] = [row.start_time, ov.start_time, row.activity]
         df.loc[1] = [ov.start_time + INT_EPS, ov.end_time, ov.activity]
         df.loc[2] = [ov.end_time + INT_EPS, row.end_time, row.activity]
     else:
         raise ValueError('Strategy not known.')
@@ -131,15 +186,15 @@
 
 
 def _merge_int_right_partial(row, ov, strat='clip_left'):
     """ merges 
         row int |~~~~|    => |~~~|---|    
         ov ints   |----|  
     """
-    df_res = _create_activity_df()
+    df_res = create_empty_activity_df()
 
     # get row stats
     row_act = row[ACTIVITY]
     row_st = row[START_TIME]
     row_et = row[END_TIME]
 
     # get overlap stats
@@ -174,15 +229,15 @@
         the submissive interval
 
     Returns
     -------
     df_res : pd.DataFrame
         the corrected activities
     """
-    df = _create_activity_df()
+    df = create_empty_activity_df()
     eps = pd.Timedelta('1ms')
 
     int1 = pd.Interval(row1.start_time, row1.end_time)
     int2 = pd.Interval(row2.start_time, row2.end_time)
 
     if int1.left <= int2.left and int1.right < int2.right:  # 1.case
         df.loc[0] = [row1.start_time, row1.end_time, row1.activity]
@@ -207,15 +262,15 @@
     Returns
     -------
     df_res : pd.DataFrame
         the corrected activities
     """
     assert row1.activity == row2.activity
 
-    df = _create_activity_df()
+    df = create_empty_activity_df()
     df.loc[0] = [row1.start_time, row2.end_time, row1.activity]
     return df
 
 
 def _merge_ints(row, overlapping, strats=['cut_at_lower'], excepts=[]):
     """ gets overlapping intervals and merges those intervals with a strategy
     Parameters
@@ -263,15 +318,15 @@
 
         # apply merging strategies
         int_dom = pd.Interval(dom.start_time, dom.end_time)
         int_ldom = pd.Interval(less_dom.start_time, less_dom.end_time)
 
         # dominant interval encloses less dominant => keep dominant, drop less dominant
         if (int_dom.left < int_ldom.left) & (int_ldom.right < int_dom.right):
-            df_res = _create_activity_df()
+            df_res = create_empty_activity_df()
             df_res.loc[0] = dom
             return df_res
 
         # less dominant interval encloses dominant => normal inclusive merge
         elif (int_ldom.left < int_dom.left) & (int_dom.right < int_ldom.right):
             return _merge_int_inclusive(less_dom, dom)
 
@@ -326,18 +381,18 @@
     corrections : list
         a list of tuples with the areas that had to be corrected and the corrections
     """
     df_act = df_act.copy()\
                    .sort_values(START_TIME)\
                    .reset_index(drop=True)
 
-    res = _create_activity_df()
+    res = create_empty_activity_df()
     corrections = []
 
-    # get all activities that have in an overlap with a direct preceding interval
+    # get all activities that have an overlap with a direct preceding interval
     mask = (df_act[START_TIME].shift(-1) -
             df_act[END_TIME]) <= pd.Timedelta('0ms')
     idxs_succ_overlaps = np.array(list(df_act[mask].index))
 
     i_l, i = 0, 0
     while i < len(idxs_succ_overlaps):
         # Append correct parts up to another overlap to result
@@ -349,15 +404,15 @@
         # this marks the point where we can copy again indices
         i_l = i_h
         i_h = _first_non_overlapped_int_after_idx(df_act, i_h)
 
         # only for last iteration
         if i == len(idxs_succ_overlaps)-1:
             area_to_correct = df_act.iloc[i_l:i_h, :]
-            result = _correct_overlapping_activities(
+            result = _correct_overlapping_segment(
                 area_to_correct, strategies, excep)
             corrections.append((area_to_correct, result))
             res = pd.concat([res, result])
             break
 
         # If the last overlapped interval exceeds any pair of overlapping indices, extent the range to
         # include them and adjust the loop iteration
@@ -377,15 +432,15 @@
                 if idx >= i_h:
                     break
                 # If the succeeding pair is in the range of the overlap skip the next outer loop iteration
                 # and set the upper overlap limit to the maximum of the included rows
                 i += 1
                 i_h = max(_first_non_overlapped_int_after_idx(df_act, idx), i_h)
         area_to_correct = df_act.iloc[i_l:i_h, :].copy()
-        result = _correct_overlapping_activities(
+        result = _correct_overlapping_segment(
             area_to_correct, strategies, excep)
 
         assert not result.empty
         corrections.append((area_to_correct, result))
         res = pd.concat([res, result])
         i += 1
         i_l = i_h
@@ -422,32 +477,36 @@
         index of the row where the interval overlaps the succeeding row(s)
 
     Returns
     -------
     res : int
         index of a row
     """
-    return list(df[df[START_TIME] > df.iloc[idx, :].end_time].index)[0]
+    try:
+        return list(df[df[START_TIME] > df.iloc[idx, :].end_time].index)[0]
+    except IndexError:
+        # The intervals overlap the whole dataframe including the last row
+        return len(df)
 
 
-def _correct_overlapping_activities(area_to_correct, strats, excepts=[]):
+def _correct_overlapping_segment(area_to_correct, strats, excepts=[]):
     """
     Parameters
     ----------
     area_to_correct : pd.DataFrame
         Acitity dataframe
     strats : list
         the strategies for merging intervals with priority in ascending order
     excepts : list
         the activities which should be preserved when merging
 
     """
     assert len(area_to_correct) >= 2, f'Test {area_to_correct}'
 
-    result = _create_activity_df()
+    result = create_empty_activity_df()
     stack = area_to_correct.copy()\
                            .sort_values(by=START_TIME)\
                            .reset_index(drop=True)
 
     while True:
         # pop first and second item from stack if they overlap otherwise
         # append to result until two items overlap
@@ -463,28 +522,31 @@
                 stack = stack.iloc[2:]  # remove first element from stack
                 break
             # the case when the current two activities of interest are the last ones
             elif stack.iloc[2:].empty:
                 result = pd.concat([result, stack])
                 return result
             else:
-                result = pd.concat([result, current_row])
+                result = pd.concat(
+                    [result, current_row.to_frame().T], ignore_index=True)
                 stack = stack.iloc[1:]
 
         new_rows = _merge_ints(current_row, ov, strats, excepts)
 
+        assert isinstance(new_rows, pd.DataFrame)
+
         if stack.empty:
-            result = pd.concat([result, new_rows])
+            result = pd.concat([result, new_rows], axis=0, ignore_index=True)
             return result
         elif len(new_rows) >= 2:
-            result = pd.concat([result, new_rows.iloc[0, :]])
+            result = pd.concat(
+                [result, new_rows.iloc[0, :].to_frame().T], ignore_index=True)
             new_rows = new_rows.iloc[1:]
-        else:  # the case if two intervals are merged that have the same name => it should get back on stack
-            new_rows = new_rows.iloc[0, :]
-        stack = pd.concat([stack, new_rows])
+
+        stack = pd.concat([stack, new_rows], axis=0, ignore_index=True)
         stack = stack.sort_values(by=START_TIME)
     return result
 
 
 def _get_overlapping_activities(df, shift=1):
     """ gets all activities that have an overlap
     """
@@ -510,14 +572,30 @@
     df = df_acts.copy()
     df['diff'] = df[END_TIME] - df[START_TIME]
     mask = (df['diff'] < pd.Timedelta('0s'))
     violating = df[mask]
     return not violating.empty
 
 
+def correct_succ_same_end_and_start_time(df: pd.DataFrame) -> pd.DataFrame:
+    """ Correct pairwise activities where the firsts end_time is equal to the seconds start_time
+        by adding a ms onto the respective start_time
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Activity dataframe
+
+    """
+    test = df[END_TIME].shift(1) - df[START_TIME]
+    mask = (test == pd.Timedelta('0s'))
+    df.loc[mask, START_TIME] += pd.Timedelta(INT_EPS)
+    return df
+
+
 def correct_activities(df, strats=[], excepts=[], retain_corrections=False):
     """ gets df in form of activities and removes overlapping activities
     Parameters
     ----------
     df : pd.DataFrame
     strats : list
         the strategies for merging intervals with priority in ascending order
@@ -532,18 +610,15 @@
     corrections: list
     """
     corrections = []
     df = df.copy()
     df = df.drop_duplicates(ignore_index=True)
 
     # Correct pairwise activities where the firsts end_time is equal to the seconds start_time
-    if True:
-        test = df[END_TIME].shift(1) - df[START_TIME]
-        mask = (test == pd.Timedelta('0s'))
-        df.loc[mask, START_TIME] += pd.Timedelta(INT_EPS)
+    df = correct_succ_same_end_and_start_time(df)
 
     # Check if an end_time is greater than a start_time
     if exists_st_before_et(df):
         raise NotImplementedError(
             'ST > ET violation. This has to be hard fixed, since there is no simple heuristic.')
 
     # Correct overlapping activities
@@ -551,7 +626,110 @@
         df, corrections = correct_activity_overlap(df, strats, excepts)
     assert not _is_activity_overlapping(df)
 
     if retain_corrections:
         return df, corrections
     else:
         return df, None
+
+
+class ActivityDict(dict):
+    """ Dictionary with activity pd.DataFrames as values and subject names as keys.
+    """
+
+    def __init__(self, obj=None):
+
+        if isinstance(obj, pd.DataFrame):
+            obj = obj.copy().reset_index(drop=True)
+            super().__init__({'subject': obj})
+        elif isinstance(obj, list):
+            if isinstance(obj[0], tuple):
+                super().__init__({name: df for (name, df) in obj})
+            else:
+                super().__init__({f'subject_{i}': df for i, df in enumerate(obj)})
+        elif isinstance(obj, ActivityDict) or isinstance(obj, dict):
+            super().__init__(obj)
+        else:
+            super().__init__()
+
+    def subjects(self) -> list:
+        return list(self.keys())
+
+    def to_json(self, date_unit="ns"):
+        """Serialize to json"""
+        tmp = {}
+        for k, df in self.items():
+            tmp[k] = df.to_json(date_unit=date_unit)
+
+        return json.dumps(tmp)
+
+    def read_json(cls, string):
+        """Serialize from json"""
+        tmp = json.loads(string)
+        for k, str in tmp.items():
+            tmp[k] = pd.read_json(str)
+        return ActivityDict(tmp)
+
+    def nr_acts(self):
+        """"""
+        return max([len(df_acts[ACTIVITY].unique()) for df_acts in self.values()])
+
+    def get_activity_union(self):
+        return list(set([item for v in self.values()
+                         for item in v[ACTIVITY].unique()]))
+
+    def apply(self, func):
+        """ Applies a function to each dataframe
+        """
+        for k, df in self.items():
+            self[k] = func(df)
+        return self
+
+    def min_starttime(self):
+        min_lst = []
+        for df_acts in self.values():
+            if not df_acts.empty:
+                min_lst.append(df_acts[START_TIME].iloc[0])
+        return min(min_lst)
+
+    def max_endtime(self):
+        max_lst = []
+        for df_acts in self.values():
+            if not df_acts.empty:
+                max_lst.append(df_acts[END_TIME].iloc[-1])
+        return max(max_lst)
+
+    def concat(self):
+        return pd.concat(self.values())
+
+    def copy(self):
+        """ Returns a deep copy of itsself
+        """
+        return ActivityDict({k: v.copy() for k, v in self.items()})
+
+    @classmethod
+    def wrap(cls, df_acts):
+        if isinstance(df_acts, pd.DataFrame):
+            df_acts = df_acts.copy().reset_index(drop=True)  # TODO not here
+            df_acts = ActivityDict({'subject': df_acts})
+            return df_acts
+        elif isinstance(df_acts, list):
+            return ActivityDict({f'subject_{i}': df for i, df in enumerate(df_acts)})
+        elif isinstance(df_acts, ActivityDict):
+            return df_acts
+        elif isinstance(df_acts, dict):
+            return ActivityDict(df_acts)
+        else:
+            raise NotImplementedError
+
+    def unwrap(self, inst_type: type):
+        if inst_type == ActivityDict:
+            return self
+        elif inst_type == list:
+            return list(self.values())
+        elif inst_type == dict:
+            return super(self)
+        elif inst_type == pd.DataFrame:
+            assert len(self) == 1
+            return list(self.values())[0]
+        else:
+            raise NotImplementedError
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/_core/devices.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/_core/devices.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from pathlib import Path
 import numpy as np
+from scipy import signal as sc_signal
 import pandas as pd
 
 from pyadlml.constants import START_TIME, END_TIME, TIME, VALUE, DEVICE, BOOL, NUM, CAT
 from pyadlml.dataset.util import df_difference, infer_dtypes
 
 CORRECTION_TS = 'correction_ts'
 CORRECTION_ONOFF_INCONS = 'correction_on_off_inconsistency'
+COLS_DEV = [TIME, DEVICE, VALUE]
 
 """
     df_devices:
         Standard representation for device dataframes.
         Exc: 
            | time      | device    | state
         ------------------------------------
@@ -73,77 +76,124 @@
     """
     if not START_TIME in df.columns or not END_TIME in df.columns \
             or not DEVICE in df.columns or len(df.columns) != 3:
         return False
     return True
 
 
-def is_device_df(df: pd.DataFrame):
+def is_device_df(df: pd.DataFrame) -> bool:
     """ Checks if a dataframe is a valid device dataframe.
     """
     return DEVICE in df.columns \
            and VALUE in df.columns \
            and TIME in df.columns \
            and len(df.columns) == 3
 
 
-def device_events_to_states(df_rep1: pd.DataFrame, extrapolate_states=False, st=None, et=None):
-    """ Transforms device dataframe from an event representation into a state representation,
-        where a row a devices state with start and end time.
+def get_index_matching_rows(df_devs, rows, tolerance='1ms'):
+
+    if isinstance(rows, list):
+        df = pd.DataFrame(rows, columns=COLS_DEV)
+        df[TIME] = pd.to_datetime(df[TIME], errors='coerce', dayfirst=True)
+    else:
+        print('went here')
+        df = rows
+
+    assert isinstance(df, pd.DataFrame)
+
+    tol = pd.Timedelta(tolerance)
+    idxs = []
+    for _, row in df.iterrows():
+        mask_st = (row[TIME]-tol < df_devs[TIME])\
+                & (df_devs[TIME] < row[TIME]+tol)
+        mask_dev = (df_devs[DEVICE] == row[DEVICE])
+        res = df_devs[mask_st & mask_dev].index.values
+        assert len(res) <= 1
+        if len(res) == 1:
+            idxs.append(*res)
+        if len(res) == 0:
+            print('Warning!!! Tried to delete device but could not')
+    return idxs
+
+
 
+
+
+
+def device_events_to_states(df_devs: pd.DataFrame, start_time=None, end_time=None, extrapolate_states=False):
+    """ Transforms device dataframe from an event representation into a state representation,
+        
     Parameters
     ----------
-    df_rep1 : pd.DataFrame
-        rep1: col (time, device, val)
+    df_devs : pd.DataFrame
+        In event representation, a dataframe with columns (time, device, value)
         example row: [2008-02-25 00:20:14, Freezer, False]
     extrapolate_states : Boolean, default=False
         Whether boolean devices should add extra states for the first occurring events
-    st : pd.Timestamp, str or default=None
+    start_time : pd.Timestamp, str or default=None
         The start time from which to
-    et : pd.Timestamp, str or default=None
+    end_time : pd.Timestamp, str or default=None
         The start time from which to
 
     Returns
     -------
     df : pd.DataFrame
-        rep: columns are (start time, end_time, device, state)
+        In state representation with columns (start time, end_time, device, value)
         example row: [2008-02-25 00:20:14, 2008-02-25 00:22:14, Freezer, True]
-    or 
+
     df, lst
     """
     epsilon = '1ns'
 
-    df = df_rep1.copy() \
+    df = df_devs.copy() \
         .reset_index(drop=True) \
         .sort_values(TIME)
 
     dtypes = infer_dtypes(df)
 
-    if st is None:
-        first_timestamp = df[TIME].iloc[0]
-    else:
-        first_timestamp = pd.Timestamp(st)
-    if et is None:
-        last_timestamp = df[TIME].iloc[-1]
-    else:
-        last_timestamp = pd.Timestamp(et)
+    first_timestamp = df[TIME].iloc[0] if start_time is None else pd.Timestamp(start_time)
+    last_timestamp  = df[TIME].iloc[-1] if end_time is None else pd.Timestamp(end_time)
 
     if extrapolate_states:
         # create additional rows in order to compensate for the state duration of the first event
         # to the selected event for boolean devices
         eps = pd.Timedelta(epsilon)
+
+        # Prevents boolean cast warning when extrapolatiing states
+        df[VALUE] = df[VALUE].astype(object)
+
         for dev in dtypes[BOOL]:
             df_dev = df[df[DEVICE] == dev]
             first_row = df_dev.iloc[0].copy()
             if first_row[TIME] != first_timestamp and first_row[TIME] - first_timestamp > pd.Timedelta('1s'):
                 first_row[VALUE] = not first_row[VALUE]
                 first_row[TIME] = first_timestamp + eps
-                df = df.append(first_row, ignore_index=True)
+                df = pd.concat([df, first_row.to_frame().T], axis=0, ignore_index=True)
             eps += pd.Timedelta(epsilon)
 
+        for dev in dtypes[CAT]:
+            df_dev = df[df[DEVICE] == dev].copy()
+            first_row = df_dev.iloc[0].copy()
+            if first_row[TIME] != first_timestamp and first_row[TIME] - first_timestamp > pd.Timedelta('1s'):
+                df_dev['value_succ'] = df_dev['value'].shift(-1)
+                # Frequencies of category i followed by j
+                f_ij = pd.crosstab(df_dev[VALUE], df_dev['value_succ'])
+                # p(j | i) = f_ij rate where first was cat_i than transitioned to cat_j
+                # therefore get max_i for cat_j to get p(i | j)
+                max_cat_i = f_ij.index[f_ij.loc[:, first_row[VALUE]].argmax()] 
+                first_row[VALUE] = max_cat_i
+                first_row[TIME] = first_timestamp + eps
+                df = pd.concat([df, first_row.to_frame().T], axis=0, ignore_index=True)
+
+            eps += pd.Timedelta(epsilon)
+
+        if dtypes[CAT]:
+            print('Warning! Extrapolated categories based on most propable category.')
+
+
     df = df.sort_values(TIME).reset_index(drop=True)
 
     lst_cat_or_bool = dtypes[CAT] + dtypes[BOOL]
     res = pd.DataFrame(columns=[START_TIME, END_TIME, DEVICE, VALUE])
 
     if lst_cat_or_bool:
         df_cat_bool = df[df[DEVICE].isin(lst_cat_or_bool)].copy()
@@ -365,41 +415,58 @@
     while _has_timestamp_duplicates(df_cor):
         df_cor = correct_device_ts_duplicates(df_cor)
     assert not _has_timestamp_duplicates(df_cor)
 
     if retain_correction:
         corrections[CORRECTION_TS] = df_difference(df, df_cor)
 
+    df_cor = df_cor.sort_values(by=TIME)\
+                   .reset_index(drop=True)
     df = df_cor.copy()
 
-    if contains_non_binary(df):
-        df_binary, df_non_binary = split_devices_binary(df)
-        non_binary_exist = True
-    else:
-        df_binary = df
-        non_binary_exist = False
+    dtypes = infer_dtypes(df)
+    df_binary = df[df[DEVICE].isin(dtypes[BOOL])].copy()
+    df_cat = df[df[DEVICE].isin(dtypes[CAT])].copy()
+    df_num = df[df[DEVICE].isin(dtypes[NUM])].copy()
 
     # correct on/off inconsistency
     if not is_on_off_consistent(df_binary):
         df_binary = correct_on_off_inconsistency(df_binary)
     assert is_on_off_consistent(df_binary)
 
-    # join dataframes
-    if non_binary_exist:
-        df = df_binary.append(df_non_binary)
-    else:
-        df = df_binary
+    # Correct same succedding categories
+    df_cat = correct_cat_inconsistency(df_cat)
+
+    df = pd.concat([df_binary, df_cat, df_num], axis=0, ignore_index=True)
+    df = df.sort_values(by=TIME).reset_index(drop=True)
 
     if retain_correction:
         corrections[CORRECTION_ONOFF_INCONS] = df_difference(df_cor, df)
 
-    df = df.sort_values(by=TIME).reset_index(drop=True)
-
     return df, corrections
 
+def correct_cat_inconsistency(df_cat: pd.DataFrame) -> pd.DataFrame:
+    """ 
+
+    Parameters
+    ----------
+    df_cat : pd.DataFrame
+        A device dataframe ['time', 'device', 'value'] where each 
+        devices value are categorical
+
+    Returns
+    ------- 
+    """
+    idxs_to_drop = [-1]
+    while len(idxs_to_drop) != 0:
+        df_cat['shifted'] = df_cat.groupby(by=DEVICE, observed=True)['value'].shift(1)
+        idxs_to_drop = df_cat[df_cat['value'] == df_cat['shifted']].index
+        df_cat = df_cat.drop(index=idxs_to_drop)
+
+    return df_cat.drop(columns=['shifted'])
 
 def on_off_consistent_func(df: pd.DataFrame, dev: list):
     """ compute for each device if it is on/off consistent
     Parameters
     ----------
     df : pd.DataFrame
         the whole activity dataframe
@@ -499,60 +566,31 @@
 def _create_empty_dev_dataframe():
     df = pd.DataFrame(data=[], columns=[TIME, DEVICE, VALUE])
     df[TIME] = pd.to_datetime(df[TIME])
     return df
 
 
 def most_prominent_categorical_values(df: pd.DataFrame):
-    tmp = df
-    tmp['conc'] = tmp[DEVICE] + ',' + tmp[VALUE]
-    dev_list = tmp[DEVICE].unique()
-    tmp = pd.concat([tmp[TIME], pd.get_dummies(tmp['conc'], dtype=int)], axis=1)
-    tmp2 = tmp.copy()
-    for dev in dev_list:
-        dev_col_cats = []
-        for col in tmp.columns:
-            if dev not in col:
-                continue
-            dev_col_cats.append(col)
-
-        for di in dev_col_cats:
-            other = dev_col_cats[:]
-            other.remove(di)
-            for o in other:
-                tmp2[di] = tmp2[di] - tmp[o]
-    tmp2 = tmp2.set_index(TIME)
-    tmp2 = tmp2.where(tmp2 != 0, np.nan)
-    tmp2 = tmp2.ffill(axis=0)
-    tmp2 = tmp2.where(tmp2 != -1, 0)
-    tmp2 = tmp2.reset_index()
-    tmp2['td'] = tmp2[TIME].shift(-1) - tmp2[TIME]
-
-    lst = []
-    for dev in dev_list:
-        dev_col_cats = []
-        for col in tmp.columns:
-            if dev not in col:
-                continue
-            dev_col_cats.append(col)
-        asdf = []
-        max_td = pd.Timedelta('0s')
-        max_cat = None
-        for di in dev_col_cats:
-            abc = tmp2[[di, 'td']].groupby(di).sum().reset_index()
-            td_on = abc.iloc[1, 1]
-            if max_td < td_on:
-                max_td = td_on
-                max_cat = di
-            asdf.append(td_on)
-        lst.append([dev, max_cat.split(',')[1]])
     ML_STATE = 'ml_state'
-    df = pd.DataFrame(data=lst, columns=[DEVICE, ML_STATE])
-    return df
+    df_cat = df.copy()
 
+    # Compute at each category row its duration to the next category change
+    df_cat = df_cat.sort_values([DEVICE, TIME])
+    df_cat['td'] = df_cat.groupby(DEVICE, observed=True)[TIME].diff().shift(-1)
+    df_cat = df_cat.sort_values(by=TIME).reset_index(drop=True).iloc[:-1]
+    nan_idxs = df_cat[df_cat.isna().any(axis=1)].index
+    df_cat.loc[nan_idxs, 'td'] = (df_cat.at[df_cat.index[-1], TIME] - df_cat.loc[nan_idxs, TIME]).values
+
+
+    df = df_cat.groupby([DEVICE, VALUE], observed=True)['td'].sum().reset_index()
+    max_rows = df.loc[df.groupby(DEVICE, observed=True)['td'].idxmax()]
+    max_rows = max_rows.reset_index(drop=True)\
+                       .drop(columns=['td'])\
+                       .rename(columns={VALUE: ML_STATE})
+    return max_rows
 
 def _get_bool_mask(df: pd.DataFrame, col: list):
     """ returns a mask where the columns are booleans"""
     if df[col].dtype == 'bool':
         # return df[col].na # TODO hack for returning
         return (df[col] == True) | (df[col] == False)
     mask = (df[col].astype(str) == 'False') | (df[col].astype(str) == 'True')
@@ -572,15 +610,15 @@
     def func(x):
         # check if every is one of
         if x[VALUE].dtype == 'bool':
             return True
         else:
             return ((x[VALUE].astype(str) == 'False') | (x[VALUE].astype(str) == 'True')).all()
 
-    return df.groupby(by=[DEVICE]).filter(func)
+    return df.groupby(by=[DEVICE], observed=True).filter(func)
 
 
 def create_device_info_dict(df_dev: pd.DataFrame) -> dict:
     """
     Infers for each device the most likely state
 
     Parameters
@@ -618,15 +656,15 @@
             res[dev][ML_STATE] = true_has_more
 
     # get most likely numerical states
     # use median for the most likely numerical state
     if dtypes[NUM]:
         df_num = df_dev.loc[df_dev[DEVICE].isin(dtypes[NUM]), [DEVICE, VALUE]].copy()
         df_num[VALUE] = pd.to_numeric(df_num[VALUE])
-        res_num = df_num.groupby(by=[DEVICE]).median()
+        res_num = df_num.groupby(by=[DEVICE], observed=True).median()
         for dev in dtypes[NUM]:
             res[dev][ML_STATE] = res_num.at[dev, VALUE]
 
     # get most likely categorical states
     if dtypes[CAT]:
         df_cat = df_dev[df_dev[DEVICE].isin(dtypes[CAT])].copy()
         res_cat = most_prominent_categorical_values(df_cat)
@@ -696,22 +734,112 @@
     current_step = 0
     for i in range(len(signal)):
         state = signal[i][0]
         steps = np.floor((signal[i][1] / max_len) * nr_bins).astype(int)
         discretized_sig[current_step:current_step + steps] = 1 if state else -1
         current_step += steps
 
+    # TODO refactor, why does the extrapolation of states do not work out???
+    # Eliminate Zeropadding
+    last_state = discretized_sig[0]
+    for i in range(1, len(discretized_sig)):
+        if discretized_sig[i] == 0:
+            discretized_sig[i] = last_state
+        last_state = discretized_sig[i] 
+
     return discretized_sig
 
 
+
+def create_sig_and_corr(df: pd.DataFrame, hit_idx: int, dt_prae_hit: pd.Timedelta, dt_post_hit: pd.Timedelta,
+                        ss_discrete: np.ndarray):
+    """ 
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        
+
+    """
+    idx, first, last = get_idxs(df, hit_idx, dt_prae_hit, dt_post_hit)
+    tmp = df.loc[idx, [VALUE, 'diff']].values
+    tmp = np.insert(tmp, 0, [[not tmp[0, 0], first]], axis=0)
+    tmp = np.append(tmp, [[not tmp[-1, 0], last]], axis=0)
+    signal = _generate_signal(tmp, dt='250ms')
+    corr = sc_signal.correlate(signal, ss_discrete, mode='full')
+    return signal, corr
+
+
+def get_idxs(df, hit_idx, dt_prae_hit, dt_post_hit):
+    """ Gets device indices of events before and after to the hit 
+        to later on process in a cross correlation.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        device dataframe of the selected device
+    hit_idx: int
+        Indice of the hit
+    dt_prae_hit: pd.Timedelta
+        How much time to consider prea hit
+    dt_prae_hit: pd.Timedelta
+        How much time to consider post hit
+
+    Returns
+    -------
+    list, 
+        The involved indices for the signal
+    """
+    get_df_idx = lambda x: df[df['index'] == x].index.values[0]
+
+    res_idxs = [hit_idx]
+    df = df.reset_index()
+
+    if get_df_idx(hit_idx) == 0:
+        first = dt_prae_hit
+    else:
+        # Iterate the events backward and finish if iterated time difference
+        # is higher than the origs. signals 
+        idx_lower = get_df_idx(hit_idx) - 1
+        dt_iter = dt_prae_hit
+        dt_prev_tmp = dt_iter - df.at[idx_lower, 'diff']
+        while dt_prev_tmp > pd.Timedelta('0s') and idx_lower >= 0:
+            dt_iter -= df.at[idx_lower, 'diff']
+            res_idxs.insert(0, df.at[idx_lower, 'index'])
+            idx_lower -= 1
+            dt_prev_tmp -= df.at[idx_lower, 'diff']
+        first = dt_iter
+
+    if get_df_idx(hit_idx) == len(df) - 1:
+        last = dt_post_hit
+    else:
+        # Iterate the events forward and finish if iterated time difference
+        # is higher than the origs. signals 
+        idx_upper = get_df_idx(hit_idx) + 1
+        dt_iter = dt_post_hit
+        dt_next_tmp = dt_iter - df.at[idx_upper, 'diff']
+        while dt_next_tmp > pd.Timedelta('0s') and idx_upper < len(df) - 1:
+            dt_iter -= df.at[idx_upper, 'diff']
+            res_idxs.append(df.at[idx_upper, 'index'])
+            idx_upper += 1
+            dt_next_tmp -= df.at[idx_upper, 'diff']
+        last = dt_iter
+
+    df = df.set_index('index')
+    return res_idxs, first, last
+
+
+
 def device_remove_state_matching_signal(df_devs: pd.DataFrame,
                                         #signal: list[tuple[bool, str], ... ],
+                                        device: str,
                                         signal: list,
-                                        state_indicator: int,
-                                        eps_state: str = '0.2s', eps_corr: float = 0.1) -> pd.DataFrame:
+                                        matching_state: int,
+                                        corr_threshold=0.2, 
+                                        eps_state: str = '0.2s') -> pd.DataFrame:
     """
     Removes states from a device dataframe that match a signal.
 
     Parameters
     ----------
     df_devs : pd.DataFrame
         A device dataframe
@@ -735,19 +863,96 @@
             (False, '4s'), \
             (True, '1s'), \
             (False, '5s') \
         ] \
     >>> df = device_remove_state_matching_signal(df, sig_original, eps_corr=2)
     """
 
+
+    matching_state_idx = matching_state
+    eps_state = '0.2s'
+    # Tolerance for cross correlation w.r.t. auto correlation to highlight as a match
+    sig_search = [(s[0], pd.Timedelta(s[1])) for s in signal]
+
+
+    # Find 
+    td = pd.Timedelta(sig_search[matching_state_idx][1])
+    state = sig_search[matching_state_idx][0]
+    eps_state = pd.Timedelta(eps_state)
+
+    from scipy import signal as sc_signal
+    # Create auto correlation and retrieve a proper threshold
+    ss_discrete = _generate_signal(sig_search, dt='250ms')
+    auto_corr = sc_signal.correlate(ss_discrete, ss_discrete, mode='full')
+    auto_corr_max = auto_corr.max()
+
+    # Compute the number of counts that the signal may deviate
+    # but still counts as a match
+    # For example if a window is 72 units long and the maximum
+    # correlation would also be 72 for a signal with the same length. Therefore
+    # the eps_corr count would be 14 if the signal is allowed to differ 20%
+    if isinstance(corr_threshold, float):
+        corr_threshold = int(len(ss_discrete)*corr_threshold)
+        corr_threshold = auto_corr_max - corr_threshold
+
+    # Count total length and length up and after matching state of signal
+    ss_total_dt, ss_dt_prae_match, ss_dt_post_match = [pd.Timedelta('0s')]*3
+    for i, (s, dt) in enumerate(sig_search):
+        ss_total_dt += dt
+        if i < matching_state_idx:
+            ss_dt_prae_match += dt
+        if i > matching_state_idx:
+            ss_dt_post_match += dt
+
+    plot_dt_around_sig = ss_total_dt*0.25
+
+
+
+    def create_hit_list(df_devs):
+        df = df_devs[df_devs[DEVICE] == device].copy()
+        df['to_convert'] = False
+        df['diff'] = pd.Timedelta('0ns')
+        df['target'] = False
+
+        df['diff'] = df[TIME].shift(-1) - df[TIME]
+        df['target'] = (td - eps_state < df['diff'])\
+                    & (df['diff'] < td + eps_state)\
+                    & (df[VALUE] == state)
+
+        # Correct the case where the first occurence is already a match
+        df.at[df.index[-1], 'diff'] = ss_total_dt
+
+        # Get indices of hits and select first match for display
+        hits = df[(df['target'] == True)].index.to_list()
+        return hits, df
+
+    hits, df = create_hit_list(df_devs)
+
+    df_sel_dev = df_devs.copy()[df_devs[DEVICE] == device].reset_index()
+
+    for h in hits:
+        sig, corr = create_sig_and_corr(df, h, ss_dt_prae_match, ss_dt_post_match, ss_discrete)
+
+        if corr.max() > corr_threshold:
+            # Get succeding dev index
+            mask = (df_sel_dev['index'] == h)
+            idxs_to_drop = df_sel_dev[mask | mask.shift(1)]['index'].values.tolist()
+            df_devs = df_devs.drop(idxs_to_drop)
+
+    return df_devs.reset_index(drop=True)
+
+
+
+
+    # Old
+
     from scipy import signal as sc_signal
-    df = df_devs.copy()
     sig_original = signal
-    td = pd.Timedelta(sig_original[state_indicator][1])
-    state = sig_original[state_indicator][0]
+    td = pd.Timedelta(sig_original[matching_state][1])
+    state = sig_original[matching_state][0]
     eps_state = pd.Timedelta(eps_state)
 
     # Create perfect correlation yielding a proper threshold
     win = _generate_signal(sig_original, dt='250ms')
     perfect_corr = sc_signal.correlate(win, win, mode='full')
     perfect_corr_max = perfect_corr.max()
 
@@ -757,17 +962,17 @@
     # correlation would also be 72 for a signal with the same length. Therefore
     # the eps_corr count would be 14 if the signal is allowed to differ 20%
     eps_corr = int(len(win)*eps_corr)
 
     # Create a timelength to append to
     tmp1 = [pd.Timedelta(s[1]) for s in sig_original]
     max_sig = sum(tmp1, pd.Timedelta('0s'))
-    states_to_past = [pd.Timedelta(sig_original[s][1]) for s in range(0, state_indicator)]
+    states_to_past = [pd.Timedelta(sig_original[s][1]) for s in range(0, matching_state)]
     dt_states_to_past = sum(states_to_past, pd.Timedelta('0s'))
-    states_to_future = [pd.Timedelta(sig_original[s][1]) for s in range(state_indicator+1, len(sig_original))]
+    states_to_future = [pd.Timedelta(sig_original[s][1]) for s in range(matching_state+1, len(sig_original))]
     dt_states_to_future = sum(states_to_future, pd.Timedelta('0s'))
 
     df = df.copy().reset_index(drop=True)
     df['to_convert'] = False
     df['diff'] = pd.Timedelta('0ns')
     df['target'] = False
 
@@ -818,46 +1023,16 @@
 
             # Aasdf
             tmp = df.loc[idx, [VALUE, 'diff']].values
             tmp = np.insert(tmp, 0, [[not tmp[0, 0], first]], axis=0)
             tmp = np.append(tmp, [[not tmp[-1, 0], last]], axis=0)
             signal = _generate_signal(tmp, dt='250ms')
 
-            #print('-'*10,f'\ndev {dev}: idx: {idx}')
-            #print(f'{len(win)} vs {len(signal)}')
             corr = sc_signal.correlate(signal, win, mode='full')
-            #print(f'max corr: {corr.max()}')
-            #print('perfect corr max: ', perfect_corr_max)
-            #if True:
-            #    import matplotlib.pyplot as plt
-            #    tmp_corr = []
-            #    if True:
-            #    #for t in range(1, len(signal)):
-            #        #s1 = signal[:t]
-            #        #s2 = win[-t:]
-            #        #tmp_corr.append((s1*s2).sum())
-            #        #fig, (ax1, ax2, ax3, ax4) = plt.subplots(4, 1, figsize=(6, 10))
-            #        fig, (ax1, ax2, ax3) = plt.subplots(3, 1, figsize=(6, 10))
-            #        ax1.plot(np.arange(len(win)), win)
-            #        ax1.scatter(np.arange(len(win)), win)
-            #        ax2.plot(np.arange(len(signal)), signal)
-            #        ax2.scatter(np.arange(len(signal)), signal)
-
-            #        ax3.plot(np.arange(len(corr)), corr, label='signal vs. window')
-            #        ax3.plot(np.arange(len(perfect_corr)), perfect_corr, label='win vs. win')
-            #        ax3.legend()
-
-            #        #ax4.plot(np.arange(len(tmp_corr)), tmp_corr, label='corr')
-            #        #ax4.plot(np.arange(len(s2)), s2, label='s2')
-            #        #ax4.plot(np.arange(len(signal)), signal, alpha=0.1, label='full s1')
-            #        #ax4.plot(np.arange(len(s1)), s1, label='s1')
-            #        #ax4.legend()
-            #        plt.savefig('tmp.png')
-            #        plt.clf()
-            #    ax3
+
 
             is_match = perfect_corr_max - corr.max() < eps_corr
             if is_match:
                 df.at[h, 'to_convert'] = True
             #if not is_match:
             #   is_match
             #print(f'match: {is_match}')
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/_core/obj.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/io/remote.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,32 @@
-from pyadlml.constants import DEVICE, ACTIVITY
-from pyadlml.dataset.io import download_from_mega, get_data_home, _ensure_dh_folder_exists, _delete_data
+from pyadlml.constants import DATA_DCT_KEY_ACTS, DATA_DCT_KEY_DEVS, DEVICE, ACTIVITY
+from pyadlml.dataset._core.activities import ActivityDict
+from .local import get_data_home, _ensure_dh_folder_exists, _delete_data
 from pathlib import Path
 import pandas as pd
 import joblib
-
-
-class Data(object):
-    def __init__(self, activities=None, devices=None, activity_list=None, device_list=None):
-
-        self.df_devices = devices
-
-        if device_list is None:
-            self.lst_devices = devices[DEVICE].unique()
-
-        if activities is not None:
-            self.df_activities = activities
-            if activity_list is None:
-                self.lst_activities = activities[ACTIVITY].unique()
-            else:
-                self.lst_activities = activity_list
-            self.act_dict = {"default": self.df_activities}
-        else:
-            self.act_dict = {}
-
-    def set_activity_list(self, lst, name=None):
-        """
-        """
-        if name is None or name == "default":
-            setattr(self, "lst_activities", lst)
-        else:
-            setattr(self, "lst_activities_{}".format(name), lst)
-
-    def set_activity_df(self, df, name=None):
-        """
-        """
-        if name is None or name == "default":
-            setattr(self, "df_activities", df)
-            self.act_dict["default"] = df
-        else:
-            setattr(self, "df_activities_{}".format(name), df)
-            self.act_dict[name] = df
-
-    def set_activity_correction(self, lst, name=None):
-        if name is None or name == "default":
-            self.correction_activities = lst
-        else:
-            setattr(self, "correction_activities_{}".format(name), lst)
-
-    def set_device_correction(self, corr_dts, corr_incons):
-        self.correction_devices_duplicate_timestamps = corr_dts
-        self.correction_devices_on_off_inconsistency = corr_incons
-
-    def get_activity_dict(self) -> dict:
-        return self.act_dict
-
-    def set_device_df(self, df):
-        self.df_devices = df
-
 from abc import ABC, abstractmethod
 
-class DatasetDownloader():
-    def __init__(self,):
-        pass
 
 
 
 class DataFetcher(ABC):
-    FN_CLEANED = 'cleaned.joblib'
-    FN_CACHED = 'cached.joblib'
+    FN_CLEANED = 'cleaned%s.joblib'
+    FN_CACHED = 'cached%s.joblib'
 
     def __init__(self, dataset_name: str,
-                       downloader: DatasetDownloader,
+                       downloader,
                        correct_activities=False,
                        correct_devices=False
         ):
 
         self.downloader = downloader
         self.ds_name = dataset_name
-        self.correct_devices = correct_devices
-        self.correct_activities = correct_activities
+        self.apply_dev_corr = correct_devices
+        self.apply_act_corr = correct_activities
 
 
         self.data_home = get_data_home()
         self._dataset_folder = None
         self._original_folder = None
 
 
@@ -96,90 +40,115 @@
     def dataset_folder(self):
         return Path(self.data_home).joinpath(self.ds_name)
 
     @property
     def original_folder(self):
         return self.dataset_folder.joinpath('original')
 
+    def correct_activities(self, subject, df_activities, ident=None):
+        """ May be overriden by child classes
+        """
+        from pyadlml.dataset._core.activities import correct_activities
+        return correct_activities(df_activities, retain_corrections = self.retain_corrections)
 
-
-    def apply_corrections(self, data:dict, retain_corrections=False):
+    def apply_corrections(self, data:dict, ident:str=None, retain_corrections=False):
         """ Applies corrections
 
+        Parameters
+        ----------
+        ident : None or str
+
+
         data : dict
             Of the form 
             {
                 'activity_list': [],
                 'device_list': [],
-                'df_devices': pd.DataFrame,
-                'df_activities_subject_M': pd.DataFrame,
+                'devices': pd.DataFrame,
+                'activities': pd.DataFrame,
                 ...
             }
         """
-        for key, df in data.items():
-            if 'df_activity' in key: 
-                from pyadlml.dataset._core.activities import correct_activities
-                if self.correct_activities:
-                    df, corr = correct_activities(df, retain_corrections)
-                    data[key] = df
-                    if retain_corrections:
-                        data[key + "_corrections"] = corr
-                else:
-                    data[key] = df
+        if self.apply_act_corr:
+            acts = data[DATA_DCT_KEY_ACTS]
+            unpack = isinstance(acts, pd.DataFrame)
+            if unpack:
+                acts = ActivityDict.wrap(acts)
+
+            for key, df in acts.items():
+                df_acts, corrections = self.correct_activities(key, df, ident)
+                acts[key] = df_acts
+                if corrections:
+                    if 'correction_activities' not in data.keys():
+                        data['correction_activities'] = {}
+                    data['correction_activities'][key] = corrections
+
+            if unpack:
+                data[DATA_DCT_KEY_ACTS] = df_acts
+                if corrections:
+                    data['correction_activities'] = data['correction_activities'][list(acts.keys())[0]]
 
-        if self.correct_devices:
+        if self.apply_dev_corr:
             from pyadlml.dataset._core.devices import correct_devices
-            df_dev, correction_dev_dict = correct_devices(data['df_devices'], retain_correction=retain_corrections)
-            data['df_devices'] = df_dev
-            if retain_corrections:
-                data[key + "_corrections"] = corr
+            df_dev, correction_dev_dict = correct_devices(data[DATA_DCT_KEY_DEVS], 
+                                retain_correction=retain_corrections)
+            data[DATA_DCT_KEY_DEVS] = df_dev
+            if correction_dev_dict:
+                data.update(correction_dev_dict)
 
         return data
 
+    def _gen_filenames_cached(self, identifier):
+        """ Creates unique cache names when i.e. more subjecta have to be 
+            loaded.
+        """
+        
+        if identifier is None:
+            cached_name = self.FN_CACHED%('')
+            cleaned_name = self.FN_CLEANED%('')
+        else:
+            cached_name = self.FN_CACHED%('_' + str(identifier))
+            cleaned_name = self.FN_CLEANED%('_' + str(identifier))
+
+        return self.dataset_folder.joinpath(cached_name),\
+               self.dataset_folder.joinpath(cleaned_name)
 
-    def __call__(self, cache=False, keep_original=False, retain_corrections=False, load_cleaned=False, folder_path=None, *args, **kwargs):
+
+    def __call__(self, cache=False, keep_original=False, retain_corrections=False, load_cleaned=False, folder_path=None, apply_corrections=True, 
+                *args, **kwargs):
+
+
+        self.retain_corrections = retain_corrections
 
         # Resolve folders
         self._create_exp_folder()
 
-        sel = None
-        for a in kwargs.keys():
-            sel = a
-
-        if sel is not None:
-            # TODO, when do I get here
-            cached_name = FN_CACHED.split(
-                '.')[0] + '_' + kwargs[sel] + '.' + FN_CACHED.split('.')[1]
-            cleaned_name = FN_CLEANED.split(
-                '.')[0] + '_' + kwargs[sel] + '.' + FN_CLEANED.split('.')[1]
-            fp_cached_dataset = self.dataset_folder.joinpath(cached_name)
-            fp_cleaned_dataset = self.dataset_folder.joinpath(cleaned_name)
-        else:
-            fp_cached_dataset = self.dataset_folder.joinpath(self.FN_CACHED)
-            fp_cleaned_dataset = self.dataset_folder.joinpath(self.FN_CLEANED)
+        ident = kwargs.get('ident')
+        fp_cached_dataset, fp_cleaned_dataset = self._gen_filenames_cached(ident) 
 
 
         # Only download data if it was not already fetched
         # and no cached version exists that should be loaded
         # and the load_cleaned flag is not set
         if not (self.original_folder.exists() or (fp_cached_dataset.is_file() and cache)
                 or folder_path is not None) and not load_cleaned:
             self.original_folder.mkdir(parents=True, exist_ok=True)
-            self.download()
+            self.downloader.download(self.original_folder)
 
         elif load_cleaned and not fp_cleaned_dataset.exists():
-            self.download_cleaned(self.dataset_folder)
+            fp_cleaned_dataset.parent.mkdir(parents=True, exist_ok=True)
+            self.downloader.download_cleaned(fp_cleaned_dataset, ident)
 
 
         # Load from cached version if available and cache flag is set
             # or load from cleaned version
             # otherwise load from the function
         if fp_cached_dataset.is_file() and cache and not load_cleaned:
             data = joblib.load(fp_cached_dataset)
-        elif fp_cleaned_dataset.is_file() and load_cleaned and not cache:
+        elif fp_cleaned_dataset.is_file() and load_cleaned:
             data = joblib.load(fp_cleaned_dataset)
         else:
             data = self.load_data(folder_path=self.original_folder, **kwargs)
 
         # Save dataset if downloaded and not already cached
         if cache and not fp_cached_dataset.is_file() and not load_cleaned:
             joblib.dump(data, fp_cached_dataset)
@@ -187,38 +156,22 @@
         # Clean up data
         if not cache and fp_cached_dataset.is_file():
             fp_cached_dataset.unlink()
         if not keep_original and self.original_folder.exists():
             _delete_data(self.original_folder)
 
         # Correct devices or activities
-        self.apply_corrections(data)
+        if apply_corrections:
+            self.apply_corrections(data, ident, retain_corrections)
 
         return data
 
-    def download(self):
-        self.downloader.download(self.original_folder)
-
-    def download_cleaned(self):
-        self.downloader.download_cleaned(self.dataset_folder)
-
 
     @abstractmethod
     def load_data(self, *args, **kwargs):
         raise NotImplementedError
 
 
 
-class MegaDownloader(DatasetDownloader):
-    def __init__(self, url, fn, url_cleaned, fn_cleaned):
-        self.mega_url =  url
-        self.fn = fn
-        self.url_cleaned = url_cleaned
-        self.fn_cleaned = fn_cleaned
-    
-    
-    def download_cleaned(self, dest: Path) -> None:
-        """ Download from mega"""
-        download_from_mega(dest, self.fn_cleaned, self.url_cleaned, unzip=False)
 
-    def download(self, dest: Path) -> None:
-        download_from_mega(dest, self.fn, self.mega_url, unzip=True)
+
+
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/amsterdam.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/amsterdam.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,65 @@
 import pandas as pd
-from pyadlml.dataset._core.obj import Data, MegaDownloader
+from pathlib import Path
+from pyadlml.dataset.io import MegaDownloader
 from pyadlml.constants import ACTIVITY, VALUE, \
     START_TIME, END_TIME, TIME, NAME, DEVICE
-from pyadlml.dataset._core.activities import correct_activities
-from pyadlml.dataset._core.devices import correct_devices, CORRECTION_TS, CORRECTION_ONOFF_INCONS
 from pyadlml.dataset._core.devices import device_boolean_on_states_to_events
-from pyadlml.dataset.io import fetcher, correct_acts_and_devs, download_from_mega
-import os
-from pathlib import Path
-from pyadlml.dataset._core.obj import DataFetcher
+from pyadlml.dataset.io import DataFetcher
 
 AMSTERDAM_URL = 'https://mega.nz/file/AYhzDLaS#n-CMzBO_raNAgn2Ep1GNgbhah0bHQzuA48PqO_ODEAg'
 AMSTERDAM_CLEANED_URL = 'https://mega.nz/file/9R5zxKiT#Ko5NLmAWofmOTGJr0dvjHzjkX8xvKGtZw_Dy5AQ1ogY'
 AMSTERDAM_FILENAME = 'amsterdam.zip'
 AMSTERDAM_CLEANED_FILENAME = 'amsterdam_cleaned.joblib'
 DEVICES_FN = "kasterenSenseData.txt"
 ACTIVITIES_FN = "kasterenActData.txt"
 
 __all__ = ['fetch_amsterdam']
 
 
 class AmsterdamFetcher(DataFetcher):
-    def __init__(self, *args, **kwargs):
-
+    def __init__(self):
         downloader = MegaDownloader(
             url=AMSTERDAM_URL,
             fn=AMSTERDAM_FILENAME,
             url_cleaned=AMSTERDAM_CLEANED_URL,
             fn_cleaned=AMSTERDAM_CLEANED_FILENAME,
         )
 
         super().__init__(
             dataset_name='amsterdam',
             downloader=downloader,
-            # TODO change to true
-            correct_activities=False,
-            correct_devices=False
+            correct_activities=True,
+            correct_devices=True,
         )
 
     def load_data(self, folder_path):
         device_fp = Path(folder_path).joinpath(DEVICES_FN)
         activity_fp = Path(folder_path).joinpath(ACTIVITIES_FN)
 
-        df_act = _load_activities(activity_fp)
-        df_dev = _load_devices(device_fp)
-        df_dev = device_boolean_on_states_to_events(df_dev)
-
-        lst_act = df_act[ACTIVITY].unique()
-        lst_dev = df_dev[DEVICE].unique()
+        df_acts = _load_activities(activity_fp)
+        df_devs = _load_devices(device_fp)
+        df_devs = device_boolean_on_states_to_events(df_devs)
+        df_devs[DEVICE] = df_devs[DEVICE].astype('category')
+        lst_act = df_acts[ACTIVITY].unique()
+        lst_dev = df_devs[DEVICE].unique()
 
         return dict(
-            df_activities=ActivityDict(df_act),
-            df_devices=df_dev,
+            activities=df_acts,
+            devices=df_devs,
             activity_list=lst_act,
             device_list=lst_dev
         )
 
 
 def fetch_amsterdam(keep_original=False, cache=True, load_cleaned=False,
                     retain_corrections=False, folder_path=None):
     """
     Fetches the amsterdam dataset from the internet. The original dataset or its cached version
-    is stored in the :ref:`data home <storage>` folder.
+    is stored in the data_home folder.
 
     Parameters
     ----------
     keep_original : bool, default=False
         Determines whether the original dataset is deleted after downloading
         or kept on the hard drive.
     cache : bool, default=True
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/aras.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/aras.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from pathlib import Path
 import pandas as pd
 from pyadlml.constants import VALUE, TIME, DEVICE, END_TIME, START_TIME, ACTIVITY
-from pyadlml.dataset._core.obj import Data, DataFetcher, MegaDownloader
-from pyadlml.dataset.io import fetcher, correct_acts_and_devs, download_from_mega
+from pyadlml.dataset._core.activities import ActivityDict
+from pyadlml.dataset.io import DataFetcher, MegaDownloader
 
 ARAS_URL = 'https://mega.nz/file/hVpRADoZ#GLLZDV4Y-vgdEeEDTXnFxeG3eKllhTljMM1RK-eGyh4'
 ARAS_FILENAME = 'aras.zip'
 
 RES_1 = 'resident1'
 RES_2 = 'resident2'
 
@@ -22,50 +22,48 @@
             url_cleaned=None,
             fn_cleaned=None,
         )
 
         super().__init__(
             dataset_name='aras',
             downloader=downloader,
-            # TODO change to true
-            correct_activities=False,
-            correct_devices=False
+            correct_activities=True,
+            correct_devices=True
         )
 
     def load_data(self, folder_path: Path) -> dict:
 
         device_map = _get_device_map(folder_path)
         activity_map = _get_activity_map(folder_path)
         df = _read_data(folder_path, activity_map, device_map)
 
         df_res1_act = _create_activity_df(df, RES_1)
         df_res2_act = _create_activity_df(df, RES_2)
 
         df_dev = _create_device_df(df)
         lst_dev = df_dev[DEVICE].unique()
-        from pyadlml.dataset.plotly.util import ActivityDict
         act_dict = ActivityDict({
                 RES_1:df_res1_act,
                 RES_2:df_res2_act,
         })
         return dict(
-            df_devices=df_dev,
+            devices=df_dev,
             device_list=lst_dev,
-            df_activities=act_dict,
+            activities=act_dict,
             activity_list={
                 RES_1: df_res1_act[ACTIVITY].unique(),
                 RES_2: df_res2_act[ACTIVITY].unique(),
             }
         )
 
 def fetch_aras(keep_original=True, cache=True, retain_corrections=False,
                folder_path=None):
     """
     Fetches the aras dataset from the internet. The original dataset or its cached version
-    is stored in the :ref:`data home <storage>` folder.
+    is stored in the data_home folder.
 
     Parameters
     ----------
     keep_original : bool, default=True
         Determines whether the original dataset is deleted after downloading
         or kept on the hard drive.
     cache : bool, default=True
@@ -110,15 +108,15 @@
     devices = pd.DataFrame(columns=cols)
     with open(os.path.join(data_path, 'README'), 'r') as file:
         lines = file.readlines()
         # create header
         for line in lines[7:27]:
             s = list(filter(None, line.split('\t')))
             s[-1:] = [s[-1:][0][:-1]]
-            devices.loc[len(devices), :] = s[1:]
+            devices.loc[len(devices), :] = [a.strip() for a in s[1:]]
 
     return devices
 
 
 def _get_activity_map(data_path):
     """
     Parameters
@@ -188,15 +186,15 @@
     df_end = df[mask_end].reset_index(drop=True)
     
     df_start[END_TIME] = df_end['index']
     
     df = df_start[[START_TIME, END_TIME, res_name]]
     df = df.sort_values(by=START_TIME)
     df = df.rename(columns={res_name: ACTIVITY})
-    df = df[df[ACTIVITY] != 'Other'] # remove Other activity as it is the same concept as 'idle'
+    df = df[df[ACTIVITY] != 'Other'] # remove Other activity as it is the same concept as 'other'
     return df
 
 
 def _create_device_df(df):
     """ gets a raw representation and returns devices in rep1
     Parameters
     ----------
@@ -221,9 +219,11 @@
         tmp.columns = [TIME, VALUE]
         tmp[DEVICE] = device
         
         res = pd.concat([res, tmp])
     
     res = res.sort_values(by=TIME).reset_index(drop=True)
     res[VALUE] = res[VALUE].astype(bool)
+    res[DEVICE] = res[DEVICE].astype('category')
+    res[TIME] = pd.to_datetime(res[TIME])
     return res
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/homeassistant.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/homeassistant.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,50 +32,48 @@
     df : pd.DataFrame
     """
     limit=5000000
 
     """ weird new requirement 
     """
     if 'sqlite' in db_url:
-        lc_null_fix = ",iif(last_changed is NULL,last_updated,last_changed) as last_changed"
+        lc_null_fix = ",iif(last_changed_ts is NULL,last_updated_ts,last_changed_ts) as last_changed_ts"
     elif 'mariadb' in db_url:
-        lc_null_fix = ",if(last_changed is NULL,last_updated,last_changed) as last_changed"
+        lc_null_fix = ",if(last_changed_ts is NULL,last_updated_ts,last_changed_ts) as last_changed_ts"
     elif 'postgresql' in db_url:
-        lc_null_fix = ',(case when last_changed is NULL then last_updated else last_changed end)'
+        lc_null_fix = ',(case when last_changed_ts is NULL then last_updated_ts else last_changed_ts end)'
     else:
         print("WARNING: LAST_CHANGED may be null not substituted")
         lc_null_fix = ''
 
-
-    if start_time == None and end_time == None:
-        query = f"""
-        SELECT entity_id, state, last_updated
-        {lc_null_fix}
-        FROM states
-        WHERE
-            state NOT IN ('unknown', 'unavailable')
-        ORDER BY last_updated DESC
-        LIMIT {limit}
-        """
-    else:
-        if end_time == None:
-            end_time = datetime.datetime.utcnow()
-        query = f"""
-        SELECT entity_id, state, last_updated
-        {lc_null_fix}
-        FROM states
-        WHERE
-            state NOT IN ('unknown', 'unavailable') AND
-            last_updated BETWEEN 
-            '{start_time}' AND '{end_time}'
-        ORDER BY last_updated ASC
-        LIMIT {limit}
-        """
+    # Convert timestamps to seconds
+    start_time_nx = pd.Timestamp(start_time).timestamp()
+    end_time_nx = pd.Timestamp(end_time).timestamp()
+
+    if start_time is None and end_time is None:
+        cond_time = ''
+    if start_time is None and end_time is not None:
+        raise NotImplementedError
+    if start_time is not None and end_time is None:
+        raise NotImplementedError
+    if start_time is not None and end_time is not None:
+        cond_time = f"AND last_updated_ts BETWEEN '{start_time_nx}' AND '{end_time_nx}'"
+    
+    query = f"""
+    SELECT entity_id, state, last_updated_ts
+    {lc_null_fix}
+    FROM states
+    WHERE
+        state NOT IN ('unknown', 'unavailable')
+        {cond_time}
+    LIMIT {limit}
+    """
     df = pd.read_sql_query(query, db_url)
-    df = df.drop(columns='last_updated')
+    df['last_changed_ts'] = pd.to_datetime(df['last_changed_ts'], unit='s', origin='unix')
+    df = df.drop(columns='last_updated_ts')
     return df
 
 def load_homeassistant_devices(db_url, device_list, start_time=None, end_time=None):
     """
     Creates a device dataframe for selected devices within a certain timeframe.
 
     Parameters
@@ -104,20 +102,20 @@
     """
     
     df = load_homeassistant(db_url, start_time=start_time, end_time=end_time)
 
 
     # Bring into pyadlml structure
     df = df[df['entity_id'].isin(device_list)]
-    df = df.rename(columns={'entity_id': DEVICE, 'state': VALUE, 'last_changed': TIME})
+    df = df.rename(columns={'entity_id': DEVICE, 'state': VALUE, 'last_changed_ts': TIME})
     df = df[[TIME, DEVICE, VALUE]]
 
     # Convert to proper datatypes
     df[TIME] = pd.to_datetime(df[TIME])
 
     # Map binary device values to -> True, False
-    # TODO critical, what happens if a non-binary-device 
     #      is on or off or if binary-device is not on or off
-    df[VALUE] = df[VALUE].replace(to_replace='on', value=1)
-    df[VALUE] = df[VALUE].replace(to_replace='off', value=0)
+    df[VALUE] = df[VALUE].replace(to_replace='on', value=True)
+    df[VALUE] = df[VALUE].replace(to_replace='off', value=False)
+    df[DEVICE] = df[DEVICE].astype('category')
 
     return df
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/kasteren_2010.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/kasteren_2010.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,89 @@
+import os
 from pathlib import Path
-
 import pandas as pd
-from pyadlml.dataset._core.obj import Data
 from pyadlml.constants import ACTIVITY, VALUE, \
     START_TIME, END_TIME, TIME, NAME, DEVICE
-from pyadlml.dataset._core.activities import correct_activities
-from pyadlml.dataset._core.devices import correct_devices, CORRECTION_TS, CORRECTION_ONOFF_INCONS
-from pyadlml.dataset.io import fetcher, correct_acts_and_devs, download_from_mega
 import numpy as np
 from pyadlml.dataset._core.devices import device_boolean_on_states_to_events
-import os
+from pyadlml.dataset.io.downloader import MegaDownloader
+from pyadlml.dataset.io.remote import DataFetcher
 
 """
 Transferring Knowledge of Activity Recognition across Sensor Networks
 T.L.M. van Kasteren, G. Englebienne and B.J.A. Kr�se
 In Proceedings of the Eighth International Conference on Pervasive Computing (Pervasive 2010). Helsinki, Finland, 2010. 
 
 """
 
 
 KASTEREN_2010_URL = 'https://mega.nz/file/VIhnxAxB#3UI77ZA1uh0tRiT6vHTfhYolm-uxbAXuV2TxxIyQ2AU'
 KASTEREN_2010_FILENAME = 'kasteren_2010.zip'
 
+KASTEREN_2010_A_CLEANED_URL = 'https://mega.nz/file/RJYmlKrB#9UuLiAS0yhtud98TmRc4D7uRfEYdFh5USWVMnUekWyo'
+KASTEREN_2010_A_CLEANED_FN = 'cleaned_kasteren_2010_A.joblib'
+
+KASTEREN_2010_B_CLEANED_URL = 'https://mega.nz/file/8QgFDCAT#2nQRGyelCE82VgA_N28W5edOU6hyTA8mjv_MNW-WBGk'
+KASTEREN_2010_B_CLEANED_FN = 'cleaned_kasteren_2010_B.joblib'
+
+KASTEREN_2010_C_CLEANED_URL = 'https://mega.nz/file/8Ihj0a6S#WNPJlS0eO1Gx5GkQlleR-d2t1_Ih3xC_sstnSgQXRoY'
+KASTEREN_2010_C_CLEANED_FN = 'cleaned_kasteren_2010_C.joblib'
+
+
+
+class KasterenFetcher(DataFetcher):
+    def __init__(self, auto_corr_acts=True):
+
+        downloader = MegaDownloader(
+            url=KASTEREN_2010_URL,
+            fn=KASTEREN_2010_FILENAME,
+            url_cleaned={
+                'A': KASTEREN_2010_A_CLEANED_URL,
+                'B': KASTEREN_2010_B_CLEANED_URL,
+                'C': KASTEREN_2010_C_CLEANED_URL,
+            },
+            fn_cleaned={
+                'A': KASTEREN_2010_A_CLEANED_FN,
+                'B': KASTEREN_2010_B_CLEANED_FN,
+                'C': KASTEREN_2010_C_CLEANED_FN,
+            },
+        )
+
+        super().__init__(
+            dataset_name='kasteren_2010',
+            downloader=downloader,
+            correct_activities=auto_corr_acts,
+            correct_devices=True
+        )
+
+    def load_data(self, folder_path, ident: str) -> dict:
+        assert ident in ['A', 'B', 'C']
+
+        # Load activity structure
+        path = Path(folder_path).joinpath('datasets', 'house%s'%ident)
+        df_acts = _load_activities(path, ident)
+        df_devs = _load_devices(path, ident)
+
+        lst_act = df_acts[ACTIVITY].unique()
+        lst_dev = df_devs[DEVICE].unique()
+
+        return dict(
+            activities=df_acts,
+            devices=df_devs,
+            activity_list=lst_act,
+            device_list=lst_dev
+        )
+
+
+
+
 #@correct_acts_and_devs
-@fetcher('kasteren_2010', download_from_mega, KASTEREN_2010_FILENAME, KASTEREN_2010_URL)
-def fetch_kasteren_2010(house='A', keep_original=False, cache=True,
-                        retain_corrections=False, folder_path=None):
+def fetch_kasteren_2010(house:str ='A', keep_original=False, cache=True,
+                        auto_corr_activities=True, load_cleaned=False,
+                        retain_corrections=False, folder_path=None) -> dict:
     """
     Fetches the amsterdam dataset from the internet. The original dataset or its cached version
     is stored in the :ref:`data home <storage>` folder.
 
     Parameters
     ----------
     house : str one of {'A', 'B', 'C'}, default='A'
@@ -37,51 +91,43 @@
         different time.
     keep_original : bool, default=False
         Determines whether the original dataset is deleted after downloading
         or kept on the hard drive.
     cache : bool, default=True
         Determines whether the data object should be stored as a binary file for quicker access.
         For more information how caching is used refer to the :ref:`user guide <storage>`.
+    load_cleaned : bool, default=False
+        Whether to load the 
+    auto_corr_activities : bool, default=True
+        Return activities and devices as is, without applying any correction. You have 
+        entered the danger zone.
     retain_corrections : bool, default=False
         When set to *true*, data points that change or drop during preprocessing
         are listed in respective attributes of the data object. Fore more information
         about error correction refer to the :ref:`user guide <error_correction>`.
     folder_path : str, default=None
         If set the dataset is loaded from the specified folder.
 
     Examples
     --------
     >>> from pyadlml.dataset import fetch_kasteren
-    >>> data = fetch_kasteren_2010()
-    >>> dir(data)
-    >>> [..., df_activities, df_devices, ...]
+    >>> data = fetch_kasteren_2010(house='B')
+    >>> data['activities']
+        {...}
 
     Returns
     -------
-    data : object
+    dict
+        A dictionary containing device and activity dataframes
     """
-    assert house in ['A', 'B', 'C']
-
-    # load activity structure
-    path = Path(folder_path).joinpath('datasets', 'house%s'%(house))
-    df_act = _load_activities(path, house)
-    df_dev = _load_devices(path, house)
-
-    lst_act = df_act[ACTIVITY].unique()
-    lst_dev = df_dev[DEVICE].unique()
-
-    data = Data(df_act, df_dev,
-                activity_list=lst_act,
-                device_list=lst_dev
+    return KasterenFetcher(auto_corr_acts=auto_corr_activities)(keep_original=keep_original, cache=cache, #load_cleaned=load_cleaned,
+                              retain_corrections=retain_corrections, folder_path=folder_path,
+                              ident=house, load_cleaned=load_cleaned
     )
 
-    return data
-
-
-
 def _load_activities(path, house):
 
     from scipy.io import loadmat
     tmp = loadmat(str(path.joinpath(f'actStructHouse{house}.mat')))
     acts = tmp['activityStructure'][0][0][0]
 
     # load act and devs
@@ -129,14 +175,18 @@
     # load device labels
     if house == 'A':
         dev_map = {}
         dev_labels = tmp['sensor_labels']
         nr_devs = dev_labels.shape[0]
         for i in range(nr_devs):
             dev_map[dev_labels[i][0][0][0]] = dev_labels[i][1][0]
+        
+        # The sensor names are flipped in the original dataset
+        dev_map[5] = 'Hall-Bathroom door'
+        dev_map[6] = 'Hall-Toilet door'
     elif house == 'B':
         dev_map = _dev_map_House_B()
     elif house == 'C':
         dev_map = _dev_map_House_C()
 
     df_dev = pd.DataFrame({START_TIME: devs[:, 0], END_TIME: devs[:, 1], DEVICE: devs[:, 2]})
     df_dev[START_TIME] = df_dev[START_TIME].apply(matlab_date_to_timestamp)
@@ -148,14 +198,15 @@
         # therefore those two entries are dropped
         #                     start_time                   end_time  device
         #2003 2009-07-24 16:16:20.999997 2009-07-24 16:16:22.000001    23.0
         #2005 2009-07-24 16:22:09.000000 2009-07-24 16:22:10.999999    23.0
         df_dev = df_dev.dropna()
 
     df_dev = device_boolean_on_states_to_events(df_dev)
+    df_dev[DEVICE] = df_dev[DEVICE].astype('category')
     return df_dev
 
 from datetime import datetime, timedelta
 def matlab_date_to_timestamp(matlab_datenum):
     """ converts a matlab datenum representation to pandas timestamp"""
     # convert matlab dateformat to python
     # copied from @actstruct/actstruct.m
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/mitlab.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/mitlab.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,96 @@
 import pandas as pd
 from pathlib import Path
 from pyadlml.constants import ACTIVITY, DEVICE, START_TIME, END_TIME
-from pyadlml.dataset._core.activities import _create_activity_df
+from pyadlml.dataset._core.activities import create_empty_activity_df
 from pyadlml.dataset._core.devices import device_boolean_on_states_to_events
-from pyadlml.dataset._core.obj import Data
-from pyadlml.dataset.io import fetcher, correct_acts_and_devs, download_from_mega
+from pyadlml.dataset.io.downloader import MegaDownloader
+from pyadlml.dataset.io.remote import DataFetcher
 
 MITLAB_URL = 'https://mega.nz/file/MB4BFL6S#8MjAQoS-j0Lje1UFoWUMOCay2FcdpVfla6p9MTe4SQM'
 MITLAB_FILENAME = 'mitlab.zip'
-
 SUB1 = 'subject1'
 SUB2 = 'subject2'
 
-@correct_acts_and_devs
-@fetcher('mitlab', download_from_mega, MITLAB_FILENAME, MITLAB_URL)
+__all__ = ['fetch_mitlab']
+
+class MitLabFetcher(DataFetcher):
+    def __init__(self, *args, **kwargs):
+
+        downloader = MegaDownloader(
+            url=MITLAB_URL,
+            fn=MITLAB_FILENAME,
+            url_cleaned=None,
+            fn_cleaned=None,
+        )
+
+        super().__init__(
+            dataset_name='mitlab',
+            downloader=downloader,
+            correct_activities=True,
+            correct_devices=True
+        )
+
+
+    def load_data(self, folder_path, ident):
+
+        assert ident in [SUB1, SUB2]
+
+        act_path = Path(folder_path).joinpath(ident, "Activities.csv")
+        dev_path = Path(folder_path).joinpath(ident, "sensors.csv")
+        data_path = Path(folder_path).joinpath(ident, "activities_data.csv")
+
+        df_dev_map = _load_device_map(dev_path)
+        df_act_map = _load_activity_map(act_path)
+        df_dev, df_act = _read_data(data_path, df_dev_map, df_act_map)
+        df_dev = device_boolean_on_states_to_events(df_dev)
+        df_dev[DEVICE] = df_dev[DEVICE].astype('category')
+        lst_act = df_act[ACTIVITY].unique()
+        lst_dev = df_dev[DEVICE].unique()
+
+        return dict(
+            activities=df_act,
+            devices=df_dev,
+            activity_list=lst_act,
+            device_list=lst_dev
+        )
+
+
+
 def fetch_mitlab(subject='subject1', keep_original=False, cache=True,
-                 retain_corrections=False, folder_path=None):
+                 retain_corrections=False, folder_path=None) -> dict:
     """
     Fetches the :ref:`mitlab <ds_mitlab>` dataset from the internet. The original dataset or its cached version
-    is stored in the :ref:`data home <storage>` folder.
+    is stored in the data_home folder.
 
     Parameters
     ----------
     subject : str of {'subject1', 'subject2'}
-        Determines which dataset is loaded.
+        Identifies which dataset is loaded.
     keep_original : bool, default=True
         Determines whether the original dataset is deleted after downloading
         or kept on the hard drive.
     cache : bool, default=True
         Determines whether the data object should be stored as a binary file for quicker access.
         For more information how caching is used refer to the :ref:`user guide <storage>`.
     retain_corrections : bool, default=False
         When set to *true*, data points that change or drop during preprocessing
         are listed in respective attributes of the data object. Fore more information
         about error correction refer to the :ref:`user guide <error_correction>`.
 
     Returns
     -------
-    data : object
+    dict
     """
-    assert subject in [SUB1, SUB2]
-
-    act_path = Path(folder_path).joinpath(subject, "Activities.csv")
-    dev_path = Path(folder_path).joinpath(subject, "sensors.csv")
-    data_path = Path(folder_path).joinpath(subject, "activities_data.csv")
-
-    df_dev_map = _load_device_map(dev_path)
-    df_act_map = _load_activity_map(act_path)
-    df_dev, df_act = _read_data(data_path, df_dev_map, df_act_map)
-    df_dev = device_boolean_on_states_to_events(df_dev)
-
-    lst_act = df_act[ACTIVITY].unique()
-    lst_dev = df_dev[DEVICE].unique()
+    return MitLabFetcher()(keep_original=keep_original, cache=cache, #load_cleaned=load_cleaned,
+                           retain_corrections=retain_corrections, folder_path=folder_path, 
+                           ident=subject
+    )
 
-    data = Data(df_act, df_dev, activity_list=lst_act, device_list=lst_dev)
 
-    return data
 
 
 def _load_device_map(path_to_file):
     df_subx_dev = pd.read_csv(path_to_file, sep=",", header=None)
     df_subx_dev.columns = ['id', 'room', 'device']
 
     df_subx_dev['device'] = df_subx_dev['id'].astype(str) + ' - ' \
@@ -94,15 +125,15 @@
     df_devices : pd.DataFrame
     
     df_activities : pd.DataFrame
         
     """
     # create empy dataframes for devices and activities
     df_devices = pd.DataFrame(columns=[START_TIME, END_TIME, DEVICE])
-    df_activities = _create_activity_df()
+    df_activities = create_empty_activity_df()
 
     act_list = df_act['Subcategory'].values
     
     with open(path_to_file, 'r') as f_o:
         i = 0
         read_in_device = False
         date = None
@@ -119,15 +150,16 @@
                 """
                 if date == '4/31/2003':
                     date = '5/1/2003'
                 new_row = {'activity':s[0], 
                            'start_time':pd.Timestamp(date +'T'+s[2]), 
                            'end_time':pd.Timestamp(date +'T'+s[3])
                           }
-                df_activities = df_activities.append(new_row, ignore_index=True)
+                df_activities = pd.concat([df_activities, pd.Series(data=new_row).to_frame().T],\
+                                           ignore_index=True, axis=0)
                 continue      
                 
             # check if the line represents a device
             elif not read_in_device:
                 try:
                     read_in_device = True
                     devices = s
@@ -164,15 +196,16 @@
                         
                 # create rows
                 for dev, ts_start, ts_end in zip(devices, ts_act, ts_deact):
                     new_row = {DEVICE:dev,
                                START_TIME:pd.Timestamp(date +'T' + ts_start),
                                END_TIME:pd.Timestamp(date +'T' + ts_end)
                               }
-                    df_devices = df_devices.append(new_row, ignore_index=True)                
+                    df_devices = pd.concat([df_devices, pd.Series(data=new_row).to_frame().T],\
+                                           ignore_index=True, axis=0)
                 i = 0
                 read_in_device = False
                 
         f_o.close()
         
     # map device ids to strings    
     df_devices[DEVICE] = df_devices[DEVICE].astype(int)
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/tuebingen_2019.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/tuebingen_2019.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import pyadlml.dataset._datasets.activity_assistant as act_assist
 from pyadlml.constants import ACTIVITY
-from pyadlml.dataset.io import fetcher, correct_acts_and_devs, download_from_mega
+from pyadlml.dataset.io.downloader import MegaDownloader
+from pyadlml.dataset.io.remote import DataFetcher
 
 TUE_2019_URL = 'https://mega.nz/file/sRIT0ILI#us-EtWRCMtvzoqkbsz8UofAbqomn3Px3CLXw1NxSCxY'
 TUE_2019_FILENAME = 'tuebingen_2019.zip'
 TUE_2019_CLEANED_URL = 'https://mega.nz/file/wcRhWayA#itY_OorjDdU60RCwY4WMCansb3GqPqvzb6R1o3crNs0'
 TUE_2019_CLEANED_FILENAME = 'tuebingen_2019_cleaned.zip'
 
 
 # The activity and device corrections are already applied from act_assist.load
-@fetcher('tuebingen_2019', download_from_mega, TUE_2019_FILENAME, TUE_2019_URL,\
-         TUE_2019_CLEANED_FILENAME, TUE_2019_CLEANED_URL)
 def fetch_tuebingen_2019(keep_original=False, cache=True, load_cleaned=False,\
                          retain_corrections=False, folder_path=None):
     """
     Fetches the tuebingen_2019 dataset from the internet. The original dataset or its cached version
-    is stored in the :ref:`data home <storage>` folder.
+    is stored in the data_home folder.
 
     Parameters
     ----------
     keep_original : bool, default=True
         Determines whether the original dataset is deleted after downloading
         or kept on the hard drive.
     cache : bool, default=True
@@ -31,8 +30,30 @@
         are listed in the respective attributes of the data object.  Fore more information
         about the attributes refer to the :ref:`user guide <error_correction>`.
 
     Returns
     -------
     data : object
     """
-    return act_assist.load(folder_path, subjects=['M'], retain_corrections=retain_corrections)
+
+    class TueFetcher(DataFetcher):
+        def load_data(self, folder_path):
+            return act_assist.load(fp=folder_path)
+
+
+    downloader = MegaDownloader(
+        url=TUE_2019_URL,
+        fn=TUE_2019_FILENAME,
+        url_cleaned=TUE_2019_CLEANED_URL,
+        fn_cleaned=TUE_2019_CLEANED_FILENAME,
+    )
+
+    data_fetch = TueFetcher(
+        dataset_name='tuebingen_2019',
+        downloader=downloader,
+        correct_activities=True,
+        correct_devices=True
+    )
+
+    
+    return data_fetch(keep_original=keep_original, cache=cache, load_cleaned=load_cleaned,
+            retain_corrections=retain_corrections, folder_path=folder_path)
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/_datasets/uci_adl_binary.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/_datasets/activity_assistant.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,133 +1,204 @@
+import functools
+import os
 import pandas as pd
+import numpy as np
+from pathlib import Path
+from pyadlml.constants import AREA, START_TIME, END_TIME, DEVICE, VALUE, TIME, ACTIVITY, STRFTIME_PRECISE
+from pyadlml.dataset._core.activities import ActivityDict
+from pyadlml.dataset.util import extract_kwargs
+
+DATA_NAME = 'devices.csv'
+DEV_MAP_NAME = 'device_map.csv'
+ACT_MAP_NAME = 'activity_map.csv'
+DEV2AREA_NAME = 'device_area_map.csv'
+ACT2AREA_NAME = 'activity_area_map.csv'
+ACT_NAME = 'activities_subject_%s.csv'
+MAP_ID = 'id'
+
 
-from pyadlml.constants import ACTIVITY, DEVICE, END_TIME, START_TIME
-from pyadlml.dataset._core.activities import correct_activities
-from pyadlml.dataset._core.devices import device_boolean_on_states_to_events
-from pyadlml.dataset._core.obj import Data
-from pyadlml.dataset.io import fetcher, correct_devs, download_from_mega
-import os
 
-UCI_ADL_BINARY_URL = 'https://mega.nz/file/AQIgDQJD#oximAQFjexTKwNP3WYzlPnOGew06YSQ2ef85vvWGN94'
-UCI_ADL_BINARY_FILENAME = 'uci_adl_binary.zip'
-ORD_A = 'OrdonezA'
-ORD_B = 'OrdonezB'
+def _folder2filename(filename):
+    def deco(func):
+        @extract_kwargs
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            path = kwargs.pop('path')
+            path = Path(path) if isinstance(path, str) else path
+            if not path.is_file() and path.is_dir():
+                # If there is no file and the path is maps to a directory
+                # create the filename after convention
+                kwargs['path'] = path.joinpath(filename)
+            else:
+                kwargs['path'] = path       
+
+            return func(*args, **kwargs)
+        return wrapper
+    return deco
 
 
-@correct_devs   # only correct devices as activities are explicitly handled in function body
-@fetcher('uci_adl_binary', download_from_mega, UCI_ADL_BINARY_FILENAME, UCI_ADL_BINARY_URL)
-def fetch_uci_adl_binary(subject='OrdonezA', keep_original=True, cache=True,
-                         retain_corrections=False, folder_path=None) -> Data:
+@_folder2filename(ACT_NAME)
+def read_activities(path: Path, act_map: dict = None):
     """
+    """
+    df_acts = pd.read_csv(path)
 
-    Parameters
-    ----------
-    subject : str of {'OrdonezA', 'OrdonezB'}, default='OrdonezA'
-        decides which dataset of the two houses is loaded.
-    keep_original : bool, default=True
-        Determines whether the original dataset is deleted after downloading
-        or kept on the hard drive.
-    cache : bool
-        Determines whether the data object should be stored as a binary file for quicker access.
-        For more information how caching is used refer to the :ref:`user guide <storage>`.
-    retain_corrections : bool
-        When set to *true* data points that are changed or dropped during preprocessing
-        are listed in the respective attributes of the data object.  Fore more information
-        about the attributes refer to the :ref:`user guide <error_correction>`.
+    if act_map is not None:
+        df_acts[ACTIVITY] = df_acts[ACTIVITY].map(act_map)
 
+    df_acts[ACTIVITY] = df_acts[ACTIVITY].astype('category')
+    df_acts[START_TIME] = pd.to_datetime(df_acts[START_TIME], format=STRFTIME_PRECISE)
+    df_acts[END_TIME] = pd.to_datetime(df_acts[END_TIME], format=STRFTIME_PRECISE)
+    return df_acts
 
-    Returns
-    -------
-    data : object
+@_folder2filename(ACT_NAME)
+def write_activities(df: pd.DataFrame, path) -> None:
+    df.to_csv(path, index=False, date_format=STRFTIME_PRECISE)
+
+
+@_folder2filename(DATA_NAME)
+def write_devices(df, path):
+    df.to_csv(path, index=False, date_format=STRFTIME_PRECISE)
+
+@_folder2filename(DATA_NAME)
+def read_devices(path: Path, dev_map: dict = None):
     """
-    assert subject in [ORD_A, ORD_B]
+    Parameters
+    ----------
+    path: Path
+        either path to file direct, or path to folder conatining
+        'devices.csv' file
+    """
+    df_devs = pd.read_csv(path)
 
-    # fix path and Ordonez B activity file
-    sub_dev_file = os.path.join(folder_path, '{}_Sensors.txt'.format(subject))
-    if subject == ORD_B:
-        fix_OrdonezB_ADLS(os.path.join(folder_path, 'OrdonezB_ADLs.txt'))
-        sub_act_file = os.path.join(folder_path, '{}_ADLs_corr.txt'.format(subject))
-    else:
-        sub_act_file = os.path.join(folder_path, '{}_ADLs.txt'.format(subject))
-
-    # load activities and devices
-    df_act = _load_activities(sub_act_file)
-    df_dev, df_loc = _load_devices(sub_dev_file)
-    df_dev = device_boolean_on_states_to_events(df_dev)
-
-    lst_act = df_act[ACTIVITY].unique()
-    lst_dev = df_dev[DEVICE].unique()
-
-    data = Data(None, df_dev, activity_list=lst_act, device_list=lst_dev)
-    data.df_dev_rooms = df_loc
-
-    # manual activity correction for OrdonezB
-    if subject == ORD_B:
-        # the activity grooming is often overlapped by sleeping
-        # Since grooming is more important make it the dominant activity (opinionated)
-        df_act, correction_act = correct_activities(df_act, excepts=['Grooming'], retain_corrections=retain_corrections)
-
-    elif subject == ORD_A:
-        # Manually replace 3 rows where START_TIME > END_TIME in the activity files
-        # 72 "2011-12-01 19:28:51  2011-12-01 16:29:59  Toileting"
-        # to "2011-12-01 19:28:51  2011-19-01 16:29:59  Toileting"
-        # 81 "2011-12-02 12:20:41  2011-12-01 10:20:59  Grooming"
-        # to "2011-12-02 12:20:41  2011-12-01 12:20:59  Grooming"
-        # 83 "2011-12-02 12:27:47  2011-12-01 11:35:49  Breakfast"
-        # to "2011-12-02 12:27:47  2011-12-01 12:35:49  Breakfast"
-        df_act.iat[69, 1] = pd.Timestamp('2011-12-01 19:29:59')
-        df_act.iat[78, 1] = pd.Timestamp('2011-12-02 12:20:59')
-        df_act.iat[80, 1] = pd.Timestamp('2011-12-02 12:35:49')
-
-        df_act, correction_act = correct_activities(df_act, retain_corrections=retain_corrections)
-
-    data.set_activity_df(df_act, subject)
+    if dev_map is not None:
+        df_devs[DEVICE] = df_devs[DEVICE].map(dev_map)
 
-    if retain_corrections:
-        data.set_activity_correction(correction_act, subject)
+    # TODO refactor, ensure that True, False mapping is only applied
+    #      to devices with two values 
+    df_devs[VALUE] = df_devs[VALUE].astype(str).replace({
+        "0": False, "0.0": False, 
+        "1": True, "1.0": True,
+        "True":True, "False": False,
+        "true":True, "false": False,
+    })
+    df_devs[TIME] = pd.to_datetime(df_devs[TIME], format=STRFTIME_PRECISE)
+    df_devs[DEVICE] = df_devs[DEVICE].astype('category')
+    df_devs = df_devs.reset_index(drop=True)
+    return df_devs
+
+@_folder2filename(DEV2AREA_NAME)
+def read_device2area(path: Path, dev_map: dict) -> pd.DataFrame:
+    """"""
+    dev2area = pd.read_csv(path, sep=";")
+    dev2area[DEVICE] = dev2area[DEVICE].map(dev_map)
+    assert (dev2area.columns == np.array([DEVICE, AREA])).all()
+    return dev2area
+
+@_folder2filename(DEV2AREA_NAME)
+def write_device2area(df: pd.DataFrame, path: Path):
+    assert (df.columns == np.array([DEVICE, AREA])).all()
+    raise NotImplementedError
+    df.to_csv(path, sep=',', index=False)
+
+
+@_folder2filename(ACT2AREA_NAME)
+def read_activity2area(path: Path, act_map: dict) -> pd.DataFrame:
+    """"""
+    act2area = pd.read_csv(path, sep=";")
+    act2area[ACTIVITY] = act2area[ACTIVITY].map(act_map)
+    act2area[AREA] = act2area[AREA].apply(lambda x: x[1:-1].split(','))
+    assert (act2area.columns == np.array([ACTIVITY, AREA])).all()
+    return act2area
+
+@_folder2filename(ACT2AREA_NAME)
+def write_activity2area(df: pd.DataFrame, path: Path):
+    assert (df.columns == np.array([ACTIVITY, AREA])).all()
+    df.to_csv(path, sep=';', index=False)
+
+
+@_folder2filename(DEV_MAP_NAME)
+def read_device_map(path: Path) -> dict: 
+    return pd.read_csv(path, index_col=MAP_ID)\
+                .to_dict()[DEVICE]
+
+@_folder2filename(DEV_MAP_NAME)
+def write_device_map(df: pd.DataFrame, path: Path):
+    assert (df.columns == np.array(['id', DEVICE])).all()
+    df.to_csv(path, sep=',', index=False)
+
+@_folder2filename(ACT_MAP_NAME)
+def read_activity_map(path: Path) -> dict:
+    return pd.read_csv(path, index_col=MAP_ID)\
+                .to_dict()[ACTIVITY]
+
+@_folder2filename(ACT_MAP_NAME)
+def write_activity_map(df: pd.DataFrame, path: Path):
+    assert (df.columns == np.array(['id', ACTIVITY])).all()
+    df.to_csv(path, sep=',', index=False)    
 
-    return data
 
 
-def fix_OrdonezB_ADLS(path_to_file):
-    """ fixes inconsistent use of tabs for delimiter in the file
+def load(folder_path: str, subjects:list=[], retain_corrections=False) -> dict:
+    """
+    Loads a dataset generated by activity-assistant from a specified folder.
+
     Parameters
     ----------
-    path_to_file : str
-        path to the file OrdonezB_ADLs.csv
+    folder_path : str
+        The path to the folder where the dataset is located.
+
+    subjects : list of str
+        The subjecst names that are to be included. If the activity file
+        is named *activities_subject_foo.csv*, then *foo* is the corresponding name.
+
+    Examples
+    --------
+    The dataset ``my_dataset.zip`` is extracted in the folder ``/path/to/``.
+
+    >>> from pyadlml.dataset import load_act_assist
+    >>> data = load_act_assist('/path/to/my_dataset/', subjects=['chris'])
+
+    Returns
+    -------
+    data : object
     """
-    
-    path_corrected = path_to_file[:-17] + 'OrdonezB_ADLs_corr.txt'
-    
-    with open(path_to_file, 'r') as f_o, open(path_corrected, 'w') as f_t:
-        for i, line in enumerate(f_o.readlines()):            
-            if i in [0,1]: 
-                f_t.write(line)  
-                continue
-            s = line.split()
-            assert len(s) == 5
-            new_line = s[0]+' '+s[1]+'\t\t'+s[2]+' '+s[3]+'\t\t'+s[4]                        
-            f_t.write(new_line + "\n")
-        f_t.close()
-        f_o.close()
-
-def _load_activities(act_path):
-    df_act = pd.read_csv(act_path, delimiter='\t+', skiprows=[0,1], 
-                         names=[START_TIME, END_TIME, ACTIVITY], engine='python')
-    df_act[START_TIME] = pd.to_datetime(df_act[START_TIME])
-    df_act[END_TIME] = pd.to_datetime(df_act[END_TIME])
-    return df_act
-
-def _load_devices(dev_path):
-    df_dev = pd.read_csv(dev_path, delimiter='\t+', skiprows=[0, 1], 
-                         names=[START_TIME, END_TIME, 'Location', 'Type', 'Place'], 
-                         engine='python')
-    df_dev[DEVICE] = df_dev['Place'] + ' ' + df_dev['Location'] + ' ' + df_dev['Type']
-    
-    # get room mapping devices
-    df_locs = df_dev.copy().groupby([DEVICE, 'Type', 'Place', 'Location']).sum()
-    df_locs = df_locs.reset_index().drop([START_TIME, END_TIME], axis=1)
-
-    df_dev = df_dev[[START_TIME, END_TIME, DEVICE]]
-    df_dev[START_TIME] = pd.to_datetime(df_dev[START_TIME])
-    df_dev[END_TIME] = pd.to_datetime(df_dev[END_TIME])
-    return df_dev, df_locs
+    assert isinstance(folder_path, str) or isinstance(folder_path, Path)
+    assert isinstance(subjects, list)
+    fp = Path(folder_path) 
+
+
+    # Get mappings
+    act_map = read_activity_map(fp.joinpath(ACT_MAP_NAME))
+    dev_map = read_device_map(fp.joinpath(DEV_MAP_NAME))
+
+    # Get dev and act list
+    lst_dev = dev_map.values()
+    lst_act = act_map.values()
+
+    # Get area mappings
+    dev2area = read_device2area(fp.joinpath(DEV2AREA_NAME), dev_map)
+    act2area = read_activity2area(fp.joinpath(ACT2AREA_NAME), act_map)
+
+
+    df_dev = read_devices(fp.joinpath(DATA_NAME), dev_map)
+
+    # If no subjects where specified read the files from the folder following the naming schemata
+    if not subjects:
+        for file in Path(fp).iterdir():
+            if ACT_NAME[:18] in file.name:
+                subjects.append(file.name[19:-4])
+
+    act_dct = ActivityDict()
+    for subject in subjects:
+        df_act = read_activities(Path(fp).joinpath(ACT_NAME%(subject)),
+                                  act_map)
+        act_dct[subject] = df_act
+
+    return dict(
+        devices=df_dev,
+        device_list=lst_dev,
+        activities=act_dct,
+        activity_list=lst_act,
+        dev2area=dev2area,
+        act2area=act2area
+    )
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/bokeh/activities.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/plot/_bokeh/activities.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from bokeh.models import ColumnDataSource, RadioButtonGroup, CustomJS, CheckboxGroup, Select, DataRange, DataRange1d, \
     FuncTickFormatter, LogTickFormatter, Panel, Tabs
 
 from pyadlml.dataset import ACTIVITY
 from  pyadlml.dataset.stats.activities import activities_duration_dist, activity_duration,\
     activities_transitions, activities_count, activity_duration, activities_dist
 from pyadlml.dataset._core.activities import add_other_activity
-from pyadlml.dataset.plot.util import func_formatter_seconds2time_log, ridgeline, \
-    func_formatter_seconds2time, heatmap, annotate_heatmap, heatmap_square, savefig, \
+from pyadlml.dataset.plot.util import fmt_seconds2time_log, ridgeline, \
+    fmt_seconds2time, heatmap, annotate_heatmap, heatmap_square, savefig, \
     _num_bars_2_figsize, _num_boxes_2_figsize, \
     _num_items_2_heatmap_square_figsize, _num_items_2_ridge_figsize,\
     _num_items_2_ridge_ylimit
 from pyadlml.util import get_sequential_color, get_secondary_color, get_primary_color, get_diverging_color
 from bokeh.plotting import figure, show
 
 def hist_counts(df_acts=None, lst_acts=None, df_ac=None):
@@ -356,15 +356,15 @@
     ax.set_xlabel(xlabel)
     ax.set_xscale('log')
 
     # create secondary axis with time format 1s, 1m, 1d
     ax_top = ax.secondary_xaxis('top', functions=(lambda x: x, lambda x: x))
     #ax_top.set_xlabel('time')
     ax_top.xaxis.set_major_formatter(
-        ticker.FuncFormatter(func_formatter_seconds2time))
+        ticker.FuncFormatter(fmt_seconds2time))
 
     if file_path is not None:
         savefig(fig, file_path)
         return 
     else:
         return fig
 
@@ -415,15 +415,15 @@
 
     title = 'Cummulative activity durations'
     x_label = 'seconds'
     freq = 'seconds'
 
     if df_dur is None:
         df_acts = add_other_activity(df_acts.copy())
-        df = activity_duration(df_acts, lst_acts=lst_acts, time_unit=freq)
+        df = activity_duration(df_acts, lst_acts=lst_acts, unit=freq)
     else:
         df = df_dur
     df = df.sort_values(by=[freq], axis=0)
 
     # create a new plot with a title and axis labels
     from bokeh.io import output_file, show
     from bokeh.models import ColumnDataSource
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/act_and_devs.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/plot/matplotlib/act_and_devs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pyadlml.dataset._core.activities import add_other_activity
 from pyadlml.dataset.stats import contingency_states as stat_cont_st, contingency_events as stat_cont_ev, cross_correlogram as stat_cc
 from .devices import _plot_device_states
 from .util import func_formatter_seconds2time, save_fig, \
     heatmap_square, heatmap, annotate_heatmap, heatmap_contingency, map_time_to_numeric, \
     get_qualitative_cmap, plot_cc, create_todo, xaxis_format_time, xaxis_format_time2, \
     dev_raster_data_gen,plot_grid
-from pyadlml.dataset.plotly.util import format_device_labels 
+from pyadlml.dataset.plot.plotly.util import format_device_labels 
 from pyadlml.dataset.util import select_timespan, infer_dtypes, str_to_timestamp
 
 from pyadlml.dataset.stats.activities import activity_order_by_duration
 
 DEV_CON_HM = {(8, 12): (8, 7), (8, 14): (8, 8), (8, 3): (12, 10), (26, 20): (10, 10), (11, 17): (10, 10)}
 DEV_CON_01_HM = {(8, 14): (12, 10), (11, 24): (12, 6), (11, 34): (16, 12)}
 DEV_CON_01_HM_WT = {(10, 24): (14, 7), (7, 28): (16, 10)}
@@ -44,16 +44,16 @@
         devices = corr_data[2]
         activities = corr_data[3]
 
     return plot_cc(ccg, bins, title=title, x_label=activities, y_label=devices, axis=axis, figsize=figsize)
 
 
 @save_fig
-def contingency_events(df_devs=None, df_acts=None, df_con_tab=None, idle=False, per_state=False, \
-                       scale=None, numbers=True, figsize=None, file_path=""):
+def contingency_events(df_devs=None, df_acts=None, df_con_tab=None, other=False, per_state=False, \
+                       scale=None, numbers=True, figsize=None, file_path="", n_jobs=1):
     """ Computes a table where the device triggers are counted per activity
 
     Parameters
     ----------
     df_devs : pd.DataFrame, optional
         recorded devices from a dataset. For more information refer to
         :ref:`user guide<device_dataframe>`. If the parameter *df_devs* is not set,
@@ -70,20 +70,22 @@
         If set events are
     figsize : (float, float), optional
         width, height in inches. If not provided, the figsize is inferred by automatically.
     scale : {"log", "linear"}, default: 'log'
         The axis scale type to apply.
     numbers : bool, default: True
         Whether to display numbers inside the heatmaps fields or not.
-    idle : bool, default: False
+    other : bool, default: False
         Determines whether gaps between activities should be assigned
-        the activity *idle* or be ignored.
+        the activity *other* or be ignored.
     file_path : str, optional
         If set, saves the plot under the given file path and return *None* instead
         of returning the figure.
+    n_jobs : int, default=1
+        The number of parallel threads to use for computing the statistics.
 
     Examples
     --------
     >>> from pyadlml.plot import plot_contingency_events
     >>> plot_contingency_events(data.df_activities, data.df_activities)
 
     .. image:: ../_static/images/plots/cont_hm_trigger.png
@@ -114,18 +116,19 @@
     cbarlabel = 'counts'
     textcolors = ("white", "black")
     # if log than let automatically infer else
     log = (scale == 'log')
     valfmt = (None if log else "{x:.0f}")
 
     if df_con_tab is None:
-        ct = stat_cont_ev(df_devs, df_acts, idle=idle, per_state=per_state)
+        ct = stat_cont_ev(df_devs, df_acts, other=other, per_state=per_state, n_jobs=n_jobs)
     else:
         ct = df_con_tab.copy()
 
+    # First column are devices
     vals = ct.iloc[:, 1:].values.T
     acts = ct.columns[1:].values
     devs = ct[DEVICE].values
 
     # format labels
     dtypes = infer_dtypes(df_devs)
     if per_state:
@@ -142,15 +145,15 @@
 
     return fig
 
 
 
 @save_fig
 def plot_contingency_states(df_devs: pd.DataFrame = None, df_acts: pd.DataFrame = None, df_con_tab: pd.DataFrame = None,
-                            figsize: tuple = None, z_scale: str = 'log', idle: bool = False, numbers: bool = True,
+                            figsize: tuple = None, z_scale: str = 'log', other: bool = False, numbers: bool = True,
                             file_path: str = "") -> object:
     """
     Plots a heatmap the device on and off intervals are measured against
     the activities
 
     Parameters
     ----------
@@ -168,17 +171,17 @@
         in :ref:`stats <stats_dna_con_dur>`.
     figsize : (float, float), optional
         width, height in inches. If not provided, the figsize is inferred by automatically.
     z_scale : {"log", "linear"}, default: 'log'
         The axis scale type to apply.
     numbers : bool, default: True
         Whether to display numbers inside the heatmaps fields or not.
-    idle : bool, default: False
+    other : bool, default: False
         Determines whether gaps between activities should be assigned
-        the activity *idle* or be ignored.
+        the activity *other* or be ignored.
     file_path : str, optional
         If set, saves the plot under the given file path and return *None* instead
         of returning the figure.
 
     Examples
     --------
     >>> from pyadlml.dataset import fetch_amsterdam
@@ -203,15 +206,15 @@
 
     assert (df_devs is not None and df_acts is not None) or df_con_tab is not None
 
     title = 'Activity vs. device states'
     cbarlabel = 'time in seconds'
 
     if df_con_tab is None:
-        if idle:
+        if other:
             df_acts = add_other_activity(df_acts.copy())
         df_con = stat_cont_st(df_devs, df_acts)
     else:
         df_con = df_con_tab
 
     # convert time (ns) to seconds
     df_con = df_con.astype(int)/1000000000
@@ -257,15 +260,15 @@
         When set, a string representing the time where the plots ends
     figsize : tuple, default=(20,8)
         The plots figure given in (width, height)
     file_path : str, default=""
         When set the file
 
     Returns
-    ------
+    -------
     fig or None
         Either a figure or nothing depending on if file_path is set.
     """
     title='Activities vs. device events'
     y_label = 'Devices'
     event_color = 'grey'
 
@@ -343,15 +346,15 @@
         When set, a string representing the time where the plots ends
     figsize : tuple, default=(20,8)
         The plots figure given in (width, height)
     file_path : str, default=""
         When set the file
 
     Returns
-    ------
+    -------
     fig or None
         Either a figure or nothing depending on if file_path is set.
     """
 
     ylabel = 'Devices'
     title = 'Device states'
     binary_on_label = 'on'
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/activities.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/plot/matplotlib/activities.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,31 +10,30 @@
 from .util import func_formatter_seconds2time_log, ridgeline, \
     func_formatter_seconds2time, heatmap, annotate_heatmap, heatmap_square, savefig, \
     _num_bars_2_figsize, _num_boxes_2_figsize, \
     _num_items_2_heatmap_square_figsize, _num_items_2_ridge_figsize, \
     _num_items_2_ridge_ylimit, xaxis_format_one_day, save_fig, get_qualitative_cmap, plot_grid, xaxis_format_time2, \
     map_time_to_numeric
 from pyadlml.util import get_sequential_color, get_secondary_color, get_primary_color, get_diverging_color
-from ..util import activity_order_by
-
+from pyadlml.dataset.util import activity_order_by
 
 @save_fig
 def count(df_acts=None, df_ac=None, scale="linear", other=False,
           figsize=None, color=None, file_path=None):
     """
     Plot a bar chart displaying how often activities are occurring.
 
     Parameters
     ----------
     df_acts : pd.DataFrame, optional
         recorded activities from a dataset. Fore more information refer to the
         :ref:`user guide<activity_dataframe>`.
     other : bool, default: False
         Determines whether gaps between activities should be assigned
-        the activity *idle* or be ignored.
+        the activity *other* or be ignored.
     scale : {"log", "linear"}, default: linear
         The axis scale type to apply.
     figsize : (float, float), default: None
         width, height in inches. If not provided, the figsize is inferred by automatically.
     color : str, optional
         sets the color of the plot. When not set, the primary theming color is used.
         Learn more about theming in the :ref:`user guide <theming>`
@@ -43,15 +42,15 @@
         of returning the figure.
 
     Examples
     --------
     >>> from pyadlml.plot import plot_activities_count
     >>> from pyadlml.dataset import fetch_amsterdam
     >>> data = fetch_amsterdam()
-    >>> plot_activities_count(data.df_activities, idle=True)
+    >>> plot_activities_count(data.df_activities, other=True)
 
     .. image:: ../_static/images/plots/act_bar_cnt.png
        :height: 300px
        :width: 500 px
        :scale: 90 %
        :alt: alternate text
        :align: center
@@ -176,32 +175,32 @@
     ax_top.xaxis.set_major_formatter(
         ticker.FuncFormatter(func_formatter_seconds2time))
 
     return fig
 
 
 @save_fig
-def duration(df_acts=None, df_dur=None, scale='linear', idle=False,
+def duration(df_acts=None, df_dur=None, scale='linear', other=False,
              figsize=None, color=None, file_path=None):
     """
     Plots the cumulative duration for each activity in a bar plot.
 
     Parameters
     ----------
     df_acts : pd.DataFrame, optional
         recorded activities from a dataset. Fore more information refer to the
         :ref:`user guide<activity_dataframe>`.
     lst_acts : lst of str, optional
         A list of activities that are included in the statistic. The list can be a
         subset of the recorded activities or contain activities that are not recorded.
     scale : {"log", "linear"}, default: None
         The axis scale type to apply.
-    idle : bool, default: False
+    other : bool, default: False
         Determines whether gaps between activities should be assigned
-        the activity *idle* or be ignored.
+        the activity *other* or be ignored.
     figsize : (float, float), default: None
         width, height in inches. If not provided, the figsize is inferred by automatically.
     color : str, optional
         sets the color of the plot. When not set, the primary theming color is used.
         Learn more about theming in the :ref:`user guide <theming>`
     file_path : str, optional
         If set, saves the plot under the given file path and return *None* instead
@@ -229,17 +228,17 @@
 
     title = 'Cummulative activity durations'
     xlabel = 'seconds'
     freq = 'seconds'
     color = (get_primary_color() if color is None else color)
 
     if df_dur is None:
-        if idle:
+        if other:
             df_acts = add_other_activity(df_acts.copy())
-        df = activity_duration(df_acts, time_unit=freq)
+        df = activity_duration(df_acts, unit=freq)
     else:
         df = df_dur
     df = df.sort_values(by=[freq], axis=0)
 
     num_act = len(df)
     figsize = (_num_bars_2_figsize(num_act) if figsize is None else figsize)
     
@@ -259,15 +258,15 @@
         ticker.FuncFormatter(func_formatter_seconds2time))
 
     return fig
 
 
 @save_fig
 def transitions(df_acts=None, df_trans=None, scale="linear",
-                figsize=None, idle=False, numbers=True, grid=True,
+                figsize=None, other=False, numbers=True, grid=True,
                 cmap=None, file_path=None):
     """
     Parameters
     ----------
     df_acts : pd.DataFrame, optional
         recorded activities from a dataset. Fore more information refer to the
         :ref:`user guide<activity_dataframe>`.
@@ -277,17 +276,17 @@
         in :ref:`stats <stats_acts_trans>`.
     figsize : (float, float), default: None
         width, height in inches. If not provided, the figsize is inferred by automatically.
     scale : {"log", "linear"}, default: None
         The axis scale type to apply.
     numbers : bool, default: True
         Whether to display numbers inside the heatmaps fields or not.
-    idle : bool, default: False
+    other : bool, default: False
         Determines whether gaps between activities should be assigned
-        the activity *idle* or be ignored.
+        the activity *other* or be ignored.
     cmap : str or Colormap, optional
         The Colormap instance or registered colormap name used to map scalar
         data to colors. This parameter is ignored for RGB(A) data.
         Defaults 'viridis'.
     grid : bool, default: True
         determines whether to display a white grid, seperating the fields or not.
     file_path : str, optional
@@ -315,15 +314,15 @@
     assert scale in ['linear', 'log'], 'scale has to be either of type None or log'
     assert not (df_acts is None and df_trans is None)
 
     title = 'Activity transitions'
     z_label = 'count'
 
     if df_trans is None:
-        df_acts = add_other_activity(df_acts) if idle else df_acts
+        df_acts = add_other_activity(df_acts) if other else df_acts
         df = activities_transitions(df_acts)
     else:
         df = df_trans
 
     # get the list of cross tabulations per t_window
     act_lst = list(df.columns)
 
@@ -346,15 +345,15 @@
         texts = annotate_heatmap(im, textcolors=("white", "black"),log=log, valfmt=valfmt)
     ax.set_title(title)
     
     return fig
 
 
 @save_fig
-def density(df_acts=None, df_act_dist=None, idle=False, dt=None,
+def density(df_acts=None, df_act_dist=None, other=False, dt=None,
             n=1000, ylim_upper=None, color=None, figsize=None, file_path=None):
     """
     Plots the activity density distribution over one day.
 
     Parameters
     ----------
     df_acts : pd.DataFrame, optional
@@ -373,17 +372,17 @@
         The offset from the top of the plot to the first ridge_line. Set this if
         the automatically determined value is not satisfying.
     figsize : (float, float), default: None
         width, height in inches. If not provided, the figsize is inferred by automatically.
     color : str, optional
         sets the color of the plot. When not set, the primary theming color is used.
         Learn more about theming in the :ref:`user guide <theming>`
-    idle : bool, default: False
+    other : bool, default: False
         Determines whether gaps between activities should be assigned
-        the activity *idle* or be ignored.
+        the activity *other* or be ignored.
     file_path : str, optional
         If set, saves the plot under the given file path and return *None* instead
         of returning the figure.
 
     Examples
     --------
     >>> from pyadlml.plot import plot_activity_density
@@ -405,15 +404,15 @@
 
     title = 'Activity density over one day'
     xlabel = 'Time'
     color = (get_primary_color() if color is None else color)
 
 
     if df_act_dist is None:
-        if idle:
+        if other:
             df_acts = add_other_activity(df_acts)
         df = activities_dist(df_acts.copy(), n=n, dt=dt, relative=True)
         if df.empty:
             raise ValueError("no activity was recorded and no activity list was given.")
     else:
         df = df_act_dist
 
@@ -470,34 +469,22 @@
 
 
     Parameters
     ----------
     df_acts : pd.DataFrame, optional
         recorded activities from a dataset. Fore more information refer to the
         :ref:`user guide<activity_dataframe>`.
-    lst_acts : lst of str, optional
-        A list of activities that are included in the statistic. The list can be a
-        subset of the recorded activities or contain activities that are not recorded.
     df_act_dist : pd.DataFrame, optional
         A precomputed activity density distribution. If the *df_trans* parameter is given, parameters
         *df_acts* and *lst_acts* are ignored. The transition table can be computed
         in :ref:`stats <stats_acts_trans>`.
-    n : int, default=1000
-        The number of monte-carlo samples to draw.
-    ylim_upper: float, optional
-        The offset from the top of the plot to the first ridge_line. Set this if
-        the automatically determined value is not satisfying.
-    figsize : (float, float), default: None
-        width, height in inches. If not provided, the figsize is inferred by automatically.
+
     color : str, optional
         sets the color of the plot. When not set, the primary theming color is used.
         Learn more about theming in the :ref:`user guide <theming>`
-    idle : bool, default: False
-        Determines whether gaps between activities should be assigned
-        the activity *idle* or be ignored.
     file_path : str, optional
         If set, saves the plot under the given file path and return *None* instead
         of returning the figure.
 
     Examples
     --------
     >>> from pyadlml.dataset import fetch_amsterdam
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/devices.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/plot/matplotlib/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import numpy as np
 from datetime import timedelta
 import pandas as pd
 import matplotlib.pyplot as plt
 import matplotlib.colors as colors
 
-from pyadlml.stats import device_state_fractions
+from pyadlml.stats import device_state_fraction
 from pyadlml.constants import DEVICE, TIME, VALUE, BOOL, CAT, START_TIME, END_TIME, NUM
 from pyadlml.dataset.stats.devices import state_cross_correlation as stat_scc, \
     inter_event_intervals as stat_iei, event_cross_correlogram as stat_event_cc, events_one_day, \
     event_count as stats_event_count, event_cross_correlogram2
 
 from .util import heatmap_square, func_formatter_seconds2time, \
     heatmap, annotate_heatmap, savefig, _num_bars_2_figsize, save_fig, \
     _num_items_2_heatmap_square_figsize, _num_boxes_2_figsize, \
     _num_items_2_heatmap_one_day_figsize, _num_items_2_heatmap_square_figsize_ver2, LOG, xaxis_format_one_day, \
     sort_devices, add_top_axis_time_format, map_time_to_numeric, plot_cc, create_todo, xaxis_format_time, \
     dev_raster_data_gen, xaxis_format_time2, get_qualitative_cmap, plot_grid
 
-from pyadlml.dataset.plotly.util import format_device_labels
+from pyadlml.dataset.plot.plotly.util import format_device_labels
 from pyadlml.dataset._core.devices import _is_dev_rep2, device_events_to_states, split_devices_binary, contains_non_binary
 from pyadlml.dataset.stats.util import comp_tds_sums, comp_tds_sums_mean, comp_tds_sums_median
 from pyadlml.dataset.util import select_timespan, infer_dtypes, str_to_timestamp, device_order_by
 from pyadlml.util import get_sequential_color, get_secondary_color, get_primary_color, get_diverging_color
 
 
 @save_fig
@@ -68,20 +68,20 @@
     -------
     res : fig or None
         Either a figure if file_path is not specified or nothing.
 
 
     """
     assert not (df_devices is None and inter_event_intervals is None)
-    title='Devices Inter-event-intervals'
+    title='Device Inter-event-times'
     log_sec_col = 'total_log_secs'
     sec_col = 'total_secs'
     ylabel='count'
     xlabel_top = 'time'
-    ax1label = '$\Delta t$ count'
+    ax1label = '$\Delta t$'
     ax3label = 'imputed events'
     xlabel = 'log seconds' if scale == 'log' else 'seconds'
     color = (get_primary_color() if color is None else color)
     color2 = get_secondary_color()
 
     if inter_event_intervals is None:
         X = stat_iei(df_devices.copy())
@@ -536,24 +536,24 @@
 
     from pyadlml.dataset.util import infer_dtypes
     dtypes = infer_dtypes(df_devs)
 
 
     # Figure Size 
     fig, ax = plt.subplots(figsize=figsize)
-    plt.title(title)
-    plt.xlabel(xlabel)
-    plt.ylabel(ylabel)
+    ax.set_title(title)
+    ax.set_xlabel(xlabel)
+    ax.set_ylabel(ylabel)
 
     # plot boolean devices
     df_bool = df[df[DEVICE].isin(dtypes[BOOL])].copy().sort_values(by=DEVICE)
     off_values = df_bool.loc[(df_bool[VALUE] == False), 'frac'].values
-    plt.barh(dtypes[BOOL], off_values, label=off_label, color=color)
+    ax.barh(dtypes[BOOL], off_values, label=off_label, color=color)
     # careful: notice "bottom" parameter became "left"
-    plt.barh(dtypes[BOOL], (1-off_values), left=off_values, label=on_label, color=color2)
+    ax.barh(dtypes[BOOL], (1-off_values), left=off_values, label=on_label, color=color2)
 
     # set the text centers for the boolean devices to the middle for the greater fraction
     first_number_left = True
     for i, dev in enumerate(dtypes[BOOL]):
         text_in_off = (off_values[i] >= 0.5)
         center = off_values[i]/2 if text_in_off else (1 - off_values[i])/2 + off_values[i]
         text = off_values[i] if text_in_off else (1 - off_values[i])
@@ -569,15 +569,15 @@
         cum_sum = 0
         cat_centers.append([])
         for i, cat in enumerate(categories):
             value = df.loc[(df[DEVICE] == dev) & (df[VALUE] == cat), 'frac'].values[0]
             # save the center in bar plot as well as the value for setting
             # the annotations later
             cat_centers[j].append((cum_sum + value/2, value))
-            plt.barh([dev], [value], label=dev + ' : ' + cat, left=[cum_sum])
+            ax.barh([dev], [value], label=dev + ' : ' + cat, left=[cum_sum])
             cum_sum += value
 
 
     # set the text centers for categorical devices into the middle for each category
     for c, y in zip(range(len(dtypes[CAT])), range(len(dtypes[BOOL]), num_dev-1)):
         for center, text in cat_centers[c]:
             ax.text(center, y, '{:.4f}'.format(text), ha='center', va='center', color='white')
@@ -756,15 +756,15 @@
     plt.xlabel(x_label)
     plt.ylabel(y_label)
     return fig
 
 
 @save_fig
 def event_cross_correlogram(df_devices=None, corr_data=(None, None, None), bin_size='1s', max_lag='2m', axis='off',
-                            figsize=(5, 5), file_path=None):
+                            figsize=(5, 5), file_path=None, use_dask=False):
     #Plot cross-correlograms of all pairs.
     #   plotCCG(ccg,bins) plots a matrix of cross(auto)-correlograms for
     #   all pairs of clusters. Inputs are:
     #       ccg     array of cross correlograms           #bins x #clusters x #clusters
     #       bins    array with bin timings                #nbins x 0
 
     title = 'Event cross-correlogram'
@@ -773,15 +773,15 @@
         ccg, bins = event_cross_correlogram2(df_devices, binsize=bin_size, maxlag=max_lag)
         devices = df_devices[DEVICE].unique()
     else:
         ccg = corr_data[0]
         bins = corr_data[1]
         devices = corr_data[2]
 
-    fig = plot_cc(ccg, bins, title=title, y_label=devices, axis=axis, figsize=figsize)
+    fig = plot_cc(ccg, bins, title=title, y_label=devices, axis=axis, figsize=figsize, use_dask=use_dask)
 
     return fig
 
 
 @save_fig
 def states(df_devices, start_time=None,end_time=None, figsize=(20, 8),
            order='alphabetical', grid=False, file_path=""):
@@ -847,15 +847,15 @@
         The number of colors used up for different devices.
     """
     col_bar_start = 'num_st'
     col_bar_len = 'diff'
 
     # do preprocessing
     dtypes = infer_dtypes(df_devs)
-    df_devs = device_events_to_states(df_devs, extrapolate_states=True, st=start_time, et=end_time)
+    df_devs = device_events_to_states(df_devs, extrapolate_states=True, start_time=start_time, end_time=end_time)
 
     df_devs['num_st'], _, _ = map_time_to_numeric(df_devs[START_TIME], start_time, end_time)
     df_devs['num_et'], _, _ = map_time_to_numeric(df_devs[END_TIME], start_time, end_time)
     df_devs['diff'] = df_devs['num_et'] - df_devs['num_st']
 
 
     j = 0
@@ -882,12 +882,12 @@
                 ax.broken_barh(values, (i-0.25, 0.5), facecolors=tab(j), label=dev + ' - ' + cat)
                 j += 1
 
         elif dev in dtypes[NUM]:
             values = pd.to_numeric(df[VALUE])
             values = (values-values.min())/(values.max() - values.min())*0.5
             values = values + i - 0.25
-            ax.plot(df['num_st'], values, color=color_num, linestyle='--', marker='o')
+            ax.plot(df['num_st'], values, color=color_num, linestyle='--', marker='o', markersize=1)
 
     if return_nr_categories_used:
         return j
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/discrete.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/plot/matplotlib/discrete.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,161 @@
-from pyadlml.dataset.stats.discrete import contingency_table_01, cross_correlation
-from pyadlml.dataset.plot.util import heatmap_contingency as hm_cont
-from pyadlml.dataset.plot.util import annotate_heatmap, heatmap, heatmap_square, \
+import functools
+from pyadlml.dataset.stats.discrete import contingency_table_01 as cn01, cross_correlation as cc
+from pyadlml.dataset.plot.matplotlib.util import heatmap_contingency as hm_cont, save_fig
+from pyadlml.dataset.plot.matplotlib.util import annotate_heatmap, heatmap, heatmap_square, \
     _num_bars_2_figsize, func_formatter_log_1
-from pyadlml.util import get_primary_color, get_diverging_color
+from pyadlml.dataset.util import extract_kwargs
+from pyadlml.util import get_primary_color, get_diverging_color, get_secondary_color
 import matplotlib.pyplot as plt
-import matplotlib
 import pandas as pd 
 import numpy as np
 
-def heatmap_contingency(X, y, rep='', z_scale=None, figsize=None, numbers=True):
+
+
+def ensure_yis_series(func):
+    @extract_kwargs
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        y = kwargs.pop('y')
+        if isinstance(y, pd.DataFrame) and len(y.columns) == 1:
+            y = y.iloc[:,0]
+        kwargs['y'] = y
+        return func(*args, **kwargs)
+    return wrapper
+
+
+@save_fig
+@ensure_yis_series
+def contingency_table(X, y, rep='', z_scale=None, figsize=None, numbers=True, file_path=None):
     """ plots the contingency between features and labels of data
     Parameters
     ----------
     X: pd.DataFrame
         one of the representation raw, lastfired, changepoint
     y: pd.DataFrame
         a series of labels
     rep: string
         the name of the representation to add to the title
     """
     title = rep + " On/Off contingency"
     cbarlabel = 'counts'
     valfmt = ("{x:.0f}" if z_scale!='log' else func_formatter_log_1)
 
-    df_con = contingency_table_01(X, y)
+    df_con = cn01(X, y)
     vals = df_con.values.T
     acts = df_con.columns.values
     devs = list(df_con.index)
     
     # format labels by replacing every 'on'
     for i, dev in enumerate(devs):
         if 'On' in dev:
             devs[i] = 'On'
-    return hm_cont(acts, devs, vals, title, cbarlabel, z_scale=z_scale, figsize=figsize, valfmt=valfmt, numbers=numbers)
+    fig =  hm_cont(acts, devs, vals, title, cbarlabel, z_scale=z_scale, figsize=figsize, valfmt=valfmt, numbers=numbers)
+    plt.tight_layout()
+    return fig
+
+@save_fig
+def device_fraction(X, figsize=(9,4), color=None, file_path=None):
+
+    title = 'Fraction'
+    x_label = 'count'
+
+    color = (get_primary_color() if color is None else color)
+    color2 = get_secondary_color()
+
+
+    df = X.apply(lambda x: x.value_counts())
+    off_values = df.loc[0,:]
+    on_values = df.loc[1,:]
+
+
+    fig, ax = plt.subplots(figsize=figsize)
+    ax.set_title(title)
+    ax.set_xlabel(x_label)
+
+
+    # Plot 0os 
+    ax.barh(df.columns, off_values, label='0', color=color)
+    ax.barh(df.columns, on_values, left=off_values, label='1', color=color2)
+
+    return fig
+
+@save_fig
+@ensure_yis_series
+def activity_count(y, scale="linear", color=None, figsize=(9,3), file_path=None):
+    """ Plot activity count
 
-def hist_activities(y, scale=None, color=None, figsize=(9,3)):
-    """
     Parameters
     ----------
-    y: np array
+    y: np array or pd.Series
         label of strings
     scale: None or log
+
     """
-    title = 'Label occurence'
+    assert scale in ['linear', 'log']
+
+    title = 'Label frequency'
     xlabel = 'counts'
     color = (get_primary_color() if color is None else color)
 
     ser = pd.Series(data=y).value_counts()
     ser = ser.sort_values(ascending=True)
 
     figsize = (_num_bars_2_figsize(len(ser)) if figsize is None else figsize)
     fig, ax = plt.subplots(1, 1, figsize=figsize)
 
     if scale == 'log': 
         plt.xscale('log')
 
     ax.barh(ser.index, ser.values, orientation='horizontal', color=color)
-    plt.xlabel(xlabel)
+    ax.set_xlabel(xlabel)
     fig.suptitle(title)
 
+    plt.tight_layout()
+    return fig
+
+
+@save_fig
+def mutual_info(X, y, scale="linear", color=None, figsize=(9,3), file_path=None):
+    """ Plot activity count
+
+    Parameters
+    ----------
+    X: array-like, (n_samples, n_features)
+        asdf
+    y: np array or pd.Series
+        label of strings
+    X
+    scale: None or log
+
+    """
+    assert scale in ['linear', 'log']
+
+    title = 'Mutual Information: I(X,y) = H(y)-H(y|X)'
+    xlabel = 'I(X,y)'
+    color = (get_primary_color() if color is None else color)
+
+    from sklearn.feature_selection import mutual_info_classif
+    mi = mutual_info_classif(X, y, discrete_features=True)
+
+
+    figsize = (_num_bars_2_figsize(len(X.columns)) if figsize is None else figsize)
+    fig, ax = plt.subplots(1, 1, figsize=figsize)
+
+    if scale == 'log': 
+        plt.xscale('log')
+
+    ax.barh(X.columns, mi, orientation='horizontal', color=color)
+    ax.set_xlabel(xlabel)
+    fig.suptitle(title)
+
+    plt.tight_layout()
+    return fig
+
+
 
 def corr_devices_01(rep, figsize=(19,14)):
     """ correlation between the on and off states of every device.
     Parameters
     ----------
     rep: pd.DataFrame
         A dataframe where columns are devices and rows are a binary representation
@@ -110,22 +203,24 @@
     texts = annotate_heatmap(im, textcolors=("black", "white"), valfmt="{x:.2f}")
     
     ax1.set_title("Correlation of on-on signals")
     ax2.set_title("Correlation of on-off signals")
     fig.tight_layout()
     plt.show()
 
+
+
 def heatmap_cross_correlation(df_dev, figsize=(10,8)):
 
 
     title = 'Devices cross-correlation'
     cmap = get_diverging_color()
     cbarlabel = 'similarity'
 
-    ct = cross_correlation(df_dev)
+    ct = cc(df_dev)
     vals = ct.values.T.astype(np.float64)
     devs = list(ct.index)
     
     fig, ax = plt.subplots(figsize=figsize)
     im, cbar = heatmap_square(vals, devs, devs, ax=ax, cmap=cmap, cbarlabel=cbarlabel,
                        vmin=-1, vmax=1)
     annotate_heatmap(im, textcolors=("black", "white"), valfmt="{x:.2f}", threshold=0.6)
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/image.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/plot/matplotlib/image.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/matplotlib/util.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/plot/matplotlib/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1027,28 +1027,50 @@
 def add_top_axis_time_format(axis, top_label=None):
     ax_top = axis.secondary_xaxis('top', functions=(lambda x: x, lambda x: x))
     ax_top.xaxis.set_major_formatter(
         ticker.FuncFormatter(func_formatter_seconds2time))
     if top_label is not None:
         ax_top.set_xlabel(top_label)
 
+def add_axis_time_format(axis, position='top', scale='linear', label=None):
+    assert position in ['top', 'bottom', 'right', 'left']
+
+    func_formatter = func_formatter_seconds2time if scale == 'linear' else func_formatter_seconds2time_log
+    if position in ['top', 'bottom']:
+        ax_sec = axis.secondary_xaxis(position, functions=(lambda x: x, lambda x: x))
+        ax_sec.xaxis.set_major_formatter(
+            ticker.FuncFormatter(func_formatter))
+        if label is not None:
+                    ax_sec.set_xlabel(label)
+
+
+    else:
+        ax_sec = axis.secondary_yaxis(position, functions=(lambda x: x, lambda x: x))
+        ax_sec.yaxis.set_major_formatter(
+            ticker.FuncFormatter(func_formatter))
+
+        if label is not None:
+            ax_sec.set_ylabel(label)
+
+
+
 
 def plot_hist(ax, bins, counts, color='k'):
     """ plot a histogram given bins and counts for the bins
     from https://gist.github.com/hitvoice/47c63728754713d0e56eb8366bfafe56
     """
     assert len(bins) == len(counts) + 1
     centroids = (bins[1:] + bins[:-1]) / 2  # values in the middle between each bin
 
     # plot for every centroid one occurrence  that is multiplied with the weight -> real height
     counts_, bins_, _ = ax.hist(centroids, bins=len(counts), weights=counts, range=(min(bins), max(bins)), color=color)
     assert np.allclose(bins_, bins)
     assert np.allclose(counts_, counts)
 
-def plot_cc(ccg, bins, title, y_label=None, x_label=None, axis='off', figsize=None):
+def plot_cc(ccg, bins, title, y_label=None, x_label=None, axis='off', figsize=None, use_dask=False):
     """
     Plots a cross correlogram of histograms
     """
 
     I = ccg.shape[0]    # nr devices
     J = ccg.shape[1]
 
@@ -1087,20 +1109,57 @@
         elif bins[-1] < 3600:
             ax.set_xticks([bins[0], 0, bins[-1]])
             bound = '{:.1f}'.format(bins[-1]/60) + 'm'
             ax.set_xticks([bins[0], -60, 60, bins[-1]])
             ax.set_xticklabels(['-' + bound, '-1m', '1m', bound], rotation='vertical')
 
 
+    if not use_dask:
+        for ix in range(I):
+            for jx in range(J):
+                ax = plt.subplot(gs[J*ix+jx], facecolor=bg)
+                #ax = plt.subplot(K,K,K*ix+jx+1, facecolor=bg)
+
+                counts = ccg[ix, jx, :]
+                # remove middle count because it is weird for a histogram to have.. TODO check in correlogram method
+                counts = np.concatenate([counts[:int(len(counts)/2)],
+                                    counts[int(len(counts)/2)+1:]])
+                if ix == jx:
+                    plot_hist(ax, bins, counts, color=colors[ix, :])
+                else:
+                    plot_hist(ax, bins, counts, color='k')
+
+                ax.set_xlim(1.2 * bins[[0, -1]])
+                ylim = np.array(list(ax.get_ylim()))
+                ax.set_ylim(np.array([0, 1.2]) * ylim)
+                ax.set_yticks([])
 
-    for ix in range(I):
-        for jx in range(J):
-            ax = plt.subplot(gs[J*ix+jx], facecolor=bg)
-            #ax = plt.subplot(K,K,K*ix+jx+1, facecolor=bg)
-
+                if ix == 0 and x_label is not None:
+                    sec_ax = ax.secondary_xaxis('top')
+                    sec_ax.set_xticks([])
+                    sec_ax.set_xlabel(x_label[jx], rotation=45)
+
+                if ix != I-1 and ix != 0:
+                    ax.set_xticks([])
+
+                if ix == I-1:
+                    set_x_ticks(ax, I)
+
+                if jx == 0:
+                    ax.set_yticks([])
+                    if y_label is not None:
+                        ax.set_ylabel(y_label[ix], rotation='horizontal', ha='right')
+
+                if ix != jx:
+                    ax.plot(0, 0, '*', c=colors[jx, :])
+        #plt.tight_layout()
+        fig.show()
+        return fig
+    else:
+        def func(ax, ix, jx):
             counts = ccg[ix, jx, :]
             # remove middle count because it is weird for a histogram to have.. TODO check in correlogram method
             counts = np.concatenate([counts[:int(len(counts)/2)],
                                 counts[int(len(counts)/2)+1:]])
             if ix == jx:
                 plot_hist(ax, bins, counts, color=colors[ix, :])
             else:
@@ -1125,18 +1184,25 @@
             if jx == 0:
                 ax.set_yticks([])
                 if y_label is not None:
                     ax.set_ylabel(y_label[ix], rotation='horizontal', ha='right')
 
             if ix != jx:
                 ax.plot(0, 0, '*', c=colors[jx, :])
-    #plt.tight_layout()
-    fig.show()
-    return fig
+        import dask
 
+        res = []
+        for ix in range(I):
+            for jx in range(J):
+                ax = plt.subplot(gs[J*ix+jx], facecolor=bg)
+                #ax = plt.subplot(K,K,K*ix+jx+1, facecolor=bg)
+                res.append(dask.delayed(func)(ax, ix, jx))
+        res = dask.compute(*res)
+        fig.show()
+        return fig
 
 def save_fig(func):
     """ Decorator that saves a figure to a filepath rather then returning it
         if the keyword file_path is given.
     """
     @functools.wraps(func)
     def wrapper_save_fig(*args, **kwargs):
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/acts_and_devs.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/plot/plotly/acts_and_devs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import math
 from collections import OrderedDict
 import plotly.express as px
-from .util import ActivityDict, _style_colorbar, _dyn_y_label_size
+from pyadlml.dataset.stats.activities import _get_freq_func
+
+from pyadlml.dataset.stats.devices import event_cross_correlogram3
+from .util import dyn_event_marker_size, legend_current_items, _style_colorbar, dyn_y_label_size, remove_whitespace_around_fig
 import plotly
 import pandas as pd
 import numpy as np
 
 from plotly.subplots import make_subplots
 import plotly.graph_objects as go
 from plotly.express import IdentityMap
@@ -13,20 +16,21 @@
     get_label, make_trace_kwargs, get_decorated_label, init_figure, make_trendline_spec, configure_axes, \
     configure_animation_controls, process_dataframe_timeline, one_group, \
     get_groups_and_orders
 
 #from plotly.subplots import _subplot_type_for_trace_type, _set_trace_grid_reference
 from plotly.validators.choropleth import ColorscaleValidator
 from pyadlml.constants import DEVICE, TIME, ACTIVITY, START_TIME, END_TIME, VALUE, NUM, BOOL, \
-    CAT, STRFTIME_DATE
+    CAT, STRFTIME_PRECISE
 import plotly.express as px
 
 from pyadlml.dataset._core.devices import device_events_to_states
-from pyadlml.dataset.plotly.util import format_device_labels
-from pyadlml.dataset.plotly.activities import _set_compact_title
+from pyadlml.dataset._core.activities import ActivityDict, create_empty_activity_df
+from pyadlml.dataset.plot.plotly.util import format_device_labels
+from pyadlml.dataset.plot.plotly.activities import _set_compact_title
 from pyadlml.dataset.stats.acts_and_devs import contingency_table_states, contingency_table_events
 from pyadlml.dataset.util import select_timespan, df_difference, activity_order_by, device_order_by, infer_dtypes
 
 
 __all__ = ['activities_and_devices', 'contingency_states', 'contingency_events']
 
 def _dynamic_and_height(nr_subj, nr_devs):
@@ -37,15 +41,16 @@
     height = int(m*possible_rows + b)
     print(f'height: {height} = {m}*{possible_rows} + {b}')
     return min(height, 1000)
 
 
 
 def _plot_device_states_into_fig(fig: go.Figure, df_devs: pd.DataFrame,  df_devs_usel: pd.DataFrame,
-                                 df_devs_outside: pd.DataFrame, dev_order: list, st=None, et=None) -> go.Figure:
+                                 df_devs_outside: pd.DataFrame, dev_order: list, st=None, et=None,
+                                 row=1, col=1) -> go.Figure:
     """
     Parameters
     ----------
     df_devs_outside : list of dicts
         Each dictionary contains the key 'df' and a 'color' and a 'opacity'
 
 
@@ -58,72 +63,42 @@
     #marker = dict(size=5, symbol=42, line=dict(color=EVENT_COLOR, width=1))
 
     df_devs = df_devs.copy()\
                         .sort_values(by=TIME)\
                         .reset_index(drop=True)
     devs = df_devs[DEVICE].unique()
     dtypes = infer_dtypes(df_devs)
-    df_devs = device_events_to_states(df_devs, extrapolate_states=True,
-                                      st=st, et=et).reset_index(drop=True)
+    df_devs = device_events_to_states(df_devs, start_time=st, end_time=et,
+                                      extrapolate_states=True).reset_index(drop=True)
 
     if df_devs_usel is not None:
         mark_selected = {}
         df_devs_usel = df_devs_usel.rename(columns={TIME: START_TIME})
         if END_TIME not in df_devs_usel.columns:
             tmp = df_devs.copy()
             comp_df = tmp[[START_TIME, DEVICE, VALUE]]\
                       .merge(df_devs_usel, indicator=True, how='left')
             mask = (comp_df['_merge'] == 'both')
             tmp2 = tmp[mask]
             df_devs_usel = tmp2
         df_devs_usel = _endtime_to_offset(df_devs_usel, replace=False)
 
         mask_bool = df_devs_usel[DEVICE].isin(dtypes[BOOL])
-        df_devs_usel[mask_bool, VALUE] = df_devs_usel.loc[mask_bool, VALUE].map({True: ON, False: OFF})
+        df_devs_usel.loc[mask_bool, VALUE] = df_devs_usel.loc[mask_bool, VALUE].map({True: ON, False: OFF})
 
     # Create offset and color
     df_devs = _endtime_to_offset(df_devs, replace=False)
     mask_bool = df_devs[DEVICE].isin(dtypes[BOOL])
     df_devs.loc[mask_bool, VALUE] = df_devs.loc[mask_bool, VALUE].map({True: ON, False: OFF})
 
     # A mapping from device to data index
     #data_dict = {}
     j = 0
-    #first_bool = True
     set_legendgroup_title = 'States'
 
-    #def create_trace_boolean(df, state):
-    #    nonlocal set_legendgroup_title
-
-    #    df['diff'] = (df[END_TIME] - df[START_TIME]).astype(str)
-    #    cd = df[['diff', END_TIME]].values
-    #    # Add state information to custom_data
-    #    vals = np.expand_dims(np.full(cd.shape[0], state), axis=1)
-    #    cd = np.hstack([cd, vals])
-    #    marker_color = COL_ON if state == ON else COL_OFF
-
-    #    trace = go.Bar(name=state,
-    #                    base=df[START_TIME],
-    #                    meta=dev,
-    #                    x=df['offset'],
-    #                    y=df[DEVICE],
-    #                    legendgrouptitle_text=set_legendgroup_title,
-    #                    marker_color=marker_color,
-    #                    customdata=cd,
-    #                    legendgroup=state,
-    #                    orientation='h',
-    #                    width=0.3,
-    #                    textposition='auto',
-    #                    showlegend=first_bool,
-    #                    hovertemplate=hover_template,
-    #    )
-    #    # The very first time create the states for the categorical legend group titles
-    #    set_legendgroup_title = None 
-    #    return trace
-
     def create_traces_categorical(df):
         """ df [TIME, DEVICE, VALUE] of only one device
         """
         nonlocal set_legendgroup_title
         nonlocal cat_idx
         nonlocal hover_template
 
@@ -135,26 +110,30 @@
         df['diff'] = (df[END_TIME] - df[START_TIME]).astype(str)
 
 
 
         categories = df[VALUE].unique()
         trace_lst = []
         for cat in categories:
-
-            if cat not in _legend_current_items(fig):
+            
+            # TODO refactor, when categories of devices and activities overlap 
+            # commented line below does not work
+            #if cat not in legend_current_items(fig):
+            if cat not in cat_col_map.keys():
                 showlegend = True
                 if cat not in cat_col_map.keys():
                     cat_col_map[cat] = cat_colors[cat_idx]
                     cat_idx +=1
             else:
                 showlegend = False
+
             marker_color = cat_col_map[cat]
             mask_cat = (df[VALUE] == cat)
 
-            cd = df.loc[mask_cat, ['diff', END_TIME]].values
+            cd = df.loc[mask_cat, [DEVICE, 'diff', END_TIME]].values
             vals = np.expand_dims(np.full(cd.shape[0], cat), axis=1)
             cd = np.hstack([cd, vals])
 
             trace = go.Bar(name=cat,
                            meta=dev,
                            base=df.loc[mask_cat, START_TIME],
                            x=df.loc[mask_cat, 'offset'],
@@ -175,19 +154,19 @@
         return trace_lst
 
 
     cat_colors = px.colors.qualitative.Pastel1 \
                + px.colors.qualitative.Pastel2
     cat_col_map = {ON:COL_ON, OFF:COL_OFF}
     cat_idx = 0
-    hover_template = '%{y}<br>' + \
-                        'Start_time: %{base|' + STRFTIME_DATE + '}<br>' + \
-                        'End_time: %{customdata[1]|' + STRFTIME_DATE + '}<br>' + \
-                        'Duration: %{customdata[0]}<br>' + \
-                        'State: %{customdata[2]}<extra></extra>'
+    hover_template = '%{customdata[0]}<br>' + \
+                        'Start_time: %{base|' + STRFTIME_PRECISE + '}<br>' + \
+                        'End_time: %{customdata[2]|' + STRFTIME_PRECISE + '}<br>' + \
+                        'Duration: %{customdata[1]}<br>' + \
+                        'State: %{customdata[3]}<extra></extra>'
 
     for i, dev in enumerate(devs):
         df = df_devs[df_devs[DEVICE] == dev].copy()
 
         if dev in dtypes[BOOL]:
             df_on = df[df[VALUE] == ON]
             df_off = df[df[VALUE] == OFF]
@@ -199,87 +178,97 @@
                 comp_df2 = df_off.copy().merge(df_devs_usel, indicator=True, how='left')
                 tmp2 = np.where((comp_df2['_merge'] == 'both').values)[0]
                 mark_selected[dev][ON] = tmp
                 mark_selected[dev][OFF] = tmp2
 
             traces = create_traces_categorical(df)
             fig.add_traces(traces)
-            #trace_on = create_trace_boolean(df_on, ON)
-            #trace_off = create_trace_boolean(df_off, OFF)
-            #data_dict[dev] = [len(fig.data), len(fig.data)+1]
-            #fig.add_traces([trace_on, trace_off])
 
-            #first_bool = False
         elif dev in dtypes[CAT]:
             traces = create_traces_categorical(df)
             fig.add_traces(traces)
             j += 1
 
         elif dev in dtypes[NUM]:
             values = pd.to_numeric(df[VALUE])
             # [min, max] scaling -> [0, 1]
-            values_norm = (values-values.min())/(values.max()-values.min())
+            values_norm = (values-values.min())/(values.max()-values.min())*0.5
             #values_norm = values_norm + i - 0.25
-            print(values_norm)
+            cd = np.stack([values, df[START_TIME].apply(str)], dtype=object).T
             trace = go.Scatter(
                 name=dev,
                 meta=dev,
                 mode='lines',
                 x=df[START_TIME],
                 y=values_norm,
+                customdata=cd,
+                hovertemplate=f'{dev}' + '<br>time:%{customdata[1]}<br>value:%{customdata[0]}<extra></extra>'
             )
+
             trace._subplot_row = 1
             trace._subplot_col = 1
-            
 
-            fig = make_subplots(
-                #rows=1,
-                #cols=1,
-                row_heights=[1.0],
-                horizontal_spacing=0.02,
-                vertical_spacing=0.03,
-                shared_xaxes='all',
-                shared_yaxes='all',
-                column_widths=[1.0],
-                specs=[[{"type":"xy", "secondary_y": True}]], 
-                figure=fig,
-            )
+            # Enable to secondary y axis if necessary
+            from _plotly_utils.exceptions import PlotlyKeyError
+            try:
+                fig.layout['yaxis2']
+            except PlotlyKeyError:
+                fig = make_subplots(figure=fig, 
+                                    specs=[[{"secondary_y": True}]]
+                ) 
+                # TODO critical, +1 for activity 
+                fig.update_yaxes(range=[0, len(devs) + 1], secondary_y=True) 
+            #fig = make_subplots(
+            #    #rows=1,
+            #    #cols=1,
+            #    row_heights=[1.0],
+            #    horizontal_spacing=0.02,
+            #    vertical_spacing=0.03,
+            #    shared_xaxes='all',
+            #    shared_yaxes='all',
+            #    column_widths=[1.0],
+            #    specs=[[{"type":"xy", "secondary_y": True}]], 
+            #    figure=fig,
+            #)
             #fig = make_subplots(
 
             #    shared_xaxes='all',
             #    shared_yaxes='all',
             #    start_cell="bottom-left",
             #    horizontal_spacing=0.02,
             #    vertical_spacing=0.03,
             #    subplot_titles=[],
             #    column_widths=[1.0],
             #    row_heights=[1.0],
             #    specs=[[{'type': 'xy'}]],
             #    figure=fig)
             #trace.update({'xaxis': 'x', 'yaxis': 'y'})
+
+            # Add dummy bar plot as placeholder
             fig.add_trace(go.Bar(
                             name=dev,
-                            base=df[START_TIME],
-                            x=df['offset'],
-                            y=df[DEVICE],
-                            orientation='h'
+                            base=[df[START_TIME].iat[0]],
+                            x=[df['offset'].iat[0]],
+                            y=[df[DEVICE].iat[0]],
+                            orientation='h',
+                            showlegend=False
             ))
+
             fig.add_trace(trace, secondary_y=True)
-            fig.update_yaxes(range=[0, len(devs)], secondary_y=True) 
 
 
         # Create user_selection for each trace
         if df_devs_usel is not None:
             if dev in (dtypes[BOOL] + dtypes[CAT]): 
                 for cat in df[VALUE].unique():
                     fig.update_traces(selector=dict(meta=dev, name=cat),
                             selectedpoints=mark_selected[dev][cat],
                             selected={'marker': {'opacity': 1.0, 'color': cat_col_map[cat]}},
                             unselected={'marker': {'opacity': 0.3, 'color': cat_col_map[cat]}})
-                # TODO not for 
+                # TODO not for, flag for deletion 
                 #fig.update_traces(selector=dict(meta=dev, name=OFF),
                 #           selectedpoints=mark_selected[dev][OFF],
                 #           selected={'marker': {'opacity': 1.0, 'color': COL_OFF}},
                 #           unselected={'marker': {'opacity': 0.3, 'color': COL_OFF}})
                 #fig.update_traces(selector=dict(meta=dev, name=ON),
                 #           selectedpoints=mark_selected[dev][ON],
                 #           selected={'marker': {'opacity': 1.0, 'color': COL_ON}},
@@ -287,16 +276,41 @@
             else:
                 raise NotImplementedError
 
 
     fig.update_layout(yaxis_type='category')
     fig.update_yaxes(categoryorder='array', categoryarray=np.flip(dev_order))
 
+    if dtypes[NUM]:
+        # Reorder categorical devices
+        for dev in dtypes[NUM]:
+            dev_idx = np.where(fig.layout['yaxis1']['categoryarray'] == dev)[0][0]
+            y = list(fig.select_traces(selector=dict(name=dev, type='scatter')))[0]['y']
+            # Since data is scaled to 0.5 add 0.25 to center around dev_idx
+            y = y + dev_idx + 0.25
+            fig.update_traces(dict(y=y), selector=dict(type='scatter', name=dev))
+
     return fig
 
+def _abbreviate_long_names(arr: np.ndarray) -> np.ndarray:
+    THRESHOLD = 10
+    def func(x):
+        if len(x) > THRESHOLD:
+            # REmove preafix i.e. binary_sensor.blablbla
+            x = "".join([s for s in x.split('.')[0]])
+        if len(x) > THRESHOLD:
+            x = "".join([s[:3] for s in x.split('_')])
+        if len(x) > THRESHOLD:
+            x = x[:THRESHOLD]
+        else:
+            return x
+    vf = np.vectorize(func)
+    arr = vf(arr) 
+    return arr
+
 
 def _plot_device_events_into_fig(fig: go.Figure, df_devs: pd.DataFrame,  df_devs_usel: pd.DataFrame,
                                  df_devs_outside: pd.DataFrame, dev_order: list,
                                  marker_height=5,
                                  ) -> go.Figure:
     """
     Parameters
@@ -305,23 +319,23 @@
         Each dictionary contains the key 'df' and a 'color' and a 'opacity'
 
 
     """
     # Enable webgl rendering
     scatter = go.Scattergl if len(df_devs) > 15000 else go.Scatter
     EVENT_COLOR = 'Black'
-    hover_template = '%{y}<br>%{x|' + STRFTIME_DATE + '}<br>Event: %{customdata} <extra></extra>'
+    hover_template = '%{customdata[1]}<br>%{x|' + STRFTIME_PRECISE + '}<br>Event: %{customdata[0]} <extra></extra>'
 
 
     marker = dict(size=marker_height, symbol=42, line=dict(color=EVENT_COLOR, width=1))
     fig.update_layout(yaxis_type='category')
     fig.update_yaxes(categoryorder='array', categoryarray=np.flip(dev_order))
     fig.add_trace(scatter(
         mode='markers', y=df_devs[DEVICE], x=df_devs[TIME],
-        customdata=df_devs[VALUE],
+        customdata=df_devs[[VALUE, DEVICE]].values,
         hovertemplate=hover_template,
         showlegend=False, marker=marker))
 
     if not df_devs_outside.empty:
         marker['opacity'] = 0.1
         marker['line']['color'] = 'Grey'
         fig.add_trace(scatter(mode='markers', y=df_devs_outside[DEVICE],
@@ -369,24 +383,14 @@
     else:
         # Draw the line only if the given end is the left-most
         draw_end_line = (min(et, data_et) == et)
         et = min(et, data_et)
     return st, et, draw_start_line, draw_end_line
 
 
-
-def ActDictLoop(func):
-    def func_wrapper(*args, **kwargs):
-        if isinstance(df_acts_sel, pd.DataFrame):
-            df_acts_sel = ActivityDict(dict(tmp=df_acts_sel))
-        if isinstance(df_acts, pd.DataFrame):
-            df_acts = ActivityDict(dict(tmp=df_acts))
-            
-    return 
-
 def act_difference(df_acts_sel, df_acts, st, et):
     """ Get outside activities with enveloping activities correctly clipped
 
     Parameters
     ----------
     df_acts_sel : pd.DataFrame or ActivityDict or List
         asdf
@@ -450,16 +454,16 @@
     diff = df[END_TIME] - df[START_TIME]
     df['mid_point'] = df[START_TIME] + diff/2
     y_label = label
     df['y'] = y_label
 
     marker = dict(size=5, symbol=5, line=dict(color='Red', width=1))
     hover_template = 'Activity: %{customdata[2]}<br>' + \
-                     'Start_time: %{customdata[0]|' + STRFTIME_DATE + '}<br>' + \
-                     'End_time: %{customdata[1]|' + STRFTIME_DATE + '}<br>' + \
+                     'Start_time: %{customdata[0]|' + STRFTIME_PRECISE + '}<br>' + \
+                     'End_time: %{customdata[1]|' + STRFTIME_PRECISE + '}<br>' + \
                      '<extra></extra>'
 
     fig.add_trace(go.Scatter(
         mode='markers', y=df['y'], x=df['mid_point'],
         customdata=cd,
         marker=marker,
         hovertemplate=hover_template,
@@ -485,22 +489,22 @@
         df[END_TIME] = df[TIME].copy()
         for dev in dtypes[BOOL] + dtypes[CAT]:
             df_tmp = df_devs[df_devs[DEVICE] == dev].copy()
             df_tmp[END_TIME] = df_tmp[TIME].shift(-1)
             mask = (dev == df[DEVICE])
             times = df.loc[mask, TIME]
             vals = df_tmp[df_tmp[TIME].isin(times)]
-            df.at[mask, END_TIME] = vals
+            df.loc[mask, END_TIME] = vals[END_TIME]
 
         df[START_TIME] = df[TIME]
         df[TIME] = df[TIME] + (df[END_TIME] - df[TIME])/2
         custom_data = df[[DEVICE, START_TIME, END_TIME]].values
         hover_template = 'Device: %{customdata[0]}<br>' + \
-                         'Start_time: %{customdata[1]|' + STRFTIME_DATE + '}<br>' + \
-                         'End_time: %{customdata[2]|' + STRFTIME_DATE + '}<br>' + \
+                         'Start_time: %{customdata[1]|' + STRFTIME_PRECISE + '}<br>' + \
+                         'End_time: %{customdata[2]|' + STRFTIME_PRECISE + '}<br>' + \
                          '<extra></extra>'
     else:
         custom_data = df[DEVICE]
         hover_template = 'Device: %{customdata}<br>Time: %{x}<extra></extra>'
     marker = dict(size=5, symbol=5, line=dict(color='Red', width=1))
     fig.add_trace(go.Scatter(
         mode='markers', y=df['y'], x=df[TIME],
@@ -510,69 +514,78 @@
         showlegend=False))
     y_axis_order = [y_label, *list(fig.layout.yaxis.categoryarray)]
     fig.update_yaxes(categoryarray=y_axis_order)
     return fig
 
 
 
-def activities_and_devices(df_acts, df_devs, states=False, st=None, et=None,
-                           act_order='alphabetical', dev_order='alphabetical',
+def activities_and_devices(df_devs, df_acts, states=False, st=None, et=None,
+                           act_order='alphabetical', dev_order='alphabetical', dev2area=None,
                            df_acts_usel=None, df_devs_usel=None, devs_usel_state=None,
-                           height=350
+                           height=None, zoomed_range=[], fig=None, row=None, col=None
                            ):
     """
 
     Parameters
     ----------
     df_acts : pd.Dataframe or List of dataframes or dict of  
     """
 
+    st = pd.Timestamp(st) if st is not None else st
+    et = pd.Timestamp(et) if et is not None else et
+
     # Determines if device markers indicate the event or a states midpoint
     if states:
         devs_usel_state = states if devs_usel_state is None else devs_usel_state
     else:
         devs_usel_state = False
     assert isinstance(devs_usel_state, bool), 'devs_usel_state has to be set with either a boolean or None'
 
     dct_acts = ActivityDict.wrap(df_acts)
     if df_acts_usel is not None:
         dct_acts_usel = ActivityDict.wrap(df_acts_usel)
     else:
         dct_acts_usel = None
 
 
-
-    for k, df in dct_acts.items():
-        dct_acts[k] = df.copy() 
+    dct_acts = dct_acts.copy()
     df_devs = df_devs.copy()
 
+ 
+
     # Determine the start and endpoint with regard to optional given parameters
     st, et, draw_start_line, draw_end_line = _determine_start_and_end(dct_acts, df_devs, st, et)
 
     # Select the active displayed parts
     df_devs_sel, dct_acts_sel = select_timespan(df_devs, dct_acts, st, et, clip_activities=True)
 
     # Get the y-axis and label order
     act_order = activity_order_by(dct_acts_sel.concat(), rule=act_order)
-    dev_order = device_order_by(df_devs_sel, rule=dev_order)
+    dev_order = device_order_by(df_devs_sel, rule=dev_order, dev2area=dev2area)
 
 
     # determinte visual properties
     nr_devs = len(dev_order)
     nr_subjs = len(dct_acts)
-    height = _dynamic_and_height(nr_devs, nr_subjs)
-    marker_height = 3 if nr_devs > 15 else 5
-    y_label_size = _dyn_y_label_size(height, nr_devs)
+    height = _dynamic_and_height(nr_devs, nr_subjs) if height is None else height
+    marker_height = dyn_event_marker_size(height, nr_devs)
+    y_label_size = dyn_y_label_size(height, nr_devs)
 
     # Reconstruct outside parts
     df_devs_outside = df_difference(df_devs_sel, df_devs)
     dct_acts_outside = act_difference(dct_acts_sel, dct_acts, st, et)
 
     title = 'Activities and device events'
-    fig = go.Figure()
+    if fig is None:
+        col, row = 1,1
+        fig = make_subplots(rows=row, cols=col)
+    else:
+        row = 1 if row is None else row
+        col = 1 if col is None else col
+
 
     for key in reversed(list(dct_acts.keys())):
         if df_acts_usel is not None:
             try:
                 usel = dct_acts_usel[key]
             except: 
                 usel = None
@@ -582,15 +595,15 @@
                                         dct_acts_outside[key], act_order,
                                         y_label=f'Acts: {key}'
                                         )
 
 
     if states:
         fig = _plot_device_states_into_fig(fig, df_devs_sel, df_devs_usel,
-                                           df_devs_outside, dev_order, st, et)
+                                           df_devs_outside, dev_order, st, et, row, col)
     else:
         fig = _plot_device_events_into_fig(fig, df_devs_sel, df_devs_usel, df_devs_outside, 
                                            dev_order, marker_height)
 
 
 
     # Plot markers into trace
@@ -608,14 +621,20 @@
     if draw_end_line:
         fig.add_vline(x=et, line_width=1, line_color="Grey")
 
     _set_compact_title(fig, title)
     fig.update_yaxes(title=None, fixedrange=True, tickfont=dict(size=y_label_size),
                      ticklabeloverflow='allow'
                      )
+    if zoomed_range:
+        zr_st = pd.Timestamp(zoomed_range[0])
+        zr_et = pd.Timestamp(zoomed_range[1])
+        fig.update_xaxes(type='date', range=[zr_st, zr_et])
+
+
     fig.update_layout(margin=dict(l=0, r=0, b=0, t=30, pad=0), height=height)
     return fig
 
 
 def _endtime_to_offset(df_act, replace=True):
     """Compute the end_time as numerical offset in ms"""
     x_start = pd.to_datetime(df_act[START_TIME])
@@ -646,15 +665,18 @@
         df['y_label'] = y_label
         df = df[['y_label', START_TIME, END_TIME, ACTIVITY]]
         df['dur'] = (df[END_TIME] - df[START_TIME]).astype(str)
         return df
 
 
     df_acts = _helper_1(df_acts)
-    df_acts_outside = _helper_1(df_acts_outside)
+    if df_acts_outside is None:
+        df_acts_outside = create_empty_activity_df()
+    else:
+        df_acts_outside = _helper_1(df_acts_outside)
 
     if df_acts_usel is not None:
         df_acts_usel = _helper_1(df_acts_usel)
         df_acts_usel = _endtime_to_offset(df_acts_usel)
 
     args = dict(data_frame=df_acts,
                 x_start=START_TIME,
@@ -703,41 +725,39 @@
             continue
 
         # Get dataframe with of only activity
         df_sel_act = grouped.get_group(act_name)
 
         # Create the trace
         # TODO showlegend
-        showlegend = act_name not in _legend_current_items(fig)
-        trace = go.Bar(name=act_name)
-
-        trace.update(legendgroup=act_name, 
-                     showlegend=showlegend,
-                     legendgrouptitle_text=set_legendgrouptitle,
-                     alignmentgroup=True, 
-                     offsetgroup=act_name)
-        set_legendgrouptitle = None
-        # Init subplot row/col
-        trace._subplot_row = 1
-        trace._subplot_col = 1
-
+        showlegend = act_name not in legend_current_items(fig)
         m = grouped_mappings[0]
         trace_color = m.val_map[act_name]
-        m.updater(trace, trace_color)
+
         hover_template = '<b>' + act_name + '</b><br>'\
-                         + 'Start_time: %{base|' + STRFTIME_DATE + '}<br>' \
-                         + 'End_time: %{x| ' + STRFTIME_DATE + '}' \
+                         + 'Start_time: %{base|' + STRFTIME_PRECISE + '}<br>' \
+                         + 'End_time: %{x| ' + STRFTIME_PRECISE + '}' \
                          + '<br>Duration: %{customdata}<extra></extra>'
-        trace.update(dict(textposition='auto', orientation='h',
-                          base=df_sel_act[START_TIME],
-                          x=df_sel_act[END_TIME],
-                          y=df_sel_act['y_label'],
-                          customdata=df_sel_act['dur'],
-                          hovertemplate=hover_template
-        ))
+
+        trace = go.Bar(name=act_name,
+                       legendgroup=act_name, 
+                       showlegend=showlegend,
+                       legendgrouptitle_text=set_legendgrouptitle,
+                       marker_color=trace_color,
+                       alignmentgroup=True, 
+                       offsetgroup=act_name,
+                       textposition='auto', 
+                       orientation='h',
+                       base=df_sel_act[START_TIME],
+                       x=df_sel_act[END_TIME],
+                       y=df_sel_act['y_label'],
+                       customdata=df_sel_act['dur'],
+                       hovertemplate=hover_template
+        )
+        set_legendgrouptitle = None
 
         trace_lst.append(trace)
 
         # Create user_selection for each trace
         if df_acts_usel is not None:
             # Get the indices in the trace where
             comp_df = df_sel_act.copy().merge(df_acts_usel, indicator=True, how='left')
@@ -781,41 +801,41 @@
         subplot_titles=[],
         column_widths=[1.0],
         row_heights=[1.0],
         specs=[[{'type': 'xy'}]],
         figure=fig)
 
 
-    # Position traces in subplots
-    for trace in trace_lst:
-        trace.update({'xaxis': 'x', 'yaxis': 'y'})
-
     # Add traces, layout and frames to figure
     fig.add_traces(trace_lst)
+
+    # Resizes bars to full size
     fig.update_layout({'barmode': 'overlay',
                        'legend': {'tracegroupgap': 0}
                        })
-    configure_axes(args, go.Bar, fig, orders)
+    fig.update_xaxes(type="date")
 
     return fig
 
 
-def contingency_events(df_acts=None, df_devs=None, con_tab=None, scale='linear', height=350,
-                       act_order='alphabetical', dev_order='alphabetical', distributed=False
+
+
+def contingency_events(df_devs=None, df_acts=None, con_tab=None, scale='linear', height=350,
+                       act_order='alphabetical', dev_order='alphabetical', n_jobs=1,
                        ) -> plotly.graph_objects.Figure:
     """
     """
     title = 'Activities vs device events'
     cbarlabel = 'count' if scale == 'linear' else 'log count'
 
     # get the list of cross tabulations per t_window
     if con_tab is not None:
         df_con = con_tab.copy()    # :pd.DataFrame
     else:
-        df_con = contingency_table_events(df_devs, df_acts)
+        df_con = contingency_table_events(df_devs, df_acts, n_jobs=n_jobs)
 
     df_con = df_con.set_index('device')
 
     act_order = activity_order_by(df_acts, rule=act_order)
     dev_order = device_order_by(df_devs, rule=dev_order)
     df_con = df_con[np.flip(act_order)]     # change order of rows
     df_con = df_con.reindex(dev_order)      # change order of columns
@@ -840,27 +860,28 @@
     fig.update_xaxes(tickangle=45)
     fig.update_layout(margin=dict(l=0, r=0, b=0, t=30, pad=0), height=height)
     _style_colorbar(fig, cbarlabel)
 
     return fig
 
 
-def contingency_states(df_acts=None, df_devs=None, con_tab=None, scale='linear', height=350,
-                       act_order='alphabetical', dev_order='alphabetical', distributed=False
+def contingency_states(df_devs=None, df_acts=None, con_tab=None, scale='linear', height=350,
+                       act_order='alphabetical', dev_order='alphabetical', n_jobs=1
                        ) -> plotly.graph_objects.Figure:
     """
     """
     title = 'Activities vs device states'
     cbarlabel = 'seconds' if scale == 'linear' else 'log seconds'
 
     # get the list of cross tabulations per t_window
     if con_tab is not None:
         df_con = con_tab.copy()    # :pd.DataFrame
+        df_con.index.name = DEVICE
     else:
-        df_con = contingency_table_states(df_devs, df_acts, distributed=distributed)
+        df_con = contingency_table_states(df_devs, df_acts, n_jobs=n_jobs)
 
     # Determine device and activity labels order
     act_order = activity_order_by(df_acts, rule=act_order)
     df_con = df_con[np.flip(act_order)]     # change order of rows
     devs = df_con.index.values
 
     # Reorder and format devices
@@ -910,13 +931,158 @@
 
     fig.update_xaxes(tickangle=45)
     fig.update_layout(margin=dict(l=0, r=0, b=0, t=30, pad=0), height=height)
     _style_colorbar(fig, cbarlabel)
 
     return fig
 
-def _legend_current_items(fig):
-    legend_current_items = [] 
-    for trace in fig.data:
-        if isinstance(trace, go.Bar):
-            legend_current_items.append(trace.legendgroup)
-    return legend_current_items
+
+def event_correlogram(df_devs: pd.DataFrame, df_acts: pd.DataFrame, fix=[], to=[], maxlag='2min', binsize='2s', use_dask=False):
+
+    from pyadlml.dataset.plot.plotly.devices import plotly_event_correlogram
+
+    # Wrap if not list
+    fix = [fix] if isinstance(fix, str) else fix
+    to = [to] if isinstance(to, str) else to
+
+    activities = df_acts[ACTIVITY].unique().tolist()
+    if fix:
+        assert np.array([e in activities for e in fix]).all()
+        activities = fix
+    
+    devices = df_devs[DEVICE].unique().tolist()
+    if to:
+        assert np.array([e in devices for e in to]).all()
+        devices = to
+
+    df_acts[VALUE] = 1
+    df_acts = df_acts.rename(columns={ACTIVITY: DEVICE})
+
+    df_act_st = df_acts[[START_TIME, DEVICE, VALUE]].copy()
+    df_act_st = df_act_st.rename(columns={START_TIME:TIME})
+    df_act_et = df_acts[[END_TIME, DEVICE, VALUE]].copy()
+    df_act_et = df_act_et.rename(columns={END_TIME:TIME})
+
+    df_comb_st = pd.concat([df_devs, df_act_st], axis=0)\
+                    .sort_values(by=TIME)\
+                    .reset_index(drop=True)
+    df_comb_et = pd.concat([df_devs, df_act_et], axis=0)\
+                    .sort_values(by=TIME)\
+                    .reset_index(drop=True)
+
+    cc_st, bins, rows, cols = event_cross_correlogram3(
+        df_comb_st, fix=activities, to=devices, maxlag=maxlag, binsize=binsize,
+        use_dask=use_dask
+    )
+    cc_et, bins, rows, cols = event_cross_correlogram3(
+        df_comb_et, fix=activities, to=devices, maxlag=maxlag, binsize=binsize,
+        use_dask=use_dask
+    )
+    mid_point = int(np.floor(len(bins)/2))
+    for i in range(len(devices)):
+        for j in range(len(activities)):
+            # Overwrite right half of st not including the odd zero bin
+            cc_st[i,j, mid_point+1:] = cc_et[i,j,mid_point+1:]
+            cc_st[i,j, mid_point] += cc_et[i,j, mid_point]
+
+    return plotly_event_correlogram(
+        cc_data=[cc_st, bins, rows, cols]
+    )
+
+
+
+@remove_whitespace_around_fig
+def activity_vs_device_events_hist(df_devs, df_acts, device, activity, n_bins=20, normalize=False, height=600):
+    fig = make_subplots(rows=2, cols=1, shared_xaxes=True, row_heights=[0.9, 0.1],
+                        vertical_spacing=0.01, 
+    
+    )
+
+    df_acts = df_acts[df_acts[ACTIVITY] == activity].sort_values(by=START_TIME)\
+                                                    .reset_index(drop=True)
+    df_devs = df_devs[df_devs[DEVICE] == device].sort_values(by=TIME)\
+                                                .reset_index(drop=True)
+
+    counts = np.zeros((n_bins,))
+
+    if not normalize:
+        df_acts['dt'] = df_acts[END_TIME] - df_acts[START_TIME]
+        df_acts['minutes'] = df_acts['dt'].apply(_get_freq_func('minutes'))
+        total_dt = max(df_acts['minutes'])
+    else:
+        total_dt = 1
+
+
+    for _, act_ser in df_acts.iterrows():
+        if normalize:
+            dt2zeroone = lambda x : (x - act_ser[START_TIME])/(act_ser[END_TIME] - act_ser[START_TIME])
+
+        dev_mask = (act_ser[START_TIME] < df_devs[TIME]) \
+                    & (df_devs[TIME] < act_ser[END_TIME])
+        devs = df_devs[dev_mask].copy() 
+
+        if devs.empty:
+            continue
+
+        if normalize:
+            vals = devs[TIME].apply(dt2zeroone).values
+        else:
+            vals = (devs[TIME] - act_ser[START_TIME]).apply(_get_freq_func('minutes')).values
+
+        add, bins = np.histogram(vals, bins=n_bins, range=(0,total_dt), density=False)
+        counts += add
+
+
+    if not 'bins' in locals():
+        # Case when no device event happened during given activities
+        bins = np.linspace(0, total_dt, n_bins)
+        print('Warning! No device event happend during activity')
+
+
+    # Plot histogramm 
+    # Move bars into intervals
+    bar_width = (bins[-1] - bins[-2])*.8
+    midpoints = bins[:-1] + (bins[1:] - bins[:-1])/2
+    customdata = np.array([f'({b[0]:.3f}, {b[1]:.3f}]' for b in zip(bins[:-1], bins[1:])])
+
+
+    fig.add_trace(
+        go.Bar(
+            x=midpoints,
+            y=counts,
+            name=device,
+            width=bar_width,
+            customdata=customdata,
+            hovertemplate='%{customdata} %{y} times <extra></extra>',
+            opacity=1,
+            showlegend=True,
+            marker=dict(line_width=0)
+        ),row=1, col=1
+    )
+    fig.update_yaxes(title_text='counts', row=1, col=1)
+
+    if normalize:
+        fig.add_trace(
+            go.Bar(
+                x=[0,1],
+                y=[activity]*2,
+                orientation='h',
+                opacity=1,
+                showlegend=False,
+                marker=dict(line_width=0)
+            ),row=2, col=1
+        )
+    else:
+        fig.add_trace(
+            go.Box(
+                name=activity,
+                x=df_acts['minutes'],
+            ),row=2, col=1
+        )
+    if normalize:
+        fig.update_xaxes(range=[0,1], title_text='normalized range', row=2, col=1)
+    else:
+        fig.update_xaxes(title_text='minutes', row=2, col=1)
+
+    fig.update_layout(title_text="Device events over one activity", height=height)
+
+    return fig
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/dashboard/dashboard.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/plot/plotly/dashboard/dashboard.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,37 +5,40 @@
 import dash.html as html
 import dash_bootstrap_components as dbc
 import pandas as pd
 from dash.dependencies import *  # TODO remove if nothing else is imported
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 from dask.delayed import delayed
-
+import numpy as np
 from pyadlml.constants import (ACTIVITY, DEVICE, END_TIME, START_TIME, TIME,
                                VALUE)
-from pyadlml.dataset._core._dataset import label_data
-from pyadlml.dataset._core.activities import _create_activity_df
+from pyadlml.dataset._core.acts_and_devs import label_data, label_data2
+from pyadlml.dataset._core.activities import add_other_activity, create_empty_activity_df
 from pyadlml.dataset._datasets.aras import _create_device_df
-from pyadlml.dataset.plotly.activities import *
-from pyadlml.dataset.plotly.acts_and_devs import *
-from pyadlml.dataset.plotly.dashboard.callbacks import (
-    _create_activity_tab_callback, _initialize_activity_toggle_cbs)
-from pyadlml.dataset.plotly.dashboard.layout import (
-    DEV_DENS_SLIDER, activities_layout, acts_n_devs_layout,
+from pyadlml.dataset.plot.plotly.util import dash_get_trigger_element, dash_get_trigger_value
+from pyadlml.dataset.plot.plotly.activities import *
+from pyadlml.dataset.plot.plotly.acts_and_devs import *
+from pyadlml.dataset.plot.plotly.dashboard.callbacks import (
+    _create_activity_tab_callback, _create_acts_vs_devs_tab_callback, _initialize_activity_toggle_cbs)
+from pyadlml.dataset.plot.plotly.dashboard.layout import (
+    BIN_SIZE_SLIDER, DEV_DENS_SLIDER, LAG_SLIDER, activities_layout, acts_n_devs_layout,
     acts_vs_devs_layout, device_layout_graph_bottom, devices_layout)
-from pyadlml.dataset.plotly.devices import bar_count as dev_bar_count
-from pyadlml.dataset.plotly.devices import boxplot_state
-from pyadlml.dataset.plotly.devices import device_iei as dev_iei
-from pyadlml.dataset.plotly.devices import event_density
-from pyadlml.dataset.plotly.util import ActivityDict
+from pyadlml.dataset.plot.plotly.devices import bar_count as dev_bar_count
+from pyadlml.dataset.plot.plotly.devices import boxplot_state
+from pyadlml.dataset.plot.plotly.devices import device_iei as dev_iei
+from pyadlml.dataset.plot.plotly.devices import event_density
+from pyadlml.dataset._core.activities import ActivityDict
 from pyadlml.dataset.stats.acts_and_devs import (contingency_table_events,
                                                  contingency_table_states)
-from pyadlml.dataset.util import (device_order_by, num_to_timestamp,
+from pyadlml.dataset.util import (activity_order_by, device_order_by, num_to_timestamp,
                                   select_timespan, timestamp_to_num)
-
+from pyadlml.dataset.plot.plotly.devices import plotly_event_correlogram as dev_cc
+from pyadlml.dataset.plot.plotly.util import deserialize_range, serialize_range, range_from_fig
+from pyadlml.constants import ts2str, str2ts
 
 def _get_plot_height_devs(nr_devs):
     # Determine the plot height and fontsize for activity plots
     if nr_devs < 20:
         return 350
     elif nr_devs < 30:
         return 400
@@ -52,28 +55,27 @@
         return 350
     elif nr_acts < 25:
         return 450
     else:
         return 350
 
 
-def dashboard(app, name, embedded=False, df_acts=None, df_devs=None, start_time=None, end_time=None):
+def dashboard(app, name, embedded=False, df_acts=None, df_devs=None, dev2area=None, start_time=None, end_time=None):
     """ Creates a dashboard
 
     Note
     -----
     All parameter may be 'None' if the app is populated during runtime
 
     """
 
-    # Since performance rendering issues arise with numbers greater than 40000
-    # device datapoints make a preselection
     df_acts = ActivityDict.wrap(df_acts)
-    assert isinstance(df_acts, dict)
 
+    # Since performance rendering issues arise with numbers greater than 40000
+    # device datapoints make a preselection
     max_points = 40000
     if df_devs is not None and len(df_devs) > max_points:
         set_et = df_devs.iat[max_points, df_devs.columns.get_loc(TIME)]
         curr_df_devs, curr_df_acts = select_timespan(
             df_acts=df_acts, df_devs=df_devs, start_time=start_time,
             end_time=set_et, clip_activities=True
         )
@@ -82,90 +84,121 @@
         curr_df_acts = df_acts
         set_et = end_time
     
     nr_devs = len(df_devs[DEVICE].unique()) if df_devs is not None else 0
     nr_acts = df_acts.nr_acts() if df_acts is not None else 0
 
     if start_time is None:
-        start_time = min(df_devs[TIME].iloc[0], *[df_acts[k][START_TIME].iloc[0] for k in df_acts.keys()])
+        start_time = min(df_devs[TIME].iloc[0], df_acts.min_starttime())
         start_time = start_time.floor('D')
     if end_time is None:
-        end_time = max(df_devs[TIME].iloc[-1], *[df_acts[k][END_TIME].iloc[-1] for k in df_acts.keys()])
+        end_time = max(df_devs[TIME].iloc[-1], df_acts.max_endtime())
         end_time = end_time.ceil('D')
 
     # TODO refactor: ugly as hell defined in 76
     if df_devs is None or len(df_devs) <= max_points:
         set_et = end_time
 
     plot_height_devs = _get_plot_height_devs(nr_devs)
     plot_height_acts = _get_plot_height_acts(nr_acts)
+    is_top_down_view = (nr_devs < 60)
+    plot_height_ands = (plot_height_devs+50 if is_top_down_view else 1300)
 
     # Get Layout
-    layout_activities = [activities_layout(df, k, plot_height_acts) for k, df in curr_df_acts.items()]
+    layout_activities = [activities_layout(df, k, plot_height_acts) 
+                         for k, df in curr_df_acts.items()]
     layout_devices = devices_layout(curr_df_devs, True, plot_height_devs)
-    layout_acts_vs_devs = acts_vs_devs_layout(
-        list(curr_df_acts.values())[0],        # TODO, check how to do this in future
-        curr_df_devs,
-        True,
-        plot_height_acts
-    )
+    layout_acts_vs_devs = [acts_vs_devs_layout(df, k, df_devs, plot_height=plot_height_acts) 
+                           for k, df in curr_df_acts.items()]
+
+    # Generate tabs for multiple persons
+    activity_tabs = [dbc.Tab(l, label=f'Act: {act_name}', tab_id=f'tab-acts-{act_name}') 
+                     for act_name, l in zip(curr_df_acts.keys(), layout_activities)]
+    acts_vs_devs_tabs = [
+                 dbc.Tab(l, label=f'Act: {act_name} ~ Devices', tab_id=f'tab-acts_vs_devs-{act_name}')
+                 for act_name, l in zip(curr_df_acts.keys(), layout_acts_vs_devs)]
+    
+    def layout_content(and_layout, tabs_and_content):
+        if is_top_down_view:
+            return [
+                and_layout, 
+                html.Br(),
+                html.Div([
+                    *tabs_and_content
+                ]),
+            ]
+        else:
+            return [
+                dbc.Row([
+                    dbc.Col([
+                        and_layout, 
+                    ], md=7),
+                    dbc.Col([
+                        html.Div([
+                            *tabs_and_content
+                        ]),
+                    ], md=5),
+                ], style=dict(width="2800px", height="1500px"))
+            ]
 
-    activity_tabs = [dbc.Tab(l, label=f'Act: {act_name}', tab_id=f'tab-acts-{act_name}') for act_name, l in zip(curr_df_acts.keys(), layout_activities)]
     content = [
-            dcc.Input(id='act_assist_path', type='hidden', value='filler text'),
-            dcc.Input(id='subject_names', type='hidden', value='filler text'),
-            html.H2(children=f'Dashboard: {name}'),
-            acts_n_devs_layout(df_acts, df_devs, start_time, end_time,
-                               set_et, plot_height_devs+50),
-            html.Br(),
-        html.Div([
-            dbc.Tabs(
+        dcc.Input(id='act_assist_path', type='hidden', value='filler text'),
+        dcc.Input(id='subject_names', type='hidden', value='filler text'),
+        html.H2(children=f'Dashboard: {name}'),
+
+        *layout_content(
+            acts_n_devs_layout(df_devs, df_acts, start_time, end_time, set_et, plot_height_ands),
+            [dbc.Tabs(
                 [*activity_tabs,
-                 dbc.Tab(layout_devices, label='Devices', tab_id='tab-devs'),
-                 dbc.Tab(layout_acts_vs_devs, label='Activities ~ Devices', tab_id='tab-acts_vs_devs'),
-                 ], id='tabs', active_tab=f'tab-acts-{list(curr_df_acts.keys())[0]}',
+                    dbc.Tab(layout_devices, label='Devices', tab_id='tab-devs'),
+                    *acts_vs_devs_tabs
+                    ], id='tabs', active_tab=f'tab-acts-{list(curr_df_acts.keys())[0]}',
             ),
-            html.Div(id="content"),
-        ]),
-        # Store intermediate values of hard to compute values
-        # dcc.Store(id='current-df-acts'),
+            html.Div(id="content"),]
+        )
     ]
 
     if embedded:
         layout = dbc.Container(
             children=content, 
-            style={'width': 1000, 'margin': 'auto'}
+            style={'width': 1300, 'margin': 'auto'}
         )
     else:
+        width = 1320 if is_top_down_view else 2200
         layout = dbc.Container(
             children=content,
-            style={'margin': 'auto'}
+            style={'width': width}
         )
     app.layout = layout
 
+    df_acts.apply(add_other_activity)
 
-    create_callbacks(app, df_acts, df_devs, start_time, end_time, plot_height_acts, plot_height_devs)
+    create_callbacks(app, df_acts, df_devs, start_time, end_time, dev2area, 
+                     plot_height_acts, plot_height_devs, plot_height_ands
+    )
 
 def _sel_avd_event_click(avd_event_select, curr_df_acts, curr_df_devs):
     """Select devices and activities from click data of the event contingency table"""
+
+    # Get relevant acts and devs
+    activity = avd_event_select['points'][0]['y']
+    device = avd_event_select['points'][0]['x']
+    df_devs = curr_df_devs[curr_df_devs[DEVICE] == device].copy()
+    df_acts = curr_df_acts[curr_df_acts[ACTIVITY] == activity].copy()
+
     # Select devices
-    a = avd_event_select['points'][0]['y']
-    d = avd_event_select['points'][0]['x']
-    df_tmp = curr_df_devs[curr_df_devs[DEVICE] == d]
-    df_tmp = label_data(df_tmp, curr_df_acts)
-    df_tmp = df_tmp[df_tmp[ACTIVITY] == a]
-    sel_devices = df_tmp[[TIME, DEVICE, VALUE]]
+    sel_devices = label_data2(df_devs, df_acts).dropna()
+    sel_devices = sel_devices[[TIME, DEVICE, VALUE]]
 
     # Select activities
-    sel_activities = _create_activity_df()
+    sel_activities = create_empty_activity_df()
     for _, sel_dev in sel_devices.iterrows():
-        mask = (curr_df_acts[START_TIME] < sel_dev[TIME]) \
-               & (sel_dev[TIME] < curr_df_acts[END_TIME])
-        tmp = curr_df_acts[mask]
-        sel_activities = pd.concat([sel_activities, tmp])
+        mask = (df_acts[START_TIME] < sel_dev[TIME]) \
+               & (sel_dev[TIME] < df_acts[END_TIME])
+        sel_activities = pd.concat([sel_activities, df_acts[mask]])
     sel_activities = sel_activities.drop_duplicates()
     return sel_devices, sel_activities
 
 
 def _sel_point_to_activities(selection):
     """ Gets the selected activities from the boxplot or violin-plot and
         asdf
@@ -248,15 +281,15 @@
         df_res = pd.concat([df_res, df_devs[mask]])
 
     return df_res
 
 
 def _sel_dev_density(selection, df_devs, dt):
 
-    from pyadlml.dataset.plotly.dashboard.layout import DEV_DENS_SLIDER
+    from pyadlml.dataset.plot.plotly.dashboard.layout import DEV_DENS_SLIDER
     df = df_devs.copy().set_index(TIME, drop=False)
     dt = pd.Timedelta(DEV_DENS_SLIDER[dt])
     df_res = pd.DataFrame(columns=[TIME, DEVICE, VALUE])
 
     for p in selection['points']:
         dev = p['y']
         count = p['z']
@@ -293,30 +326,14 @@
     return df4
 
 
 def _initialize_toggle_callbacks(app):
 
 
     @app.callback(
-        Output("clps-avd-state", "is_open"),
-        [Input("clps-avd-state-button", "n_clicks")],
-        [State("clps-avd-state", "is_open")],
-    )
-    def toggle_collapse(n, is_open):
-        return bool(n) ^ bool(is_open)
-
-    @app.callback(
-        Output("clps-avd-event", "is_open"),
-        [Input("clps-avd-event-button", "n_clicks")],
-        [State("clps-avd-event", "is_open")],
-    )
-    def toggle_collapse(n, is_open):
-        return bool(n) ^ bool(is_open)
-
-    @app.callback(
         Output("clps-acts-n-devs", "is_open"),
         [Input("clps-acts-n-devs-button", "n_clicks")],
         [State("clps-acts-n-devs", "is_open")],
     )
     def toggle_collapse(n, is_open):
         return bool(n) ^ bool(is_open)
 
@@ -348,38 +365,59 @@
         Output("clps-dev-density", "is_open"),
         [Input("clps-dev-density-button", "n_clicks")],
         [State("clps-dev-density", "is_open")],
     )
     def toggle_collapse_act_bp(n, is_open):
         return bool(n) ^ bool(is_open)
 
+    @app.callback(
+        Output("clps-dev-cc", "is_open"),
+        [Input("clps-dev-cc-button", "n_clicks")],
+        [State("clps-dev-cc", "is_open")],
+    )
+    def toggle_collapse_act_bp(n, is_open):
+        return bool(n) ^ bool(is_open)
 
-def create_callbacks(app, dct_acts, df_devs, start_time, end_time, plt_height_acts, plt_height_devs):
+def create_callbacks(app, dct_acts, df_devs, start_time, end_time, dev2area, plt_height_acts, plt_height_devs, plt_height_ands):
 
     def gen_trigger(id, val):
         return html.Div(id=id, style=dict(display="none"), **{"data-value": val})
 
     _initialize_toggle_callbacks(app)
 
     for key in dct_acts.keys():
         _initialize_activity_toggle_cbs(app, key)
 
     @app.callback(
         Output("and_clipboard", "content"),
         Input("graph-acts_n_devs", "clickData"),
-        State("and_dev-type", "value")
+        Input("and_btn_copy_range", "n_clicks"),
+        State("and_dev-type", "value"),
+        State("graph-acts_n_devs", "figure")
     )
-    def element_to_clipboard(tmp, dev_type):
-        if tmp is None:
+    def element_to_clipboard(tmp, btn_cr, dev_type, fig_and):
+
+        ctx = dash.callback_context
+        trigger_val =  dash_get_trigger_value(ctx)
+        trigger = dash_get_trigger_element(ctx)
+        is_copy_range = (trigger == 'and_btn_copy_range')
+        if trigger_val is None\
+            or (tmp is None and not is_copy_range):
             raise PreventUpdate
-        dp = tmp['points'][0]
-        is_activity = (dp['y'] == 'Activity')
-        is_dev_state = not is_activity and dev_type == 'state'
-        is_dev_event = not is_activity and dev_type == 'event'
-        if is_activity:
+
+        if not is_copy_range:
+            dp = tmp['points'][0]
+            is_activity = (dp['y'] == 'Activity')
+            is_dev_state = not is_activity and dev_type == 'state'
+            is_dev_event = not is_activity and dev_type == 'event'
+
+        if is_copy_range:
+            range = range_from_fig(fig_and)
+            s = f'{ts2str(range[0])},{ts2str(range[1])}'
+        elif is_activity:
             start_time = dp['base']
             end_time = dp['x']
             s = f'\'{start_time}\',\'{end_time}\',#activity'
         elif is_dev_state:
             start_time = dp['base']
             end_time = dp['customdata'][1]
             dev = dp['y']
@@ -398,32 +436,33 @@
     act_inputs = []
     act_states = []
     for subj_name  in dct_acts.keys():
         act_outputs.extend([
             Output(f'act-trigger-{subj_name}', 'children'),
             Output(f'act-curr-sel-{subj_name}', 'children'),
             Output(f'act-curr-sel-store-{subj_name}', 'data'),
+            Output(f'avd-trigger-{subj_name}', 'children'),
         ])
         act_inputs.extend([
             Input(f'acts_graph-boxplot-{subj_name}', 'selectedData'),
             Input(f'acts_graph-transition-{subj_name}', 'clickData'),
             Input(f'acts_graph-bar-{subj_name}', 'clickData'),
+            Input(f'avd_graph-event-contingency-{subj_name}', 'clickData'),
         ])
         act_states.extend([
             State(f'act-curr-sel-store-{subj_name}', 'data'), 
             State(f'act-curr-sel-{subj_name}', 'children'),
         ])
 
     @app.callback(
         output=[
             Output('graph-acts_n_devs', 'figure'),
             Output('and_act-order', 'data'),
             Output('and_dev-order', 'data'),
             Output('and_reset_sel', 'disabled'),
-            Output('avd-trigger', 'children'),
             Output('dev-trigger', 'children'),
             Output('dev-curr-sel', 'children'),
             Output('dev-curr-sel-store', 'data'),
             *act_outputs
         ],
         inputs=[
             # Input methods
@@ -437,15 +476,14 @@
             # Selected devices
             Input('devs_graph-bar', 'clickData'),
             Input('devs_graph-boxplot', 'selectedData'),
             Input('devs_graph-iei', 'selectedData'),
             Input('devs_graph-fraction', 'clickData'),
 
             Input('devs_graph-density', 'clickData'),
-            Input('avd_graph-event-contingency', 'clickData'),
             Input('and_reset_sel', 'n_clicks'),
 
             # Selected activities
             *act_inputs
         ],
         state=[
             State('devs_dens-slider', 'value'),
@@ -458,39 +496,41 @@
             *act_states
         ]
     )
     def update_acts_n_devs(*args):
 
         nr_subjects = len(dct_acts.keys())
 
-        idx = 13
+        idx = 12
         rng, sel_activities, sel_devices, act_order_trigger, dev_order_trigger, dev_type_trigger, \
         dev_bar_select, dev_boxplot_select, dev_iei_select, dev_fraction_select, \
-        dev_density_select, avd_event_select, reset_sel = args[:idx]    # [0:13] -> 1el, ..., 13 el
+        dev_density_select, reset_sel = args[:idx]    # [0:12] -> 1el, ..., 12 el
 
         for i, subj_name in enumerate(dct_acts.keys()):
-            j, k, l = idx+i+i*nr_subjects, idx+i+i*nr_subjects+1, idx+i+i*nr_subjects+2
+            j = idx+i+i*nr_subjects
+            k, l, m = j+1, j+2, j+3
             locals()[f'act_boxplot_select_{subj_name}'] = args[j]   # [13] -> 14 el  
             locals()[f'act_trans_select_{subj_name}'] = args[k]     # [14] -> 15 el
             locals()[f'act_bar_select_{subj_name}'] = args[l]       # [15] -> 16 el
+            locals()[f'avd_event_select_{subj_name}'] = args[m]     # [16] -> 17 el
 
-        idx = idx+3*nr_subjects # 15 - [16:24] -> 18el,...,24 el
+        idx = idx+4*nr_subjects # 16 - [17:25] -> 19el,...,25 el
         dev_density_dt, dev_iei_scale, dev_iei_fig, act_order, dev_order,  \
         dev_curr_sel, dev_curr_sel_store =  args[idx:idx+7]
 
         idx = idx+7
         for i, subj_name in enumerate(dct_acts.keys()):
             j, k = idx+i*nr_subjects, idx+i*nr_subjects+1
             locals()[f'act_curr_sel_store_{subj_name}'] = args[j]
             locals()[f'act_curr_sel_{subj_name}'] = args[k]
 
 
         ctx = dash.callback_context
 
-        if _get_trigger_value(ctx) is None:
+        if dash_get_trigger_value(ctx) is None:
             raise PreventUpdate
 
         # Catch block if no act-order or dev-order is initialized
         try:
             act_order = json.loads(act_order)
         except TypeError:
             act_order = None
@@ -557,39 +597,50 @@
             df_act_curr_sel = ActivityDict.read_json(act_curr_sel_store)
         except:
             df_act_curr_sel = ActivityDict()
 
         devs_usel_state = None
         # Create activity and device order if needed
         if _is_trigger(ctx, 'and_dev-order-trigger') or dev_order is None:
-            dev_order = device_order_by(curr_df_devs, dev_order_trigger)
+            dev_order = device_order_by(curr_df_devs, dev_order_trigger, dev2area)
         if _is_trigger(ctx, 'and_act-order-trigger') or act_order is None:
             act_order = activity_order_by(curr_dct_acts, act_order_trigger)
 
 
         # Create dataframes with user selection
         for subj in dct_acts.subjects():
             if (_is_trigger(ctx, f'acts_graph-transition-{subj}') \
                 or locals()[f'act_curr_sel_{subj}']  == f'acts_graph-transition-{subj}')\
                 and not reset_selection:
                 df_act_curr_sel[subj] = _sel_act_trans_sel(locals()[f'act_trans_select_{subj}'],
                                                     df_acts=curr_dct_acts[subj])
-                act_curr_sel = f'acts_graph-transition-{subj}'
+                locals()[f'act_curr_sel_{subj_name}'] = f'acts_graph-transition-{subj}'
 
             if (_is_trigger(ctx, f'acts_graph-boxplot-{subj}') \
                 or locals()[f'act_curr_sel_{subj}'] == f'acts_graph-boxplot-{subj}')\
                 and not reset_selection:
                 df_act_curr_sel[subj] = _sel_point_to_activities(locals()[f'act_boxplot_select_{subj}'])
-                act_curr_sel = f'acts_graph-boxplot-{subj}'
+                locals()[f'act_curr_sel_{subj_name}'] = f'acts_graph-boxplot-{subj}'
 
             if (_is_trigger(ctx, f'acts_graph-bar-{subj}') \
                 or locals()[f'act_curr_sel_{subj}'] == f'acts_graph-bar-{subj}')\
                 and not reset_selection:
                 df_act_curr_sel[subj] = _sel_act_bar(locals()[f'act_bar_select_{subj}'], df_acts=curr_dct_acts[subj])
-                act_curr_sel = f'acts_graph-bar-{subj}'
+                locals()[f'act_curr_sel_{subj_name}'] = f'acts_graph-bar-{subj}'
+
+            if _is_trigger(ctx, f'avd_graph-event-contingency-{subj}')\
+                and not reset_selection:
+                df_dev_curr_sel, df_act_curr_sel[subj] = _sel_avd_event_click(
+                    locals()[f'avd_event_select_{subj_name}'],
+                    curr_dct_acts[subj],
+                    curr_df_devs
+                )
+                locals()[f'act_curr_sel_{subj_name}'] = f'avd_graph-event-contingency-{subj}'
+                dev_curr_sel = f'avd_graph-event-contingency-{subj}'
+                devs_usel_state = False
 
         #if update_devices:
         if (_is_trigger(ctx, 'devs_graph-bar') or dev_curr_sel == 'devs_graph-bar')\
             and not reset_selection:
             df_dev_curr_sel = _sel_dev_bar(dev_bar_select, df_devs=curr_df_devs)
             dev_curr_sel = 'devs_graph-bar'
             devs_usel_state = False
@@ -615,33 +666,28 @@
 
         if (_is_trigger(ctx, 'devs_graph-density') or dev_curr_sel == 'devs_graph-density')\
             and not reset_selection:
             df_dev_curr_sel = _sel_dev_density(dev_density_select, curr_df_devs, dev_density_dt)
             dev_curr_sel = 'devs_graph-density'
             devs_usel_state = False
 
-        if _is_trigger(ctx, 'avd_graph-event-contingency') and not reset_selection:
-            df_dev_curr_sel, df_act_curr_sel = _sel_avd_event_click(avd_event_select,
-                                                               curr_dct_acts,
-                                                               curr_df_devs)
-            act_curr_sel = 'avd_graph-event-contingency'
-            dev_curr_sel = 'avd_graph-event-contingency'
-            devs_usel_state = False
+
 
         if reset_selection:
             df_act_curr_sel = None
             df_dev_curr_sel = None
-            act_curr_sel = ''
+            for subj in dct_acts.subjects():
+                locals()[f'act_curr_sel_{subj_name}'] = ''
             dev_curr_sel = ''
 
         states = (dev_type_trigger == 'state')
-        fig_and = activities_and_devices(dct_acts1, df_devs1, st=st, et=et,
+        fig_and = activities_and_devices(df_devs1, dct_acts1, st=st, et=et,
                                          states=states, act_order=act_order, dev_order=dev_order,
                                          df_acts_usel=df_act_curr_sel, df_devs_usel=df_dev_curr_sel,
-                                         devs_usel_state=devs_usel_state, height=plt_height_devs+50
+                                         devs_usel_state=devs_usel_state, height=plt_height_ands
                                          )
 
         # Determine reset selection button values
         if user_sel_activities or user_sel_devices:
             disable_reset = False
         else:
             disable_reset = True
@@ -681,33 +727,37 @@
         try:
             dev_curr_sel_store = df_dev_curr_sel.to_json(date_unit="ns"),
         except:
             dev_curr_sel_store = ''
 
         tmp = []
         for subj_name in dct_acts.subjects():
-            tmp.append(act_update)              # TODO update both activities 
-            tmp += [locals()[f'act_curr_sel_{subj_name}'],
-                    locals()[f'act_curr_sel_store_{subj_name}']]
+            tmp += [
+                act_update, # TODO update both individually
+                locals()[f'act_curr_sel_{subj_name}'],
+                locals()[f'act_curr_sel_store_{subj_name}'],
+                avd_update
+            ]
 
         ret_arguments = (
                fig_and, act_order, dev_order, disable_reset, 
-               avd_update, dev_update, dev_curr_sel, dev_curr_sel_store,
+               dev_update, dev_curr_sel, dev_curr_sel_store,
                *tmp
         )
         return ret_arguments
 
 
     @app.callback(
        output=[
             Output('devs_graph-iei', 'figure'),
             Output('devs_graph-density', 'figure'),
             Output('devs_graph-bar', 'figure'),
             Output('devs_graph-fraction', 'figure'),
             Output('devs_graph-boxplot', 'figure'),
+            Output('devs_graph-cc', 'figure'),
             Output('devs_order', 'data'),
         ],
         inputs=[
             Input('dev-trigger', 'children'),
             Input('range-slider', 'value'),
             Input('select-devices', 'value'),
             Input('tabs', 'active_tab'),
@@ -716,57 +766,69 @@
 
             Input('devs_iei-scale', 'value'),
             Input('devs_iei-per-device', 'on'),
             Input('devs_bp-scale', 'value'),
             Input('devs_bp-binary-state', 'value'),
             Input('devs_dens-slider', 'value'),
             Input('devs_dens-scale', 'value'),
+
+            Input('devs_cc-sel-fix', 'value'),
+            Input('devs_cc-sel-to', 'value'),
+            Input('devs_cc-lag-slider', 'value'),
+            Input('devs_cc-binsize-slider', 'value'),
         ],
         state=[
             State('devs_graph-iei', 'figure'),
             State('devs_graph-density', 'figure'),
             State('devs_graph-bar', 'figure'),
             State('devs_graph-fraction', 'figure'),
             State('devs_graph-boxplot', 'figure'),
+            State('devs_graph-cc', 'figure'),
             State('devs_order', 'data'),
         ]
     )
     def update_dev_tab(dev_trigger, rng, sel_devices,
                        active_tab, bar_scale, bar_order, iei_scale, iei_per_dev,
-                       bp_scale, bp_binary_state, dens_slider, dens_scale,
-                       fig_iei, fig_dens, fig_left, fig_frac, fig_bp, dev_order, 
+                       bp_scale, bp_binary_state, dens_slider, dens_scale, cc_fix, cc_to, cc_slider_lag, cc_slider_bin,
+                       fig_iei, fig_dens, fig_left, fig_frac, fig_bp, fig_cc, dev_order, 
                        ):
         ctx = dash.callback_context
-        if _get_trigger_value(ctx) is None or active_tab != 'tab-devs':
+        if dash_get_trigger_value(ctx) is None or active_tab != 'tab-devs':
             raise PreventUpdate
 
         try:
             dev_order = json.loads(dev_order)
         except TypeError:
             dev_order = None
 
         # Filter selected timeframe, activities and devices
         st = num_to_timestamp(rng[0], start_time=start_time, end_time=end_time)
         et = num_to_timestamp(rng[1], start_time=start_time, end_time=end_time)
         curr_df_devs = select_timespan(df_devs=df_devs, start_time=st, end_time=et,
                                        clip_activities=True)
         curr_df_devs = curr_df_devs[curr_df_devs[DEVICE].isin(sel_devices)]
-        from pyadlml.dataset.plotly.devices import bar_count
-        from pyadlml.dataset.plotly.devices import fraction as dev_fraction
+        from pyadlml.dataset.plot.plotly.devices import bar_count
+        from pyadlml.dataset.plot.plotly.devices import fraction as dev_fraction
 
         is_trigger_bar_drop = _is_trigger(ctx, 'devs_bar-drop')
         is_trigger_bar_scale = _is_trigger(ctx, 'devs_bar-scale')
         is_trigger_bp_scale = _is_trigger(ctx, 'devs_bp-scale')
         is_trigger_bp_state = _is_trigger(ctx, 'devs_bp-binary-state')
         is_trigger_iei_per_device = _is_trigger(ctx, 'devs_iei-per-device')
         is_trigger_iei_scale = _is_trigger(ctx, 'devs_iei-scale')
         is_trigger_dens_scale = _is_trigger(ctx, 'devs_dens-scale')
         is_trigger_dens_slider = _is_trigger(ctx, 'devs_dens-slider')
         is_trigger_sel_dev = _is_trigger(ctx, 'select-devices')
         is_trigger_dev_update = _is_trigger(ctx, 'dev-trigger') or is_trigger_sel_dev
+
+        is_trigger_cc_fix = _is_trigger(ctx, 'devs_cc-sel-fix')
+        is_trigger_cc_to = _is_trigger(ctx, 'devs_cc-sel-to')
+        is_trigger_cc_slider_lag = _is_trigger(ctx, 'devs_cc-lag-slider')
+        is_trigger_cc_slider_bin = _is_trigger(ctx, 'devs_cc-binsize-slider')
+
         order_update = _is_trigger(ctx, 'devs_bar-order')
         new_data_signal = (is_trigger_dev_update and dev_trigger == 'new_data')
 
         update_bar = is_trigger_bar_drop or order_update or is_trigger_bar_scale \
                     or new_data_signal
         update_bp = is_trigger_bp_scale or order_update or is_trigger_bp_state \
                     or (is_trigger_dev_update and dev_trigger == 'dens_clicked') \
@@ -774,14 +836,16 @@
                     or (is_trigger_dev_update and dev_trigger == 'reset_sel') \
                     or new_data_signal
         update_iei = is_trigger_iei_scale or is_trigger_iei_per_device \
                     or new_data_signal
         update_frac = order_update or new_data_signal
         update_density = is_trigger_dens_slider or order_update \
                     or new_data_signal or is_trigger_dens_scale
+        update_cc = is_trigger_cc_fix or is_trigger_cc_slider_lag or is_trigger_cc_to \
+                    or is_trigger_cc_slider_bin or new_data_signal
 
         if order_update or dev_order is None or is_trigger_dev_update or is_trigger_sel_dev:
             dev_order = device_order_by(curr_df_devs, rule=bar_order)
 
 
 
         def f_update_frac(fig_frac, cd_dev, order, uf):
@@ -799,172 +863,39 @@
                 return event_density(cd_dev, dt=DEV_DENS_SLIDER[dens_slider], show_colorbar=False,
                                      scale=scale, order=order, height=plt_height_devs)
             else:
                 return fig_dens
         def f_update_iei(u_iei, fig_iei, cd_dev, scale, per_dev):
             return dev_iei(cd_dev, scale=scale, per_device=per_dev, height=plt_height_devs) if u_iei else fig_iei
 
+        def f_update_cc(u_cc, fig_cc, fix, to, scale, binsize):
+            if u_cc:
+                return dev_cc(df_devs, height=plt_height_devs, fix=fix, to=to, max_lag=LAG_SLIDER[scale], binsize=BIN_SIZE_SLIDER[binsize])
+            else:
+                return fig_cc
+
+
         import dask
         figs = [
             dask.delayed(f_update_iei)(update_iei, fig_iei, curr_df_devs, iei_scale, iei_per_dev),
             dask.delayed(f_update_density)(update_density, fig_dens, curr_df_devs,
                                            dens_slider, dens_scale, dev_order),
             dask.delayed(f_update_bar)(update_bar, fig_left, curr_df_devs, bar_scale, dev_order),
             dask.delayed(f_update_frac)(fig_frac, curr_df_devs, dev_order, update_frac),
             dask.delayed(f_update_bp)(update_bp, fig_bp, curr_df_devs, dev_order, bp_scale,
                                       bp_binary_state),
+            dask.delayed(f_update_cc)(update_cc, fig_cc, cc_fix, cc_to, cc_slider_lag, cc_slider_bin),
         ]
         figs = dask.compute(figs)[0]
 
-        return figs[0], figs[1], figs[2], figs[3], figs[4], json.dumps(list(dev_order))
+        return figs[0], figs[1], figs[2], figs[3], figs[4], figs[5], json.dumps(list(dev_order))
 
 
     for subj_name in dct_acts.keys():
         _create_activity_tab_callback(app, subj_name, dct_acts[subj_name], start_time, end_time, plt_height_acts)
-
-
-    @app.callback(
-        output=[
-            Output('avd_graph-event-contingency', 'figure'),
-            Output('avd_graph-state-contingency', 'figure'),
-            Output('loading-output', 'children'),
-            Output('avd-update', 'children'),
-            Output('avd_state-contingency', 'data'),
-            Output('avd_event-contingency', 'data'),
-            Output('avd_activity-order', 'data'),
-            Output('avd_device-order', 'data'),
-        ],
-        inputs=[
-            Input('tabs', 'active_tab'),
-            Input('avd-trigger', 'children'),
-            Input('avd-update', 'children'),
-            Input('avd_state-scale', 'value'),
-            Input('avd_event-scale', 'value'),
-            Input('avd_act-order-trigger', 'value'),
-            Input('avd_dev-order-trigger', 'value'),
-        ],
-        state=[
-            State('range-slider', 'value'),
-            State('select-activities', 'value'),
-            State('select-devices', 'value'),
-            State('avd_state-contingency', 'data'),
-            State('avd_event-contingency', 'data'),
-            State('avd_activity-order', 'data'),
-            State('avd_device-order', 'data'),
-        ]
-    )
-    def update_acts_vs_devs_tab(active_tab, trigger, update,  state_scale,  event_scale,
-                                 act_order_trigger, dev_order_trigger,
-                                rng, sel_activities, sel_devices,
-                                state_cont, event_cont, act_order, dev_order,
-                                
-        ):
-        ctx = dash.callback_context
-
-        if _get_trigger_value(ctx) is None or active_tab != 'tab-acts_vs_devs':
-            raise PreventUpdate
-
-        try:
-            df_con_states = pd.read_json(state_cont)
-            df_con_states = df_con_states.astype('timedelta64[ns]')
-            df_con_events = pd.read_json(event_cont)
-        except ValueError:
-            df_con_states = None
-            df_con_events = None
-        except BaseException as err:
-            print(f"Unexpected {err=}, {type(err)=}")
-            raise
-
-        try:
-            act_order = json.loads(act_order)
-            dev_order = json.loads(dev_order)
-        except TypeError:
-            act_order = None
-            dev_order = None
-
-
-        # Filter selected timeframe, activities and devices
-        st = num_to_timestamp(rng[0], start_time=start_time, end_time=end_time)
-        et = num_to_timestamp(rng[1], start_time=start_time, end_time=end_time)
-        curr_df_devs, curr_df_acts = select_timespan(df_acts=dct_acts, df_devs=df_devs,
-                                                     start_time=st, end_time=et, clip_activities=True)
-        curr_df_acts = curr_df_acts[curr_df_acts[ACTIVITY].isin(sel_activities)]
-        curr_df_devs = curr_df_devs[curr_df_devs[DEVICE].isin(sel_devices)]
-        # TODO refactor, where is the y_label column coming from
-        curr_df_acts = curr_df_acts[[START_TIME, END_TIME, ACTIVITY]]
-
-        # If the activity-order is changed or the bar plot is changed
-        # and would change the order
-        is_data_update = _is_trigger(ctx, 'new_data')
-        is_trigger_act_order = _is_trigger(ctx, 'avd_act-order-trigger')
-        is_trigger_dev_order = _is_trigger(ctx, 'avd_dev-order-trigger')
-        order_update = is_trigger_act_order or is_trigger_dev_order\
-                       or act_order is None or dev_order is None
-
-        if order_update:
-            act_order = activity_order_by(curr_df_acts, act_order_trigger)
-            dev_order = device_order_by(curr_df_devs, dev_order_trigger)
-
-
-        # If data has changed the contingency tables have to be recomputed
-        if is_data_update or df_con_states is None or df_con_events is None:
-            # Recompute state contingency
-            df_con_states = contingency_table_states(curr_df_devs, curr_df_acts,
-                                                     distributed=True)
-            df_con_events = contingency_table_events(curr_df_devs, curr_df_acts)
-            update_data = True
-        else:
-            update_data = False
-
-        if active_tab != 'tab-acts_vs_devs' and is_data_update:
-            return dash.no_update, dash.no_update, dash.no_update, 'updated', \
-                   df_con_states.to_json(), df_con_events.to_json(), \
-                   json.dumps(list(act_order)), json.dumps(list(dev_order))
-        elif active_tab != 'tab-acts_vs_devs':
-            raise PreventUpdate
-
-        # Create figures
-        fig_adec = contingency_events(
-                    con_tab=df_con_events, scale=event_scale,
-                    act_order=act_order, dev_order=dev_order
-        )
-        fig_adsc = contingency_states(
-                    df_devs=curr_df_devs,   # for event order
-                    con_tab=df_con_states, scale=state_scale,
-                    act_order=act_order, dev_order=dev_order
-        )
-
-        if update_data:
-            state_dump, event_dump = df_con_states.to_json(date_unit="ns"), df_con_events.to_json()
-        else:
-            state_dump, event_dump = dash.no_update, dash.no_update
-
-        return fig_adec, fig_adsc, None, 'needs update', state_dump, event_dump, \
-               json.dumps(list(act_order)), json.dumps(list(dev_order))
-
-
-    #@app.callback(
-    #    Output('graph-acts_n_devs', 'figure'),
-    #    Input('and_dev-type', 'value'),
-    #    State('act_assist_path', 'value'),
-    #    State('subject_names', 'value'),
-    #)
-    #def update_acts_n_devs(dev_type_trigger, act_assist_path, subject_names):
-    #    data = load_act_assist(act_assist_path, subjects=subject_names)
-
-    #    df_acts = [data[f'df_activities_{sub}'] for sub in subject_names]
-    #    df_devs = data['df_devices']
-
-    #    states = (dev_type_trigger == 'state')
-    #    fig_and = activities_and_devices(df_acts[0], df_devs, states=states)
-    #    return fig_and
-
-
-
+        _create_acts_vs_devs_tab_callback(app, subj_name, dct_acts[subj_name], df_devs, start_time, end_time, dev2area)
 
 
 def _is_trigger(ctx, val):
     return ctx.triggered[0]['prop_id'].split('.')[0] == val
 
 
-def _get_trigger_value(ctx):
-    return ctx.triggered[0]['value']
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/plotly/dashboard/layout.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/plot/plotly/dashboard/layout.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 import dash
 import dash.dcc as dcc
+import numpy as np
 import dash_daq as daq
 import dash.html as html
 import pandas as pd
 from dash.exceptions import PreventUpdate
 import dash_bootstrap_components as dbc
-from pyadlml.dataset.plotly.activities import bar_count as act_bar_count, \
+from pyadlml.dataset.plot.plotly.activities import bar_count as act_bar_count, \
     boxplot_duration as act_boxplot_duration, density as act_density, \
     heatmap_transitions as act_heatmap_transitions
-from pyadlml.dataset.plotly.devices import bar_count as dev_bar_count, \
-    device_iei as dev_iei, fraction as dev_fraction, event_density, boxplot_state
-from pyadlml.dataset.plotly.acts_and_devs import *
+from pyadlml.dataset.plot.plotly.acts_and_devs import activity_vs_device_events_hist, event_correlogram
+from pyadlml.dataset.plot.plotly.devices import bar_count as dev_bar_count, \
+    device_iei as dev_iei, fraction as dev_fraction, event_density, boxplot_state, \
+    plotly_event_correlogram as dev_cc
+from pyadlml.dataset.plot.plotly.acts_and_devs import *
 from dash.dependencies import *
 from plotly.graph_objects import Figure
 
-from pyadlml.dataset import fetch_amsterdam, set_data_home
 from pyadlml.constants import TIME, START_TIME, END_TIME, ACTIVITY, DEVICE
-from pyadlml.dataset.plotly.util import ActivityDict
+from pyadlml.dataset._core.activities import ActivityDict
 from pyadlml.dataset.util import select_timespan, timestamp_to_num, num_to_timestamp
 
-DEV_DENS_SLIDER = {
-    0: '10s',
-    1: '30s',
-    2: '1min',
-    3: '5min',
-    4: '30min',
-    5: '1h',
-    6: '2h',
-    9: '6h',
-    10: '12h'
-}
+DEV_DENS_SLIDER = {i: e for i, e in enumerate(
+    ['10s', '30s', '1min', '5min', '30min', '1h', '2h', '6h', '12h']
+)}
+
+LAG_SLIDER = {i: e for i, e in enumerate(
+    ['10s', '30s', '1min', '2min', '5min', '30min', '1h', '2h']
+)}
+
+BIN_SIZE_SLIDER = {i: e for i, e in enumerate(
+    ['1s', '5s', '10s', '20s', '30s', '1min', '2min', '5min', '10min']
+)}
+
+
 def _np_dt_strftime(ts, format):
     return pd.to_datetime(ts).strftime(format)
 
 
 def _build_log_radio_buttons(id):
     return dcc.RadioItems(
         id=id,
@@ -57,53 +61,65 @@
         id=id,
         options=[{'label': i, 'value': i} for i in ['alphabetical', 'value', 'area']],
         value='value',
         labelStyle={'display': 'inline-block', 'marginTop': '5px'}
     )
 
 
-def _build_checklist(df_acts):
+def _build_choice_activity(df_acts, id, sel=None, multi=True):
     def create_option(name):
         return {'label': name, 'value': name}
     df_acts =  ActivityDict.wrap(df_acts)
     acts = df_acts.get_activity_union()
+    if sel is None:
+        act_sel = acts
+    elif isinstance(sel, str) and multi:
+        act_sel = np.array([sel])
+    else:
+        act_sel = sel
+
     options = [create_option(a) for a in acts]
     options = [create_option('other'), *options]
-    return dcc.Dropdown(id='select-activities',
-                        multi=True,
+    return dcc.Dropdown(id=id,
+                        multi=multi,
                         options=options,
-                        value=acts,
+                        value=act_sel,
                         clearable=False,
                         )
 
 
-def _build_choice_devices(df_devs):
+def _build_choice_devices(df_devs, id, sel=None, multi=True):
     def create_option(name):
         return {'label': name, 'value': name}
-
     devs = df_devs[DEVICE].unique()
+    if sel is None:
+        devs_sel = devs
+    elif isinstance(sel, str) and multi:
+        devs_sel = np.array([sel])
+    else:
+        devs_sel = sel
     options = [create_option(dev) for dev in devs]
-    return dcc.Dropdown(id='select-devices',
-                        options=options,
-                        multi=True,
-                        value=devs,
-                        clearable=False,
-                        )
+    return dcc.Dropdown(
+        id=id,
+        options=options,
+        multi=multi,
+        value=devs_sel,
+        clearable=False,
+    )
 
 
-def _build_range_slider(df_acts, df_devs, start_time, end_time, set_end_time):
+def _build_range_slider(start_time, end_time, set_start_time=None, set_end_time=None):
+    strf_time = '%d.%m.%Y'
     def create_mark(ts, format):
         return {'label': _np_dt_strftime(ts, format), 'style': {"transform": "rotate(45deg)"}}
 
-    marks = {0: create_mark(start_time, '%Y.%m.%d'),
-             1: create_mark(end_time, '%Y.%m.%d')}
+    marks = {0: create_mark(start_time, strf_time), 1: create_mark(end_time, strf_time)}
     #marks[0]['style']['margin'] = '10px 0 0 0'      # top right bottom left
     #marks[1]['style']['margin'] = '10px 15px 0 0'    # top right bottom left
 
-
     # Determine the marker frequency
     diff = end_time - start_time
     if diff < pd.Timedelta('8W'):       # 2 Month -> daily frequency
         # Dataset Amsterdam, Mitlab_1/2W, Mitlab_2/2W, Aras/4W, UCIA/2W
         # UCIA/3W
         rng = pd.date_range(start_time, end_time, freq='D')[1:-1]
     elif diff < pd.Timedelta('16W'):    # 4 Months
@@ -112,18 +128,27 @@
     elif diff < pd.Timedelta('32W'):    # 8 Months
         # Dataset Casas Aruba
         rng = pd.date_range(start_time, end_time, freq='W')[1:-1]
     else:
         rng = pd.date_range(start_time, end_time, freq='2W')[1:-1]
 
     for day in rng:
-        marks[timestamp_to_num(day, start_time, end_time)] = create_mark(day, '%m.%d')
-    set_end_time = timestamp_to_num(set_end_time, start_time, end_time)
+        marks[timestamp_to_num(day, start_time, end_time)] = create_mark(day, strf_time[:-3])
+    if set_end_time is not None:
+        set_end_time = timestamp_to_num(set_end_time, start_time, end_time)
+    else:
+        set_end_time = 1
+    
+    if set_start_time is not None:
+        set_start_time = timestamp_to_num(set_start_time, start_time, end_time)
+    else:
+        set_start_time = 0
+
     return dcc.RangeSlider(id='range-slider', min=0, max=1, step=0.001,
-                           value=[0, set_end_time], marks=marks)
+                           value=[set_start_time, set_end_time], marks=marks)
 
 
 def _build_plot_header(h_id, title, op_id):
     """ Creates a header for a graph """
     return dbc.Row(
         dbc.Col(children=[
                     html.H6(title, id=h_id),
@@ -134,83 +159,174 @@
 def _build_options_btn(op_id):
     """ Creates options button to link to graph options"""
     return dbc.Row(justify='end',
                    children=dbc.Col(width=3,
                                     children=dbc.Button('options', style={'marginTop': '-18px'},
                                                         id=op_id, color='link', size='sm')))
 
-def acts_vs_devs_layout(df_acts, df_devs, initialize=False, plot_height=False):
+def acts_vs_devs_layout(df_acts, act_id, df_devs, plot_height=False):
     """
 
+
+    Note
+    ----
+    Since the contingency table calculation may take very long the layout is initalized 
+    with placeholders and the real figures are computed later on demand
     """
-    # If the layout is initalized the space is filled with placeholder figures
-    # to reduce first loading time
-    if initialize:
-        fig_dummy = Figure()
-    else:
-        fig_adec = contingency_events(df_acts, df_devs, height=plot_height)
+    from copy import deepcopy
+    df_acts = deepcopy(df_acts)
+
+    activities = df_acts[ACTIVITY].unique()
+    devices = df_devs[DEVICE].unique()
+
+    cc_act_selected = np.random.choice(activities, 3).tolist()
+    cc_dev_selected = np.random.choice(devices, 4).tolist()
+
+    fig_cc = event_correlogram(
+        df_devs, 
+        df_acts, 
+        to=cc_dev_selected,
+        maxlag='1min', 
+        binsize='2s'
+    )
+
+    fig_avd_hist = activity_vs_device_events_hist(
+        df_devs,
+        df_acts,
+        device=cc_dev_selected[0],
+        activity=cc_act_selected[0],
+        normalize=True,
+        height=250,
+    )
 
     layout_acts_vs_devs = dbc.Container([
-        dcc.Store('avd_activity-order'),
-        dcc.Store('avd_device-order'),
-        dcc.Store('avd_state-contingency'),
-        dcc.Store('avd_event-contingency'),
-        html.Div(id="avd-trigger", style=dict(display="none")),
-        html.Div(id="dev-trigger", style=dict(display="none")),
-        html.Div(id="avd-update", style=dict(display="none")),
+        dcc.Store(f'avd_activity-order-{act_id}'),
+        dcc.Store(f'avd_device-order-{act_id}'),
+        dcc.Store(f'avd_state-contingency-{act_id}'),
+        dcc.Store(f'avd_event-contingency-{act_id}'),
+        html.Div(id=f"avd-trigger-{act_id}", style=dict(display="none")),
+        html.Div(id=f"avd-update-{act_id}", style=dict(display="none")),
         dbc.Row([
-            dcc.Graph(id='avd_graph-event-contingency',
+            dcc.Graph(id=f'avd_graph-event-contingency-{act_id}',
                       style=dict(height='100%',width='100%'),
-                      figure=fig_dummy,
+                      figure=Figure(),
                       config=dict(displaylogo=False, displayModeBar=True,
                                   responsive=False,
                                   modeBarButtonsToRemove=_buttons_to_use('resetScale2d'),
                      ),
             ),
-            _build_options_btn('clps-avd-event-button'),
-            dbc.Collapse(id='clps-avd-event',
+            _build_options_btn(f'clps-avd-event-button-{act_id}'),
+            dbc.Collapse(id=f'clps-avd-event-{act_id}',
                         style={'paddingLeft': '2rem',
                                 'paddingBottom': '2rem',
                     },
                 children=_option_grid(
                      labels=['Scale:', 'Activity order: ', 'Device order'],
                      values=[
                         _build_row_radio_button(
-                            rd_id='avd_event-scale',
+                            rd_id=f'avd_event-scale-{act_id}',
                             options=['linear', 'log'],
                             value='log'),
                         _build_row_radio_button(
-                            rd_id='avd_act-order-trigger',
+                            rd_id=f'avd_act-order-trigger-{act_id}',
                             options=['alphabetical', 'duration', 'count', 'area'],
                             value='alphabetical'),
                         _build_row_radio_button(
-                            rd_id='avd_dev-order-trigger',
+                            rd_id=f'avd_dev-order-trigger-{act_id}',
                             options=['alphabetical', 'count', 'area'],
                             value='alphabetical'),
                 ])),
-            ]),
-            dbc.Spinner(html.Div(id='loading-output')),
-            dcc.Graph(id='avd_graph-state-contingency',
+        ]),
+        dbc.Row([
+            dbc.Spinner(html.Div(id=f'loading-output-{act_id}')),
+            dcc.Graph(id=f'avd_graph-state-contingency-{act_id}',
                       style=dict(height='100%',width='100%'),
-                      figure=fig_dummy,
+                      figure=Figure(),
                       config=dict(displaylogo=False, displayModeBar=True)
             ),
-            _build_options_btn('clps-avd-state-button'),
-            dbc.Collapse(id='clps-avd-state',
+            _build_options_btn(f'clps-avd-state-button-{act_id}'),
+            dbc.Collapse(id=f'clps-avd-state-{act_id}',
              style={'paddingLeft': '2rem',
                     'paddingBottom': '2rem',
                     },
             children=_option_grid(
                  labels=['Scale:', 'Activity order: ', 'Device order'],
                  values=[
                     _build_row_radio_button(
-                        rd_id='avd_state-scale',
+                        rd_id=f'avd_state-scale-{act_id}',
                         options=['linear', 'log'],
                         value='log'),
             ])),
+        ]),
+        dbc.Row(
+            children=[
+                dbc.Col(width=12, children=[
+                            dbc.Row(dcc.Graph(id=f'avd_graph-cc-{act_id}',
+                                            figure=fig_cc,
+                                            style=dict(height='100%',width='100%'),
+                                            config=dict(displaylogo=False,
+                                                    displayModeBar=True,
+                                                    modeBarButtonsToRemove=_buttons_to_use('resetScale2d'),
+                                                )
+                            )),
+                            _build_options_btn(f'clps-avd-cc-button-{act_id}'),
+                            dbc.Collapse(id=f'clps-avd-cc-{act_id}',
+                                        style={'paddingLeft': '2rem',
+                                                'paddingRight': '2rem',
+                                                'paddingBottom': '2rem',
+                                                },
+                                        children=_option_grid(
+                                             labels=['Fix:', 'To:', 'Max lag:', 'Binsize:'],
+                                             lwidth=3, rwidth=9,
+                                             values=[
+                                                _build_choice_activity(df_acts, id=f'avd_cc-sel-fix-{act_id}', sel=cc_act_selected),
+                                                _build_choice_devices(df_devs, id=f'avd_cc-sel-to-{act_id}', sel=cc_dev_selected),
+                                                dcc.Slider(id=f'avd_cc-lag-slider-{act_id}', min=0, max=len(LAG_SLIDER), step=None, value=3,
+                                                        marks={i:{'label':LAG_SLIDER[i], 'style': {"transform": "rotate(45deg)"}} for i in range(0, len(LAG_SLIDER))}
+                                                ),
+                                                dcc.Slider(id=f'avd_cc-binsize-slider-{act_id}', min=0, max=len(BIN_SIZE_SLIDER), step=None, value=3,
+                                                        marks={i:{'label':BIN_SIZE_SLIDER[i], 'style': {"transform": "rotate(45deg)"}} for i in range(0, len(BIN_SIZE_SLIDER))}
+                                                ),
+                                            ]
+                                        )
+                            )
+                ]),
+        ]),
+        dbc.Row([
+                dbc.Col(width=12, children=[
+                            dbc.Row(dcc.Graph(id=f'avd_graph-hist-{act_id}',
+                                          figure=fig_avd_hist,
+                                          style=dict(height='100%',width='100%'),
+                                          config=dict(displaylogo=False,
+                                                displayModeBar=True,
+                                                modeBarButtonsToRemove=_buttons_to_use(
+                                                        'zoom2d', 'pan2d',  'lasso2d', 'resetScale2d'
+                                                ),
+                                          )
+                                ),
+                            ),
+                            _build_options_btn(f'clps-avd-hist-button-{act_id}'),
+                            dbc.Collapse(id=f'clps-avd-hist-{act_id}',
+                                        style={'paddingLeft': '2rem',
+                                            'paddingRight': '2rem',
+                                            'paddingBottom': '2rem',
+                                            },
+                                    children=_option_grid(
+                                            labels=['Normalize:', 'Device:', 'Activity: '],
+                                            lwidth=4, rwidth=8,
+                                            values=[
+                                            _build_row_radio_button(
+                                                    rd_id=f'avd_hist-normalize-{act_id}',
+                                                    options=['True', 'False'],
+                                                    value='True'),
+                                            _build_choice_devices(df_devs, id=f'avd_hist-sel-dev-{act_id}', sel=cc_dev_selected[0], multi=False),
+                                            _build_choice_activity(df_acts, id=f'avd_hist-sel-act-{act_id}', sel=cc_act_selected[0], multi=False),
+                            ]))
+                ]),
+        ])
     ])
     return layout_acts_vs_devs
 
 def _buttons_to_use(*use):
     """Returns the buttons to remove in order to get the buttons to use"""
     buttons = ['toImage', 'zoom2d', 'pan2d',  'select2d', 'lasso2d', 'zoomIn2d', 'zoomOut2d',
                'autoScale2d', 'resetScale2d',
@@ -218,29 +334,29 @@
     ]
     res = []
     for b in buttons:
         if b not in use:
             res.append(b)
     return res
 
-def acts_n_devs_layout(df_acts, df_devs, start_time, end_time, set_end_time, plot_height=350):
+def acts_n_devs_layout(df_devs, df_acts, start_time, end_time, set_end_time, plot_height=350):
     """
     TODO
 
     """
     if df_acts is None or df_devs is None:
         fig_and = Figure()
         time_slider = dcc.RangeSlider(id='range-slider', min=0, max=1, step=0.001, value=[0, 1])
         checklist_act = dcc.Dropdown(id='select-activities', multi=True, options=[], value=[], clearable=False)
         choice_device = dcc.Dropdown(id='select-devices', options=[], multi=True, value=[], clearable=False)
     else:
-        fig_and = activities_and_devices(df_acts, df_devs, st=start_time, et=set_end_time, height=plot_height)
-        time_slider = _build_range_slider(None, None, start_time, end_time, set_end_time)
-        checklist_act = _build_checklist(df_acts)
-        choice_device = _build_choice_devices(df_devs)
+        fig_and = activities_and_devices(df_devs, df_acts, st=start_time, et=set_end_time, height=plot_height)
+        time_slider = _build_range_slider(None, None, start_time, end_time, None, set_end_time)
+        checklist_act = _build_choice_activity(df_acts, id='select-activities')
+        choice_device = _build_choice_devices(df_devs, id='select-devices')
 
     return html.Div(children=[
 
                    dbc.Row(dbc.Col(
                             dcc.Graph(id='graph-acts_n_devs',
                                       style=dict(height='100%',width='100%'),
                                       figure=fig_and,
@@ -258,14 +374,15 @@
                             children=[dbc.ButtonGroup([
                                 dbc.Button('reset selection', id='and_reset_sel', disabled=True, color='link', size='sm'),
                                 dbc.Button('options',
                                    id='clps-acts-n-devs-button',
                                    color='link',
                                    size='sm',
                                    n_clicks=0),
+                                dbc.Button('cr', id='and_btn_copy_range', color='link', style={'fontsize': 10}),
                                 dcc.Clipboard(id='and_clipboard', style={'fontsize': 10}),
                             ]),
                             ])),
             dcc.Store(id='and_act-order'),
             dcc.Store(id='and_dev-order'),
             dbc.Collapse(id='clps-acts-n-devs',
                 children=[
@@ -382,35 +499,40 @@
                         ),
             html.Div(children=to_hide, style={'display': 'none'})
             ]
 
 
 def devices_layout(df_devs, initialize=False, plot_height=350):
 
+    cc_dev_selected = np.random.choice(df_devs[DEVICE].unique(), 4).tolist()
+
     if df_devs is not None and not df_devs.empty:
+        order = 'count'
         fig_bar_count = dev_bar_count(df_devs, height=plot_height)
-        fig_bp_state = boxplot_state(df_devs, height=plot_height)
+        fig_bp_state = boxplot_state(df_devs, height=plot_height, scale='log', order=order)
         fig_ev_density = event_density(df_dev=df_devs, show_colorbar=False,
-                                    height=plot_height
+                                    height=plot_height, order=order
                                     )
         fig_iei = dev_iei(df_devs, height=plot_height)
-        fig_fraction = dev_fraction(df_devs, height=plot_height)
+        fig_fraction = dev_fraction(df_devs, height=plot_height, order=order)
+
+        # Choose random first device for presentation
+        fig_cc = dev_cc(df_devs, height=plot_height, fix=cc_dev_selected, to=cc_dev_selected)
     else:
         fig_bar_count = Figure()
         fig_bp_state = Figure()
         fig_ev_density = Figure()
         fig_iei = Figure()
+        fig_cc = Figure()
         fig_fraction = Figure()
 
-
-
-
     layout_devices = dbc.Container([
         dcc.Store('devs_density-data'),
         dcc.Store('devs_order'),
+        html.Div(id="dev-trigger", style=dict(display="none")),
         html.Div(children='', id=f"dev-curr-sel", style=dict(display="none")),
         dcc.Store(id=f'dev-curr-sel-store'),
         dbc.Row([
             dbc.Col(width=6, children=[
                         dbc.Row(dcc.Graph(id='devs_graph-bar',
                                           figure=fig_bar_count,
                                           style=dict(height='100%',width='100%'),
@@ -459,15 +581,15 @@
                                     children=_option_grid(
                                          labels=['Plot:', 'Binary state:', ],
                                          lwidth=4, rwidth=8,
                                          values=[
                                             _build_row_radio_button(
                                                 rd_id='devs_bp-scale',
                                                 options=['linear', 'log'],
-                                                value='linear'),
+                                                value='log'),
                                             _build_row_radio_button(
                                                 rd_id='devs_bp-binary-state',
                                                 options=['off', 'on'],
                                                 value='on'),
                         ]))
             ]),
         ]),
@@ -494,71 +616,26 @@
                                                 'paddingRight': '2rem',
                                                 'paddingBottom': '2rem',
                                                 },
                                          children=_option_grid(
                                              labels=['Resolution', 'Scale'],
                                              lwidth=3, rwidth=9,
                                              values=[
-                                                dcc.Slider(id='devs_dens-slider', min=0, max=10, step=None, value=5,
-                                                           marks={
-                                                               0: {'label': DEV_DENS_SLIDER[0], 'style': {"transform": "rotate(45deg)"}},
-                                                               1: {'label': DEV_DENS_SLIDER[1], 'style': {"transform": "rotate(45deg)"}},
-                                                               2: {'label': DEV_DENS_SLIDER[2], 'style': {"transform": "rotate(45deg)"}},
-                                                               3: {'label': DEV_DENS_SLIDER[3], 'style': {"transform": "rotate(45deg)"}},
-                                                               4: {'label': DEV_DENS_SLIDER[4], 'style': {"transform": "rotate(45deg)"}},
-                                                               5: {'label': DEV_DENS_SLIDER[5], 'style': {"transform": "rotate(45deg)"}},
-                                                               6: {'label': DEV_DENS_SLIDER[6], 'style': {"transform": "rotate(45deg)"}},
-                                                               9: {'label': DEV_DENS_SLIDER[9], 'style': {"transform": "rotate(45deg)"}},
-                                                               10: {'label': DEV_DENS_SLIDER[10], 'style': {"transform": "rotate(45deg)"}},
-                                                           }
+                                                dcc.Slider(id='devs_dens-slider', min=0, max=len(DEV_DENS_SLIDER), step=None, value=5,
+                                                           marks={i:{'label':DEV_DENS_SLIDER[i], 'style': {"transform": "rotate(45deg)"}} for i in range(0, len(DEV_DENS_SLIDER))}
                                                 ),
                                                  _build_row_radio_button(
                                                       rd_id='devs_dens-scale',
                                                       options=['linear', 'log'],
                                                       value='linear'),
                                             ]
                                         )
                             )
 
                         ]),
-                        dbc.Tab(label='IEI', tab_id='devs_tab-iei',
-                            label_style={'fontSize': '12px', 'padding': '5px'},
-                            children=[
-                                dcc.Graph(id='devs_graph-iei',
-                                          figure=fig_iei,
-                                          style=dict(height='100%',width='100%'),
-                                          config=dict(displaylogo=False,
-                                                displayModeBar=True,
-                                                modeBarButtonsToRemove=_buttons_to_use(
-                                                        'zoom2d', 'pan2d',  'lasso2d', 'resetScale2d'
-                                                ),
-                                          )
-                                ),
-                                _build_options_btn('clps-dev-iei-button'),
-                                dbc.Collapse(id='clps-dev-iei',
-                                         style={'paddingLeft': '2rem',
-                                                'paddingRight': '2rem',
-                                                'paddingBottom': '2rem',
-                                                },
-                                        children=_option_grid(
-                                             labels=['Scale:', 'Per device:'],
-                                             lwidth=4, rwidth=8,
-                                             values=[
-                                                _build_row_radio_button(
-                                                      rd_id='devs_iei-scale',
-                                                      options=['linear', 'log'],
-                                                      value='linear'),
-                                                  daq.BooleanSwitch(
-                                                      id='devs_iei-per-device',
-                                                      on=False,
-                                                      persisted_props=[]
-                                                )]
-                                        )
-                            )
-                    ]),
                     ])
                 ]
             ),
             dbc.Col(width=5,
                     children=[
                         dbc.Row(style={'marginTop': '29px'},
                             children=dcc.Graph(id='devs_graph-fraction',
@@ -570,15 +647,82 @@
                                                     'zoom2d', 'pan2d', 'resetScale2d'
                                               ),
                                             )
                         )),
 
             ])
 
-        ])
+        ]),
+        dbc.Row(
+            children=[
+                dbc.Col(width=7, children=[
+                            dbc.Row(dcc.Graph(id='devs_graph-cc',
+                                            figure=fig_cc,
+                                            style=dict(height='100%',width='100%'),
+                                            config=dict(displaylogo=False,
+                                                    displayModeBar=True,
+                                                    modeBarButtonsToRemove=_buttons_to_use('resetScale2d'),
+                                                )
+                            )),
+                            _build_options_btn('clps-dev-cc-button'),
+                            dbc.Collapse(id='clps-dev-cc',
+                                        style={'paddingLeft': '2rem',
+                                                'paddingRight': '2rem',
+                                                'paddingBottom': '2rem',
+                                                },
+                                        children=_option_grid(
+                                             labels=['Fix:', 'To:', 'Max lag:', 'Binsize:'],
+                                             lwidth=3, rwidth=9,
+                                             values=[
+                                                _build_choice_devices(df_devs, id='devs_cc-sel-fix', sel=cc_dev_selected),
+                                                _build_choice_devices(df_devs, id='devs_cc-sel-to', sel=cc_dev_selected),
+                                                dcc.Slider(id='devs_cc-lag-slider', min=0, max=len(LAG_SLIDER), step=None, value=3,
+                                                        marks={i:{'label':LAG_SLIDER[i], 'style': {"transform": "rotate(45deg)"}} for i in range(0, len(LAG_SLIDER))}
+                                                ),
+                                                dcc.Slider(id='devs_cc-binsize-slider', min=0, max=len(BIN_SIZE_SLIDER), step=None, value=3,
+                                                        marks={i:{'label':BIN_SIZE_SLIDER[i], 'style': {"transform": "rotate(45deg)"}} for i in range(0, len(BIN_SIZE_SLIDER))}
+                                                ),
+                                            ]
+                                        )
+                            )
+                ]),
+                dbc.Col(width=5, children=[
+                            dbc.Row(dcc.Graph(id='devs_graph-iei',
+                                          figure=fig_iei,
+                                          style=dict(height='100%',width='100%'),
+                                          config=dict(displaylogo=False,
+                                                displayModeBar=True,
+                                                modeBarButtonsToRemove=_buttons_to_use(
+                                                        'zoom2d', 'pan2d',  'lasso2d', 'resetScale2d'
+                                                ),
+                                          )
+                                ),
+                            ),
+                            _build_options_btn('clps-dev-iei-button'),
+                            dbc.Collapse(id='clps-dev-iei',
+                                        style={'paddingLeft': '2rem',
+                                            'paddingRight': '2rem',
+                                            'paddingBottom': '2rem',
+                                            },
+                                    children=_option_grid(
+                                            labels=['Scale:', 'Per device:'],
+                                            lwidth=4, rwidth=8,
+                                            values=[
+                                            _build_row_radio_button(
+                                                    rd_id='devs_iei-scale',
+                                                    options=['linear', 'log'],
+                                                    value='log'),
+                                                daq.BooleanSwitch(
+                                                    id='devs_iei-per-device',
+                                                    on=False,
+                                                    persisted_props=[]
+                            )]))
+                ]),
+                
+            ])
 
     ]),
 
     return layout_devices
 
 def _option_grid(labels, values,lwidth=2, rwidth=10):
     """ generates sth. like this:
@@ -601,15 +745,15 @@
     if df_acts is not None and not df_acts.empty:
         fig_bar_count = act_bar_count(df_acts, height=plot_height)
         fig_density = act_density(df_acts, height=plot_height)
         try:
             fig_transition = act_heatmap_transitions(df_acts, height=plot_height)
         except:
             fig_transition = Figure()
-        fig_duration = act_boxplot_duration(df_acts, height=plot_height)
+        fig_duration = act_boxplot_duration(df_acts, height=plot_height, scale='log')
     else:
         fig_bar_count = Figure()
         fig_density = Figure()
         fig_transition = Figure()
         fig_duration = Figure()
 
     layout_activities = dbc.Container([
@@ -681,15 +825,15 @@
                                             dcc.Dropdown(id=f'acts_bp-drop-{act_id}', value='bp', options=[
                                                                               {'label': 'boxplot', 'value': 'bp'},
                                                                               {'label': 'voilin', 'value': 'vp'}]
                                             ),
                                             _build_row_radio_button(
                                                 rd_id=f'acts_bp-scale-{act_id}',
                                                 options=['linear', 'log'],
-                                                value='linear'),
+                                                value='log'),
                                          ])
                         ),
             ]),
         ]),
         dbc.Row([
             dbc.Col(width=6,
                     children=[
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/stats/__init__.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/stats/activities.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/stats/activities.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pandas as pd
 import numpy as np
 from pyadlml.constants import START_TIME, END_TIME, ACTIVITY, TIME
-from pyadlml.dataset._core.activities import add_other_activity
-from pyadlml.dataset.plotly.util import ActivityDict
+from pyadlml.dataset._core.activities import add_other_activity, ActivityDict
 from pyadlml.dataset.stats.util import df_density_binned
 from datetime import timezone, datetime
 
 
 def activity_order_by_duration(df_acts: pd.DataFrame) -> list:
     """ Computes a list of activities ordered by the cumulated time per activity
 
@@ -18,17 +17,18 @@
     Returns
     -------
     list
         An ordered list where the first is the most prominent activity, followed by the second most prominent ...
     """
     if isinstance(df_acts, pd.DataFrame):
         dct_acts = ActivityDict.wrap(df_acts)
-    else: 
+    else:
         dct_acts = df_acts
-    dfs = [activity_duration(df).set_index(ACTIVITY) for df in dct_acts.values()]
+    dfs = [activity_duration(df).set_index(ACTIVITY)
+           for df in dct_acts.values()]
 
     df = pd.concat(dfs, axis=1).fillna(0)
     df['sum'] = df.sum(axis=1)
     df = df.sort_values(by='sum', ascending=False)
     return df.index.to_list()
 
 
@@ -43,17 +43,18 @@
     Returns
     -------
     list
         An ordered list where the first is the most prominent activity, followed by the second most prominent ...
     """
     if isinstance(df_acts, pd.DataFrame):
         dct_acts = ActivityDict.wrap(df_acts)
-    else: 
+    else:
         dct_acts = df_acts
-    dfs = [activities_count(df).set_index(ACTIVITY) for df in dct_acts.values()]
+    dfs = [activities_count(df).set_index(ACTIVITY)
+           for df in dct_acts.values()]
 
     df = pd.concat(dfs, axis=1).fillna(0)
     df['sum'] = df.sum(axis=1)
     df = df.sort_values(by='sum', ascending=False)
     return df.index.to_list()
 
 
@@ -71,14 +72,15 @@
     if freq == 'seconds' or freq == 's':
         return lambda x: x.total_seconds()
     elif freq == 'minutes' or freq == 'm':
         return lambda x: x.total_seconds()/60
     else:
         return lambda x: x.total_seconds()/3600
 
+
 def coverage(df_activities, df_devices, datapoints=False):
     """ Computes the activity coverage for the devices.
 
     Parameters
     ----------
     df_activities : pd.DataFrame
         Todo
@@ -88,80 +90,85 @@
 
     Returns
     -------
     cov : float
         The percentage covered by activities
     """
     if datapoints:
-        from pyadlml.dataset._core._dataset import label_data
+        from pyadlml.dataset._core.acts_and_devs import label_data2
         df_acts = df_activities.copy()
-        lbl_devs = label_data(df_devices, df_acts)
+        lbl_devs = label_data2(df_devices, df_acts)
         nr_nans = lbl_devs[ACTIVITY].isna().sum()
         return 1 - nr_nans/len(lbl_devs)
     else:
-        durations = activity_duration(df_activities, idle=True)
+        durations = activity_duration(
+            df_activities, other=True).set_index('activity')
         total = durations['minutes'].sum()
-        amount_idle = durations.loc[(durations[ACTIVITY] == 'idle'), 'minutes'].values[0]
-        return 1 - amount_idle/total
+        amount_other = durations.at['other', 'minutes']
+        return 1 - amount_other/total
 
-def activities_duration_dist(df_acts, lst_acts=None, freq='minutes', idle=False):
+
+def activities_duration_dist(df_acts, lst_acts=None, freq='minutes', other=False):
     """ Computes the activity distribution.
 
     Parameters
     ----------
     df_acts : pd.DataFrame
         All recorded activities from a dataset. Fore more information refer to the
         :ref:`user guide<activity_dataframe>`.
     lst_acts : list, optional
         A list of activities that are included in the statistic. The list can be a
         subset of the recorded activities or contain activities that are not recorded.
     freq : str, optional
         Defaults to 1000.
         Can be one of 'minutes', 'seconds', 'hours', 'm', 'h', 's'.
-    idle : bool, default=False
-        Whether to include the idle activity. More in user guide
+    other : bool, default=False
+        Whether to include the other activity. More in user guide
 
     Returns
     -------
     df : pd.DataFrame
         First column activity names second column total time in frequency.
 
     Example
     -------
     .. code python::
         TODO
 
     """
     df = df_acts.copy()
-    if idle:
+    if other:
         df = add_other_activity(df)
 
     # integrate the time difference for activities
     diff = 'total_time'
     df[diff] = df[END_TIME] - df[START_TIME]
     df = df[[ACTIVITY, diff]]
 
     # if no data is logged for a certain activity append 0.0 duration value
-    #if lst_acts is not None:
+    # if lst_acts is not None:
     #    for activity in set(lst_acts).difference(set(list(df[ACTIVITY]))):
     #        df = df.append(pd.DataFrame(
     #            data=[[activity, pd.Timedelta('0ns')]],
     #            columns=df.columns, index=[len(df)]))
 
     df[freq] = df[diff].apply(_get_freq_func(freq))
     return df.sort_values(by=ACTIVITY)
 
-def activity_duration(df_acts, time_unit='minutes', normalize=False, idle=False):
+
+def activity_duration(df_acts, unit='minutes', stat='sum', normalize=False, other=False):
     """ Compute how much time an inhabitant spent performing an activity
 
     Parameters
     ----------
     df_acts : pd.DataFrame
         All recorded activities from a dataset. Fore more information refer to the
         :ref:`user guide<activity_dataframe>`.
+    stat : str one of ['sum', 'mean', 'median']
+        The summary statistic to compute
     time_unit : str of {'minutes', 'seconds', 'hours', 'm', 's', 'h'}
         The unit of time the durations are returned in.
     normalize : bool, default=False
         If set to *true* rather than returning the durations in a specified
         time unit, the fraction of the durations is returned.
 
     Returns
@@ -180,27 +187,38 @@
     2        leave house  22169.883333
     3  prepare Breakfast     63.500000
     4     prepare Dinner    338.899967
     5        take shower    209.566667
     6         use toilet    195.249567
 
     """
-    df = activities_duration_dist(df_acts, freq=time_unit, idle=idle)
+    assert stat in ['sum', 'mean', 'median', 'std']
+    df = activities_duration_dist(df_acts, freq=unit, other=other)
     if df.empty:
         raise ValueError("no activity was recorded")
-    df = df.groupby(ACTIVITY).sum().reset_index()
-    df.columns = [ACTIVITY, time_unit]
+    grouped = df.groupby(ACTIVITY)
+    if stat == 'sum':
+        df = grouped.sum(numeric_only=True)
+    elif stat == 'mean':
+        df = grouped.mean(numeric_only=True)
+    elif stat == 'std':
+        df = grouped.std(numeric_only=True)
+    else:
+        df = grouped.median(numeric_only=True)
+    df = df.reset_index()
+    df.columns = [ACTIVITY, unit]
 
     # compute fractions of activities to each other
     if normalize:
-        normalize = df[time_unit].sum()
-        df[time_unit] = df[time_unit].apply(lambda x: x / normalize)
+        normalize = df[unit].sum()
+        df[unit] = df[unit].apply(lambda x: x / normalize)
 
     return df.sort_values(by=ACTIVITY)
 
+
 def activities_count(df_acts: pd.DataFrame) -> pd.DataFrame:
     """ Computes how many times a certain activity occurs within the dataset.
 
     Parameters
     ----------
     df_acts : pd.DataFrame
         All recorded activities from a dataset. Fore more information refer to the
@@ -230,23 +248,23 @@
 
     # Count the occurences of the activity
     df = df.groupby(ACTIVITY).count().reset_index()
     df = df.drop(columns=[END_TIME])
     df.columns = [ACTIVITY, res_col_name]
 
     # correct for missing activities
-    #if lst_acts is not None:
+    # if lst_acts is not None:
     #    diff = set(lst_acts).difference(set(list(df[ACTIVITY])))
     #    for activity in diff:
     #        df = df.append(pd.DataFrame(data=[[activity, 0.0]], columns=df.columns, index=[len(df) + 1]))
 
     return df.sort_values(by=ACTIVITY)
 
 
-def activities_transitions(df_acts):
+def activities_transitions(df_acts, other=False):
     """  Compute a transition matrix that displays how often one
     activity was followed by another.
 
     Parameters
     ----------
     df_acts : pd.DataFrame
         All recorded activities from a dataset. Fore more information refer to the
@@ -275,14 +293,18 @@
         prepare Breakfast          1          0  ...           8
         prepare Dinner             7          0  ...           4
         take shower                0          0  ...           1
         use toilet                 5         46  ...          18
     """
 
     df = df_acts.copy()
+
+    if other:
+        df = add_other_activity(df)
+
     df = df[[ACTIVITY]]
     df['act_after'] = df[ACTIVITY].shift(-1)
     df = pd.crosstab(df[ACTIVITY], df['act_after'])
 
     cols = list(df.columns)
     rows = list(df.index)
     for r in rows:
@@ -295,15 +317,16 @@
         row_diff = set(df.columns).difference(set(list(df.index)))
         col_diff = set(df.index).difference(set(list(df.columns)))
         for activity in col_diff:
             # when columns are missing
             df[activity] = 0
         for activity in row_diff:
             # when rows are missing
-            df = df.append(pd.DataFrame(data=0.0, columns=df.columns, index=[activity]))
+            df = df.append(pd.DataFrame(
+                data=0.0, columns=df.columns, index=[activity]))
 
     # sort activities alphabetically
     df = df.sort_index(axis=0)
     df = df.sort_index(axis=1)
 
     return df
 
@@ -348,35 +371,35 @@
     #        solves the problem that beyond interval limits there can't be
     #        any sample
     # Todo include range for day or week
 
     df = df_acts.copy()
     activities = df_acts[ACTIVITY].unique()
 
-    #res = pd.DataFrame(index=range(n), columns=activities, data=0)
-    res = pd.DataFrame(index=range(len(activities)*n), columns=[TIME, ACTIVITY], dtype=object)
+    # res = pd.DataFrame(index=range(n), columns=activities, data=0)
+    res = pd.DataFrame(index=range(len(activities)*n),
+                       columns=[TIME, ACTIVITY], dtype=object)
 
     # sample for each column separately
     for i, activity in enumerate(activities):
-        series = _sample_ts(df.loc[df[ACTIVITY] == activity, [START_TIME, END_TIME]], n)
+        series = _sample_ts(
+            df.loc[df[ACTIVITY] == activity, [START_TIME, END_TIME]], n)
         res.loc[n*i:n*i+n-1, TIME] = series.values
         res.loc[n*i:n*i+n-1, ACTIVITY] = activity
 
     if relative and dt is None:
         res[TIME] = pd.to_datetime('1/1/2000 - ' + res[TIME])
         res[TIME] = res[TIME] - np.datetime64("2000-01-01 00:00:00")
         res[TIME] = res[TIME] / np.timedelta64(1, 's')
 
     if dt is not None:
         res[TIME] = pd.to_datetime('1/1/2000 - ' + res[TIME])
         res = df_density_binned(res, column_str=ACTIVITY, dt=dt)
 
     return res
-    
-
 
 
 def _sample_ts(df, n):
     """ Samples one column of activities. First chooses one activity at random and then samples a timepoint from
         within that activities interval
 
     Parameters
@@ -400,15 +423,15 @@
 
         # convert to unix timestamp
         unx_min = interval.start_time.replace(tzinfo=timezone.utc).timestamp()
         unx_max = interval.end_time.replace(tzinfo=timezone.utc).timestamp()
 
         # sample uniform and convert back to timestamp
         try:
-            unx_sample = np.random.randint(unx_min, unx_max)
+            unx_sample = np.random.uniform(low=unx_min, high=unx_max)
         except ValueError:
             if unx_min == unx_max:
                 unx_sample = unx_min
             else:
                 raise ValueError('Sampling interval went wrong')
         xs[i] = datetime.utcfromtimestamp(unx_sample).strftime('%H:%M:%S')
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/stats/acts_and_devs.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/stats/acts_and_devs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import pandas as pd
 import numpy as np
-from pyadlml.dataset._core._dataset import label_data
+from pyadlml.dataset._core.acts_and_devs import label_data
 from pyadlml.dataset._core.devices import create_device_info_dict
+from pyadlml.dataset.stats.activities import _get_freq_func
 from pyadlml.util import get_npartitions, get_parallel
 from pyadlml.constants import START_TIME, END_TIME, TIME, DEVICE, VALUE, ACTIVITY, CAT, NUM, BOOL
 from pyadlml.dataset.util import infer_dtypes, categorical_2_binary
-from pyadlml.dataset._representations.raw import create_raw
+import dask.dataframe as dd
+from pyadlml.dataset._representations.state import create_state
 #import __logger__
 
 
-def cross_correlogram(df_devices, df_activities, maxlag, binsize,idle=False):
+def cross_correlogram(df_devices, df_activities, maxlag, binsize, other=False):
     """
     Computes the cross-correlogram between activity beginning and ending and device events.
 
     Parameters
     ----------
     df_devices : pd.DataFrame
         All recorded devices from a dataset. For more information refer to
         :ref:`user guide<device_dataframe>`.
     df_activities : pd.DataFrame
         All recorded activities from a dataset. Fore more information refer to the
         :ref:`user guide<activity_dataframe>`.
-    idle : bool, default=False
+    other : bool, default=False
         Determines whether gaps between activities should be assigned
-        the activity *idle* or be ignored.
+        the activity *other* or be ignored.
 
     Returns
     -------
     pd.DataFrame
 
     """
     ET = 'event_times'
@@ -80,31 +82,33 @@
 
         split = int(np.floor(n_bins/2))
         ccg[i, j, :] = np.concatenate([result_right[:split], [0], result_left[split+1:]])
 
     return ccg, bins
 
 
-def contingency_table_events(df_devices, df_activities, per_state=False, idle=False):
+def contingency_table_events(df_devices, df_activities, per_state=False, other=False, n_jobs=1):
     """
     Compute the amount of device triggers occuring during the different activities.
 
     Parameters
     ----------
     df_devices : pd.DataFrame
         All recorded devices from a dataset. For more information refer to
         :ref:`user guide<device_dataframe>`.
     df_activities : pd.DataFrame
         All recorded activities from a dataset. Fore more information refer to the
         :ref:`user guide<activity_dataframe>`.
     per_state : bool, default=False
         Determines whether events are plotted
-    idle : bool, default=False
+    other : bool, default=False
         Determines whether gaps between activities should be assigned
-        the activity *idle* or be ignored.
+        the activity *other* or be ignored.
+    n_jobs : int, default=1
+        The numberof parallel threads to start for computing the statistics
 
     Examples
     --------
     >>> from pyadlml.stats import contingency_events
     >>> contingency_events(data.df_devices, data.df_activities)
     activity            get drink  go to bed  ...  use toilet
     device
@@ -121,15 +125,15 @@
     ON = 'on'
     OFF = 'off'
 
     # Save original devices and activities
     devs = df_devices[DEVICE].unique()
     acts = df_activities[ACTIVITY].unique()
 
-    df = label_data(df_devices, df_activities, idle=idle)
+    df = label_data(df_devices, df_activities, other=other, n_jobs=n_jobs)
     if not per_state:
         df[VALUE] = 1
         df = pd.pivot_table(df, columns=ACTIVITY, index=DEVICE, values=VALUE, aggfunc=len, fill_value=0)\
 
         # Add activities where no event occurs to table
         if len(df.columns) != len(acts):
             for act in set(acts).difference(set(df.columns)):
@@ -196,30 +200,30 @@
     assert i1.overlaps(i2)
     mi = max([i1.left, i2.left])
     ma = min([i1.right, i2.right])
     #return pd.Interval(mi, ma)
     return ma-mi
 
 
-def contingency_table_states_old(df_devs, df_acts, idle=False, distributed=False):
+def contingency_table_states_old(df_devs, df_acts, other=False, distributed=False):
     """
     Compute the time a device is "on" or "off" respectively
     during the different activities.
 
     Parameters
     ----------
     df_devs : pd.DataFrame
         All recorded devices from a dataset. For more information refer to
         :ref:`user guide<device_dataframe>`.
     df_acts : pd.DataFrame
         All recorded activities from a dataset. Fore more information refer to the
         :ref:`user guide<activity_dataframe>`.
-    idle : bool
+    other : bool
         Determines whether gaps between activities should be assigned
-        the activity *idle* or be ignored.
+        the activity *other* or be ignored.
 
     Examples
     --------
     >>> from pyadlml.stats import contingency_duration
     >>> contingency_duration(data.df_devs, data.df_activities)
     activity                     get drink ...             use toilet
     Hall-Bedroom door Off  0 days 00:01:54 ... 0 days 00:12:24.990000
@@ -299,15 +303,15 @@
     dtypes = infer_dtypes(df_devs)
 
     # drop numerical devices
     df_devs = df_devs.loc[~df_devs[DEVICE].isin(dtypes[NUM]), :]
 
     dataset_info = create_device_info_dict(df_devs)
     df_devs = df_devs.sort_values(by=TIME)
-    raw = create_raw(df_devs, dataset_info)
+    raw = create_state(df_devs, dataset_info)
 
     # raw representation one-hot-encode categorical devices and create on-boolean and off-boolean devices
     raw = pd.get_dummies(data=raw, columns=dtypes[CAT], prefix_sep=SEP, dtype=bool)
 
     for dev in dtypes[BOOL]:
         raw[dev + SEP + OFF_praefix] = ~raw[dev]
         raw = raw.rename(columns={dev: dev + SEP + ON_praefix})
@@ -340,15 +344,15 @@
         df = ddf.compute()
 
     # Check the case when an activity does not match any device states
     return df.T
 
 
 
-def contingency_table_states(df_devs, df_acts, other=False, distributed=False):
+def contingency_table_states(df_devs, df_acts, other=False, n_jobs=1):
     """
     Compute the time a device is "on" or "off" respectively
     during the different activities.
 
     Parameters
     ----------
     df_devs : pd.DataFrame
@@ -377,83 +381,236 @@
     df : pd.DataFrame
     """
     TD = 'td'
     ON_praefix = 'on'
     OFF_praefix = 'off'
     SEP = ':'
 
-    df_devs = df_devs.copy()
-    df_acts = df_acts.copy()
+    df_devs = df_devs.copy().reset_index(drop=True).sort_values(by=TIME)
+    df_acts = df_acts.copy().reset_index(drop=True).sort_values(by=START_TIME)
     df_acts[TD] = df_acts[END_TIME] - df_acts[START_TIME]
 
     dtypes = infer_dtypes(df_devs)
-    start_time = df_acts.iat[0, 0]
-    end_time = df_acts.iat[-1, 1]
+    start_time = df_acts.iat[0, 0] - pd.Timedelta('1s')
+    end_time = df_acts.iat[-1, 1] + pd.Timedelta('1s')
     from pyadlml.dataset._core.devices import device_events_to_states
     df_devs = device_events_to_states(df_devs, extrapolate_states=True,
-                                      st=start_time, et=end_time)
+                                      start_time=start_time, end_time=end_time)
     bool_mask_true = (df_devs[DEVICE].isin(dtypes[BOOL])) & (df_devs[VALUE] == True)
     bool_mask_false = (df_devs[DEVICE].isin(dtypes[BOOL])) & (df_devs[VALUE] == False)
     mask_cat = (df_devs[DEVICE].isin(dtypes[CAT]))
 
     df_devs.loc[bool_mask_true, DEVICE] = df_devs.loc[bool_mask_true, DEVICE] + SEP + ON_praefix
     df_devs.loc[bool_mask_false, DEVICE] = df_devs.loc[bool_mask_false, DEVICE] + SEP + OFF_praefix
     df_devs.loc[mask_cat, DEVICE] = df_devs.loc[mask_cat, DEVICE] + SEP + df_devs.loc[mask_cat, VALUE]
     df = df_devs.drop(columns=VALUE)
 
     for act in df_acts[ACTIVITY].unique():
         df[act] = pd.Timedelta('0ns')
 
     def func(row, df_acts):
-        mask_inside = (row.start_time < df_acts[START_TIME]) & (df_acts[END_TIME] < row.end_time)
+        assert row.end_time - row.start_time > pd.Timedelta('0ns')
+        mask_inside = (row.start_time <= df_acts[START_TIME]) & (df_acts[END_TIME] <= row.end_time)
         mask_right_ov = (df_acts[START_TIME] < row.end_time) & (row.end_time < df_acts[END_TIME])\
                       & (row.start_time < df_acts[START_TIME])
         mask_left_ov = (df_acts[START_TIME] < row.start_time) & (row.start_time < df_acts[END_TIME])\
                       & (df_acts[END_TIME] < row.end_time)
-        mask_total_ov = (df_acts[START_TIME] < row.start_time) & (row.end_time < df_acts[END_TIME])
+        mask_total_ov = (df_acts[START_TIME] <= row.start_time) & (row.end_time <= df_acts[END_TIME])
 
+        overlap_ins = df_acts[mask_inside]
+        overlap_left = df_acts[mask_left_ov]
+        overlap_right = df_acts[mask_right_ov]
         overlap_total = df_acts[mask_total_ov]
+
         if not overlap_total.empty:
+            assert overlap_ins.empty and overlap_left.empty and overlap_right.empty
             assert len(overlap_total) == 1, 'trouble double dup dup.'
             # One activity overlaps the whole state
             ol = overlap_total.iloc[0]
             row[ol[ACTIVITY]] = row.end_time - row.start_time
             return row
 
-        overlap_ins = df_acts[mask_inside]
-        overlap_left = df_acts[mask_left_ov]
-        overlap_right = df_acts[mask_right_ov]
-
-        if overlap_ins.empty and overlap_right.empty and overlap_right.empty:
+        if overlap_ins.empty and overlap_right.empty and overlap_left.empty:
             # No matching activity return row
             return row
 
-        skip_acts = []
         if not overlap_left.empty:
+            assert len(overlap_left) == 1, 'trouble double dup dup.'
             ol = overlap_left.iloc[0]
-            row[ol[ACTIVITY]] = ol[END_TIME] - row.start_time
-            skip_acts.append(ol[ACTIVITY])
+            row[ol[ACTIVITY]] += ol[END_TIME] - row.start_time
 
         if not overlap_right.empty:
+            assert len(overlap_right) == 1, 'trouble double dup dup.'
             ol = overlap_right.iloc[0]
-            row[ol[ACTIVITY]] = row.end_time - ol[START_TIME]
-            skip_acts.append(ol[ACTIVITY])
+            row[ol[ACTIVITY]] += row.end_time - ol[START_TIME]
 
         assert len(overlap_right) < 2 and len(overlap_left) < 2, 'Trouble trouble double dup.'
 
-        if overlap_ins.empty:
-            return row
-        else:
+        if not overlap_ins.empty:
             ins_acts = overlap_ins[ACTIVITY].unique()
             state_agg = overlap_ins[[TD, ACTIVITY]].groupby(by=[ACTIVITY])[TD].sum()
             for act in ins_acts:
-                row.at[act] = state_agg[act]
-            return row
+                row.at[act] += state_agg[act]
+
+        return row
+
+    if n_jobs > 1:
+        import dask.dataframe as dd
+        ddf = dd.from_pandas(df, npartitions=n_jobs)
+
+        meta = {**{START_TIME: 'datetime64[ns]', END_TIME: 'timedelta64[ns]', DEVICE: 'object'}, 
+                **{name: 'object' for name in df.columns[3:]}}
+
+        ddf = ddf.map_partitions(lambda dff: dff.apply(func, args=[df_acts], axis=1), meta=meta)
+
+        ddf = ddf.drop(columns=[START_TIME, END_TIME])
+        ddf = ddf.groupby(DEVICE, observed=True).sum()
+
+        # Visualize as graph
+        #ddf.visualize(filename='test.svg')
+        df = ddf.compute()
 
-    if distributed:
-        df = df.parallel_apply(func, args=[df_acts], axis=1)
     else:
         df = df.apply(func, args=[df_acts], axis=1)
-    df = df.drop(columns=[START_TIME, END_TIME])
-    df = df.groupby(DEVICE).sum()
+        df = df.drop(columns=[START_TIME, END_TIME])
+        df = df.groupby(DEVICE, observed=True).sum()
+
+    # Add row for categories for binary devices that are not present 
+    devices_in_index = df.index.values
+    zero_line = {col: pd.Timedelta('0ns') for col in df.columns}
+    for dev in dtypes['boolean']:
+        dev_on_name = dev + SEP + ON_praefix
+        dev_off_name = dev + SEP + OFF_praefix
+        if dev_on_name not in devices_in_index:
+           df = pd.concat([df, pd.Series(name=dev_on_name, data=zero_line).to_frame().T], axis=0)
+        if dev_off_name not in devices_in_index:
+           df = pd.concat([df, pd.Series(name=dev_off_name, data=zero_line).to_frame().T], axis=0)
+    
+    return df
+
+
+def mutual_info_states(df_devs, df_acts):
+    raise NotImplementedError
+
+
+def mutual_info_events(df_devs: pd.DataFrame, df_acts: pd.DataFrame, kind='pointwise', other=True) -> pd.DataFrame:
+    """ Compute the mututal information between events and activities. How much does the 
+        occurence, pattern of events from a certain device reduce the uncertainty in observing 
+        some activity. This method provides
+
+        - pointwise mutual information measures the co-occurence of events during activities 
+          :math:`I(X,Y) = \log_2 \\frac{p(x,y)}{p(x)p(y)}` where :math:`p(x) = \\frac{o_x}{N}` 
+          with :math:`o_x` being the event number of device :math:`x` and :math:`N` the total 
+          number of events :math:`o_y` being the number of events labeled as an activity :math:`y` 
+          and finally :math:`p(x,y) = \frac{o_{xy}}{N}`
+
+          for further reading https://en.wikipedia.org/wiki/Pointwise_mutual_information.
+
+        - event count mi 
+        - latency of first event after activity onset
+        - coarse resolution binary pattern represenation of device event activity
+
+    Parameters
+    ----------
+    df_devs: pd.DataFrame
+        TODO add desc
+    df_acts: pd.DataFrame
+        TODO add desc
+    kind : str one of ['pointwise', 'timetofirstevent', '']
+
+    Returns 
+    -------
+
+    """
+    assert kind in ['pointwise', 'eventcount', 'timetofirstevent', 'binary_pattern']
+
+    if kind == 'pointwise':
+        c_xy_events = contingency_table_events(df_devs, df_acts)
+        c_xy_events = c_xy_events.set_index('device')
+
+        p_xy = c_xy_events.values
+        N = p_xy.sum()
+        p_y = np.tile(p_xy.sum(axis=0), (p_xy.shape[0], 1))/N
+        p_x = np.tile(p_xy.sum(axis=1), (p_xy.shape[1], 1)).T/N
+        p_xy = p_xy/N
+        mi = np.log2(p_xy / np.multiply(p_x, p_y))
+
+        return pd.DataFrame(data=mi, index=c_xy_events.index, columns=c_xy_events.columns)
+
+    if kind == 'eventcount':
+        """
+        compute 
+        """
+        df = label_data(df_devs, df_acts, other=other)
+        # Id each trial
+        df['trial_id'] = (df[ACTIVITY].shift(1) != df[ACTIVITY]).astype(int)
+        df_grp = df.groupby(by=[ACTIVITY, DEVICE, 'trial_id'], observed=True).count()
+        devs = df_devs[DEVICE].unique()
+        acts = df_acts[ACTIVITY].unique()
+        from itertools import product
+        # Get the event count over all trials for each 
+        event_count = pd.DataFrame(index=devs, columns=acts, dtype=object)
+        for (dev, act) in product(dev, act):
+            event_count.at[dev, act] = df_grp.loc[(act, dev)][VALUE].values
+
+        print()
+    if kind == 'chi2':
+        c_xy_events = contingency_table_events(df_devs, df_acts)
+        c_xy_events = c_xy_events.set_index('device')
+        from sklearn.feature_selection import chi2
+        c2 = chi2(c_xy_events.values) * (1/(2*np.log(2)))
+
+
+    
+    return mi
+
+
+
+def time_dependent_firing_rate(df_devs, df_acts, device, activity, bin_width='10s'):
+    """
+    A trial is when an activity is performed.
+
+    time t is measured w.r. to the start of the activity.
+    The number of occurrences of events :math:`n_K(t;t+ \delta t)
+    Same as the peri-stimulus time histogram.
+
+    Parameters
+    ----------
+
+    bin_width : str one of ['xs', ]
+        The bin width :math:`delta_t`
+
+
+    """
+
+    df_acts = df_acts[df_acts[ACTIVITY] == activity].sort_values(by=START_TIME)\
+                                                    .reset_index(drop=True)
+    df_devs = df_devs[df_devs[DEVICE] == device].sort_values(by=TIME)\
+                                                .reset_index(drop=True)
+    bin_width = pd.Timedelta(bin_width)
+    
+    n_bins = np.ceil(max((df_acts[END_TIME] - df_acts[START_TIME])/bin_width))
+    max_dt = n_bins*bin_width
+
+    # the number of occurrences of event n_K(t; t+\Delta t)
+    counts = np.zeros(n_bins)
+
+    # Number of trials
+    K = df_acts.shape[0]
+
+    for _, act_ser in df_acts.iterrows():
+
+        dev_mask = (act_ser[START_TIME] < df_devs[TIME]) \
+                    & (df_devs[TIME] < act_ser[END_TIME])
+        devs = df_devs[dev_mask].copy() 
+
+        if devs.empty:
+            continue
+        vals = (devs[TIME] - act_ser[START_TIME]).apply(_get_freq_func('minutes')).values
+
+        add, bins = np.histogram(vals, bins=n_bins, range=(0,max_dt), density=False)
+        counts += add
+
+    # Compute event density as p(t) = 1/(\delta t) (n_k(t;t+\deltat))/K
+    counts = (1/bin_width)*counts/K
 
-    return df
+    return counts, bins
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/stats/discrete.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/stats/discrete.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import pandas as pd
 import numpy as np
+from pyadlml.constants import ACTIVITY
 
 ON_APPENDIX = " On"
 OFF_APPENDIX = " Off"
 def contingency_table_01(X, y):
     """ creates a contingency table for the matrix X and labels y
     Parameters
     ----------
     X : pd.Series or DataFrame
         matrix of 0-1 vectors as rows representing a state of 
         the smart home
-    y : np array of string
+    y : pd.Series
         labels for X
     
     Returns
     ---------
     pd.DataFrame
     """
+    assert len(X) == len(y), 'Shape mismatch'
+    assert isinstance(y, pd.Series)
 
-    X = X.copy()
-    if isinstance(y, pd.DataFrame):
-        y = y['activity']
+    X = X.copy().reset_index(drop=True)
+    y = y.copy().reset_index(drop=True)
 
-    X = X.reset_index(drop=True)
     first_dev = X.columns[0]
     index = X[first_dev]
     res = pd.crosstab(index=index, columns=y)
     res.index = _set_onoffappendix(res.index, first_dev)
 
     for dev_name in X.columns[1:]:
         tmp = pd.crosstab(index=X[dev_name], columns=y)
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/stats/util.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/stats/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pyadlml.constants import TIME, VALUE
 import numpy as np
 import pandas as pd
 
-from pyadlml.preprocessing import SequenceSlicer
+from pyadlml.preprocessing import EventWindow
 
 
 def get_tds_per_batch(X, window_size, stride, seq_type):
     """ returns the time deltas for each batch
 
     Parameters
     ----------
@@ -26,15 +26,15 @@
     """
     # extract time to index mapping
     time = X[TIME]
     index = X.index.values[:, np.newaxis]
 
     # print(index.shape)
     # slice and dice data
-    ss = SequenceSlicer(rep=seq_type, window_size=window_size, stride=stride)
+    ss = EventWindow(rep=seq_type, window_size=window_size, stride=stride)
     tmp, _ = ss.fit_transform(index)
 
     diffs = []
     for i in range(tmp.shape[0]):
         batch = time[tmp[i].squeeze()]
 
         # compute td difference to successor
@@ -72,15 +72,15 @@
     df : pd.DataFrame
         df of with columns [time, column_str]
     """
 
     df[TIME] = df[TIME].dt.floor(freq=dt).dt.time
 
     df[VALUE] = 1
-    df = df.groupby([TIME, column_str]).sum().unstack()
+    df = df.groupby([TIME, column_str], observed=True).sum().unstack()
     df = df.fillna(0)
     df.columns = df.columns.droplevel(0)
 
     # Add times bins where no sample hits anything
     range = pd.date_range(start='1/1/2000', end='1/2/2000', freq=dt).time
     df2 = pd.DataFrame(data=0, dtype=float, columns=df.columns, index=[d for d in range[:-1]])
     df2.update(df)
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/dataset/util.py` & `pyadlml-0.0.8.0a0/pyadlml/dataset/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 import functools
 import inspect
+import joblib
 from copy import copy
 
 import pandas as pd
 import numpy as np
 
-from pyadlml.constants import TIME, END_TIME, START_TIME, DEVICE, VALUE, BOOL, CAT, ACTIVITY
+from pyadlml.constants import DATASET_STRINGS, TIME, END_TIME, START_TIME, DEVICE, VALUE, BOOL, \
+    CAT, ACTIVITY
 from pandas.api.types import infer_dtype
-from pyadlml.dataset._core.activities import _is_activity_overlapping, correct_activity_overlap
-from pyadlml.dataset.plotly.util import ActivityDict
+from pyadlml.dataset._core.activities import ActivityDict, _is_activity_overlapping, \
+    correct_activity_overlap, is_activity_df
 
 """
     includes generic methods for manpulating dataframes
 """
 
+
 def print_df(df):
-    with pd.option_context('display.max_rows', None, 'display.max_columns', None):  # more options can be specified also
+    # more options can be specified also
+    with pd.option_context('display.max_rows', None, 'display.max_columns', None):
         print(df)
 
+def memory_usage(df, unit='MB'):
+    assert unit in ['MB', 'GB', 'B']
+    if unit == 'MB':
+        denom  = (1024 * 1024)
+    elif unit == 'GB':
+        unit =  (1024 * 1024 * 1024)
+    else:
+        unit = 1
+    return df.memory_usage().sum() / denom
+
 def unitsfromdaystart(ts, unit='s'):
     """ Computes units passed from the start of the day until the timestamp
     """
     ts = pd.Timestamp(ts) if not isinstance(ts, pd.Timestamp) else ts
     seconds = ts.hour*3600 + ts.minute*60 + ts.second
     if unit == 's':
         return int(seconds)
@@ -29,17 +43,14 @@
         return int(seconds/60)
     elif unit == 'h':
         return int(seconds/3600)
     else:
         raise ValueError
 
 
-
-
-
 def timestr_2_timedeltas(t_strs):
     """
         gets either a string or a list of strings to convert to a list of 
         timedeltas
     """
     if isinstance(t_strs, list):
         return [timestr_2_timedelta(t_str) for t_str in t_strs]
@@ -51,16 +62,16 @@
     """
         t_str (string)
         of form 30s, 30m
     """
     ttype = t_str[-1:]
     val = int(t_str[:-1])
 
-    assert ttype in ['h','m','s']
-    assert (val > 0 and val <=12 and ttype == 'h')\
+    assert ttype in ['h', 'm', 's']
+    assert (val > 0 and val <= 12 and ttype == 'h')\
         or (val > 0 and val <= 60 and ttype == 'm')\
         or (val > 0 and val <= 60 and ttype == 's')
     import datetime as dt
     if ttype == 's':
         return pd.Timedelta(seconds=val)
     if ttype == 'm':
         return pd.Timedelta(seconds=val*60)
@@ -68,18 +79,18 @@
         return pd.Timedelta(seconds=val*3600)
 
 
 def time2int(ts, t_res='30m'):
     """
     rounds to the next lower min bin or hour bin
     """
-    assert t_res[-1:] in ['h','m']
+    assert t_res[-1:] in ['h', 'm']
     val = int(t_res[:-1])
 
-    assert (val > 0 and val <=12 and t_res[-1:] == 'h')\
+    assert (val > 0 and val <= 12 and t_res[-1:] == 'h')\
         or (val > 0 and val <= 60 and t_res[-1:] == 'm')
 
     import datetime as dt
     zero = dt.time()
 
     if t_res[-1:] == 'h':
         hs = val
@@ -90,15 +101,14 @@
         ms = val
         m_bin = int(ts.minute/ms)*ms
         return dt.time(hour=ts.hour, minute=m_bin)
     else:
         raise ValueError
 
 
-
 def fill_nans_ny_inverting_first_occurence(df):
     """
     fills up true or false values
     :param df:
                 Name           0      1         10
         time                                     
         2008-02-25 00:20:14    NaN    NaN   ...    True
@@ -112,15 +122,15 @@
         2008-02-25 00:22:57    True   False ... False 
         2008-02-25 09:33:41    True   True  ... True 
         2008-02-25 09:33:42    False   NaN  ... False 
     """
     for col_label in df.columns:
         col = df[col_label]
 
-        # get timestamp of first valid index and replace previous Nans 
+        # get timestamp of first valid index and replace previous Nans
         #   by opposite
         ts = col.first_valid_index()
         idx = df.index.get_loc(ts)
         col.iloc[0:idx] = not col[ts]
     return df
 
 
@@ -157,18 +167,19 @@
         df_cat = pd.concat([df_cat, df_new])
 
     mask = df_cat[DEVICE].isin(cat_list)
     df_cat.loc[mask, DEVICE] = df_cat.loc[mask, 'new_device']
     df_cat = df_cat.drop(columns='new_device')
 
     df_devices = pd.concat([df_devices[~mask_cat], df_cat])\
-                    .sort_values(by=TIME)\
-                    .reset_index(drop=True)
+        .sort_values(by=TIME)\
+        .reset_index(drop=True)
     return df_devices
 
+
 def infer_dtypes(df_devices):
     """ Infers automatically the datatypes for each device of a device dataframe
     and returns a dictionary containing data types mapped to device names
 
     Parameters
     ----------
     df_devices : pd.DataFrame
@@ -192,18 +203,19 @@
             try:
                 pd.to_numeric(vals.dropna().unique())
                 dev_num.append(dev)
             except:
                 dev_cat.append(dev)
         elif inf == 'boolean':
             dev_bool.append(dev)
-        elif inf == 'floating':
+        elif inf == 'floating' or 'integer':
             dev_num.append(dev)
         else:
-            raise ValueError('could not infer correct dtype for device {}'.format(dev))
+            raise ValueError(
+                'could not infer correct dtype for device {}'.format(dev))
 
     return {'categorical': dev_cat, 'boolean': dev_bool, 'numerical': dev_num}
 
 
 def select_timespan(df_devs=None, df_acts=None, start_time=None, end_time=None, clip_activities=False):
     """ Selects a subset of a device and an activity dataframe based on a time span given
     Parameters
@@ -211,40 +223,42 @@
     df_devices : pd.DataFrame or None
         A device dataframe
     df_activities : pd.DataFrame, dict containing dataframes or None
         An activity dataframe
     start_time : str or None
         The start time from
     end_time : str or None
-    
+
     clip_activities : bool, default=False
         If set then the activities are clipped to the start and end time
 
     Returns
     -------
     df_d, df_a : the two subsets
     """
     # Cast to pandas timestamp
-    start_time = str_to_timestamp(start_time) if isinstance(start_time, str) else start_time
-    end_time = str_to_timestamp(end_time) if isinstance(end_time, str) else end_time
+    start_time = str_to_timestamp(start_time) if isinstance(
+        start_time, str) else start_time
+    end_time = str_to_timestamp(end_time) if isinstance(
+        end_time, str) else end_time
 
     if df_devs is not None:
         if start_time is not None:
             dev_start_sel = (df_devs[TIME] >= start_time)
         else:
             dev_start_sel = np.full(len(df_devs), True)
         if end_time is not None:
             dev_end_sel = (df_devs[TIME] < end_time)
         else:
             dev_end_sel = np.full(len(df_devs), True)
-        df_devs = df_devs[dev_start_sel & dev_end_sel]
+        df_devs = df_devs[dev_start_sel & dev_end_sel].copy()
 
     if df_acts is not None:
         df_acts_inst_type = type(df_acts)
-        df_acts = ActivityDict.wrap(df_acts)
+        df_acts = ActivityDict.wrap(df_acts).copy()
 
         for k in df_acts.keys():
             df_activity = df_acts[k]
             if start_time is not None:
                 act_start_sel = ~(df_activity[END_TIME] < start_time)
             else:
                 act_start_sel = np.full(len(df_activity), True)
@@ -254,243 +268,135 @@
                 act_end_sel = np.full(len(df_activity), True)
 
             df_activity = df_activity[act_start_sel & act_end_sel]
 
             # clip activities if they extend in regions that are not in the timespan
             if not df_activity.empty and start_time is not None \
                     and (start_time < df_activity[END_TIME].iat[0] and start_time > df_activity[START_TIME].iat[0]):
-                df_activity[START_TIME].iat[0] = start_time
+                df_activity.at[df_activity.index[0], START_TIME] = start_time
             if not df_activity.empty and clip_activities and end_time is not None \
-            and end_time < df_activity[END_TIME].iat[-1]:
-                df_activity[END_TIME].iat[-1] = end_time
-                
+                    and end_time < df_activity[END_TIME].iat[-1]:
+                df_activity.at[df_activity.index[-1], END_TIME] = end_time
+
             df_acts[k] = df_activity
 
-        df_acts = df_acts.unwrap(df_acts_inst_type) 
+        df_acts = df_acts.unwrap(df_acts_inst_type)
 
     if df_acts is None:
         return df_devs
     elif df_devs is None:
         return df_acts
     else:
         return df_devs, df_acts
 
 
-
-
-
-def str_to_timestamp(val):
-    """ Converts a datetime string to a panda Timestamp.
-    the day-first format is used.
+def get_last_states(df_devs: pd.DataFrame, left_bound=-1) -> dict:
+    """ Creates a dictionary where every device maps to its last known value.
 
     Parameters
     ----------
-    val : list or string
+    df_devs : pd.DataFrame
+        TODO add description 
+    left_bound : int
+        The index of the first event from which the states are determined directed
+        at the past 
 
     Returns
     -------
-    pd.Timestamp
-
+    res : dict
+        A device mapping to initial values
     """
-    return pd.to_datetime(val, dayfirst=True)
+    left_bound = len(df_devs) if left_bound == -1 else left_bound
+    return df_devs.iloc[:left_bound, :]\
+        .sort_values(by=TIME)\
+        .groupby(DEVICE, observed=True)\
+        .last()[VALUE]\
+        .to_dict()
 
-def remove_days(df_devices, df_activities, days=[], offsets=[], retain_corrections=False):
-    """ Removes the given days from activities and devices and shifts the succeeding days by that amount
-        forward.
+
+def get_first_states(df_devs: pd.DataFrame) -> dict:
+    """ Creates a dictionary where every device maps to its first known value.
 
     Parameters
     ----------
-    df_devices : pd.DataFrame
-    df_activities : pd.DataFrame
-    days : list
-        List of strings
-    offsets : list
-        Offsets that are added to the corresponding days.
-
-    Returns
-        df_devices : pd.DataFrame
-        df_activities : pd.DataFrame
-    """
-    nr_days = len(days)
-    df_devs = df_devices.copy()
-    df_acts = df_activities.copy()
-
-    # Add offsets to the days specified
-    for i in range(len(days)):
-        days[i] = str_to_timestamp(days[i])
-        if i < len(offsets):
-            days[i] = days[i] + pd.Timedelta(offsets[i])
-
-    # sort days from last to first
-    days = np.array(days)[np.flip(np.argsort(days))]
-    dtypes = infer_dtypes(df_devs)
-
-
-    # 1. remove iteratively the latest day and shift the succeeding part accordingly
-    for day in days:
-        # when day is e.g 2008-03.23 00:00:00 then day after will be 2008-03-24 00:00:00
-        # these variables have to be used as only timepoints can be compared as seen below
-        day_after = day + pd.Timedelta('1D')
-
-        # Remove devices events within the selected day
-        mask = (day < df_devs[TIME]) & (df_devs[TIME] < day_after)
-        removed_devs = df_devs[mask].copy()
-        df_devs = df_devs[~mask]
-
-        # shift the succeeding days timeindex one day in the past
-        succeeding_days = (day_after < df_devs[TIME])
-        df_devs.loc[succeeding_days, TIME] = df_devs[TIME] - pd.Timedelta('1D')
-
-        # Binary devices that change an odd amount of states in that day will have
-        # a wrong state for the succeeding days until the next event
-        nr_dev_triggers = removed_devs.groupby(by=[DEVICE]).count()
-        for dev in nr_dev_triggers.index:
-            nr = nr_dev_triggers.loc[dev, 'time']
-            if nr % 2 != 0 and (dev in dtypes[BOOL] or dev in dtypes[CAT]):
-                print(f'Warning: Removed odd #events: device {dev} => inconsistent device states. Correction advised!')
-
-
-        # Remove activities in that day that do not extend from the previous day into the selected
-        # day or extend from the selected day into the next day
-        mask_act_within_day = (day < df_acts[START_TIME]) & (df_acts[END_TIME] < day_after)
-        df_acts = df_acts[~mask_act_within_day]
-
-        # Special case where one activity starts before the selected day and ends after the selected day
-        mask_special = (df_acts[START_TIME] < day) & (day_after < df_acts[END_TIME])
-        if mask_special.any():
-            # Adjust the ending by removing one day
-            df_acts.loc[mask_special, END_TIME] = df_acts[END_TIME] - pd.Timedelta('1D')
-
-        # Shift Activities that start in or after the selected day by one day
-        succeeding_days = (day <= df_acts[START_TIME]) & (day_after < df_acts[END_TIME])
-        df_acts.loc[succeeding_days, START_TIME] = df_acts[START_TIME] - pd.Timedelta('1D')
-        df_acts.loc[succeeding_days, END_TIME] = df_acts[END_TIME] - pd.Timedelta('1D')
-        df_acts['shifted'] = False
-        df_acts.loc[succeeding_days, 'shifted'] = True
-
-        # Special case where one activity starts before the selected day and ends inside the selected day
-        # and there is no activity after the selected day
-        #  | day_before | Sel day      | day after
-        #     |-------------|
-        #    I can't just move the ending one day before as this would reverse START_TIME and END_TIME order
-        # -> The last activity ending is clipped to the start of the selected day
-        # TODO has to be done before any activity is shifted
-        #mask_last_true = pd.Series(np.zeros(len(df_acts), dtype=np.bool_))
-        #mask_last_true.iat[-1] = True
-        #mask_special = (df_acts[START_TIME] < day) & (df_acts[END_TIME] <= day_after) & mask_last_true
-        #if mask_special.any():
-        #    assert mask_special.sum() == 1
-        #    df_acts.loc[mask_special, END_TIME] = day
-
-        df_acts = df_acts.sort_values(by=START_TIME).reset_index(drop=True)
-        # Merge activities from the day_before that overlap with the shifted activities from day after
-        # there are 4 cases where overlaps into the respective days have to be handled
-        #                           |   db  |   sd  |   da  |=>|   db  |   sd  |   da  |=>|   db  |   sd  |   da  |
-        # 1. db overlaps da            |--------|    |~|          |--------|                 |-----|~|
-        #                                                              |~|
-        # 2. db intersect into  da      |------|     |~~~~|         |------|                   |----|~~~~|
-        #                                                               |~~~~|
-        # 3. da overlaps db             |-|   |~~~~~~~|            |-|                       |-|~~~|
-        #                                                       |~~~~~~~|
-        # 4. da intersect into db       |---|  |~~~~~|          |---|                        |---|~~~|
-        #                                                         |~~~~~|
-        # 5. da intersect into db         |----||~~~~~|            |-----|                 |---|~~~|
-        #                                                      |~~~~~~|
-        # case 1:
-        # select activities that cross the boundary between days
-        mask_db_into_sd = (df_acts[START_TIME] < day) & (df_acts[END_TIME] > day) & (df_acts[END_TIME] < day_after)
-        idxs = np.where(mask_db_into_sd)[0]
-        assert len(idxs) <= 2
-        if len(idxs) == 2:
-            # case 5: case when both activities extend into each days
-            # clip both to midnight
-            df_acts.iat[idxs[0], 2] = day
-            df_acts.iat[idxs[1], 1] = day + pd.Timedelta('1ms')
-        if len(idxs) == 1:
-            idx_overlapping = idxs[0]
-
-            # Check if the overlapping activity is part of the shifted or not
-            if df_acts.iat[idx_overlapping, 3]:
-                # Case when the shifted activities extend into the day before the selected day
-                last_unshifted_act = df_acts.loc[(df_acts[END_TIME] < day), :]\
-                                .copy().sort_values(by=END_TIME, ascending=True)\
-                                .iloc[-1, :]
+    df_devs : pd.DataFrame
+        TODO add description 
 
-                # clip extending activities start_time to the end_time of the first shifted activity
-                df_acts.iat[idx_overlapping, 0] = last_unshifted_act[END_TIME] + pd.Timedelta('1ms')
-            else:
-                # Case when the previous activities extends into the selected day
-                first_shifted_act = df_acts.loc[(df_acts[START_TIME] > day) & (df_acts[END_TIME] < day_after), :]\
-                                            .copy().sort_values(by=START_TIME, ascending=True)\
-                                            .iloc[0, :]
+    Returns
+    -------
+    res : dict
+        A device mapping to initial values
+    """
+    return df_devs.copy()\
+        .sort_values(by=TIME)\
+        .groupby(DEVICE, observed=True)\
+        .first()[VALUE]\
+        .to_dict()
 
-                # clip extending activities end_time to the start of the first shifted activity
-                df_acts.iat[idx_overlapping, 1] = first_shifted_act[START_TIME] - pd.Timedelta('1ms')
 
-        df_acts = df_acts.drop(columns='shifted')
+def str_to_timestamp(val):
+    """ Converts a datetime string to a panda Timestamp.
+    the day-first format is used.
 
-        from pyadlml.dataset._core.devices import correct_devices
-        df_devs, corrections_dev = correct_devices(df_devs, retain_corrections)
+    Parameters
+    ----------
+    val : list or string
 
-        #assert not _is_activity_overlapping(df_acts)
+    Returns
+    -------
+    pd.Timestamp
 
-    if retain_corrections:
-        try:
-            corrections_act
-        except:
-            corrections_act = []
-        try:
-            corrections_dev
-        except:
-            corrections_dev = []
-        return df_devs, df_acts, corrections_act, corrections_dev
-    else:
-        return df_devs, df_acts
+    """
+    return pd.to_datetime(val, dayfirst=True)
 
 
-def df_difference(df1: pd.DataFrame, df2: pd.DataFrame, which=None):
+def df_difference(df1: pd.DataFrame, df2: pd.DataFrame, which=None, return_mask=False):
     """Find rows which are different between two DataFrames.
 
     Parameters
     ----------
     df1 : pd.DataFrame
         TODO
     df2 : pd.DataFrame
         TODO
     which : None or str, default=None
-        TODO
-
+        When set to 'left' returns the elements where the 
+        first dataframe differs from the second
+    return_mask: book, default=False
 
     Returns
     -------
 
     """
     from pyadlml.dataset._core.devices import is_device_df
     from pyadlml.dataset._core.activities import is_activity_df
 
     comparison_df = df1.copy().merge(
         df2.copy(),
         indicator=True,
         how='outer'
     )
     if which is None:
-        diff_df = comparison_df[comparison_df['_merge'] != 'both']
+        mask = (comparison_df['_merge'] != 'both')
     else:
-        diff_df = comparison_df[comparison_df['_merge'] == which]
+        mask = (comparison_df['_merge'] == which)
+
+    if return_mask:
+        return mask
+    else:
+        diff_df = comparison_df[mask]
 
     if is_activity_df(df1):
         return diff_df[[START_TIME, END_TIME, ACTIVITY]]
     elif is_device_df(df1):
         return diff_df[[TIME, DEVICE, VALUE]]
     else:
         return diff_df
 
 
-
-
 def event_times(df_devices, start_time=None, end_time=None):
     """
     Parameters
     ----------
     time_array : nd.array or pd.Series or pd.DataFrame
     start_time : pd.Timestamp
 
@@ -522,18 +428,20 @@
     return res, start_time, end_time
 
 
 def num_to_timestamp(val, start_time, end_time):
     """Converts value [0,1] into timestamp between start_time and end_time"""
     return start_time + val*(end_time - start_time)
 
+
 def timestamp_to_num(ts, start_time, end_time):
     """Converts timestamp between start_time and end_time into value in [0,1]"""
     return float((ts - start_time)/(end_time - start_time))
 
+
 def get_sorted_index(df: pd.DataFrame, rule='alphabetical', area: pd.DataFrame = None) -> np.ndarray:
     """ Returns a new dataframes index that is sorted after a specific rule
 
     Parameters
     ----------
     df : pd.DataFrame
         Has to contain the column 'activity' or 'device'
@@ -575,26 +483,29 @@
         assert order_changed, '"activity" or "device" was not present in dataframe'
     elif rule == 'alphabetical':
         if ACTIVITY in df.columns:
             df = df.sort_values(by=ACTIVITY)
         elif DEVICE in df.columns:
             df = df.sort_values(by=DEVICE)
         else:
-            raise KeyError(f"Tried to sort alphabetical but no activity or device column was found, only {rule}")
+            raise KeyError(
+                f"Tried to sort alphabetical but no activity or device column was found, only {rule}")
     elif rule == 'value':
         # The case when the column other than ACTIVITY or order should be used
         cs = df.columns
         col = [i for i in cs if i not in [ACTIVITY, DEVICE, 'order']]
-        assert len(col) == 1, 'When value is specified there must be only one remaining column.'
+        assert len(
+            col) == 1, 'When value is specified there must be only one remaining column.'
         if ACTIVITY in df.columns:
             df = df.sort_values(by=col[0])
         elif DEVICE in df.columns:
             df = df.sort_values(by=col[0])
         else:
-            raise KeyError(f"Tried to sort alphabetical but no activity or device column was found, only {rule}")
+            raise KeyError(
+                f"Tried to sort alphabetical but no activity or device column was found, only {rule}")
     elif rule == 'areas':
         raise NotImplementedError
     elif isinstance(rule, str):
         assert rule in df.columns, f'The rule {rule} was not in the dataframes columns.'
         df = df.sort_values(by=rule)
     else:
         raise KeyError()
@@ -626,62 +537,105 @@
 
 def check_order(func):
     @extract_kwargs
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         o = kwargs['order']
         assert o in ['alphabetical', 'occurence'] or isinstance(o, list) \
-               or isinstance(o, np.ndarray), f'Sort rule is either "alphabetical", a custom string or a iterable. Found {o}'
+            or isinstance(o, np.ndarray), f'Sort rule is either "alphabetical", a custom string or a iterable. Found {o}'
         tmp = func(*args, **kwargs)
         return tmp
     return wrapper
 
+
 def check_scale(func):
     @extract_kwargs
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         assert kwargs['scale'] in ['linear', 'log']
         return func(*args, **kwargs)
     return wrapper
 
 
-def device_order_by(df_devs, rule='alphabetical'):
-    """Return a list with ordered devices
+def device_order_by(df_devs: pd.DataFrame, rule='alphabetical', dev2area=None, only_keep_existing=True) -> list:
+    """Create a list of devices ordered by some rule
+
+    Returns
+    -------
+    list of strings
     """
-    is_iterable = isinstance(rule, list) or isinstance(rule, np.ndarray)
-    if is_iterable:
+    if isinstance(rule, list) or isinstance(rule, np.ndarray):
         return rule
 
-    assert rule in ['alphabetical', 'count', 'area'], f'rule{rule} not in assertion.'
+    allowed_combis = ['alphabetical', 'count',
+                      'area', 'area+alphabetical', 'area+count']
+    assert rule in allowed_combis, f'rule{rule} not in assertion.'
 
     if rule == 'alphabetical':
-        dev_order = df_devs[DEVICE].unique()
-        dev_order.sort()
+        dev_order = df_devs[DEVICE].unique().tolist()
+        dev_order.sort()  # CAVE returns None, do not change ^^
     elif rule == 'count':
         from pyadlml.dataset.stats.devices import device_order_by_count
         dev_order = device_order_by_count(df_devs)
-    else:
-        raise NotImplementedError('The order has still to be implemented')
+    elif 'area' in rule:
+        assert dev2area is not None, 'When selecting area as sorting measure, an area mapping must be given as parameter.'
+        split = rule.split('+')
+        dev2area['area'] = dev2area['area'].fillna('-na')
+        if len(split) == 1 or split[1] == 'alphabetical':
+            dev_order = dev2area.groupby('area')\
+                                .apply(lambda x: x.sort_values(by=DEVICE))\
+                                .reset_index(drop=True)[DEVICE].to_list()
+        elif split[1] == 'count':
+            from pyadlml.dataset.stats.devices import device_order_by_count
+            ordered_by_count = device_order_by_count(df_devs)
+            dev_order = pd.DataFrame(
+                zip(range(len(ordered_by_count), ordered_by_count)), columns=['count', DEVICE])
+            dev_order = dev_order.set_index(DEVICE)
+            tmp = dev2area.set_index(DEVICE)
+            tmp['count'] = dev_order['count']
+            dev_order = dev2area.groupby('area')\
+                                .apply(lambda x: x.sort_values(by='count'))\
+                                .reset_index(drop=True)[DEVICE].to_list()
+        if only_keep_existing:
+            dev_order = [d for d in dev_order if d in df_devs[DEVICE].unique()]
+
     return dev_order
 
-def activity_order_by(dct_acts, rule='alphabetical'):
+
+def activity_order_by(dct_acts, rule: str = 'alphabetical') -> list:
     """ Return a list with ordered activities
+
+    Parameters
+    ----------
+    dct_acts: pd.DataFrame or ActivityDict
+    rule: str
+        The rule one of:
+            - alphabetical
+            - duration
+            - count
+            - area
+    Returns
+    -------
+    list of str
+        The ordered activity names
     """
     is_iterable = isinstance(rule, list) or isinstance(rule, np.ndarray)
     if is_iterable:
-        if all(isinstance(item, int) for item in rule):
+        # TODO refactor, negate: any not int and not dct is none than below
+        if all(isinstance(item, int) for item in rule) or dct_acts is None:
             return rule
 
         # Filter out activities that are not in df_acts
         rule = copy(list(rule))
         for act_not_in_df in set(rule) - set(dct_acts[ACTIVITY].unique()):
             rule.remove(act_not_in_df)
         return rule
 
-    assert rule in ['alphabetical', 'duration', 'count', 'area'], f'rule{rule} not in assertion.'
+    assert rule in ['alphabetical', 'duration', 'count',
+                    'area'], f'rule{rule} not in assertion.'
 
     if isinstance(dct_acts, pd.DataFrame):
         dct_acts = ActivityDict.wrap(dct_acts)
 
     if rule == 'alphabetical':
         act_order = dct_acts.get_activity_union()
         act_order.sort()
@@ -692,112 +646,329 @@
         from pyadlml.dataset.stats.activities import activity_order_by_count
         act_order = activity_order_by_count(dct_acts)
     else:
         raise NotImplementedError('Area has still to be implemented.')
 
     return act_order
 
-DATASET_STRINGS = [
-    'casas_aruba',
-    'amsterdam',
-    'mitlab_1',
-    'mitlab_2',
-    'aras',
-    'kasteren_A',
-    'kasteren_B',
-    'kasteren_C',
-    'tuebingen_2019',
-    'uci_ordonezA',
-    'uci_ordonezB',
-    'act_assist',
-    'dump'
-]
-def fetch_data_by_string(dataset: str, cache=True, identifier=None):
-    """ Fetches data based on a given string representation
+
+def fetch_by_name(dataset: str, identifier=None, **kwargs) -> dict:
+    """ Fetches a dataset based on a given string. 
 
     Parameters
     ----------
     dataset: str
 
-    identifier: str, default=None
-        Identifies a custom dataset in the data home. In the case
-        of an act_assist dataset this is the folder name. In the case
-        of a dumped dataframe with pyadlml.io.dump this is the name.
 
     Returns
     -------
-    data : pyadlml.dataset.obj
+    dict
     """
+    error_msg = f'No suitable option specified: {dataset}.\nAvailable are {DATASET_STRINGS}'
+    assert dataset in DATASET_STRINGS + ['joblib'], error_msg
 
     from pyadlml.dataset import fetch_amsterdam, \
-                                fetch_mitlab, fetch_aras, fetch_kasteren_2010, \
-                                fetch_casas_aruba, fetch_tuebingen_2019, \
-                                fetch_uci_adl_binary, load_act_assist
+        fetch_mitlab, fetch_aras, fetch_kasteren_2010, \
+        fetch_tuebingen_2019, fetch_casas,\
+        fetch_uci_adl_binary, load_act_assist
     if dataset == DATASET_STRINGS[0]:
-        data = fetch_casas_aruba(cache=cache)
-    elif dataset == DATASET_STRINGS[1]:
-        data = fetch_amsterdam(cache=cache)
-    elif dataset == DATASET_STRINGS[2]:
-        data = fetch_mitlab(subject='subject1', cache=cache)
-    elif dataset == DATASET_STRINGS[3]:
-        data = fetch_mitlab(subject='subject2', cache=cache)
-    elif dataset == DATASET_STRINGS[4]:
-        data = fetch_aras(cache=cache)
+        return fetch_casas(testbed='aruba', **kwargs)
+    if dataset == DATASET_STRINGS[1]:
+        return fetch_casas(testbed='kyoto_2010', **kwargs)
+    if dataset == DATASET_STRINGS[2]:
+        return fetch_casas(testbed='milan', **kwargs)
+    if dataset == DATASET_STRINGS[3]:
+        return fetch_casas(testbed='cairo', **kwargs)
+    if dataset == DATASET_STRINGS[4]:
+        return fetch_casas(testbed='tulum', **kwargs)
     elif dataset == DATASET_STRINGS[5]:
-        data = fetch_kasteren_2010(house='A', cache=cache)
+        return fetch_amsterdam(**kwargs)
     elif dataset == DATASET_STRINGS[6]:
-        data = fetch_kasteren_2010(house='B', cache=cache)
+        return fetch_mitlab(subject='subject1', **kwargs)
     elif dataset == DATASET_STRINGS[7]:
-        data = fetch_kasteren_2010(house='C', cache=cache)
+        return fetch_mitlab(subject='subject2', **kwargs)
     elif dataset == DATASET_STRINGS[8]:
-        data = fetch_tuebingen_2019(cache=cache)
+        return fetch_aras(**kwargs)
     elif dataset == DATASET_STRINGS[9]:
-        data = fetch_uci_adl_binary(subject='OrdonezA', cache=cache)
+        return fetch_kasteren_2010(house='A', **kwargs)
     elif dataset == DATASET_STRINGS[10]:
-        data = fetch_uci_adl_binary(subject='OrdonezB', cache=cache)
+        return fetch_kasteren_2010(house='B', **kwargs)
     elif dataset == DATASET_STRINGS[11]:
-        data = load_act_assist(identifier)
+        return fetch_kasteren_2010(house='C', **kwargs)
     elif dataset == DATASET_STRINGS[12]:
-        from pyadlml.dataset._core.devices import is_device_df
-        from pyadlml.dataset.io import load
-        from pyadlml.dataset._core.activities import is_activity_df
-        df_lst = load(identifier)
-
-        df_devs = None
-        df_acts = None
-        for df in df_lst:
-            if is_device_df(df):
-                df_devs = df
-            elif is_activity_df(df):
-                df_acts = df
-            else:
-                raise ValueError('At least one of the dataframes has to be a device dataframe')
-        assert df_devs is not None and df_acts is not None
-        data = Data(df_acts, df_devs)
-
-    else:
-        raise ValueError(f'No suitable option specified: {dataset}.\nAvailable are {DATASET_STRINGS}')
-
-    return data
+        return fetch_tuebingen_2019(**kwargs)
+    elif dataset == DATASET_STRINGS[13]:
+        return fetch_uci_adl_binary(subject='OrdonezA', **kwargs)
+    elif dataset == DATASET_STRINGS[14]:
+        return fetch_uci_adl_binary(subject='OrdonezB', **kwargs)
+    elif dataset == DATASET_STRINGS[15]:
+        return load_act_assist(identifier)
+    elif dataset == 'joblib':
+        return joblib.load(identifier)
 
 
 def get_dev_row_where(df, time, dev, state):
+    raise ValueError('deprecated: use get_index_matchingrows instead')
     time = pd.Timestamp(time)
-    df = df.copy().reset_index().set_index(TIME)
     mask = (df[DEVICE] == dev) \
-           & (df.index == time) \
-           & (df[VALUE] == state)
+        & (df[TIME] == time) \
+        & (df[VALUE] == state)
     df = df.reset_index().set_index('index')
     return df[mask.values].copy()
 
+
 def get_dev_rows_where(df_devs, rows):
+    raise ValueError('deprecated: use get_index_matchingrows instead')
     res = [get_dev_row_where(df_devs, r[0], r[1], r[2]) for r in rows]
     return pd.concat(res)
 
+
 def append_devices(df_devs, rows):
+    raise ValueError('deprecated: use get_index_matchingrows instead')
     df = pd.DataFrame(data=rows, columns=[TIME, DEVICE, VALUE])
     df[TIME] = pd.to_datetime(df[TIME])
     return pd.concat([df_devs, df])
 
+
 def remove_devices(df_devs, rows):
-    idx_to_drop = [get_dev_row_where(df_devs, r[0], r[1], r[2]).index[0] for r in rows]
+    raise ValueError('deprecated: use get_index_matchingrows instead')
+    idx_to_drop = [get_dev_row_where(
+        df_devs, r[0], r[1], r[2]).index[0] for r in rows]
     return df_devs.drop(index=idx_to_drop)
+
+
+def to_sktime(df_devs: pd.DataFrame, df_acts: pd.DataFrame = None, return_type: str = None,
+              return_X_y: bool = False):
+    """
+
+    Parameters
+    ----------
+    df_devs: pd.DataFrame
+        TODO 
+
+    df_acts: pd.DataFrame, optional
+        TODO
+
+    return_type: str or None, default=None
+        Memory data format specification to return X in, None = “nested_univ” type. str can be any supported sktime Panel mtype,
+        for list of mtypes, see datatypes.MTYPE_REGISTER for specifications, see examples/AA_datatypes_and_datasets.ipynb
+        commonly used specifications:
+            - “nested_univ: nested pd.DataFrame, pd.Series in cells 
+            - “numpy3D”/”numpy3d”/”np3D”: 3D np.ndarray (instance, variable, time index) 
+
+    return_X_y: bool, default=False
+        it returns two objects, if False, it appends the class labels to the dataframe.
+
+
+
+    Returns 
+    -------
+    X: pd.DataFrame
+        The time series data for the problem with n_cases rows and either n_dimensions or n_dimensions+1 columns. Columns 1 to n_dimensions are the series associated with each case. If return_X_y is False, column n_dimensions+1 contains the class labels/target variable.
+    y: numpy array, optional
+        The class labels for each case in X, returned separately if return_X_y is True, or appended to X if False
+
+    """
+    from pyadlml.preprocessing.preprocessing import LabelMatcher
+
+    return_type = 'nested_univ' if return_type is None else return_type
+    return_type = 'numpy3d' if return_type in [
+        'numpy3D', 'np3D', 'np3d'] else return_type
+
+    if return_type in ["pd-multiindex", "numpy2d"]:
+        err_txt = "BasicMotions loader: Error, attempting to load into a numpy2d array, but cannot because it is a multivariate problem. Use numpy3d instead"
+        raise ValueError(err_txt)
+
+    assert return_type in ["numpy3d", "nested_univ"]
+
+    if df_acts is not None:
+        y = LabelMatcher(other=False).fit_transform(df_acts, df_devs).values
+        y = y[:, 1].astype(np.dtype('U'))
+    else:
+        y = None
+
+    if return_type == "nested_univ":
+        """
+        nested dataframe
+        , TIME, DEVICE, VALUE 
+        0, [S_T, S_D, S_V]
+        """
+        columns = [TIME, DEVICE, VALUE]
+        index = 'RangeIndex'
+        data = {TIME: [df_devs[TIME]], DEVICE: [
+            df_devs[DEVICE]], VALUE: [df_devs[VALUE]]}
+        X = pd.DataFrame(columns=columns, index=[0], data=data)
+        if y is not None:
+            if return_X_y:
+                return X, y
+            else:
+                X.loc[0, 'class_val'] = y
+                return X
+        else:
+            return X
+
+    elif return_type == "numpy3d":
+        """ 
+        Create array [S, F, T] with S being # sequences/recordings, F being
+        the number of features (possible F + 1 for y) and T being the sequence length
+        """
+        X = np.swapaxes(np.expand_dims(df_devs.values, 0), 1, 2)
+        if y is not None:
+            if return_X_y:
+                return X, y
+            else:
+                return np.append(X, y.reshape(1, 1, -1), axis=1)
+        else:
+            return X
+
+    else:
+        raise
+
+
+def to_sktime2(df_X: pd.DataFrame, df_y: pd.DataFrame, return_type: str = None,
+               return_X_y: bool = False):
+    """
+
+    Parameters
+    ----------
+    df_X: pd.DataFrame
+        A dataframe where the columns are the features. There must be at least 
+        one column named 'time' in order to correclty match the labels. For 
+        example a device dataframe with features [TIME, DEVICE, VALUE]
+
+    df_acts: pd.DataFrame, optional
+        TODO
+
+    return_type: str or None, default=None
+        Memory data format specification to return X in, None = “nested_univ” type. str can be any supported sktime Panel mtype,
+        for list of mtypes, see datatypes.MTYPE_REGISTER for specifications, see examples/AA_datatypes_and_datasets.ipynb
+        commonly used specifications:
+            - “nested_univ: nested pd.DataFrame, pd.Series in cells 
+            - “numpy3D”/”numpy3d”/”np3D”: 3D np.ndarray (instance, variable, time index) 
+
+    return_X_y: bool, default=False
+        it returns two objects, if False, it appends the class labels to the dataframe.
+
+
+
+    Returns 
+    -------
+    X: pd.DataFrame
+        The time series data for the problem with n_cases rows and either n_dimensions or n_dimensions+1 columns. Columns 1 to n_dimensions are the series associated with each case. If return_X_y is False, column n_dimensions+1 contains the class labels/target variable.
+    y: numpy array, optional
+        The class labels for each case in X, returned separately if return_X_y is True, or appended to X if False
+
+    """
+
+    from pyadlml.dataset._core.devices import is_device_df
+    return_type = 'nested_univ' if return_type is None else return_type
+    return_type = 'numpy3d' if return_type in [
+        'numpy3D', 'np3D', 'np3d'] else return_type
+
+    if return_type in ["pd-multiindex", "numpy2d"]:
+        err_txt = "BasicMotions loader: Error, attempting to load into a numpy2d array, but cannot because it is a multivariate problem. Use numpy3d instead"
+        raise ValueError(err_txt)
+
+    assert return_type in ["numpy3d", "nested_univ"]
+
+    """
+    Create appropriate targets depending on given input
+    """
+    if is_activity_df(df_y):
+        from pyadlml.preprocessing.preprocessing import LabelMatcher
+        y = LabelMatcher(other=False).fit_transform(df_y, df_X).values
+        y = y[:, 1].astype(np.dtype('U'))
+    else:
+        # Ensure there are no other things such as timestamps choose the last dimension as
+        y = df_y[:, :, -1] if len(df_y.shape) == 3 else df_y
+
+        if len(y.shape) == 2 and y.shape[1] > 1:
+            # When the windows were produces with many-to-many relationship reduce to many-to-one
+            # since
+            y = y[:, -1]
+            print(
+                'Warning!!! Reducing many-to-many into many-to-one. Check if this was the intended measure.')
+        y = y.squeeze()
+        assert len(y.shape) == 1
+
+    X = df_X.copy()
+
+    assert y.shape[0] == X.shape[
+        0], f"Shape mismatch between X and y: {y.shape[0]} vs. {X.shape[0]}"
+
+    if return_type == "nested_univ" and len(X.shape) == 2:
+        """ Convert a 2d dataframe or numpy array 
+        """
+        if isinstance(X, np.ndarray):
+            X = pd.DataFrame(X, columns=[f'dim_{i}'for i in range(X.shape[1])])
+
+        if not is_device_df(X):
+            # TODO do sth. here??
+            pass
+
+        """
+        nested dataframe
+        , TIME, DEVICE, VALUE 
+        0, [S_T, S_D, S_V]
+        """
+        F = len(X.columns)
+
+        X['target'] = y
+        X['tmp'] = (X['target'].shift(1) != X['target']).astype(int)
+        y = X[X['tmp'] == 1].loc[:, 'target'].copy().reset_index(drop=True)
+        X['tmp'] = X['tmp'].cumsum()
+
+        """
+        Produce [N, F, s]
+        where N is the number of each subsequence
+        """
+        data_X = []
+        for yi, (_, Xi) in zip(y, X.groupby(by='tmp')):
+            datum = {col: Xi[col] for col in Xi.columns[:-2]}
+            if not return_X_y:
+                datum['class_val'] = yi
+            data_X.append(datum)
+
+        X = pd.DataFrame(data_X)
+        if return_X_y:
+            return X, y
+        else:
+            return X
+    elif return_type == "nested_univ" and len(X.shape) == 3:
+        """ Convert a 3d ndarray to nested_univ. This is the case when a windowing
+            approach is used before Sktime.
+
+            X has the shape (S, T, F) where S is the number of sequences, T the sequence length 
+            and F the number of features
+        """
+        data_X = []
+        for i in range(len(y)):
+            # Xi of shape (T, F) where T is the sequence length and F are the number of features
+            Xi, yi = X[i], y[i]
+            datum = {f'dim_{f}': pd.Series(Xi[:, f])
+                     for f in range(Xi.shape[1])}
+            if not return_X_y:
+                datum['class_val'] = yi
+            data_X.append(datum)
+
+        X = pd.DataFrame(data_X)
+        if return_X_y:
+            return X, y
+        else:
+            return X
+    elif return_type == "numpy3d":
+        """ 
+        Create array [S, F, T] with S being # sequences/recordings, F being
+        the number of features (possible F + 1 for y) and T being the sequence length
+        """
+        raise NotImplementedError
+        X = np.swapaxes(np.expand_dims(df_devs.values, 0), 1, 2)
+        if y is not None:
+            if return_X_y:
+                return X, y
+            else:
+                return np.append(X, y.reshape(1, 1, -1), axis=1)
+        else:
+            return X
+
+    else:
+        raise
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/feature_extraction.py` & `pyadlml-0.0.8.0a0/pyadlml/feature_extraction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 import pandas as pd
 from sklearn.base import TransformerMixin, BaseEstimator
 from pyadlml.constants import TIME, DEVICE
 
+
 def _tres_2_pd_res(res):
     if _is_hour(res) or _is_sec(res):
         return res
     if _is_min(res):
         return res[:-1] + 'min'
 
 
 def _tres_2_discrete(resolution):
     """ create resolution for one day
     """
     res = []
-    range = pd.date_range(start='1/1/2000', end='1/2/2000', freq=resolution).time
+    range = pd.date_range(
+        start='1/1/2000', end='1/2/2000', freq=resolution).time
     range = [str(d) for d in range]
     for t1, t2 in zip(range[:-1], range[1:]):
         res.append(t1 + '-' + t2)
     return res
 
 
 def _tres_2_vals(resolution):
     """ create resolution for one day
     """
-    ser = pd.date_range(start='1/1/2000', end='1/2/2000', freq=resolution).to_series()
+    ser = pd.date_range(start='1/1/2000', end='1/2/2000',
+                        freq=resolution).to_series()
     if _is_min(resolution):
         return ser.dt.floor(resolution).dt.minute
-    if _is_hour(resolution): return ser.dt.floor(resolution).dt.hour
+    if _is_hour(resolution):
+        return ser.dt.floor(resolution).dt.hour
     if _is_sec(resolution):
         return ser.dt.floor(resolution).dt.sec
 
 
 def _is_hour(res) -> bool:
     return res[-1:] == 'h'
 
@@ -44,16 +48,16 @@
 
 
 def _valid_tres(t_res):
     val = int(t_res[:-1])
     res = t_res[-1:]
     assert t_res[-1:] in ['h', 'm', 's']
     assert (val > 0 and val <= 12 and res == 'h') \
-           or (val > 0 and val <= 60 and res == 'm') \
-           or (val > 0 and val <= 60 and res == 's')
+        or (val > 0 and val <= 60 and res == 'm') \
+        or (val > 0 and val <= 60 and res == 's')
     return True
 
 
 def _time2intervall(ts, t_res='30m'):
     """
     rounds to the next lower min bin or hour bin """
     ts_ceil = ts.ceil(freq=t_res).time()
@@ -61,15 +65,15 @@
     return str(ts_floor) + '-' + str(ts_ceil)
 
 
 def extract_time_difference(df, normalize=False, inplace=True):
     return df
 
 
-class DayOfWeekExtractor(TransformerMixin, BaseEstimator):
+class DayOfWeek(TransformerMixin, BaseEstimator):
     """
     Appends seven columns one-hot encoded for week days to a dataframe based
         on the dataframes timestamps.
 
     Attributes
     ----------
     one_hot_encoding : bool, optional, default=False
@@ -78,15 +82,16 @@
     inplace : bool, default=True
         Determines whether to append the one-hot encoded time_bins as columns
         to the existing dataframe or return only the one-hot encoding.
 
     """
 
     WD_COL = 'weekday'
-    WEEKDAYS = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
+    WEEKDAYS = ['Monday', 'Tuesday', 'Wednesday',
+                'Thursday', 'Friday', 'Saturday', 'Sunday']
 
     def __init__(self, one_hot_encoding=False, inplace=False):
         self.one_hot_encoding = one_hot_encoding
         self.inplace = inplace
 
     def fit(self, X):
         return self
@@ -127,15 +132,15 @@
         del (df[self.WD_COL])
         if self.inplace:
             return df
         else:
             return df[self.WEEKDAYS]
 
 
-class TimeBinExtractor(TransformerMixin, BaseEstimator):
+class TimeOfDay(TransformerMixin, BaseEstimator):
     """
     Divides a day into equal-length time bins and assigns time bin as features to
     a row that falls into that bin.
 
     Attributes
     ----------
     dt: str, default='2h'
@@ -145,38 +150,58 @@
         Determines whether to append the one-hot encoded time_bins as columns
         to the existing dataframe or return only the one-hot encoding.
 
     """
     TIME_BINS = 'time_bins'
     ALLOWED_RESOLUTIONS = ['m', 's', 'h']
 
-    def __init__(self, dt='2h', one_hot_encoding=False, inplace=False):
+    def __init__(self, dt='2h', one_hot_encoding=False, inplace=False, dtype=bool):
         self.dt = dt
         self.inplace = inplace
         self.one_hot_encoding = one_hot_encoding
+        self.dtype = dtype
 
     def fit(self, X, y=None):
         assert self.dt[-1:] in self.ALLOWED_RESOLUTIONS
+        assert self.dtype in [bool, int]
         return self
 
+    def get_time_bin(self, value: pd.Timestamp) -> str:
+        return _time2intervall(value, self.dt)
+
+    def get_time_bins(self) -> list:
+        tdelta = pd.Timedelta(self.dt)
+        total_bins = (pd.Timedelta('1 day') // tdelta)
+
+        time_bins = []
+        current_time = pd.Timestamp("00:00:00")
+
+        for _ in range(total_bins):
+            time_bin = _time2intervall(
+                current_time + pd.Timedelta('1ms'), self.dt)
+            time_bins.append(time_bin)
+            current_time += tdelta
+
+        return time_bins
+
     def fit_transform(self, X, y=None, **fit_params):
         """
 
         Parameters
         ----------
         X: pd.DataFrame
            A device dataframe. The dataframe has to include a column with
            the name 'time' containing the timestamps of the representation.
 
         Returns
         -------
         df : pd.DataFrame
             One-hot encoding of the devices.
         """
-        self.fit(X,y)
+        self.fit(X, y)
 
         return self.transform(X)
 
     def transform(self, X, y=None):
         """
 
         Parameters
@@ -186,26 +211,25 @@
            named 'time' containing timestamps of the representation.
 
         Returns
         -------
         df : pd.DataFrame
             One-hot encoding of the devices.
         """
-        assert self.dt[-1:] in self.ALLOWED_RESOLUTIONS
 
         df = X.copy()
         df[self.TIME_BINS] = df[TIME].apply(_time2intervall, args=[self.dt])
 
         if not self.one_hot_encoding:
             if self.inplace:
                 return df
             else:
                 return df[self.TIME_BINS]
 
-        one_hot = pd.get_dummies(df[self.TIME_BINS]).astype(bool)
+        one_hot = pd.get_dummies(df[self.TIME_BINS]).astype(self.dtype)
         df = df.join(one_hot, on=df.index)
         del (df[self.TIME_BINS])
 
         # add columns that don't exist in the dataset
         cols = _tres_2_discrete(self.dt)
         for v in cols:
             if v not in df.columns:
@@ -213,15 +237,15 @@
 
         if self.inplace:
             return df
         else:
             return df[cols]
 
 
-class TimeDiffExtractor(TransformerMixin, BaseEstimator):
+class InterEventTime(TransformerMixin, BaseEstimator):
     """
     Extracts the time difference to either the next or previous event
 
     Attributes
     ----------
     direction : str, optional, default='to_predecessor'
         The direction to which the timedifference is calculated.
@@ -230,42 +254,42 @@
     inplace : bool, optional , default=False
         Determines whether to add the column to and return the existing dataframe or
         return a dataframe containing only the time differences.
     unit : one of {None, 'm', 's'}, default=None
         The unit in which the time difference is expressed. When nothing is specified
         transform returns pandas timedeltas otherwise integers
     """
-    BACK = 'to_predecessor'
-    FORTH = 'to_successor'
+    BACKWARD = 'to_predecessor'
+    FORWARD = 'to_successor'
     COL_NAME = 'td'
 
     def __init__(self, direction='to_predecessor', unit=None, normalize=False, inplace=False):
         self.normalize = normalize
         self.inplace = inplace
         self.direction = direction
         self.unit = unit
 
     def _compute_td(self, df):
         """
         compute the time difference to successor and predecessor
         """
-        df[self.FORTH] = df[TIME].shift(-1) - df[TIME]
-        df[self.BACK] = df[TIME] - df[TIME].shift(1)
+        df[self.FORWARD] = df[TIME].shift(-1) - df[TIME]
+        df[self.BACKWARD] = df[TIME] - df[TIME].shift(1)
         return df
 
     def fit(self, X: pd.DataFrame, y=None):
         assert TIME in X.columns
 
         # compute a dataframe with mean time diff for each device
         df = self._compute_td(X.copy())
 
         # compute average value
-        self.td_avg = df[[DEVICE, self.BACK, self.FORTH]]\
+        self.td_avg = df[[DEVICE, self.BACKWARD, self.FORWARD]]\
             .iloc[1:-1]\
-            .groupby(DEVICE)\
+            .groupby(DEVICE, observed=True)\
             .mean(numeric_only=False)\
             .reset_index()
 
         # compute the highest and lowest value
         if self.normalize:
             self.min_ = df[self.direction].max()
             self.max_ = df[self.direction].min()
@@ -292,43 +316,48 @@
         df : pd.DataFrame
         """
         assert TIME in X.columns
 
         df = self._compute_td(X.copy())
 
         # impute either last or first value with the average of the value
-        if self.direction == self.BACK:
-            del(df[self.FORTH])
+        if self.direction == self.BACKWARD:
+            del (df[self.FORWARD])
             first_device = df.iloc[0][DEVICE]
-            df.at[0, self.BACK] = self.td_avg[self.td_avg[DEVICE] == first_device][self.BACK].iloc[0]
-            df.rename(columns={self.BACK: self.COL_NAME}, inplace=True)
+            df.at[0, self.BACKWARD] = self.td_avg[self.td_avg[DEVICE]
+                                                  == first_device][self.BACKWARD].iloc[0]
+            df.rename(columns={self.BACKWARD: self.COL_NAME}, inplace=True)
 
-        elif self.direction == self.FORTH:
-            del(df[self.BACK])
+        elif self.direction == self.FORWARD:
+            del (df[self.BACKWARD])
             last_device = df.iloc[-1][DEVICE]
-            df.at[0, self.FORTH] = self.td_avg[self.td_avg[DEVICE] == last_device][self.FORTH].iloc[0]
-            df.rename(columns={self.FORTH: self.COL_NAME}, inplace=True)
+            df.at[0, self.FORWARD] = self.td_avg[self.td_avg[DEVICE]
+                                                 == last_device][self.FORWARD].iloc[0]
+            df.rename(columns={self.FORWARD: self.COL_NAME}, inplace=True)
         else:
             raise ValueError
 
         if self.normalize:
             # apply min max normalization
-            df[self.COL_NAME] = (df[self.COL_NAME] - self.min_)/(self.max_ - self.min_)
+            df[self.COL_NAME] = (df[self.COL_NAME] -
+                                 self.min_)/(self.max_ - self.min_)
 
             # clip values that don't fit
-            df[self.COL_NAME] = df[self.COL_NAME].where(df[self.COL_NAME] < 1, 1)
-            df[self.COL_NAME] = df[self.COL_NAME].where(df[self.COL_NAME] > 0, 0)
+            df[self.COL_NAME] = df[self.COL_NAME].where(
+                df[self.COL_NAME] < 1, 1)
+            df[self.COL_NAME] = df[self.COL_NAME].where(
+                df[self.COL_NAME] > 0, 0)
 
         elif self.unit is not None:
             if self.unit == 's':
                 df[self.COL_NAME] = df[self.COL_NAME].dt.seconds
             elif self.unit == 'ms':
                 df[self.COL_NAME] = df[self.COL_NAME].dt.microseconds
             elif self.unit == 'h':
                 df[self.COL_NAME] = df[self.COL_NAME].dt.hours
             else:
                 raise ValueError
 
         if self.inplace:
             return df
         else:
-            return df[self.COL_NAME]
+            return df[self.COL_NAME]
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/feature_selection.py` & `pyadlml-0.0.8.0a0/pyadlml/feature_selection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pandas as pd
 
 # compute a chi-squared dependence table
 def rep2onoff(rep):
     df = rep.copy().iloc[:,:-1] # get raw without activities
     df = df.reset_index(drop=True)
     df = df.astype(int)
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/model/_model.py` & `pyadlml-0.0.8.0a0/pyadlml/model/_model.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/model/hbhmm/hmm.py` & `pyadlml-0.0.8.0a0/pyadlml/model/hbhmm/hmm.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/model/hbhmm/pchmm.py` & `pyadlml-0.0.8.0a0/pyadlml/model/hbhmm/pchmm.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/model/hmm/_model_categorical.py` & `pyadlml-0.0.8.0a0/pyadlml/model/hmm/_model_categorical.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/model/hmm/bhmm.py` & `pyadlml-0.0.8.0a0/pyadlml/model/hmm/bhmm.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/model/hmm/bhmm_hp.py` & `pyadlml-0.0.8.0a0/pyadlml/model/hmm/bhmm_hp.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/model/hmm/bhsmm.py` & `pyadlml-0.0.8.0a0/pyadlml/model/hmm/bhsmm.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/model/hmm/hmm.py` & `pyadlml-0.0.8.0a0/pyadlml/model/hmm/hmm.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/model/hmm/util.py` & `pyadlml-0.0.8.0a0/pyadlml/model/hmm/util.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/model/rnn/rnn.py` & `pyadlml-0.0.8.0a0/pyadlml/model/rnn/rnn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from skorch.utils import to_tensor
-from skorch.utils import TeeGenerator
-from skorch import NeuralNetClassifier
+#from skorch.utils import to_tensor
+#from skorch.utils import TeeGenerator
+#from skorch import NeuralNetClassifier
 
 import torch.nn as nn
 import torch.nn.functional as F
 import torch
 
 import torch.nn as nn
 import torch.nn.functional as F
@@ -65,32 +65,32 @@
 #
 #    def get_loss(self, y_pred, y_true, X=None, training=False):
 #        loss = super().get_loss(y_pred, y_true, X=X, training=training)
 #        loss += self.lambda1 * sum([w.abs().sum() for w in self.module_.parameters()])
 #        return loss
 
 
-from skorch.utils import to_tensor
-
-class RNNClassifier(NeuralNetClassifier):
-
-    def get_loss(self, y_pred, y_true, X=None, training=False):
-        """Return the loss for this batch.
-        Parameters
-        ----------
-        y_pred : torch tensor
-          Predicted target values
-        y_true : torch tensor
-          True target values.
-        X : input data, compatible with skorch.dataset.Dataset
-        """
-        if self.module_.seq_type == 'many-to-many':
-            y_true = torch.flatten(to_tensor(y_true, device=self.device), start_dim=0, end_dim=1)
-            y_pred = torch.flatten(y_pred, start_dim=0, end_dim=1)
-
-        elif self.module_.seq_type != 'many-to-one':
-            ValueError("the sequence type of the RNN was false defined")
-
-        if isinstance(self.criterion_, torch.nn.Module):
-            self.criterion_.train(training)
-
-        return self.criterion_(y_pred, y_true)
+#from skorch.utils import to_tensor
+#
+#class RNNClassifier(NeuralNetClassifier):
+#
+#    def get_loss(self, y_pred, y_true, X=None, training=False):
+#        """Return the loss for this batch.
+#        Parameters
+#        ----------
+#        y_pred : torch tensor
+#          Predicted target values
+#        y_true : torch tensor
+#          True target values.
+#        X : input data, compatible with skorch.dataset.Dataset
+#        """
+#        if self.module_.seq_type == 'many-to-many':
+#            y_true = torch.flatten(to_tensor(y_true, device=self.device), start_dim=0, end_dim=1)
+#            y_pred = torch.flatten(y_pred, start_dim=0, end_dim=1)
+#
+#        elif self.module_.seq_type != 'many-to-one':
+#            ValueError("the sequence type of the RNN was false defined")
+#
+#        if isinstance(self.criterion_, torch.nn.Module):
+#            self.criterion_.train(training)
+#
+#        return self.criterion_(y_pred, y_true)
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/model/util.py` & `pyadlml-0.0.8.0a0/pyadlml/model/util.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/model/vrnn/vrnn.py` & `pyadlml-0.0.8.0a0/pyadlml/model/vrnn/vrnn.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/model_selection/_search.py` & `pyadlml-0.0.8.0a0/pyadlml/model_selection/_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,36 +6,33 @@
 from contextlib import suppress
 from functools import partial
 from traceback import format_exc
 import numpy as np
 
 from joblib import Parallel, delayed, logger
 from itertools import product
-from sklearn.base import MetaEstimatorMixin, BaseEstimator, is_classifier, clone, _is_pairwise
+from sklearn.base import MetaEstimatorMixin, BaseEstimator, is_classifier, clone
 from sklearn.exceptions import NotFittedError, FitFailedWarning
 from sklearn.metrics import check_scoring
 from sklearn.metrics._scorer import _check_multimetric_scoring, _MultimetricScorer
 from sklearn.model_selection import check_cv
-from sklearn.model_selection._search import _check_param_grid, ParameterGrid, _normalize_score_results
+from sklearn.model_selection._search import ParameterGrid, _normalize_score_results
 from sklearn.model_selection._validation import _aggregate_score_dicts, _score
-from sklearn.utils import _deprecate_positional_args, _message_with_time, _safe_indexing
-from sklearn.utils.fixes import MaskedArray
+from sklearn.utils import _message_with_time, _safe_indexing
 from sklearn.utils.metaestimators import if_delegate_has_method# ,_safe_split
 from sklearn.utils.validation import check_is_fitted, indexable, _check_fit_params, _num_samples
 
 from pyadlml.pipeline import EvalOnlyWrapper, TrainOnlyWrapper, Pipeline, TrainOrEvalOnlyWrapper
-from pyadlml.preprocessing import CVSubset
 from sklearn.model_selection._search import BaseSearchCV as SklearnBaseSearchCV
 
 class BaseSearchCV(SklearnBaseSearchCV):
     """Abstract base class for hyper parameter search with cross-validation.
     """
 
     @abstractmethod
-    @_deprecate_positional_args
     def __init__(self, estimator, *, scoring=None, n_jobs=None,
                  online_train_val_split=False,
                  refit=True, cv=None, verbose=0,
                  pre_dispatch='2*n_jobs', error_score=np.nan,
                  return_train_score=True):
 
         SklearnBaseSearchCV.__init__(self, estimator=estimator, scoring=scoring, n_jobs=n_jobs,
@@ -351,15 +348,15 @@
 
             refit_start_time = time.time()
             if isinstance(self.best_estimator_, Pipeline):
                 self.best_estimator_.train()
                 # set the cross val splitter training range to the whole dataset
                 if self.online_train_val_split:
                     for estim in self.best_estimator_:
-                        if isinstance(estim, CVSubset) and isinstance(estim, TrainOnlyWrapper):
+                        if isinstance(estim, CrossValSplitter) and isinstance(estim, TrainOnlyWrapper):
                             tmp = np.arange(len(X))
                             estim.set_range(tmp)
                             break
 
             if y is not None:
                 self.best_estimator_.fit(X, y, **fit_params)
             else:
@@ -379,15 +376,14 @@
         return self
 
 class GridSearchCV(BaseSearchCV):
     """Exhaustive search over specified parameter values for an estimator.
     """
     _required_parameters = ["estimator", "param_grid"]
 
-    @_deprecate_positional_args
     def __init__(self, estimator, param_grid, *, online_train_val_split=False,
                  scoring=None, n_jobs=None, refit=True, cv=None,
                  verbose=0, pre_dispatch='2*n_jobs',
                  error_score=np.nan, return_train_score=False):
         super().__init__(
             estimator=estimator, scoring=scoring,
             online_train_val_split=online_train_val_split,
@@ -523,18 +519,18 @@
     if online_train_val_split:
         # inject the train and test data into the corresponding Subset selectors
         set_train_estim = False
         set_test_estim = False
         for estim in estimator:
             if set_train_estim and set_test_estim:
                 break
-            if isinstance(estim, CVSubset) and isinstance(estim, EvalOnlyWrapper):
+            if isinstance(estim, CrossValSplitter) and isinstance(estim, EvalOnlyWrapper):
                 estim.set_range(test)
                 set_test_estim = True
-            if isinstance(estim, CVSubset) and isinstance(estim, TrainOnlyWrapper):
+            if isinstance(estim, CrossValSplitter) and isinstance(estim, TrainOnlyWrapper):
                 estim.set_range(train)
                 set_train_estim = True
             # TODO delete unti 906 above
             if isinstance(estim, CVOnlineSplitter) and isinstance(estim, TrainOrEvalOnlyWrapper):
                 estim.set_train_range(train)
                 estim.set_test_range(test)
                 set_train_estim = True
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/pipeline.py` & `pyadlml-0.0.8.0a0/pyadlml/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 )
 
 from sklearn.utils.validation import check_memory, _deprecate_positional_args
 from sklearn.pipeline import Pipeline as SklearnPipeline, _fit_one, _transform_one
 import numpy as np
 import pandas as pd
 
+
 __all__ = ['Pipeline', 'YTransformer', 'XAndYTransformer', 'XOrYTransformer',
            'EvalOnlyWrapper', 'TrainOnlyWrapper']
 
 
 class YTransformer():
     """
     a class that inherits from YTransformer signals to the pipeline
@@ -133,20 +134,25 @@
         out[key] = self.wr
         if deep and hasattr(self.wr, 'get_params'):
             deep_items = self.wr.get_params().items()
             out.update((key + '__' + k, val) for k, val in deep_items)
         return out
 
 
+    def __repr__(self) -> str:
+        return f"Wrapped({self.wr.__repr__()})"
+
+
 class TrainOrEvalOnlyWrapper(Wrapper):
     def __init__(self, wr):
         Wrapper.__init__(self, wr)
 
 
 class TrainOnlyWrapper(Wrapper):
+
     def __init__(self, wr):
         Wrapper.__init__(self, wr)
 
 
 class EvalOnlyWrapper(Wrapper):
     def __init__(self, wr):
         Wrapper.__init__(self, wr)
@@ -261,14 +267,51 @@
 
     def is_in_eval_mode(self):
         return self._eval
 
     def is_in_prod_mode(self):
         return self._prod
 
+    def get_times(self):
+        from pyadlml.preprocessing.preprocessing import FinalTimeTransformer
+        for _, name, transform in self._iter():
+            if isinstance(transform, FinalTimeTransformer):
+                return transform.times_
+
+        raise ValueError('No transformer saved the forwarded times. Readjust the pipeline')
+
+
+    def construct_y_times_and_X(self, X_val, y_val):
+        from pyadlml.preprocessing.preprocessing import FinalTimeTransformer
+        from pyadlml.preprocessing.windows import Windows
+
+        final_time_name, win_name, win_pos = None, None, -1
+
+        for i, name, transform in self._iter():
+            if isinstance(transform, FinalTimeTransformer):
+                final_time_name = name
+            if isinstance(transform, Windows):
+                win_name = name
+                win_pos = i
+
+        assert final_time_name is not None, 'No final time transformer specified'
+
+        y_times = self[final_time_name].times_
+
+        if win_name is not None:
+            y_times = self[win_name].construct_target_times(y_times)
+            Xt_prae_win, _ = self[:win_pos-len(self)].transform(X_val, y_val)
+            X_at_times = self[win_name].construct_X_at_target(Xt_prae_win)
+        else:
+            X_at_times, _ = self[:-1].transform(X_val, y_val)
+
+        return y_times, X_at_times
+                        
+
+
     def __getitem__(self, ind):
         """Returns a sub-pipeline or a single esimtator in the pipeline
         Indexing with an integer will return an estimator; using a slice
         returns another Pipeline instance which copies a slice of this
         Pipeline. This copy is shallow: modifying (or fitting) estimators in
         the sub-pipeline will affect the larger pipeline and vice-versa.
         However, replacing a value in `step` will not affect a copy.
@@ -443,21 +486,24 @@
             fit_params_last_step = fit_params_steps[self.steps[-1][0]]
             if hasattr(last_step, 'fit_transform'):
                 return last_step.fit_transform(Xt, yt, **fit_params_last_step)
             else:
                 return last_step.fit(Xt, yt,
                                      **fit_params_last_step).transform(Xt)
 
-    def _transform(self, X, y=None, **transform_params):
+    def _transform(self, X, y=None, retrieve_last_time=False, **transform_params_steps):
         """
         Extends transform behavior by allowing for transform params and x or y transformation
         """
-        transform_params_steps = self._check_fit_params(**transform_params)
+        #transform_params_steps = self._check_fit_params(**transform_params)
 
         Xt = X
+        if retrieve_last_time:
+            memory = Xt.copy()
+
         if y is None:
             for _, name, transform in self._iter():
                 Xt = transform.transform(Xt, **transform_params_steps[name])
             return Xt
         else:
             yt = y
             for _, name, transform in self._iter():
@@ -466,14 +512,22 @@
                 if isinstance(transform, YTransformer):
                     yt = transform.transform(yt, Xt, **transform_params_steps[name])
                 elif isinstance(transform, XAndYTransformer) \
                         or isinstance(transform, XOrYTransformer):
                     Xt, yt = transform.transform(Xt, yt, **transform_params_steps[name])
                 else:
                     Xt = transform.transform(Xt, **transform_params_steps[name])
+
+                if retrieve_last_time:
+                    # Check if time column is 
+                    if 'time' not in Xt.columns:
+                        return memory['time']
+                    else:
+                        memory = Xt.copy()
+
             return Xt, yt
 
     @if_delegate_has_method(delegate='_final_estimator')
     def predict(self, X, **predict_params):
         """Apply transforms to the data, and predict with the final estimator
 
         Parameters
@@ -492,49 +546,90 @@
 
             .. versionadded:: 0.20
 
         Returns
         -------
         y_pred : array-like
         """
+        predict_params_steps = self._check_fit_params(**predict_params)
         Xt = X
         # TODO BUG in evaluation mode the transformed X_t and Xt for pipe.transform have different ouput
         for _, name, transform in self._iter(with_final=False):
             if self._skip_transform(transform) or isinstance(transform, YTransformer) \
                     or isinstance(transform, XAndYTransformer):
                 continue
 
-            Xt = transform.transform(Xt)
+            Xt = transform.transform(Xt, **predict_params_steps[name])
         return self.steps[-1][-1].predict(Xt, **predict_params)
 
     @if_delegate_has_method(delegate='_final_estimator')
-    def predict_proba(self, X):
+    def predict_proba(self, X, **predict_params):
         """Apply transforms, and predict_proba of the final estimator
 
         Parameters
         ----------
         X : iterable
             Data to predict on. Must fulfill input requirements of first step
             of the pipeline.
 
         Returns
         -------
         y_proba : array-like of shape (n_samples, n_classes)
         """
+
+        predict_proba_params_steps = self._check_fit_params(**predict_params)
         Xt = X
         for _, name, transform in self._iter(with_final=False):
             if self._skip_transform(transform) or isinstance(transform, YTransformer) \
                     or isinstance(transform, XAndYTransformer):
                 continue
             elif isinstance(transform, XOrYTransformer):
-                Xt, _ = transform.transform(Xt, None)
+                Xt, _ = transform.transform(Xt, None, **predict_proba_params_steps)
             else:
-                Xt = transform.transform(Xt)
+                Xt = transform.transform(Xt, **predict_proba_params_steps)
         return self.steps[-1][-1].predict_proba(Xt)
 
+
+    def transform(self, X, y, **transform_params):
+        """Transform the data, and apply `transform` with the final estimator.
+
+        Call `transform` of each transformer in the pipeline. The transformed
+        data are finally passed to the final estimator that calls
+        `transform` method. Only valid if the final estimator
+        implements `transform`.
+
+        This also works where final estimator is `None` in which case all prior
+        transformations are applied.
+
+        Parameters
+        ----------
+        X : iterable
+            Data to transform. Must fulfill input requirements of first step
+            of the pipeline.
+
+        Returns
+        -------
+        Xt : ndarray of shape (n_samples, n_transformed_features)
+            Transformed data.
+        """
+        tparams_steps, pipe_params = self._check_transform_params(**transform_params)
+        return self._transform(X, y, **pipe_params, **tparams_steps)
+
+
+    def _check_transform_params(self, **fit_params):
+        fit_params_steps = {name: {} for name, step in self.steps if step is not None}
+        pipe_params = {}
+        for pname, pval in fit_params.items():
+            if "__" not in pname:
+                pipe_params[pname] = pval
+                continue
+            step, param = pname.split("__", 1)
+            fit_params_steps[step][param] = pval
+        return fit_params_steps, pipe_params
+
     @if_delegate_has_method(delegate='_final_estimator')
     def decision_function(self, X):
         """Apply transforms, and decision_function of the final estimator
 
         Parameters
         ----------
         X : iterable
@@ -553,36 +648,37 @@
             elif isinstance(transform, XOrYTransformer):
                 Xt, _ = transform.transform(Xt, None)
             else:
                 Xt = transform.transform(Xt)
         return self.steps[-1][-1].decision_function(Xt)
 
     @if_delegate_has_method(delegate='_final_estimator')
-    def score_samples(self, X):
+    def score_samples(self, X, **score_params):
         """Apply transforms, and score_samples of the final estimator.
 
         Parameters
         ----------
         X : iterable
             Data to predict on. Must fulfill input requirements of first step
             of the pipeline.
 
         Returns
         -------
         y_score : ndarray of shape (n_samples,)
         """
+        score_params_steps = self._check_fit_params(**score_params)
         Xt = X
-        for _, _, transformer in self._iter(with_final=False):
+        for _, name, transformer in self._iter(with_final=False):
             if self._skip_transform(transformer) or isinstance(transformer, YTransformer) \
                     or isinstance(transformer, XAndYTransformer):
                 continue
             elif isinstance(transformer, XOrYTransformer):
-                Xt, _ = transformer.fit_transform(Xt, None)
+                Xt, _ = transformer.fit_transform(Xt, None, score_params[name])
             else:
-                Xt = transformer.transform(Xt)
+                Xt = transformer.transform(Xt, **score_params[name])
         return self.steps[-1][-1].score_samples(Xt)
 
     @if_delegate_has_method(delegate='_final_estimator')
     def predict_log_proba(self, X):
         """Apply transforms, and predict_log_proba of the final estimator
 
         Parameters
@@ -603,15 +699,15 @@
             elif isinstance(transform, XOrYTransformer):
                 Xt, _ = transform.fit_transform(Xt, None)
             else:
                 Xt = transform.transform(Xt)
         return self.steps[-1][-1].predict_log_proba(Xt)
 
     @if_delegate_has_method(delegate='_final_estimator')
-    def score(self, X, y=None, sample_weight=None):
+    def score(self, X, y=None, sample_weight=None, **score_params):
         """Apply transforms, and score with the final estimator
 
         Parameters
         ----------
         X : iterable
             Data to predict on. Must fulfill input rquirements of first step
             of the pipeline.
@@ -626,29 +722,31 @@
 
         Returns
         -------
         score : float
         """
         Xt = X
         yt = y
+        score_params_steps = self._check_fit_params(**score_params)
+
         for _, name, transform in self._iter(with_final=False):
             if self._skip_transform(transform):
                 continue
             elif isinstance(transform, XOrYTransformer):
-                Xt, yt = transform.transform(Xt, yt)
+                Xt, yt = transform.transform(Xt, yt, **score_params_steps[name])
             elif isinstance(transform, YTransformer):
-                yt = transform.transform(yt, Xt)
+                yt = transform.transform(yt, Xt, **score_params_steps[name])
             elif isinstance(transform, XAndYTransformer):
-                Xt, yt = transform.transform(Xt, yt)
+                Xt, yt = transform.transform(Xt, yt, **score_params_steps[name])
             else:
-                Xt = transform.transform(Xt)
+                Xt = transform.transform(Xt, **score_params_steps[name])
         score_params = {}
         if sample_weight is not None:
             score_params['sample_weight'] = sample_weight
-        return self.steps[-1][-1].score(Xt, yt, **score_params)
+        return self.steps[-1][-1].score(Xt, yt)
 
 
 def _fit_transform_one(transformer,
                        X,
                        y,
                        weight,
                        message_clsname='',
@@ -858,8 +956,8 @@
             delayed(_transform_one)(trans, X, None, weight)
             for name, trans, weight in self._iter())
         if not Xs:
             # All transformers are None
             return np.zeros((X.shape[0], 0))
 
         Xs = self._filter_skips(Xs)
-        return self._custom_hstack(Xs)
+        return self._custom_hstack(Xs)
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/plot/__init__.py` & `pyadlml-0.0.8.0a0/pyadlml/plot/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,54 @@
-from pyadlml.dataset.matplotlib.act_and_devs import (
+from pyadlml.dataset.plot.matplotlib.act_and_devs import (
     plot_contingency_states as plot_contingency_states,
     contingency_events as plot_contingency_events,
     activities_and_device_states as plot_activities_and_states,
     activities_and_device_events as plot_activities_and_events
 )
 
-from pyadlml.dataset.plotly.acts_and_devs import (
+from pyadlml.dataset.plot.plotly.acts_and_devs import (
     contingency_states as plotly_contingency_states,
     contingency_events as plotly_contingency_events,
     activities_and_devices as plotly_activities_and_devices,
+    event_correlogram as plotly_activities_vs_devices_correlogram,
+    activity_vs_device_events_hist as plotly_activities_vs_devices_histogram
 )
 
-from pyadlml.dataset.matplotlib.activities import (
+from pyadlml.dataset.plot.matplotlib.activities import (
     count as plot_activity_count,
     boxplot as plot_activity_boxplot,
     duration as plot_activity_duration,
     transitions as plot_activity_transitions,
     density as plot_activity_density,
     correction as plot_activity_correction
 )
 
-from pyadlml.dataset.plotly.activities import (
-    density as plotly_activity_density,
-    bar_count as plotly_activity_bar_count,
+from pyadlml.dataset.plot.plotly.activities import (
+    bar_count as plotly_activity_count,
+    boxplot_duration as plotly_activity_boxplot,
+    activity_duration as plotly_activity_duration,
     heatmap_transitions as plotly_activity_transitions,
-    boxplot_duration as plotly_activity_boxplot_duration,
+    density as plotly_activity_density,
     bar_cum as plotly_activity_duration,
 )
 
-from pyadlml.dataset.matplotlib.devices import (
+from pyadlml.dataset.plot.matplotlib.devices import (
+    states as plot_device_states,
     state_fractions as plot_device_state_fractions,
     state_boxplot as plot_device_state_boxplot,
     state_similarity as plot_device_state_cross_correlation,
-    states as plot_device_states,
-    inter_event_intervals as plot_device_inter_event_intervals,
+    inter_event_intervals as plot_device_inter_event_times,
     event_density_one_day as plot_device_event_density,
     event_count as plot_device_event_count,
     event_raster as plot_device_event_raster,
     event_cross_correlogram as plot_device_event_correlogram,
 )
 
-from pyadlml.dataset.plotly.devices import (
+from pyadlml.dataset.plot.plotly.devices import (
+    state_times as plotly_device_states, 
+    fraction as plotly_device_state_fractions,
+    boxplot_state as plotly_device_state_boxplot,
     bar_count as plotly_device_event_count,
-)
-
-from pyadlml.dataset.matplotlib.util import (
-    plot_cv_impact_parameter,
+    event_density as plotly_device_event_density,
+    device_iei as plotly_device_inter_event_times,
+    plotly_device_event_correlogram as plotly_device_event_correlogram,
 )
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/plot/_benchmark.py` & `pyadlml-0.0.8.0a0/pyadlml/plot/_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/plot/explanation.py` & `pyadlml-0.0.8.0a0/pyadlml/plot/explanation.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/plot/feature_importance.py` & `pyadlml-0.0.8.0a0/pyadlml/plot/feature_importance.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/plot/interpretation.py` & `pyadlml-0.0.8.0a0/pyadlml/plot/interpretation.py`

 * *Files identical despite different names*

### Comparing `pyadlml-0.0.7.9a0/pyadlml/preprocessing.py` & `pyadlml-0.0.8.0a0/pyadlml/preprocessing/preprocessing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 import pandas as pd
 import numpy as np
+from copy import copy
+from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.preprocessing import OneHotEncoder as SkOneHotEncoder
+from sklearn.compose import ColumnTransformer
+import pandas as pd
+
 
 from sklearn.utils.metaestimators import _safe_split
 import sklearn.preprocessing as preprocessing
 from sklearn.base import BaseEstimator, TransformerMixin
 
-from pyadlml.dataset._representations.raw import create_raw, resample_raw
+from pyadlml.dataset._representations.state import create_state, resample_state
 from pyadlml.dataset._representations.changepoint import create_changepoint, resample_changepoint
 from pyadlml.dataset._representations.lastfired import create_lastfired, resample_last_fired
-from pyadlml.dataset._core._dataset import label_data
+from pyadlml.dataset._core.acts_and_devs import label_data, label_data2
 from pyadlml.constants import ACTIVITY, TIME, DEVICE, VALUE, END_TIME, START_TIME, \
-                              ENC_RAW, ENC_LF, ENC_CP, REPS
+    ENC_STATE, ENC_LF, ENC_CP, REPS
 from pyadlml.dataset._core.devices import create_device_info_dict
 from pyadlml.pipeline import XOrYTransformer, XAndYTransformer, YTransformer
+from pyadlml.constants import OTHER
+from sklearn.base import BaseEstimator, TransformerMixin
+import numpy as np
+import pandas as pd
+from plotly import graph_objects as go
+from pyadlml.constants import *
+import matplotlib.pyplot as plt
+
+__all__ = []
 
 
 class Df2Numpy(TransformerMixin, XOrYTransformer):
     """ Transforms dataframes to numpy arrays by respecting
     the column order
     """
     _x_columns = []
@@ -26,18 +41,17 @@
         pass
 
     def fit(self, X, y=None):
         self._x_columns = X.columns
         if y is not None:
             self._y_columns = y.columns
 
-
     def fit_transform(self, X, y):
-        self.fit(X,y)
-        return self.transform(X,y)
+        self.fit(X, y)
+        return self.transform(X, y)
 
     def transform(self, X, y):
         # reorder columns
         X = X[self._x_columns]
         y = y[self._y_columns]
 
         #
@@ -63,15 +77,14 @@
         assert self.y_conv in [self.Df2Numpy, self.Df2Torch]
         assert self.x_conv in [self.Df2Numpy, self.Df2Torch]
 
         self._x_columns = X.columns
         if y is not None:
             self._y_columns = y.columns
 
-
     def fit_transform(self, X, y=None):
         self.fit(X, y=y)
         return self.transform(X, y=y)
 
     def transform(self, X, y=None):
         """
         Parameters
@@ -114,18 +127,17 @@
         self.only_X = only_X
 
     def fit(self, X, y=None):
         self._x_columns = X.columns
         if y is not None:
             self._y_columns = y.columns
 
-
     def fit_transform(self, X, y):
-        self.fit(X,y)
-        return self.transform(X,y)
+        self.fit(X, y)
+        return self.transform(X, y)
 
     def transform(self, X, y):
         """
         Parameters
         ----------
         X : pd
         """
@@ -138,15 +150,15 @@
         # cast to tensors
         y_tensor = torch.tensor(y.values, dtype=torch.int64)
         X_tensor = torch.tensor(X.values, dtype=torch.float32)
 
         return X_tensor, y_tensor
 
 
-class IdentityTransformer(TransformerMixin, XOrYTransformer):
+class Identity(TransformerMixin, XOrYTransformer):
     def __init__(self):
         pass
 
     def fit(self, X, y=None):
         return self
 
     @XOrYTransformer.x_or_y_transform
@@ -165,22 +177,23 @@
         return self
 
     def fit_transform(self, X, y, **fit_params):
         self.fit(X, y)
         return self.transform(X, y)
 
     def transform(self, X, y):
-        return self.rus_.fit_resample(X,y)
+        return self.rus_.fit_resample(X, y)
 
 
 class DropNanRows(XOrYTransformer):
     """
     Drops all rows where the label or the data has a nan-value
     """
-    def fit(self, X,y=None):
+
+    def fit(self, X, y=None):
         return self
 
     def fit_transform(self, X, y=None):
         return self.transform(X, y=y)
 
     def transform(self, X, y=None):
         """
@@ -195,142 +208,156 @@
                 raise NotImplementedError
         else:
             nan_mask = X.isna().values
             return X[~nan_mask]
 
 
 class DropDuplicates(TransformerMixin, XOrYTransformer):
-    def __init__(self):
+    def __init__(self, ignore_columns=[], merge_on='time'):
         BaseEstimator.__init__(self)
         XOrYTransformer.__init__(self)
 
+        self.ignore_columns = [ignore_columns] if not isinstance(
+            ignore_columns, list) else ignore_columns
+        self.merge_on = merge_on
+
     def fit(self, X, y=None):
         return self
 
     def fit_transform(self, X, y=None, **fit_params):
         return self.transform(X, y)
 
     @XOrYTransformer.x_or_y_transform
     def transform(self, X=None, y=None):
         """  Depending if X or y is given drop either all Nans in y or all nans in X or
         all Nans in the union of X and y.
 
         """
         if y is not None and X is not None:
             assert isinstance(y, pd.DataFrame)
-            tmp = X.copy()
-            tmp['y'] = y
-            tmp = tmp.drop_duplicates()
-            y = tmp['y']
-            X = tmp.drop('y', axis=1)
+            tmp = X.copy().reset_index(drop=True)
+            y = y.copy().reset_index(drop=True)
+
+            y_cols = y.columns.to_list()
+            if len(y.columns) > 1:
+                y_cols.remove(self.merge_on)
+                tmp = tmp.merge(y, on=self.merge_on)
+            else:
+                tmp[y_cols] = y
+            comp_cols = list(set(tmp.columns) - set(self.ignore_columns))
+            dup_mask = tmp[comp_cols].duplicated()
+
+            y = y[~dup_mask].reset_index(drop=True)
+            X = X[~dup_mask].reset_index(drop=True)
+
         if y is not None and X is None:
             y = y.drop_duplicates()
-        if X is not None:
+        if X is not None and y is None:
             X = X.drop_duplicates()
         return X, y
 
 
-class DropTimeIndex(TransformerMixin, XOrYTransformer):
-    def __init__(self):
+class FinalTimeTransformer():
+    pass
+
+
+class DropTimeIndex(TransformerMixin, XOrYTransformer, FinalTimeTransformer):
+    def __init__(self, only_y=False):
         XOrYTransformer.__init__(self)
+        self.only_y = only_y
 
-    def fit_transform(self, X, y=None, **fit_params):
-        """
-        drops columns that are not time dependent
+    def __repr__(self):
+        return f'{self.__class__.__name__}()'
+
+    def fit(self, X=None, y=None):
+        return self
+
+    def fit_transform(self, X=None, y=None, **fit_params):
+        """ Drops columns that are not time dependent
         """
         return self.transform(X, y)
 
     @XOrYTransformer.x_or_y_transform
     def transform(self, X=None, y=None):
-        if X is not None:
+        if X is not None and not self.only_y:
+            self.times_ = X[TIME]
             X = X.loc[:, X.columns != TIME]
         if y is not None:
             y = y.loc[:, y.columns != TIME]
         return X, y
 
 
-class CVSubset(TransformerMixin, XOrYTransformer):
-    """ Selects the subset from the whole dataset based on a given data_range.
+class Encoder():
+    features_ = None
 
-    Attributes
-    ----------
-    data_range  : list of either indices or interval
-        Either
-    y : boolean, default=False
-        Only
-
-    """
-    def __init__(self, data_range=None, y=False):
-        self.data_range = data_range
-        XOrYTransformer.__init__(self)
+    def to_dataframe(self, X, onehot=False):
+        print()
+        raise NotImplementedError
 
-    def set_range(self, data_range):
-        self.data_range = data_range
 
-    def _extract_first_sample(self, data_range):
-        try:
-            sample = data_range[0][0]
-        except TypeError:
-            sample = data_range[0]
-        except IndexError:
-            sample = data_range[0]
-        return sample
+class IndexEncoder():
 
+    def __repr__(self):
+        return f'{self.__class__.__name__}()'
 
     def fit(self, X, y=None):
-        error_msg = "Data range has to be set to either time intervals or list of indicies. Not 'None'"
-        assert self.data_range is not None, error_msg
+        self.n_features_in_ = 3
+        self.lbl_enc = preprocessing.LabelEncoder()
+        self.lbl_enc.fit(X[DEVICE])
 
-        # determine whether the splits are made based on index ranges or timestamp tuples
-        sample = self._extract_first_sample(self.data_range)
-        self.timestamps_ = not (isinstance(sample, int) or isinstance(sample, np.int64))
+    def transform(self, X, y=None):
+        X[DEVICE] = self.lbl_enc.transform(X[DEVICE])
+        return X
 
-        return self
+    def inverse_transform(self, X):
+        return self.lbl_enc.inverse_transform(X)
 
     def fit_transform(self, X, y=None):
-        self.fit(X, y)
+        self.fit(X, y=None)
         return self.transform(X, y)
 
-    @XOrYTransformer.x_or_y_transform
-    def transform(self, X, y=None):
-        """ Selects a subset of X and y based on the data_range and the split type
+    def onehot(self, X: np.ndarray):
+        """ Create one-hot encoding for given array of indices with
+            correct feature labels assigned
         """
-        if self.timestamps_:
-            x_mask = _create_mask(X, self.data_range)
-            X = X[x_mask]
-            if y is not None:
-                assert len(X) == len(y)
-                y_mask = _create_mask(y, self.data_range)
-                y = y[y_mask]
-            return X, y
-        else:
-            X, y = _safe_split(None, X, y, self.data_range)
-            return X, y
-
-
-def _create_mask(X, date_range):
-    x_mask = (X[TIME] == 'false_init')
-    if isinstance(date_range, tuple):
-        date_range = [date_range]
-    for time_pair in date_range:
-        x_mask = x_mask | ((time_pair[0] < X[TIME]) & (X[TIME] < time_pair[1]))
-    return x_mask
+        n_values = np.max(X) + 1
+        values = list(X)
+        onehot = np.eye(n_values)[values]
+        columns = self.inverse_transform(np.arange(n_values))
+        onehot = pd.DataFrame(onehot, columns=columns)
+        return onehot
 
 
-class StateVectorEncoder(BaseEstimator, TransformerMixin):
+class DropColumn():
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}(column_name='{self.column_name}')"
+
+    def __init__(self, column_name):
+        self.column_name = column_name
+
+    def transform(self, X, y=None):
+        X = X.drop(columns=self.column_name)
+        return X
+
+    def fit_transform(self, X, y=None):
+        return self.transform(X, y)
+
+
+class Event2Vec(Encoder, BaseEstimator, TransformerMixin):
     """
-    Create a State-vector sequence from a device event stream.
+    Create a sequence of vectors from a device event stream.
     Read more in the :ref:`User Guide <preprocessing_discretization>`.
 
     Parameters
     ----------
-    encode : {'raw', 'changepoint', 'last_fired'}, default='raw'
+    encode : {'state', 'changepoint', 'last_fired'}, default='raw'
         Determines the state-vectors encoding.
 
-        raw
+        state 
             Encode the event stream as vector, where each field
             represents a device. Each entry represents the current
             state that the device is in.
 
         changepoint
             Encode the event stream as one-hot binary vector, where
             each field represents a device. A one indicates the
@@ -340,49 +367,53 @@
             Encode the event stream as one-hot binary vector,
             where each field represents a device. The device that produced
             the last event is indicated with one.
 
     dt : str, optional, default=None
         The timeslices resolution for discretizing the event stream. If
         set to None the event stream is not discretized.
+    
+    out_names: 
 
     Attributes
     ----------
     encode : string
         The encoding for the vectors
     dt : str or None
-        Determines the binsize that the event stream is discretized into
+        If not None, determines the binsize the event stream is discretized into
     data_info_ : dict or None
         Dictionary containing further device information such as most likely value
         or device datatype. This is used to speed up internal computation.
     classes_ : list
         A list of all devices. The lists order corresponds to the device order of the
         transformed state-vectors.
 
     Examples
     --------
     >>> from pyadlml.dataset import fetch_amsterdam
     >>> data = fetch_amsterdam()
-    >>> from pyadlml.preprocessing import StateVectorEncoder
-    >>> sve = StateVectorEncoder(encode='raw')
-    >>> X = sve.fit_transform(data.df_devices)
-    >>> sve2 = StateVectorEncoder(encode='changepoint+raw', dt='6s')
-    >>> X_upsampled = sve2.fit_transform(data.df_devices)
+    >>> from pyadlml.preprocessing import Event2Vec
+    >>> e2v = Event2Vec(encode='state')
+    >>> X = e2v.fit_transform(data['devices'])
+    >>> e2v_p = Event2Vec(encode='changepoint+raw', dt='6s')
+    >>> X_resampled = e2v_p.fit_transform(data['devices])
 
     """
 
-    def __init__(self, encode=ENC_RAW, dt=None):
+    def __init__(self, encode='state', dt=None, out_features=[], n_jobs=None):
+        super().__init__()
         self.encode = encode
         self.dt = dt
-        self.data_info_ = None
-        self.classes_ = []
+        self.out_features = out_features
+        self.n_jobs = n_jobs
 
     @classmethod
     def _is_valid_encoding(cls, encoding):
         from itertools import chain, permutations
+
         def helper(iterable):
             s = list(iterable)
             return chain.from_iterable(permutations(s, r) for r in range(len(s)+1))
         # generate all possible valid combinations
         valid_combos = ['+'.join(combo) for combo in helper(REPS)]
         return encoding in valid_combos
 
@@ -399,100 +430,122 @@
             Ignored. This parameter exists only for compatibility with
             :class:`~sklearn.pipeline.Pipeline`.
 
         Returns
         -------
         self
         """
-        assert StateVectorEncoder._is_valid_encoding(self.encode)
+        assert Event2Vec._is_valid_encoding(self.encode)
 
-        # create hashmap off all input features with mean for numerical
+        # Create dict off all input features with mean for numerical
         # and most common value for binary or categorical features
         self.data_info_ = create_device_info_dict(df_devs)
-        self.classes_ = self.data_info_.keys()
+        self.n_features_in_ = 3
+        self.features_in_ = [TIME, DEVICE, VALUE]
+        if self.out_features:
+            feature_names_out = self.out_features
+            del (self.out_features)
+        else:
+            feature_names_out = list(self.data_info_.keys())
+
+        feature_names_out.sort()
+        self.feature_names_out_ = [TIME] + feature_names_out
+
+        self.n_features_out = len(self.feature_names_out_)
+
         return self
 
-    def transform(self, df_devs=None,y=None, dev_pre_values={}):
+    def transform(self, df_devs=None, y=None, initial_states={}):
         """
         Discretize the data.
 
         Parameters
         ----------
         df_devs : array-like of shape (n_samples, n_features)
             The device dataframe to be transformed.
         y : None
             todo copy standard scipy sentence
-        dev_pre_values : dict
-            A dictionary containing a device-value mapping that is used
-            to fill in information . If no dictionary is given the values are infered by
-            most likely values for categorical and boolean devices.
+        initial_states : dict
+            A dictionary with device state mapping containing information about
+            the last state the device held before the first event. If no dictionary 
+            is given the states are infered by most likely values for 
+            categorical and boolean devices.
 
         Returns
         -------
         Xt : {ndarray, sparse matrix}, dtype={np.float32, np.float64}
             Data in the binned space. Will be a sparse matrix if
             `self.encode='onehot'` and ndarray otherwise.
         """
         PRAEFIX_LF = 'lf_'
         PRAEFIX_CP = 'cp_'
 
-
         df_lst = []
         iters = self.encode.split('+')
+        df_devs[DEVICE] = df_devs[DEVICE].astype('category')
         for enc in iters:
-            if enc == ENC_RAW:
-                data = create_raw(df_devs, self.data_info_, dev_pre_values=dev_pre_values)
-                if self.dt is not None:
-                    data = resample_raw(data, df_dev=df_devs, dt=self.dt,
-                                        most_likely_values=self.data_info_
-                                        )
+            if enc == ENC_STATE:
+                if self.dt is None:
+                    data = create_state(df_devs, self.data_info_,
+                                    dev_pre_values=initial_states)
+                else:
+                    data = resample_state(
+                            df_dev=df_devs, 
+                            dt=self.dt,
+                            most_likely_values=self.data_info_
+                    )
 
                 # convert boolean data into integers (1,0)
-                dev_bool = [dev for dev in self.data_info_.keys() if self.data_info_[dev]['dtype'] == 'boolean']
-                data[dev_bool] = data[dev_bool].astype(int)
+                dev_bool = [dev for dev in self.data_info_.keys() if self.data_info_[
+                    dev]['dtype'] == BOOL]
+                data[dev_bool] = data[dev_bool].applymap(
+                    lambda x: 1 if x == True else 0)
 
             elif enc == ENC_CP:
-                data = create_changepoint(df_devs)
-                if self.dt is not None:
-                    data = resample_changepoint(data, self.dt)
+                if self.dt is None:
+                    data = create_changepoint(df_devs, self.n_jobs)
+                else:
+                    data = resample_changepoint(df_devs, self.dt, self.n_jobs)
 
                 # set values that are missing in transform but were present when fitting to 0
-                dev_diff = set(self.classes_) - set(data.columns)
+                dev_diff = set(self.feature_names_out_) - set(data.columns)
                 if len(dev_diff) > 0:
                     for dev in dev_diff:
                         data[dev] = 0
 
                 # add prefix to make column names unique
                 if len(iters) > 1:
-                    data.columns = [TIME] + list(map(PRAEFIX_CP.__add__, data.columns[1:]))
-
+                    data.columns = [
+                        TIME] + list(map(PRAEFIX_CP.__add__, data.columns[1:]))
 
             elif enc == ENC_LF:
-                data = create_lastfired(df_devs)
-                if self.dt is not None:
-                    data = resample_last_fired(data, self.dt)
+                if self.dt is None:
+                    data = create_lastfired(df_devs)
+                else:
+                    data = resample_last_fired(df_devs, self.dt, self.n_jobs)
 
                 # set values that are missing in transform but were present when fitting to 0
-                dev_diff = set(self.classes_) - set(data.columns)
+                dev_diff = set(self.feature_names_out_) - set(data.columns)
                 if len(dev_diff) > 0:
                     for dev in dev_diff:
                         data[dev] = 0
 
                 # add prefix to make column names unique
                 if len(iters) > 1:
-                    data.columns = [TIME] + list(map(PRAEFIX_LF.__add__, data.columns[1:]))
+                    data.columns = [
+                        TIME] + list(map(PRAEFIX_LF.__add__, data.columns[1:]))
 
             else:
                 raise ValueError
             data = data.set_index(TIME)
             df_lst.append(data)
 
-        data = pd.concat(df_lst, axis=1).reset_index()
-        return data
-
+        df_res = pd.concat(df_lst, axis=1).reset_index()
+        # Ensure to always return feature columns in order
+        return df_res[self.feature_names_out_]
 
     def fit_transform(self, df_devs, y=None):
         """
 
         Parameters
         ----------
         df_devs : pd.DataFrame, optional
@@ -502,31 +555,56 @@
             Ignored. This parameter exists only for compatibility with
             :class:`~sklearn.pipeline.Pipeline`.
         """
         self.fit(df_devs)
         return self.transform(df_devs)
 
 
-class LabelEncoder(BaseEstimator, TransformerMixin, YTransformer):
+class LabelMatcher(BaseEstimator, TransformerMixin, YTransformer):
     """
     Labels a dataframe with corresponding activities
 
     Attributes
     ----------
-    idle : bool, default=False
+    other : bool, default=False
         If true items that are not
 
     """
-    def __init__(self, idle=False):
+
+    def __init__(self, other: bool = False, encode_labels=False, use_dask=False, classes=[]):
         """
+        Initialize the object of the class with the given parameters.
+
+        Parameters
+        ----------
+        other : bool, optional
+            A boolean parameter to indicate whether to include the 'other' activity in the processing,
+            the functionality depends on the specifics of the use case (default is False).
+
+        encode_labels : bool, optional
+            A flag to specify if labels are encoded or not. If true, labels will be encoded
+            as integers based on classes defined. (default is False).
+
+        use_dask : bool, optional
+            A flag to indicate whether to use Dask for parallel computations. If true, computations 
+            will be carried out in parallel to improve efficiency (default is False).
+
+        classes : list of str, optional
+            A list of predefined class labels for the data. This is particularly useful in scenarios 
+            such as cross-validation where some classes may not be present in the training data, 
+            but may exist in the validation data (default is []).
+
         Returns
         -------
-        self
+        None
         """
-        self.idle = idle
+        self.other = other
+        self.use_dask = use_dask
+        self.encode_labels = encode_labels
+        self.classes = classes
 
     def fit(self, y, X):
         """
         Fit label encoder.
 
         Parameters
         ----------
@@ -534,26 +612,40 @@
             recorded activities from a dataset. Fore more information refer to the
             :ref:`user guide<activity_dataframe>`.
 
         Returns
         -------
         self : returns an instance of self
         """
-        self.lbl_enc_ = preprocessing.LabelEncoder()
         self.df_acts_ = y
+        if self.classes:
+            self.classes_ = self.classes
+            del (self.classes)
+        else:
+            self.classes_ = list(y[ACTIVITY].unique())
+
+        if self.other and OTHER not in self.classes_:
+            self.classes_.append(OTHER)
+        self.classes_.sort()
 
-        # add actvities to sklearns LabelEncoder
-        activities = list(y[ACTIVITY].values)
-        if self.idle:
-            activities.append('idle')
-            # todo code-smells import constant idle activity
-        self.lbl_enc_.fit(activities)
-        self.classes_ = self.lbl_enc_.classes_
         return self
 
+    def class2int_(self, x=None):
+        f = {v: k for k, v in enumerate(self.classes_)}.get
+        if x is None:
+            return f
+        else:
+            return f(x)
+
+    def int2class_(self, x=None):
+        f = {k: v for k, v in enumerate(self.classes_)}.get
+        if x is None:
+            return f
+        else:
+            return f(x)
 
     def fit_transform(self, y, X):
         """
         Fit label encoder and return encoded labels.
 
         Parameters
         ----------
@@ -567,266 +659,463 @@
         ------
         df : pd.DataFrame
             The X dataframe with an additional column containing the corresponding activity labels
         """
         self.fit(y, X)
         return self.transform(y, X)
 
-    def inverse_transform(self, y, retain_index=False):
-        """
-        Transform labels back to original encoding.
-
-        Parameters
-        ----------
-        x : array like or pd.DataFrame or pd.Series
-            array of numbers that are transformed to labels
-        retain_index : bool, default=False
-            TODO
-
-        Returns
-        -------
-            TODO
-        """
-        raise NotImplementedError
-        #if isinstance(x, np.ndarray):
-        #    res = self._lbl_enc.inverse_transform(x)
-        #    if retain_index:
-        #        return pd.Series(data=res, index=self.df_devs.index[:len(res)])
-        #    else:
-        #        return res
-        #
-        #elif isinstance(x, pd.DataFrame) or isinstance(x, pd.Series):
-        #    tmp_index = x.index
-        #    res = self._lbl_enc.inverse_transform(x.values)
-        #    return pd.Series(data=res, index=tmp_index)
-        #else:
-        #    raise ValueError
+    def _is_iterable(self, z):
+        try:
+            iter(z)
+            return True
+        except:
+            return False
+
+    def _wrap_iterable(self, lst, iter):
+        """ list 
+        """
+        if isinstance(iter, np.ndarray):
+            return np.array(lst)
+        elif isinstance(iter, list):
+            return lst
+        elif isinstance(iter, list):
+            return lst
+        elif isinstance(iter, pd.Series):
+            tmp = pd.Series(lst)
+            tmp.index = iter.index
+            return tmp
+        else:
+            raise NotImplementedError
 
-    def transform(self, y, X=None):
+    def transform(self, y: pd.DataFrame, X: pd.DataFrame = None) -> pd.DataFrame:
         """
 
         Parameters
         ----------
         y : pd.DataFrame
             An activity dataframe
         X : pd.DataFrame
             A device dataframe
 
+        Returns
+        -------
+        pd.DataFrame
+            A dataframe with column TIME, ACTIVITY matchin the rows of X
+            TODO asdf
         """
         # normal case where X an y are provided
-        if X is not None:
-            df = label_data(X, y, self.idle)
-            # remove Nans before encoding the labels and then concatenate again
-            if not self.idle:
-                nan_mask = df[ACTIVITY].isna()
-                df_san_nan = df[~nan_mask]
-                encoded_labels = self.lbl_enc_.transform(df_san_nan[ACTIVITY].values)
-                new_san_nan = pd.DataFrame(data={TIME: df_san_nan[TIME].values, ACTIVITY: encoded_labels})
-                new_nans = pd.DataFrame(data={TIME: df[nan_mask][TIME].values, ACTIVITY: np.nan})
-                return pd.concat([new_nans, new_san_nan]).sort_values(by=TIME)
-            else:
-                encoded_labels = self.lbl_enc_.transform(df[ACTIVITY].values)
-                return pd.DataFrame(data={TIME: df[TIME].values, ACTIVITY: encoded_labels})
+        n_jobs = 1000 if self.use_dask else 1
+        df = label_data2(X, y, self.other)[
+            [TIME, ACTIVITY]].copy()
+        if self.encode_labels:
+            df[ACTIVITY] = df[ACTIVITY].map(self.class2int_())
+        return df
 
-        ## case where X is a activity dataframe
-        #if isinstance(X, pd.DataFrame) and set(X.columns) == {START_TIME, END_TIME, ACTIVITY}:
-        #    df = label_data(X, self.df_acts, self.idle)
-        #    encoded_labels = self._lbl_enc.fit_transform(df[ACTIVITY].values)
-        #    return pd.DataFrame(index=df[TIME], data=encoded_labels, columns=[ACTIVITY])
 
+class DropDevices(BaseEstimator, XAndYTransformer, TransformerMixin):
+    def __init__(self, devices=[]):
+        self.devices = devices
 
-        ## case where X is a device dataframe
-        #if isinstance(X, pd.DataFrame) and TIME in X.columns:
-        #    df = label_data(X, self.df_acts_, self.idle)
-        #    encoded_labels = self.lbl_enc_.transform(df[ACTIVITY].values)
-        #    return pd.DataFrame(data={TIME: df[TIME].values, ACTIVITY: encoded_labels})
+    def fit_transform(self, X, y):
+        return self.transform(X, y)
 
-        ## return only the labels for a nd array
-        #elif isinstance(X, np.ndarray):
-        #    return self.lbl_enc_.transform(X)
+    def transform(self, X, y):
+        idxs = X[X[DEVICE].isin(self.devices)].index.values
+        return X[idxs], y[idxs]
 
-        else:
-            raise ValueError
 
+class KeepOnlyDevices(BaseEstimator, XAndYTransformer, TransformerMixin):
+    def __init__(self, devices=[], ignore_y=False):
+        self.devices = devices
+        self.ignore_y = ignore_y
 
-class SequenceSlicer(TransformerMixin, XOrYTransformer):
-    """ Slices a sequence into batches.
+    def fit_transform(self, X, y):
+        return self.transform(X, y)
 
-    Parameters
-    ----------
+    def transform(self, X, y):
+        idxs = X[X[DEVICE].isin(self.devices)].index.values
+        y = y[idxs] if not self.ignore_y else y
+        return X.loc[idxs, :], y
 
-    .. image:: ../_static/images/many_to_many.svg
-       :height: 200px
-       :width: 500 px
-       :scale: 90%
-       :alt: alternate text
-       :align: center
 
+class Timestamp2Seqtime(BaseEstimator, TransformerMixin, XOrYTransformer, FinalTimeTransformer):
+    def __init__(self, dt='s'):
+        super().__init__()
+        self.dt = dt
 
-    .. image:: ../_static/images/reps/image.svg
-       :height: 200px
-       :width: 500 px
-       :scale: 80%
-       :alt: alternate text
-       :align: center
+    @XOrYTransformer.x_or_y_transform
+    def fit_transform(self, X, y=None):
+        X, y = self.fit(X, y)
+        return self.transform(X, y)
 
+    def fit(self, X, y=None):
+        assert self.dt in ['ms', 's', 'm', 'h']
+        return X, y
 
-    Many-To-Many
-    ^^^^^^^^^^^^
+    def transform(self, X, y=None):
+        """ Change every timestamp into unit i.e. seconds relative
+            to the first timestamp in the sequence.
+        """
+        self.time = X[TIME]
+        X[TIME] -= X[TIME].iloc[0]
+        if self.dt == 'ms':
+            X[TIME] = X[TIME]/pd.Timedelta('1milli')
+        elif self.dt == 's':
+            X[TIME] = X[TIME]/pd.Timedelta('1sec')
+        elif self.dt == 'm' or self.dt == 'min':
+            X[TIME] = X[TIME]/pd.Timedelta('1min')
+        elif self.dt == 'h':
+            X[TIME] = X[TIME]/pd.Timedelta('1hr')
+        return X, y
 
-    To get *many-to-many* batches use the window size :math:`w` to split the data
 
-    .. math::
-        f(X_{N,K},y_{N}) \rightarrow (X_{W, N,K}, y_{W, N})
+class SkTime(BaseEstimator, XAndYTransformer):
 
-    In addition you can specify a stride.
+    def __init__(self, rep='nested_univ'):
+        self.rep = rep
 
+    def fit(self, X, y):
+        assert self.rep in ['nested_univ', 'numpy3d']
 
-    .. code:: python
+    def fit_transform(self, X, y):
+        self.fit(X, y)
+        return self.transform(X, y)
 
-        from pyadlml.preprocessing import SequenceDicer
+    def transform(self, X, y):
+        from pyadlml.dataset.util import to_sktime2
+        Xt, yt = to_sktime2(X, y, return_X_y=True)
+        return Xt, yt
 
-        raw = StateVectorEncoder(encode='raw', t_res='10s')\
-              .fit_transform(data.df_devices)
-        labels = LabelEncoder().fit_transform(raw, data.df_activities)
 
-        X = raw.values
-        y = labels.values
+class OneHotEncoder(BaseEstimator, TransformerMixin):
+    def __init__(self, column_name, inplace=True, as_bool=False):
+        self.column_name = column_name
+        self.inplace = inplace
+        self.as_bool = as_bool
 
-        X, y = SequenceDicer(rep='many-to-many', window_length='5m')\
-               .fit_transform(X, y)
+    def fit(self, X, y=None):
+        self.one_hot_encoder_ = SkOneHotEncoder()
+        self.one_hot_encoder_.fit(
+            X[self.column_name].values.reshape(-1, 1))
 
-    Many-To-One
-    ^^^^^^^^^^^
+        self.categories = self.column_name + ':' + \
+            self.one_hot_encoder_.categories_[0]
+        return self
 
-    .. math::
-        f(X_{N,K},y_{N}) \rightarrow (X_{W, N, K}, y_{N})
+    def fit_transform(self, X, y=None):
+        self.fit(X, y)
+        return self.transform(X, y)
 
+    def transform(self, X, y=None):
+        is_df = isinstance(X, pd.DataFrame)
+        assert is_df or isinstance(X, pd.Series)
 
-    .. code:: python
+        if is_df:
+            ser = X[self.column_name]
+        else:
+            ser = X
 
-        from pyadlml.preprocessing import SequenceDicer
+        encoded = self.one_hot_encoder_.transform(
+            ser.values.reshape(-1, 1)).toarray()
+        df_encoded = pd.DataFrame(encoded, columns=self.categories,
+                                  dtype=bool if self.as_bool else int)
 
-        raw = StateVectorEncoder(encode='raw', t_res='10s')\
-              .fit_transform(data.df_devices)
-        labels = LabelEncoder().fit_transform(raw, data.df_activities)
+        if self.inplace and is_df:
+            X = X.drop(columns=self.column_name)
+            X = pd.concat([X, df_encoded], axis=1)
+        return X
 
-        X = raw.values
-        y = labels.values
 
-        X, y = SequenceDicer(rep='many-to-one', window_length='20s')\
-               .fit_transform(X, y)
+class TimeEncoder(BaseEstimator, TransformerMixin):
 
-    """
-    REP_M2M = 'many-to-many'
-    REP_M2O = 'many-to-one'
+    @classmethod
+    def period_length(cls, res):
+        return int(pd.Timedelta('24h')/pd.Timedelta(res))
 
-    def __init__(self, rep=REP_M2M, window_size=10, stride=1):
-        TransformerMixin.__init__(self)
-        XOrYTransformer.__init__(self)
+    @classmethod
+    def time2res(cls, Xt, res):
+        if isinstance(Xt, pd.DataFrame):
+            ser = Xt[TIME]
+        else:
+            ser = Xt
+        return (ser - ser.dt.floor('D'))/pd.Timedelta(res)
 
-        self.rep = rep
-        self.window_size = window_size
-        self.stride = stride
 
-    def fit(self, X,y=None, **fit_params):
-        # TODO not having this method throws an error ! dirty hack
+class SineCosEncoder(TimeEncoder):
+    def __init__(self, res='100ms'):
+        super().__init__()
+        self.res = res
+
+    def fit(self, X=None, y=None):
+        self.res = pd.Timedelta(self.res)
+        self.lmbd_ = int(pd.Timedelta('24h')/self.res)
+        # Calc angular frequency
+        self.w_ = (2*np.pi)/self.lmbd_
         return self
 
-    def fit_transform(self, X, y=None):
-        """
-        Parameters
-        ----------
-        X : nd.array
-            Some kind of numpy array
-        y : nd.array
+    def transform(self, X, y=None):
+        assert TIME in X.columns, "The DataFrame must include a 'time' column"
 
-        Returns
-        -------
-        x : nd.array
-            todo
-        y : nd.array
-            todo
-        """
-        return self.transform(X, y)
+        # Create a copy of the DataFrame to avoid changes to the original one
+        Xt = X.copy()
 
-    @XOrYTransformer.x_or_y_transform
-    def transform(self, X=None, y=None):
-        """
+        # We assume the time range represents a full day
+        Xt['time_in_res'] = (Xt[TIME] - Xt[TIME].dt.floor('D'))/self.res
 
-        """
-        assert self.rep in [self.REP_M2M, self.REP_M2O]
+        # Add sin_emb and cos_emb columns to the DataFrame
+        Xt['time_sin'] = np.sin(self.w_*Xt['time_in_res'])
+        Xt['time_cos'] = np.cos(self.w_*Xt['time_in_res'])
+
+        # Drop the temporary 'x' column
+        Xt = Xt.drop(columns=['time_in_res'])
+
+        return Xt
+
+    def plotly(self, X):
+        assert hasattr(self, 'w_'), 'Fit the transformer before plotting.'
+        df = self.transform(X)
+        fig = go.Figure()
+        fig.add_trace(go.Scatter(x=df[TIME], y=df['time_sin'], name='sin'))
+        fig.add_trace(go.Scatter(x=df[TIME], y=df['time_cos'], name='cos'))
+        fig.update_layout(yaxis=dict(scaleanchor="x", scaleratio=1))
+        return fig
+
+    def plotly_sin_vs_cos(self, X):
+        df = self.transform(X)
+        fig = go.Figure()
+        fig.add_trace(go.Scatter(
+            x=df['sin_emb'].values,
+            y=df['cos_emb'].values,
+            hovertemplate='Sin: %{x}<br>Cos %{y}<br>Time: %{customdata}',
+            mode='markers',
+            customdata=df.index.values)
+        )
+        fig.update_layout(
+            xaxis=dict(scaleanchor="y", scaleratio=1),
+            yaxis=dict(scaleanchor="x", scaleratio=1)
+        )
+        fig.show()
+
+
+class HalfSineEncoder(BaseEstimator, TransformerMixin):
+    def __init__(self, res='100ms'):
+        self.res = res
+
+    def fit(self, X=None, y=None):
+        self.res = pd.Timedelta(self.res)
+        self.lmbd_ = int(pd.Timedelta('24h')/self.res)
+        # Calc angular frequency
+        self.w_ = (np.pi)/self.lmbd_
+        return self
 
-        if X is not None:
-            assert self.window_size < len(X)
-            assert self.stride < len(X)
+    def transform(self, X, y=None):
+        assert 'time' in X.columns, "The DataFrame must include a 'time' column"
+        # Create a copy of the DataFrame to avoid changes to the original one
+        Xt = X.copy()
 
-            X = self._transform_X(X)
+        # We assume the time range represents a full day
+        Xt['time_in_res'] = (Xt[TIME] - Xt[TIME].dt.floor('D'))/self.res
 
-        if y is not None:
-            assert self.window_size < len(y)
-            assert self.stride < len(y)
+        # Add sin_emb and cos_emb columns to the DataFrame
+        Xt['time_sin'] = np.sin(self.w_*Xt['time_in_res'])
 
-            y = self._transform_Y(y)
+        # Drop the temporary 'x' column
+        Xt = Xt.drop(columns=['time_in_res'])
 
-        return X, y
+        return Xt
 
-    def _calc_new_N(self, n_old):
-        return int(np.floor((n_old-self.window_size)/self.stride)+1)
+    def plotly(self, X):
+        assert hasattr(self, 'w_'), 'Fit the transformer before plotting.'
+        df = self.transform(X)
+        fig = go.Figure()
+        fig.add_trace(go.Scatter(x=df[TIME], y=df['time_sin'], name='sin'))
+        fig.update_layout(yaxis=dict(scaleanchor="x", scaleratio=1))
+        return fig
 
-    def _transform_X(self, X):
-        """
 
-        """
-        n_prime = self._calc_new_N(X.shape[0])
-        new_shape =[n_prime, self.window_size, X.shape[1]]
+class PositionalEncoding(BaseEstimator, TransformerMixin):
 
-        res = np.zeros(shape=new_shape, dtype='float32')
-        if not isinstance(X, np.ndarray):
-            import torch
-            if isinstance(X, torch.Tensor):
-                try:
-                    res = torch.zeros(new_shape, dtype=torch.float32)
-                except TypeError:
-                    print('asdf')
-            else:
-                raise ValueError('X has to be either ndarray or of type torch tensor')
+    def __init__(self, d_dim, max_period=1e4, inplace=True):
+        self.d_dim = d_dim
+        self.max_period = max_period
+        self.inplace = inplace
 
-        for r, i in enumerate(range(0, n_prime*self.stride, self.stride)):
-            res[r, :, :] = X[i: i+self.window_size, :]
-        return res
+    def fit(self, X=None, y=None):
+        self.min_freq = 1/self.max_period
+        return self
 
-    def _transform_Y(self, y):
-        """
+    def get_angular_freqs(self):
+        i = np.arange(self.d_dim)//2
+        ws = np.power(self.min_freq, (2*i/self.d_dim))
+        return ws
+
+    def get_periods(self):
+        return 2*np.pi*self.get_angular_freqs()
+
+    def plot_angular_freq(self, scale='linear'):
+        assert scale in ['linear', 'log']
+
+        ws = self.get_angular_freqs()
+        fig, ax = plt.subplots()
+        ax.set_yscale(scale)
+        ax.plot(np.arange(len(ws)), ws,
+                label=f'min{min(ws):.3f}, max{max(ws):.3f}')
+        ax.set_xlabel('d - dimension')
+        ax.set_ylabel('$\omega(d)$')
+        ax.grid(True)
+        ax.legend()
+        return fig
+
+    def plot_waves(self, seq_length):
+        freqs = self.get_angular_freqs()
+
+        n_dim = len(freqs)
+        # Create a figure and an axis
+        fig, ax = plt.subplots(figsize=(10, 10))
+
+        # Loop over the range of dimensions
+        x = np.linspace(0, seq_length, 1000)
+        for d in range(n_dim):
+            oscil = np.sin if d % 2 == 0 else np.cos
+            ax.plot(x, oscil(freqs[d]*x)+2*d, label=f'pe dim={d}')
+        # Set the axis scales to be equal
+        # ax.set_aspect('equal', 'box')
+
+        # Show the legend
+        ax.legend()
+        return fig
+
+    def transform(self, X, y=None, inplace=None):
+        """ 
+
+        sin(w*t) 
+        """
+        inplace = inplace if inplace is not None else self.inplace
+
+        freqs = self.get_angular_freqs()
+        if isinstance(X, pd.DataFrame):
+            x = X[TIME].values
+        else:
+            x = X
+        assert isinstance(x, np.ndarray), 'DEBUG'
 
+        xt = self._pos_enc(freqs, x)
+        if inplace:
+            xt = pd.DataFrame(data=xt, columns=[
+                              f'pe_dim_{i}' for i in range(0, self.d_dim)])
+            X = pd.concat([X, xt], axis=1)
+        else:
+            X = xt
+        return X
 
+    def _pos_enc(self, freqs, pos):
+        pos_enc = pos.reshape(-1, 1)*freqs.reshape(1, -1)
+        pos_enc[:, ::2] = np.cos(pos_enc[:, ::2])
+        pos_enc[:, 1::2] = np.sin(pos_enc[:, 1::2])
+        return pos_enc
+
+    def plot_pe_mat(self, X):
+        ### Plotting ####
+
+        mat = self.transform(X, inplace=False)
+        fig, ax = plt.subplots()
+        im = ax.pcolormesh(mat.T, cmap='RdBu')
+        ax.set_ylabel('Depth')
+        ax.set_ylim((0, self.d_dim))
+        ax.set_xlabel('Position')
+        ax.set_title("PE matrix heat map")
+        fig.colorbar(im)
+        return fig
+
+    def plot_dotproduct_similarity(self, X, pos):
+        # let's choose the first vector
+
+        pe = self.transform(X, inplace=False)
+        first_vector = pe[pos, :]
+
+        # compute the dot products
+        dot_products = np.dot(pe, first_vector)
+
+        # visualize with matplotlib
+        fig, ax = plt.subplots(figsize=(10, 6))
+        ax.plot(dot_products)
+        ax.set_title(f'Dot products of the {pos} vector with rest')
+        ax.set_xlabel('Vector index')
+        ax.set_ylabel('Dot product')
+        ax.grid(True)
+        return fig
+
+
+class TimePositionalEncoding(PositionalEncoding):
+
+    def __init__(self, d_dim, max_period=pd.Timedelta('1D'), res=pd.Timedelta('8.64s'), inplace=True):
+        super().__init__(d_dim, max_period)  # Add super call to the parent class
+        self.res = res
+        self.inplace = inplace
+
+    def fit(self, X=None, y=None):
+        # Map timestamp values to a sequence
+        self.res = pd.Timedelta(self.res)
+        self.max_period = self._td2num(self.max_period)
+        self.min_freq = 1/self.max_period
+        return self
+
+    def _td2num(self, x):
+        if isinstance(x, str):
+            x = pd.Timedelta(x)
+
+        x = x/pd.Timedelta(self.res)
+        return x
+
+    def _num2td(self, x):
+        return pd.Timedelta(self.res)*x
+
+    def transform(self, X, y=None, inplace=None):
+        """ 
+
+        sin(w*t) 
         """
-        dtype = 'int64'
-        if self.rep == self.REP_M2M:
-            n_prime = self._calc_new_N(y.shape[0])
-            new_shape = [n_prime, self.window_size]
+        inplace = self.inplace if inplace is None else inplace
 
-            if isinstance(y, np.ndarray):
-                res = np.zeros(shape=[n_prime, self.window_size], dtype=object)
-                res = res.astype(dtype)
-            else:
-                import torch
-                if isinstance(y, torch.Tensor):
-                    res = torch.zeros(new_shape, dtype=torch.int64)
-                else:
-                    raise ValueError('X has to be either ndarray or of type torch tensor')
+        if isinstance(X, pd.DataFrame):
+            x = X[TIME]
 
-            for r, i in enumerate(range(0, n_prime*self.stride, self.stride)):
-                res[r, :] = y[i: i+self.window_size]
-            return res.squeeze()
-
-        elif self.rep == self.REP_M2O:
-            res = y[list(range(self.window_size-1, y.shape[0], self.stride))]
-            if isinstance(y, np.ndarray):
-                res = res.squeeze().astype(dtype)
-                return res
-            else:
-                import torch
-                raise NotImplementedError
-                #return res
-        else:
-            raise ValueError
+        assert isinstance(x, pd.Series), 'TimePosEnc: Sth. went wrong'
+        td = (x - pd.to_datetime(x.dt.date))
+        time_scaled = self._td2num(td).to_numpy()
+        freqs = self.get_angular_freqs()
+
+        # calc pos enc (T, d_dim)
+        xt = self._pos_enc(freqs, time_scaled)
+
+        if inplace:
+            xt = pd.DataFrame(data=xt, columns=[
+                              f'pe_dim_{i}' for i in range(0, self.d_dim)])
+            xt = pd.concat([X, xt], axis=1)
+
+        return xt
+
+
+class CyclicTimePositionalEncoding(TimePositionalEncoding):
+
+    def __init__(self, d_dim, max_period=pd.Timedelta('1D'), res=pd.Timedelta('8.64s'), base=2):
+        super().__init__(d_dim, max_period, res)  # Add super call to the parent class
+        self.base = base
+
+    def get_angular_freqs(self):
+        """period of length 1"""
+        i = np.arange(self.d_dim)//2
+        lmbd = self.max_period
+        f = 1/(lmbd/(np.minimum((self.base**i).astype(int), lmbd)))
+        ws = 2*np.pi*f
+        return ws
+
+    def get_max_base(self):
+        return np.floor(np.log10(self.max_period)/np.log10(self.base)).astype(int)
+
+    def plotly_wave_length_per_dim(self):
+        from plotly import graph_objects as go
+        fig = go.Figure()
+        x = self.get_periods()*self.res
+        x += pd.Timestamp('01.01.2000 00:00:00')
+        fig.add_trace(go.Scatter(y=np.arange(0, self.d_dim), x=x))
+        return fig
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml/stats.py` & `pyadlml-0.0.8.0a0/pyadlml/stats.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from pyadlml.dataset.stats.acts_and_devs import (
-    contingency_table_events as contingency_triggers,
-    contingency_table_states as contingency_duration
+    contingency_table_events as contingency_table_events,
+    contingency_table_states as contingency_table_states,
+    mutual_info_events as mutual_info_events,
+    mutual_info_states as mutual_info_states,
 )
 
 from pyadlml.dataset.stats.activities import (
     activities_dist as activity_dist,
     activities_count as activity_count,
     activities_transitions as activity_transition,
     activity_duration as activity_duration,
     activities_duration_dist as activity_duration_dist,
     coverage as activity_coverage
 )
 
 from pyadlml.dataset.stats.devices import (
-    event_cross_correlogram as device_trigger_sliding_window,
-    state_fractions as device_state_fractions,
-    state_times as device_on_time,
-    inter_event_intervals as device_time_diff,
-    events_one_day as device_trigger_one_day,
-    event_count as device_trigger_count,
-    state_cross_correlation as device_duration_corr,
+    event_cross_correlogram as device_event_cross_correlogram,
+    state_fractions as device_state_fraction,
+    state_times as device_state_time,
+    inter_event_intervals as device_inter_event_times,
+    events_one_day as device_events_one_day,
+    event_count as device_event_count,
+    state_cross_correlation as device_state_similarity,
+    firing_rate as device_firing_rate
 )
```

### Comparing `pyadlml-0.0.7.9a0/pyadlml.egg-info/SOURCES.txt` & `pyadlml-0.0.8.0a0/pyadlml.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,120 +4,133 @@
 pyadlml/__init__.py
 pyadlml/benchmark.py
 pyadlml/constants.py
 pyadlml/feature_extraction.py
 pyadlml/feature_selection.py
 pyadlml/metrics.py
 pyadlml/pipeline.py
-pyadlml/preprocessing.py
 pyadlml/stats.py
 pyadlml/util.py
 pyadlml.egg-info/PKG-INFO
 pyadlml.egg-info/SOURCES.txt
 pyadlml.egg-info/dependency_links.txt
 pyadlml.egg-info/requires.txt
 pyadlml.egg-info/top_level.txt
 pyadlml/dataset/__init__.py
-pyadlml/dataset/io.py
+pyadlml/dataset/act_assist.py
+pyadlml/dataset/torch.py
 pyadlml/dataset/util.py
 pyadlml/dataset/_core/__init__.py
-pyadlml/dataset/_core/_dataset.py
 pyadlml/dataset/_core/activities.py
+pyadlml/dataset/_core/acts_and_devs.py
 pyadlml/dataset/_core/devices.py
-pyadlml/dataset/_core/obj.py
 pyadlml/dataset/_datasets/__init__.py
 pyadlml/dataset/_datasets/activity_assistant.py
 pyadlml/dataset/_datasets/amsterdam.py
 pyadlml/dataset/_datasets/aras.py
-pyadlml/dataset/_datasets/casas_aruba.py
+pyadlml/dataset/_datasets/casas_houses.py
 pyadlml/dataset/_datasets/homeassistant.py
 pyadlml/dataset/_datasets/kasteren_2010.py
 pyadlml/dataset/_datasets/mitlab.py
 pyadlml/dataset/_datasets/tuebingen_2019.py
 pyadlml/dataset/_datasets/uci_adl_binary.py
 pyadlml/dataset/_representations/__init__.py
 pyadlml/dataset/_representations/changepoint.py
 pyadlml/dataset/_representations/lastfired.py
-pyadlml/dataset/_representations/raw.py
-pyadlml/dataset/bokeh/__init__.py
-pyadlml/dataset/bokeh/activities.py
-pyadlml/dataset/matplotlib/__init__.py
-pyadlml/dataset/matplotlib/act_and_devs.py
-pyadlml/dataset/matplotlib/activities.py
-pyadlml/dataset/matplotlib/devices.py
-pyadlml/dataset/matplotlib/discrete.py
-pyadlml/dataset/matplotlib/image.py
-pyadlml/dataset/matplotlib/util.py
-pyadlml/dataset/plotly/__init__.py
-pyadlml/dataset/plotly/activities.py
-pyadlml/dataset/plotly/acts_and_devs.py
-pyadlml/dataset/plotly/devices.py
-pyadlml/dataset/plotly/util.py
-pyadlml/dataset/plotly/dashboard/__init__.py
-pyadlml/dataset/plotly/dashboard/callbacks.py
-pyadlml/dataset/plotly/dashboard/dashboard.py
-pyadlml/dataset/plotly/dashboard/layout.py
+pyadlml/dataset/_representations/state.py
+pyadlml/dataset/cleaning/__init__.py
+pyadlml/dataset/cleaning/misc.py
+pyadlml/dataset/cleaning/util.py
+pyadlml/dataset/io/__init__.py
+pyadlml/dataset/io/downloader.py
+pyadlml/dataset/io/io.py
+pyadlml/dataset/io/local.py
+pyadlml/dataset/io/remote.py
+pyadlml/dataset/plot/__init__.py
+pyadlml/dataset/plot/util.py
+pyadlml/dataset/plot/_bokeh/__init__.py
+pyadlml/dataset/plot/_bokeh/activities.py
+pyadlml/dataset/plot/_bokeh/util.py
+pyadlml/dataset/plot/matplotlib/__init__.py
+pyadlml/dataset/plot/matplotlib/act_and_devs.py
+pyadlml/dataset/plot/matplotlib/activities.py
+pyadlml/dataset/plot/matplotlib/devices.py
+pyadlml/dataset/plot/matplotlib/discrete.py
+pyadlml/dataset/plot/matplotlib/image.py
+pyadlml/dataset/plot/matplotlib/util.py
+pyadlml/dataset/plot/plotly/__init__.py
+pyadlml/dataset/plot/plotly/activities.py
+pyadlml/dataset/plot/plotly/acts_and_devs.py
+pyadlml/dataset/plot/plotly/devices.py
+pyadlml/dataset/plot/plotly/discrete.py
+pyadlml/dataset/plot/plotly/util.py
+pyadlml/dataset/plot/plotly/dashboard/__init__.py
+pyadlml/dataset/plot/plotly/dashboard/callbacks.py
+pyadlml/dataset/plot/plotly/dashboard/dashboard.py
+pyadlml/dataset/plot/plotly/dashboard/layout.py
 pyadlml/dataset/stats/__init__.py
 pyadlml/dataset/stats/activities.py
 pyadlml/dataset/stats/acts_and_devs.py
 pyadlml/dataset/stats/devices.py
 pyadlml/dataset/stats/discrete.py
 pyadlml/dataset/stats/util.py
+pyadlml/ml_viz/__init__.py
+pyadlml/model/WaveNet.py
 pyadlml/model/__init__.py
 pyadlml/model/_model.py
+pyadlml/model/dummy.py
+pyadlml/model/mlp.py
 pyadlml/model/util.py
 pyadlml/model/hbhmm/__init__.py
 pyadlml/model/hbhmm/hmm.py
 pyadlml/model/hbhmm/pchmm.py
 pyadlml/model/hmm/__init__.py
 pyadlml/model/hmm/_model_categorical.py
 pyadlml/model/hmm/bhmm.py
 pyadlml/model/hmm/bhmm_hp.py
 pyadlml/model/hmm/bhsmm.py
 pyadlml/model/hmm/hmm.py
 pyadlml/model/hmm/util.py
+pyadlml/model/nn/__init__.py
+pyadlml/model/nn/util.py
 pyadlml/model/rnn/__init__.py
 pyadlml/model/rnn/rnn.py
+pyadlml/model/tpp/__init__.py
+pyadlml/model/tpp/util.py
 pyadlml/model/transformer/__init__.py
-pyadlml/model/transformer/layers.py
+pyadlml/model/transformer/vanilla.py
 pyadlml/model/vrnn/__init__.py
 pyadlml/model/vrnn/classifying_vrnn.py
 pyadlml/model/vrnn/vrnn.py
 pyadlml/model_selection/__init__.py
 pyadlml/model_selection/_search.py
 pyadlml/model_selection/_split.py
 pyadlml/plot/__init__.py
 pyadlml/plot/_benchmark.py
 pyadlml/plot/explanation.py
 pyadlml/plot/feature_importance.py
 pyadlml/plot/interpretation.py
+pyadlml/preprocessing/__init__.py
+pyadlml/preprocessing/preprocessing.py
+pyadlml/preprocessing/windows.py
+pyadlml/training/__init__.py
+pyadlml/training/trainable.py
 scripts/__init__.py
-scripts/generate_dataset_info.py
 testing/__init__.py
-testing/test_crossval.py
-testing/test_dataset_amsterdam.py
-testing/test_dataset_aras.py
-testing/test_dataset_base.py
-testing/test_dataset_casas_aruba.py
-testing/test_dataset_dirty.py
-testing/test_dataset_empty_partial.py
-testing/test_dataset_mitlab.py
-testing/test_dataset_tuebingen2019.py
-testing/test_dataset_uci_adl_binary.py
-testing/test_feature_extraction.py
-testing/test_gridsearch.py
 testing/test_imports.py
+testing/test_metrics.py
 testing/test_pipeline.py
-testing/test_preprocessing.py
+testing/test_stats.py
 testing/test_utils.py
-testing/models/__init__.py
-testing/models/hmm/__init__.py
-testing/models/hmm/testing_hass_forwardhmm.py
-testing/models/hmm/testing_hass_pchmm.py
-testing/models/hmm/testing_homeassistant.py
-testing/models/hmm/testing_kasteren.py
-testing/models/hmm/testing_kasteren_pom.py
-testing/models/hmm/testing_pendigits.py
-testing/models/hsmm/__init__.py
-testing/models/hsmm/testing_kasteren_hsmm.py
-testing/models/hsmm/testing_pyhsmm.py
-testing/models/hsmm/testing_ssm.py
+tools/__init__.py
+tools/clean_device_signals.py
+tools/correct_activities.py
+tools/dashboard.py
+tools/generate_dataset_info.py
+tools/hparam_sweep.py
+tools/label_data.py
+tools/train.py
+tools/train_debug.py
+tools/train_debug_sktime.py
+tools/configs/__init__.py
+tools/configs/models.py
+tools/configs/pipes.py
```

### Comparing `pyadlml-0.0.7.9a0/setup.py` & `pyadlml-0.0.8.0a0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,36 +6,43 @@
 with open('HISTORY.md', 'r') as history_file:
     HISTORY = history_file.read()
 
 
 # Most basic version
 install_requires = ['numpy', 'pandas', 'joblib']
 
-
-_extras_light = ['mega.py', 'dask[complete]',
-                 'matplotlib', 'scipy', 'sklearn']
+_extras_light = [
+    'mega.py',
+    'dask[complete]',
+    'matplotlib',
+    'scipy',
+    'sklearn'
+]
 
 _extras_datavis = [
     'sqlalchemy',
     'plotly',
     'dash_daq',
     'dash-bootstrap-components',
     'dash',
 ]
 
-_extras_all = _extras_light + _extras_datavis
-
+_extras_all = [
+    'torch',
+    *_extras_light,
+    *_extras_datavis
+]
 
 
 setup_args = dict(
     name="pyadlml",
-    version="0.0.7.9-alpha",
+    version="0.0.8.0alpha",
     url="https://github.com/tcsvn/pyadlml",
     author="Christian Meier",
-    description="Sklearn flavored library containing numerous Activity of Daily Livings datasets, preprocessing methods and visualizations.",
+    description="Sklearn flavored library containing numerous Activity of Daily Livings datasets, preprocessing methods, visualizations and models.",
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     author_email="account@meier-lossburg.de",
     license="MIT",
     packages=find_packages(),
     install_requires=install_requires,
     extras_require=dict(
```

### Comparing `pyadlml-0.0.7.9a0/testing/test_pipeline.py` & `pyadlml-0.0.8.0a0/testing/test_pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,113 +1,129 @@
-import sys
-import pathlib
-
+from sklearn.ensemble import RandomForestClassifier
 from sklearn.neighbors import KernelDensity
 from sklearn.svm import SVC
-
+from pyadlml.pipeline import Pipeline
+from pyadlml.preprocessing import Event2Vec, DropTimeIndex, LabelMatcher
+from pyadlml.constants import *
+from pyadlml.dataset import load_act_assist
+import unittest
+import sys
+import pathlib
 working_directory = pathlib.Path().absolute()
 script_directory = pathlib.Path(__file__).parent.absolute()
 sys.path.append(str(working_directory))
-import unittest
-from sklearn.ensemble import RandomForestClassifier
-from pyadlml.dataset import set_data_home, load_act_assist
-from pyadlml.pipeline import Pipeline
-from pyadlml.preprocessing import StateVectorEncoder, LabelEncoder, DropTimeIndex
-SUBJECT_ADMIN_NAME = 'admin'
 
 
 class TestPipeline(unittest.TestCase):
     def setUp(self):
         dataset_dir = str(script_directory) + '/datasets/partial_dataset'
-        self.data = load_act_assist(dataset_dir, subjects=[SUBJECT_ADMIN_NAME])
-        self.data.df_activities = self.data.df_activities_admin
+        self.data = load_act_assist(dataset_dir)
+        self.df_acts = self.data['activities']
+        self.df_devs = self.data['devices']
+
         self.rf_pipe = [
-            ('raw', StateVectorEncoder(encode='raw')),
-            ('lbl', LabelEncoder(idle=True)),
+            ('raw', Event2Vec(encode='raw')),
+            ('lbl', LabelMatcher(idle=True)),
             ('drop_tidx', DropTimeIndex()),
             ('classifier', RandomForestClassifier(random_state=42))
         ]
         self.kde_pipe = [
-            ('raw', StateVectorEncoder(encode='raw')),
+            ('raw', Event2Vec(encode='raw')),
             ('drop_tidx', DropTimeIndex()),
             ('classifier', KernelDensity(kernel='gaussian', bandwidth=0.5))
         ]
         self.svm_pipe = [
-            ('raw', StateVectorEncoder(encode='raw')),
-            ('lbl', LabelEncoder(idle=True)),
+            ('raw', Event2Vec(encode='raw')),
+            ('lbl', LabelMatcher(idle=True)),
             ('drop_tidx', DropTimeIndex()),
             ('classifier', SVC())
         ]
 
-
-    #def test_decision_function(self):
+    # def test_decision_function(self):
     #    #  Apply transforms, and decision_function of the final estimator
     #    pipe = Pipeline(self.svm_pipe)
-    #    pipe = pipe.fit(self.data.df_devices,
-    #                self.data.df_activities)
-    #    tmp = pipe.decision_function(self.data.df_devices)
-
+    #    pipe = pipe.fit(df_devs,
+    #                df_acts)
+    #    tmp = pipe.decision_function(df_devs)
 
     def test_fit(self):
+        df_devs, df_acts = self.df_acts.copy(), self.df_devs.copy()
         pipe = Pipeline(self.rf_pipe)
-        tmp = pipe.fit(self.data.df_devices,
-                       self.data.df_activities)
+        tmp = pipe.fit(df_devs,
+                       df_acts)
 
     def test_fit_predict(self):
         # Applies fit_predict of last step in pipeline after transforms.
+
+        df_devs, df_acts = self.df_acts.copy(), self.df_devs.copy()
         pipe = Pipeline(self.rf_pipe)
         tmp = pipe.fit_predict(
-            self.data.df_devices,
-            self.data.df_activities)
+            df_devs,
+            df_acts)
         print(tmp)
 
     def test_fit_transform(self):
-        #Fit the model and transform with the final estimator
+        # Fit the model and transform with the final estimator
+        df_devs, df_acts = self.df_acts.copy(), self.df_devs.copy()
+
         pipe = Pipeline(self.rf_pipe)
         tmp = pipe.fit_transform(
-            self.data.df_devices,
-            self.data.df_activities)
-
+            df_devs,
+            df_acts)
 
     def test_get_params(self):
-        #Get parameters for this estimator.
+        # Get parameters for this estimator.
+        df_devs, df_acts = self.df_acts.copy(), self.df_devs.copy()
+
         pipe = Pipeline(self.rf_pipe)
         tmp = pipe.get_params()
-        #print(tmp)
-
+        # print(tmp)
 
     def test_predict(self):
-        #Apply transforms to the data, and predict with the final estimator
-        pipe = Pipeline(self.rf_pipe).fit(self.data.df_devices, self.data.df_activities)
-        tmp = pipe.predict(self.data.df_devices)
+        # Apply transforms to the data, and predict with the final estimator
+        df_devs, df_acts = self.df_acts.copy(), self.df_devs.copy()
+
+        pipe = Pipeline(self.rf_pipe).fit(
+            df_devs, df_acts)
+        tmp = pipe.predict(df_devs)
         print(tmp)
 
     def test_predict_log_proba(self):
-        #Apply transforms, and predict_log_proba of the final estimator
-        pipe = Pipeline(self.rf_pipe).fit(self.data.df_devices, self.data.df_activities)
-        tmp = pipe.predict_log_proba(self.data.df_devices)
-        print(tmp)
+        # Apply transforms, and predict_log_proba of the final estimator
+        df_devs, df_acts = self.df_acts.copy(), self.df_devs.copy()
 
+        pipe = Pipeline(self.rf_pipe).fit(
+            df_devs, df_acts)
+        tmp = pipe.predict_log_proba(df_devs)
+        print(tmp)
 
     def test_predict_proba(self):
-        #Apply transforms, and predict_proba of the final estimator
-        pipe = Pipeline(self.rf_pipe).fit(self.data.df_devices, self.data.df_activities)
-        tmp = pipe.predict_proba(self.data.df_devices)
-        print(tmp)
+        # Apply transforms, and predict_proba of the final estimator
+        df_devs, df_acts = self.df_acts.copy(), self.df_devs.copy()
 
+        pipe = Pipeline(self.rf_pipe).fit(
+            df_devs, df_acts)
+        tmp = pipe.predict_proba(df_devs)
+        print(tmp)
 
     def test_score(self):
-        #Apply transforms, and score with the final estimator
-        pipe = Pipeline(self.rf_pipe).fit(self.data.df_devices, self.data.df_activities)
+        # Apply transforms, and score with the final estimator
+        df_devs, df_acts = self.df_acts.copy(), self.df_devs.copy()
+
+        pipe = Pipeline(self.rf_pipe).fit(
+            df_devs, df_acts)
         tmp = pipe.score(
-            self.data.df_devices,
-            self.data.df_activities)
+            df_devs,
+            df_acts)
         print(tmp)
 
     def test_score_samples(self):
-        #Apply transforms, and score_samples of the final estimator.
-        pipe = Pipeline(self.kde_pipe).fit(self.data.df_devices)
-        tmp = pipe.score_samples(self.data.df_devices)
+        # Apply transforms, and score_samples of the final estimator.
+        df_devs, df_acts = self.df_acts.copy(), self.df_devs.copy()
+
+        pipe = Pipeline(self.kde_pipe).fit(df_devs)
+        tmp = pipe.score_samples(df_devs)
         print(tmp)
 
+
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

### Comparing `pyadlml-0.0.7.9a0/testing/test_utils.py` & `pyadlml-0.0.8.0a0/testing/test_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,117 @@
+from pyadlml.feature_extraction import DayOfWeek, extract_time_difference
+from pyadlml.feature_extraction import extract_time_bins, extract_day_of_week
+from pyadlml.dataset import ACTIVITY, DEVICE, END_TIME, START_TIME, VAL, TIME
+import pandas as pd
+from pyadlml.constants import *
+from pyadlml.dataset import load_act_assist
+import unittest
 import sys
 import pathlib
 
 from pyadlml.dataset.util import remove_days
 
 working_directory = pathlib.Path().absolute()
 script_directory = pathlib.Path(__file__).parent.absolute()
 sys.path.append(str(working_directory))
-import unittest
-import pandas as pd
 
-from pyadlml.dataset import load_act_assist
-from pyadlml.dataset import ACTIVITY, DEVICE, END_TIME, START_TIME, VAL, TIME
-from pyadlml.feature_extraction import extract_time_bins, extract_day_of_week
 
 SUBJECT_ADMIN_NAME = 'admin'
+working_directory = pathlib.Path().absolute()
+script_directory = pathlib.Path(__file__).parent.absolute()
+sys.path.append(str(working_directory))
+
 
 def timestamp(string):
     return pd.to_datetime(string, dayfirst=True)
 
+
 def df(d):
     return pd.DataFrame(d, columns=[START_TIME, END_TIME, ACTIVITY])
 
 
 class TestDirtyDataset(unittest.TestCase):
     def setUp(self):
-        dataset_dir = str(script_directory) + '/datasets/dirty_dataset'
-        self.data = load_act_assist(dataset_dir, subjects=[SUBJECT_ADMIN_NAME])
+        dataset_dir = script_directory.joinpath('/datasets/dirty_dataset')
+        self.data = load_act_assist(dataset_dir)
+        self.df_acts = self.data['activities']
+        self.df_devs = self.data['devices']
 
         self.days_to_remove = ['02.01.2000']
         self.offsets = ['3h']
         self.data_case_1 = [
-            [timestamp('01.01.2000 12:00:00'), timestamp('02.01.2000 12:00:00'), 'act_1'],
-            [timestamp('03.01.2000 08:00:00'), timestamp('03.01.2000 10:00:00'), 'act_2'],
-            [timestamp('03.01.2000 10:00:01'), timestamp('03.01.2000 18:00:00'), 'act_3'],
+            [timestamp('01.01.2000 12:00:00'), timestamp(
+                '02.01.2000 12:00:00'), 'act_1'],
+            [timestamp('03.01.2000 08:00:00'), timestamp(
+                '03.01.2000 10:00:00'), 'act_2'],
+            [timestamp('03.01.2000 10:00:01'), timestamp(
+                '03.01.2000 18:00:00'), 'act_3'],
         ]
         self.data_case_2 = [
-            [timestamp('01.01.2000 12:00:00'), timestamp('02.01.2000 12:00:00'), 'act_1'],
-            [timestamp('03.01.2000 06:00:00'), timestamp('03.01.2000 18:00:00'), 'act_2'],
+            [timestamp('01.01.2000 12:00:00'), timestamp(
+                '02.01.2000 12:00:00'), 'act_1'],
+            [timestamp('03.01.2000 06:00:00'), timestamp(
+                '03.01.2000 18:00:00'), 'act_2'],
         ]
         self.data_case_3 = [
-            [timestamp('01.01.2000 06:00:00'), timestamp('01.01.2000 20:00:00'), 'act_1'],
-            [timestamp('01.01.2000 20:00:01'), timestamp('01.01.2000 23:00:00'), 'act_2'],
-            [timestamp('02.01.2000 18:00:00'), timestamp('03.01.2000 12:00:00'), 'act_2'],
+            [timestamp('01.01.2000 06:00:00'), timestamp(
+                '01.01.2000 20:00:00'), 'act_1'],
+            [timestamp('01.01.2000 20:00:01'), timestamp(
+                '01.01.2000 23:00:00'), 'act_2'],
+            [timestamp('02.01.2000 18:00:00'), timestamp(
+                '03.01.2000 12:00:00'), 'act_2'],
         ]
         self.data_case_4 = [
-            [timestamp('01.01.2000 18:00:00'), timestamp('01.01.2000 23:00:00'), 'act_1'],
-            [timestamp('02.01.2000 20:00:00'), timestamp('03.01.2000 12:00:00'), 'act_2'],
+            [timestamp('01.01.2000 18:00:00'), timestamp(
+                '01.01.2000 23:00:00'), 'act_1'],
+            [timestamp('02.01.2000 20:00:00'), timestamp(
+                '03.01.2000 12:00:00'), 'act_2'],
         ]
 
     def test_extract_time_bins(self):
         from pyadlml.dataset.plot.activities import correction
 
         df_activities = df(self.data_case_1)
         print('case 1: \n', df_activities)
-        _, df_activities_2 = remove_days(self.df_devices, df_activities, self.days_to_remove)
+        _, df_activities_2 = remove_days(
+            self.df_devices, df_activities, self.days_to_remove)
         print(df_activities_2, '\n', '~'*100)
-        #correction(df_activities, df_activities_2).show()
+        # correction(df_activities, df_activities_2).show()
         df_activities = df(self.data_case_2)
         print('case 2: \n', df_activities)
-        _, df_activities_2 = remove_days(df_devices, df_activities, self.days_to_remove)
+        _, df_activities_2 = remove_days(
+            df_devices, df_activities, self.days_to_remove)
         print(df_activities_2, '\n', '~'*100)
-        #correction(df_activities, df_activities_2).show()
+        # correction(df_activities, df_activities_2).show()
         df_activities = df(self.data_case_3)
         print('case 3: \n', df_activities)
-        _, df_activities_2 = remove_days(df_devices, df_activities, self.days_to_remove)
+        _, df_activities_2 = remove_days(
+            df_devices, df_activities, self.days_to_remove)
         print(df_activities, '\n', '~'*100)
         correction(df_activities, df_activities_2).show()
         df_activities = df(self.data_case_4)
         print('case 4: \n', df_activities)
-        _, df_activities_2 = remove_days(df_devices, df_activities, self.days_to_remove)
+        _, df_activities_2 = remove_days(
+            df_devices, df_activities, self.days_to_remove)
         print(df_activities, '\n', '~'*100)
         correction(df_activities, df_activities_2).show()
 
-
-
+        df_devs = self.df_devs.copy()
+        df_res2h = extract_time_difference(df_devs)
+        df_res6h = extract_time_difference(df_devs, resolution='6h')
+        df_res10m = extract_time_difference(df_devs, resolution='10m')
+        df_res40m = extract_time_difference(df_devs, resolution='40m')
+        df_res10s = extract_time_difference(df_devs, resolution='10s')
+
+        assert len(df_res2h.columns) == 12
+        assert len(df_res6h.columns) == 4
+        assert len(df_res10m.columns) == 144
+        assert len(df_res40m.columns) == 36
+        assert len(df_res10s.columns) == 8640
+
+    def test_extract_day_of_week(self):
+        df_devs = self.df_devs.copy()
+        df_dow = DayOfWeek(one_hot_encoding=False)
 
 
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

