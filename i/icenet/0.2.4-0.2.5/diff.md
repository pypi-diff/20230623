# Comparing `tmp/icenet-0.2.4.tar.gz` & `tmp/icenet-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jambyr/code/ai-lab/icenet/icenet/dist/.tmp-olhoky7y/icenet-0.2.4.tar", last modified: Thu Jun 22 07:43:10 2023, max compression
+gzip compressed data, was "/home/jambyr/code/ai-lab/icenet/icenet/dist/.tmp-mf9jewru/icenet-0.2.5.tar", last modified: Fri Jun 23 14:35:26 2023, max compression
```

## Comparing `icenet-0.2.4.tar` & `icenet-0.2.5.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.112728 icenet-0.2.4/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      291 2023-03-07 11:38:13.000000 icenet-0.2.4/AUTHORS.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3207 2022-11-22 16:24:34.000000 icenet-0.2.4/CONTRIBUTING.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      458 2022-11-22 16:27:46.000000 icenet-0.2.4/HISTORY.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1083 2022-02-03 18:27:11.000000 icenet-0.2.4/LICENSE
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      261 2022-11-22 15:17:37.000000 icenet-0.2.4/MANIFEST.in
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3212 2023-06-22 07:43:10.112728 icenet-0.2.4/PKG-INFO
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2339 2023-06-22 07:41:55.000000 icenet-0.2.4/README.md
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.066727 icenet-0.2.4/docs/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      607 2022-11-22 16:40:49.000000 icenet-0.2.4/docs/Makefile
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.036726 icenet-0.2.4/docs/_build/
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.036726 icenet-0.2.4/docs/_build/html/
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.072727 icenet-0.2.4/docs/_build/html/_static/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      673 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/ajax-loader.gif
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      756 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/comment-bright.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      829 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/comment-close.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      641 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/comment.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      222 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/down-pressed.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      202 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/down.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      286 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/file.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       90 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/minus.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       90 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/plus.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      214 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/up-pressed.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      203 2022-11-22 15:22:19.000000 icenet-0.2.4/docs/_build/html/_static/up.png
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       28 2022-02-03 18:27:11.000000 icenet-0.2.4/docs/authors.rst
--rwxrwxr-x   0 jambyr    (1000) jambyr    (1000)     4893 2023-02-02 11:23:27.000000 icenet-0.2.4/docs/conf.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       33 2022-02-03 18:27:11.000000 icenet-0.2.4/docs/contributing.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       28 2022-02-03 18:27:11.000000 icenet-0.2.4/docs/history.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      380 2022-11-22 17:17:40.000000 icenet-0.2.4/docs/icenet.data.datasets.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1099 2022-11-22 16:36:53.000000 icenet-0.2.4/docs/icenet.data.interfaces.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      872 2022-11-22 17:17:40.000000 icenet-0.2.4/docs/icenet.data.loaders.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1254 2022-11-22 16:36:53.000000 icenet-0.2.4/docs/icenet.data.processors.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1176 2022-11-22 16:42:51.000000 icenet-0.2.4/docs/icenet.data.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      505 2022-11-22 16:37:49.000000 icenet-0.2.4/docs/icenet.data.sic.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1238 2022-11-22 16:38:22.000000 icenet-0.2.4/docs/icenet.model.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      671 2022-11-22 16:38:41.000000 icenet-0.2.4/docs/icenet.plotting.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1122 2022-11-22 16:39:14.000000 icenet-0.2.4/docs/icenet.process.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      168 2022-11-22 16:39:20.000000 icenet-0.2.4/docs/icenet.results.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      444 2023-02-02 12:45:59.000000 icenet-0.2.4/docs/icenet.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      343 2022-11-22 17:17:40.000000 icenet-0.2.4/docs/icenet.tests.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      303 2022-11-22 16:39:50.000000 icenet-0.2.4/docs/index.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1110 2022-11-22 16:40:33.000000 icenet-0.2.4/docs/installation.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      768 2022-11-22 16:40:49.000000 icenet-0.2.4/docs/make.bat
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       55 2023-02-02 12:45:59.000000 icenet-0.2.4/docs/modules.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       55 2022-05-19 22:27:19.000000 icenet-0.2.4/docs/readme.rst
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       67 2022-11-22 16:41:07.000000 icenet-0.2.4/docs/usage.rst
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.072727 icenet-0.2.4/icenet/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      217 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/__init__.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.076727 icenet-0.2.4/icenet/data/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/data/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7193 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/cli.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     9106 2023-02-02 11:23:27.000000 icenet-0.2.4/icenet/data/dataset.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.077727 icenet-0.2.4/icenet/data/datasets/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-06-18 16:56:02.000000 icenet-0.2.4/icenet/data/datasets/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     8145 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/datasets/utils.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.081728 icenet-0.2.4/icenet/data/interfaces/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/data/interfaces/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    10896 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/interfaces/cds.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     6830 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/interfaces/cmems.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    23972 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/interfaces/downloader.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     9244 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/interfaces/esgf.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    14765 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/interfaces/mars.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7838 2022-11-22 15:28:41.000000 icenet-0.2.4/icenet/data/interfaces/utils.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     4068 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/loader.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.085728 icenet-0.2.4/icenet/data/loaders/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1454 2022-12-22 13:08:59.000000 icenet-0.2.4/icenet/data/loaders/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    11679 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/loaders/base.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    17301 2023-06-14 13:21:26.000000 icenet-0.2.4/icenet/data/loaders/dask.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      864 2022-11-22 15:29:16.000000 icenet-0.2.4/icenet/data/loaders/stdlib.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1536 2022-09-29 11:27:40.000000 icenet-0.2.4/icenet/data/loaders/utils.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    23399 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/process.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.087728 icenet-0.2.4/icenet/data/processors/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/data/processors/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1747 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/processors/cmip.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      988 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/processors/era5.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      995 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/processors/hres.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3534 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/processors/meta.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      984 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/processors/oras5.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2078 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/processors/osi.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     6512 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/processors/utils.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    10779 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/producers.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.088728 icenet-0.2.4/icenet/data/sic/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/data/sic/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    10059 2023-02-02 11:23:27.000000 icenet-0.2.4/icenet/data/sic/mask.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    24591 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/data/sic/osisaf.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       64 2022-06-15 11:18:18.000000 icenet-0.2.4/icenet/data/sic/utils.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7074 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/data/utils.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.092728 icenet-0.2.4/icenet/model/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/model/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     4118 2022-11-22 15:32:01.000000 icenet-0.2.4/icenet/model/callbacks.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1029 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/model/losses.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     9515 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/model/metrics.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7903 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/model/models.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7201 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/model/predict.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    16918 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/model/train.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3921 2022-11-22 16:15:24.000000 icenet-0.2.4/icenet/model/utils.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.099728 icenet-0.2.4/icenet/plotting/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/plotting/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     4593 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/plotting/data.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    75295 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/plotting/forecast.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      250 2022-11-22 16:15:42.000000 icenet-0.2.4/icenet/plotting/trend.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    15077 2023-06-22 07:41:55.000000 icenet-0.2.4/icenet/plotting/utils.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    12356 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/plotting/video.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.106728 icenet-0.2.4/icenet/process/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/process/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2491 2022-11-22 16:15:59.000000 icenet-0.2.4/icenet/process/azure.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     5714 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/process/forecasts.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1447 2022-11-22 16:16:07.000000 icenet-0.2.4/icenet/process/local.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    11256 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/process/predict.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/process/train.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      874 2022-08-11 12:13:43.000000 icenet-0.2.4/icenet/process/utils.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.108728 icenet-0.2.4/icenet/results/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.4/icenet/results/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1674 2023-02-02 11:23:27.000000 icenet-0.2.4/icenet/results/threshold.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.110728 icenet-0.2.4/icenet/tests/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       36 2022-11-22 15:25:11.000000 icenet-0.2.4/icenet/tests/__init__.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      758 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/tests/test_entry_points.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      540 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/tests/test_mod.py
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2580 2023-03-07 11:38:13.000000 icenet-0.2.4/icenet/utils.py
-drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-22 07:43:10.074727 icenet-0.2.4/icenet.egg-info/
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3212 2023-06-22 07:43:10.000000 icenet-0.2.4/icenet.egg-info/PKG-INFO
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2846 2023-06-22 07:43:10.000000 icenet-0.2.4/icenet.egg-info/SOURCES.txt
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        1 2023-06-22 07:43:10.000000 icenet-0.2.4/icenet.egg-info/dependency_links.txt
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2159 2023-06-22 07:43:10.000000 icenet-0.2.4/icenet.egg-info/entry_points.txt
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        1 2023-06-22 07:43:09.000000 icenet-0.2.4/icenet.egg-info/not-zip-safe
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      372 2023-06-22 07:43:10.000000 icenet-0.2.4/icenet.egg-info/requires.txt
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        7 2023-06-22 07:43:10.000000 icenet-0.2.4/icenet.egg-info/top_level.txt
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      173 2023-06-22 07:43:10.114728 icenet-0.2.4/setup.cfg
--rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     4419 2023-06-22 07:41:55.000000 icenet-0.2.4/setup.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.314489 icenet-0.2.5/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      291 2023-03-07 11:38:13.000000 icenet-0.2.5/AUTHORS.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3207 2022-11-22 16:24:34.000000 icenet-0.2.5/CONTRIBUTING.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      458 2022-11-22 16:27:46.000000 icenet-0.2.5/HISTORY.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1083 2022-02-03 18:27:11.000000 icenet-0.2.5/LICENSE
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      261 2022-11-22 15:17:37.000000 icenet-0.2.5/MANIFEST.in
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3212 2023-06-23 14:35:26.314489 icenet-0.2.5/PKG-INFO
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2339 2023-06-22 07:41:55.000000 icenet-0.2.5/README.md
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.298488 icenet-0.2.5/docs/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      607 2022-11-22 16:40:49.000000 icenet-0.2.5/docs/Makefile
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.277489 icenet-0.2.5/docs/_build/
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.277489 icenet-0.2.5/docs/_build/html/
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.302488 icenet-0.2.5/docs/_build/html/_static/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      673 2022-11-22 15:22:19.000000 icenet-0.2.5/docs/_build/html/_static/ajax-loader.gif
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      756 2022-11-22 15:22:19.000000 icenet-0.2.5/docs/_build/html/_static/comment-bright.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      829 2022-11-22 15:22:19.000000 icenet-0.2.5/docs/_build/html/_static/comment-close.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      641 2022-11-22 15:22:19.000000 icenet-0.2.5/docs/_build/html/_static/comment.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      222 2022-11-22 15:22:19.000000 icenet-0.2.5/docs/_build/html/_static/down-pressed.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      202 2022-11-22 15:22:19.000000 icenet-0.2.5/docs/_build/html/_static/down.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      286 2022-11-22 15:22:19.000000 icenet-0.2.5/docs/_build/html/_static/file.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       90 2022-11-22 15:22:19.000000 icenet-0.2.5/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       90 2022-11-22 15:22:19.000000 icenet-0.2.5/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      214 2022-11-22 15:22:19.000000 icenet-0.2.5/docs/_build/html/_static/up-pressed.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      203 2022-11-22 15:22:19.000000 icenet-0.2.5/docs/_build/html/_static/up.png
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       28 2022-02-03 18:27:11.000000 icenet-0.2.5/docs/authors.rst
+-rwxrwxr-x   0 jambyr    (1000) jambyr    (1000)     4893 2023-02-02 11:23:27.000000 icenet-0.2.5/docs/conf.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       33 2022-02-03 18:27:11.000000 icenet-0.2.5/docs/contributing.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       28 2022-02-03 18:27:11.000000 icenet-0.2.5/docs/history.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      380 2022-11-22 17:17:40.000000 icenet-0.2.5/docs/icenet.data.datasets.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1099 2022-11-22 16:36:53.000000 icenet-0.2.5/docs/icenet.data.interfaces.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      872 2022-11-22 17:17:40.000000 icenet-0.2.5/docs/icenet.data.loaders.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1254 2022-11-22 16:36:53.000000 icenet-0.2.5/docs/icenet.data.processors.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1176 2022-11-22 16:42:51.000000 icenet-0.2.5/docs/icenet.data.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      505 2022-11-22 16:37:49.000000 icenet-0.2.5/docs/icenet.data.sic.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1238 2022-11-22 16:38:22.000000 icenet-0.2.5/docs/icenet.model.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      671 2022-11-22 16:38:41.000000 icenet-0.2.5/docs/icenet.plotting.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1122 2022-11-22 16:39:14.000000 icenet-0.2.5/docs/icenet.process.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      168 2022-11-22 16:39:20.000000 icenet-0.2.5/docs/icenet.results.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      444 2023-02-02 12:45:59.000000 icenet-0.2.5/docs/icenet.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      343 2022-11-22 17:17:40.000000 icenet-0.2.5/docs/icenet.tests.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      303 2022-11-22 16:39:50.000000 icenet-0.2.5/docs/index.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1110 2022-11-22 16:40:33.000000 icenet-0.2.5/docs/installation.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      768 2022-11-22 16:40:49.000000 icenet-0.2.5/docs/make.bat
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       55 2023-02-02 12:45:59.000000 icenet-0.2.5/docs/modules.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       55 2022-05-19 22:27:19.000000 icenet-0.2.5/docs/readme.rst
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       67 2022-11-22 16:41:07.000000 icenet-0.2.5/docs/usage.rst
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.304489 icenet-0.2.5/icenet/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      217 2023-06-23 14:31:57.000000 icenet-0.2.5/icenet/__init__.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.306488 icenet-0.2.5/icenet/data/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.5/icenet/data/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7182 2023-06-23 14:31:57.000000 icenet-0.2.5/icenet/data/cli.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     9106 2023-02-02 11:23:27.000000 icenet-0.2.5/icenet/data/dataset.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.306488 icenet-0.2.5/icenet/data/datasets/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-06-18 16:56:02.000000 icenet-0.2.5/icenet/data/datasets/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     8145 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/data/datasets/utils.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.307489 icenet-0.2.5/icenet/data/interfaces/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.5/icenet/data/interfaces/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    10896 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/data/interfaces/cds.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     6830 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/data/interfaces/cmems.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    23972 2023-06-22 07:41:55.000000 icenet-0.2.5/icenet/data/interfaces/downloader.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     9244 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/data/interfaces/esgf.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    14765 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/data/interfaces/mars.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7838 2022-11-22 15:28:41.000000 icenet-0.2.5/icenet/data/interfaces/utils.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     4068 2023-06-22 07:41:55.000000 icenet-0.2.5/icenet/data/loader.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.308488 icenet-0.2.5/icenet/data/loaders/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1454 2022-12-22 13:08:59.000000 icenet-0.2.5/icenet/data/loaders/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    11679 2023-06-22 07:41:55.000000 icenet-0.2.5/icenet/data/loaders/base.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    17301 2023-06-14 13:21:26.000000 icenet-0.2.5/icenet/data/loaders/dask.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      864 2022-11-22 15:29:16.000000 icenet-0.2.5/icenet/data/loaders/stdlib.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1536 2022-09-29 11:27:40.000000 icenet-0.2.5/icenet/data/loaders/utils.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    23399 2023-06-22 07:41:55.000000 icenet-0.2.5/icenet/data/process.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.310488 icenet-0.2.5/icenet/data/processors/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.5/icenet/data/processors/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1747 2023-06-22 07:41:55.000000 icenet-0.2.5/icenet/data/processors/cmip.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      988 2023-06-22 07:41:55.000000 icenet-0.2.5/icenet/data/processors/era5.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      995 2023-06-22 07:41:55.000000 icenet-0.2.5/icenet/data/processors/hres.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3534 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/data/processors/meta.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      984 2023-06-22 07:41:55.000000 icenet-0.2.5/icenet/data/processors/oras5.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2078 2023-06-22 07:41:55.000000 icenet-0.2.5/icenet/data/processors/osi.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     6512 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/data/processors/utils.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    10779 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/data/producers.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.310488 icenet-0.2.5/icenet/data/sic/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.5/icenet/data/sic/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    10059 2023-02-02 11:23:27.000000 icenet-0.2.5/icenet/data/sic/mask.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    24591 2023-06-22 07:41:55.000000 icenet-0.2.5/icenet/data/sic/osisaf.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       64 2022-06-15 11:18:18.000000 icenet-0.2.5/icenet/data/sic/utils.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7074 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/data/utils.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.312488 icenet-0.2.5/icenet/model/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.5/icenet/model/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     4118 2022-11-22 15:32:01.000000 icenet-0.2.5/icenet/model/callbacks.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1029 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/model/losses.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     9515 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/model/metrics.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7903 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/model/models.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     7201 2023-06-22 07:41:55.000000 icenet-0.2.5/icenet/model/predict.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    16918 2023-06-22 07:41:55.000000 icenet-0.2.5/icenet/model/train.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3921 2022-11-22 16:15:24.000000 icenet-0.2.5/icenet/model/utils.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.312488 icenet-0.2.5/icenet/plotting/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.5/icenet/plotting/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     4593 2023-06-22 07:41:55.000000 icenet-0.2.5/icenet/plotting/data.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    75295 2023-06-22 07:41:55.000000 icenet-0.2.5/icenet/plotting/forecast.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      250 2022-11-22 16:15:42.000000 icenet-0.2.5/icenet/plotting/trend.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    15077 2023-06-22 07:41:55.000000 icenet-0.2.5/icenet/plotting/utils.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    12356 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/plotting/video.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.313488 icenet-0.2.5/icenet/process/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.5/icenet/process/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2491 2022-11-22 16:15:59.000000 icenet-0.2.5/icenet/process/azure.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     5714 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/process/forecasts.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1447 2022-11-22 16:16:07.000000 icenet-0.2.5/icenet/process/local.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)    11256 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/process/predict.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.5/icenet/process/train.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      874 2022-08-11 12:13:43.000000 icenet-0.2.5/icenet/process/utils.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.314489 icenet-0.2.5/icenet/results/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        0 2022-02-03 09:47:39.000000 icenet-0.2.5/icenet/results/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     1674 2023-02-02 11:23:27.000000 icenet-0.2.5/icenet/results/threshold.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.314489 icenet-0.2.5/icenet/tests/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)       36 2022-11-22 15:25:11.000000 icenet-0.2.5/icenet/tests/__init__.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      758 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/tests/test_entry_points.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      540 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/tests/test_mod.py
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2580 2023-03-07 11:38:13.000000 icenet-0.2.5/icenet/utils.py
+drwxrwxr-x   0 jambyr    (1000) jambyr    (1000)        0 2023-06-23 14:35:26.305488 icenet-0.2.5/icenet.egg-info/
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     3212 2023-06-23 14:35:26.000000 icenet-0.2.5/icenet.egg-info/PKG-INFO
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2846 2023-06-23 14:35:26.000000 icenet-0.2.5/icenet.egg-info/SOURCES.txt
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        1 2023-06-23 14:35:26.000000 icenet-0.2.5/icenet.egg-info/dependency_links.txt
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     2159 2023-06-23 14:35:26.000000 icenet-0.2.5/icenet.egg-info/entry_points.txt
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        1 2023-06-23 14:35:26.000000 icenet-0.2.5/icenet.egg-info/not-zip-safe
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      372 2023-06-23 14:35:26.000000 icenet-0.2.5/icenet.egg-info/requires.txt
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)        7 2023-06-23 14:35:26.000000 icenet-0.2.5/icenet.egg-info/top_level.txt
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)      173 2023-06-23 14:35:26.315488 icenet-0.2.5/setup.cfg
+-rw-rw-r--   0 jambyr    (1000) jambyr    (1000)     4419 2023-06-22 07:41:55.000000 icenet-0.2.5/setup.py
```

### Comparing `icenet-0.2.4/CONTRIBUTING.rst` & `icenet-0.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/LICENSE` & `icenet-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/PKG-INFO` & `icenet-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icenet
-Version: 0.2.4
+Version: 0.2.5
 Summary: Library for operational IceNet forecasting
 Home-page: https://github.com/icenet-ai
 Author: British Antarctic Survey / Alan Turing Institute
 Author-email: jambyr@bas.ac.uk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: icenet Version: 0.2.4 Summary: Library for
+Metadata-Version: 2.1 Name: icenet Version: 0.2.5 Summary: Library for
 operational IceNet forecasting Home-page: https://github.com/icenet-ai Author:
 British Antarctic Survey / Alan Turing Institute Author-email: jambyr@bas.ac.uk
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Natural Language :: English Classifier:
 Operating System :: POSIX Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `icenet-0.2.4/README.md` & `icenet-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/docs/Makefile` & `icenet-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/docs/_build/html/_static/ajax-loader.gif` & `icenet-0.2.5/docs/_build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/docs/_build/html/_static/comment-bright.png` & `icenet-0.2.5/docs/_build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/docs/_build/html/_static/comment-close.png` & `icenet-0.2.5/docs/_build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/docs/_build/html/_static/comment.png` & `icenet-0.2.5/docs/_build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/docs/conf.py` & `icenet-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/docs/icenet.data.interfaces.rst` & `icenet-0.2.5/docs/icenet.data.interfaces.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/docs/icenet.data.loaders.rst` & `icenet-0.2.5/docs/icenet.data.loaders.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/docs/icenet.data.processors.rst` & `icenet-0.2.5/docs/icenet.data.processors.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/docs/icenet.data.rst` & `icenet-0.2.5/docs/icenet.data.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/docs/icenet.model.rst` & `icenet-0.2.5/docs/icenet.model.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/docs/icenet.plotting.rst` & `icenet-0.2.5/docs/icenet.plotting.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/docs/icenet.process.rst` & `icenet-0.2.5/docs/icenet.process.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/docs/installation.rst` & `icenet-0.2.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/docs/make.bat` & `icenet-0.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/cli.py` & `icenet-0.2.5/icenet/data/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
     if dates:
         add_date_args(ap)
 
     ap.add_argument("-l", "--lag", type=int, default=2)
     ap.add_argument("-f", "--forecast", type=int, default=93)
     ap.add_argument("-p", "--parallel-opens",
-                    type=bool, default=False, action="store_true",
+                    default=False, action="store_true",
                     help="Allow xarray mfdataset to work with parallel opens")
 
     ap.add_argument("--abs",
                     help="Comma separated list of abs vars",
                     type=csv_arg,
                     default=[])
     ap.add_argument("--anom",
```

### Comparing `icenet-0.2.4/icenet/data/dataset.py` & `icenet-0.2.5/icenet/data/dataset.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/datasets/utils.py` & `icenet-0.2.5/icenet/data/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/interfaces/cds.py` & `icenet-0.2.5/icenet/data/interfaces/cds.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/interfaces/cmems.py` & `icenet-0.2.5/icenet/data/interfaces/cmems.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/interfaces/downloader.py` & `icenet-0.2.5/icenet/data/interfaces/downloader.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/interfaces/esgf.py` & `icenet-0.2.5/icenet/data/interfaces/esgf.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/interfaces/mars.py` & `icenet-0.2.5/icenet/data/interfaces/mars.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/interfaces/utils.py` & `icenet-0.2.5/icenet/data/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/loader.py` & `icenet-0.2.5/icenet/data/loader.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/loaders/__init__.py` & `icenet-0.2.5/icenet/data/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/loaders/base.py` & `icenet-0.2.5/icenet/data/loaders/base.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/loaders/dask.py` & `icenet-0.2.5/icenet/data/loaders/dask.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/loaders/stdlib.py` & `icenet-0.2.5/icenet/data/loaders/stdlib.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/loaders/utils.py` & `icenet-0.2.5/icenet/data/loaders/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/process.py` & `icenet-0.2.5/icenet/data/process.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/processors/cmip.py` & `icenet-0.2.5/icenet/data/processors/cmip.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/processors/era5.py` & `icenet-0.2.5/icenet/data/processors/era5.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/processors/hres.py` & `icenet-0.2.5/icenet/data/processors/hres.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/processors/meta.py` & `icenet-0.2.5/icenet/data/processors/meta.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/processors/oras5.py` & `icenet-0.2.5/icenet/data/processors/oras5.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/processors/osi.py` & `icenet-0.2.5/icenet/data/processors/osi.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/processors/utils.py` & `icenet-0.2.5/icenet/data/processors/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/producers.py` & `icenet-0.2.5/icenet/data/producers.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/sic/mask.py` & `icenet-0.2.5/icenet/data/sic/mask.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/sic/osisaf.py` & `icenet-0.2.5/icenet/data/sic/osisaf.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/data/utils.py` & `icenet-0.2.5/icenet/data/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/model/callbacks.py` & `icenet-0.2.5/icenet/model/callbacks.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/model/losses.py` & `icenet-0.2.5/icenet/model/losses.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/model/metrics.py` & `icenet-0.2.5/icenet/model/metrics.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/model/models.py` & `icenet-0.2.5/icenet/model/models.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/model/predict.py` & `icenet-0.2.5/icenet/model/predict.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/model/train.py` & `icenet-0.2.5/icenet/model/train.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/model/utils.py` & `icenet-0.2.5/icenet/model/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/plotting/data.py` & `icenet-0.2.5/icenet/plotting/data.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/plotting/forecast.py` & `icenet-0.2.5/icenet/plotting/forecast.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/plotting/utils.py` & `icenet-0.2.5/icenet/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/plotting/video.py` & `icenet-0.2.5/icenet/plotting/video.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/process/azure.py` & `icenet-0.2.5/icenet/process/azure.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/process/forecasts.py` & `icenet-0.2.5/icenet/process/forecasts.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/process/local.py` & `icenet-0.2.5/icenet/process/local.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/process/predict.py` & `icenet-0.2.5/icenet/process/predict.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/process/utils.py` & `icenet-0.2.5/icenet/process/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/results/threshold.py` & `icenet-0.2.5/icenet/results/threshold.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/tests/test_entry_points.py` & `icenet-0.2.5/icenet/tests/test_entry_points.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/tests/test_mod.py` & `icenet-0.2.5/icenet/tests/test_mod.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet/utils.py` & `icenet-0.2.5/icenet/utils.py`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet.egg-info/PKG-INFO` & `icenet-0.2.5/icenet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icenet
-Version: 0.2.4
+Version: 0.2.5
 Summary: Library for operational IceNet forecasting
 Home-page: https://github.com/icenet-ai
 Author: British Antarctic Survey / Alan Turing Institute
 Author-email: jambyr@bas.ac.uk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: icenet Version: 0.2.4 Summary: Library for
+Metadata-Version: 2.1 Name: icenet Version: 0.2.5 Summary: Library for
 operational IceNet forecasting Home-page: https://github.com/icenet-ai Author:
 British Antarctic Survey / Alan Turing Institute Author-email: jambyr@bas.ac.uk
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Natural Language :: English Classifier:
 Operating System :: POSIX Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `icenet-0.2.4/icenet.egg-info/SOURCES.txt` & `icenet-0.2.5/icenet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/icenet.egg-info/entry_points.txt` & `icenet-0.2.5/icenet.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `icenet-0.2.4/setup.py` & `icenet-0.2.5/setup.py`

 * *Files identical despite different names*

