# Comparing `tmp/material_zui-0.1.1.tar.gz` & `tmp/material_zui-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "material_zui-0.1.1.tar", max compression
+gzip compressed data, was "material_zui-0.1.2.tar", max compression
```

## Comparing `material_zui-0.1.1.tar` & `material_zui-0.1.2.tar`

### file list

```diff
@@ -1,79 +1,102 @@
--rw-r--r--   0        0        0     1014 2023-05-22 02:20:08.172393 material_zui-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      260 2023-05-01 15:33:57.972869 material_zui-0.1.1/src/material_zui/.pypirc
--rw-r--r--   0        0        0      555 2023-03-21 08:40:33.421115 material_zui-0.1.1/src/material_zui/ResizeImage.py
--rw-r--r--   0        0        0       39 2023-05-21 04:19:03.692146 material_zui-0.1.1/src/material_zui/array/__init__.py
--rw-r--r--   0        0        0      188 2023-05-21 04:22:47.696141 material_zui-0.1.1/src/material_zui/array/common.py
--rw-r--r--   0        0        0       71 2023-05-21 04:23:10.983205 material_zui-0.1.1/src/material_zui/array/index.py
--rw-r--r--   0        0        0     2405 2023-05-20 11:57:06.283965 material_zui-0.1.1/src/material_zui/automation/Constant.py
--rw-r--r--   0        0        0       44 2023-05-21 02:36:24.004618 material_zui-0.1.1/src/material_zui/automation/__init__.py
--rw-r--r--   0        0        0      110 2023-05-21 04:26:37.532312 material_zui-0.1.1/src/material_zui/automation/index.py
--rw-r--r--   0        0        0        0 2023-05-21 02:38:12.347239 material_zui-0.1.1/src/material_zui/automation/pinterest.py
--rw-r--r--   0        0        0     5167 2023-05-21 12:06:03.029430 material_zui-0.1.1/src/material_zui/automation/tiktok.py
--rw-r--r--   0        0        0      310 2023-05-21 14:22:10.812226 material_zui-0.1.1/src/material_zui/automation/type.py
--rw-r--r--   0        0        0     8776 2023-05-22 02:09:15.260250 material_zui-0.1.1/src/material_zui/automation/youtube.py
--rw-r--r--   0        0        0       38 2023-05-15 08:52:40.288888 material_zui-0.1.1/src/material_zui/bard/__init__.py
--rw-r--r--   0        0        0      543 2023-05-15 09:14:12.082997 material_zui-0.1.1/src/material_zui/bard/google_bard.py
--rw-r--r--   0        0        0       77 2023-05-15 09:15:57.588848 material_zui-0.1.1/src/material_zui/bard/index.py
--rw-r--r--   0        0        0       42 2023-05-07 05:09:56.400820 material_zui-0.1.1/src/material_zui/compress/__init__.py
--rw-r--r--   0        0        0       74 2023-05-07 05:16:12.115224 material_zui-0.1.1/src/material_zui/compress/index.py
--rw-r--r--   0        0        0     2131 2023-05-07 05:22:45.101162 material_zui-0.1.1/src/material_zui/compress/text.py
--rw-r--r--   0        0        0       36 2023-05-02 13:44:44.126257 material_zui-0.1.1/src/material_zui/crawl/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 13:44:44.126257 material_zui-0.1.1/src/material_zui/crawl/index.py
--rw-r--r--   0        0        0       41 2023-05-11 04:24:47.172982 material_zui-0.1.1/src/material_zui/crontab/__init__.py
--rw-r--r--   0        0        0      638 2023-05-11 04:23:06.569200 material_zui-0.1.1/src/material_zui/crontab/index.py
--rw-r--r--   0        0        0       43 2023-05-07 14:15:59.556081 material_zui-0.1.1/src/material_zui/date_time/__init__.py
--rw-r--r--   0        0        0       60 2023-05-07 14:15:59.604081 material_zui-0.1.1/src/material_zui/date_time/date_time.py
--rw-r--r--   0        0        0       49 2023-05-07 14:16:28.308295 material_zui-0.1.1/src/material_zui/date_time/index.py
--rw-r--r--   0        0        0      692 2023-05-07 14:16:10.888166 material_zui-0.1.1/src/material_zui/date_time/time.py
--rw-r--r--   0        0        0       36 2023-05-21 13:41:44.819759 material_zui-0.1.1/src/material_zui/dict/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 13:45:02.045051 material_zui-0.1.1/src/material_zui/dict/common.py
--rw-r--r--   0        0        0        0 2023-05-21 13:41:44.819759 material_zui-0.1.1/src/material_zui/dict/index.py
--rw-r--r--   0        0        0       37 2023-05-15 08:36:55.132989 material_zui-0.1.1/src/material_zui/env/__init__.py
--rw-r--r--   0        0        0      183 2023-05-15 09:09:28.356336 material_zui-0.1.1/src/material_zui/env/env.py
--rw-r--r--   0        0        0       52 2023-05-15 08:46:26.760087 material_zui-0.1.1/src/material_zui/env/index.py
--rw-r--r--   0        0        0       38 2023-05-19 02:12:30.886319 material_zui-0.1.1/src/material_zui/fake/__init__.py
--rw-r--r--   0        0        0       62 2023-05-19 02:24:23.295278 material_zui-0.1.1/src/material_zui/fake/index.py
--rw-r--r--   0        0        0      254 2023-05-21 05:39:54.079978 material_zui-0.1.1/src/material_zui/fake/number.py
--rw-r--r--   0        0        0       38 2023-05-21 03:57:08.912678 material_zui-0.1.1/src/material_zui/file/__init__.py
--rw-r--r--   0        0        0      946 2023-05-21 13:48:05.374204 material_zui-0.1.1/src/material_zui/file/download.py
--rw-r--r--   0        0        0       83 2023-05-21 13:48:26.988466 material_zui-0.1.1/src/material_zui/file/index.py
--rw-r--r--   0        0        0       37 2023-05-15 08:50:53.425688 material_zui-0.1.1/src/material_zui/gpt/__init__.py
--rw-r--r--   0        0        0     1057 2023-05-15 05:15:31.650338 material_zui-0.1.1/src/material_zui/gpt/gpt_vietnam.py
--rw-r--r--   0        0        0       62 2023-05-15 08:50:53.385689 material_zui-0.1.1/src/material_zui/gpt/index.py
--rw-r--r--   0        0        0      216 2023-05-11 09:54:07.451440 material_zui-0.1.1/src/material_zui/image/__init__.py
--rw-r--r--   0        0        0     2199 2023-05-05 09:48:58.874264 material_zui-0.1.1/src/material_zui/image/colorization.py
--rw-r--r--   0        0        0     2921 2023-05-11 09:52:23.138728 material_zui-0.1.1/src/material_zui/image/combine.py
--rw-r--r--   0        0        0     5490 2023-05-11 10:24:19.669145 material_zui-0.1.1/src/material_zui/image/common.py
--rw-r--r--   0        0        0     2808 2023-05-11 10:13:26.444992 material_zui-0.1.1/src/material_zui/image/convert.py
--rw-r--r--   0        0        0       78 2023-05-06 06:26:57.697131 material_zui-0.1.1/src/material_zui/image/data.py
--rw-r--r--   0        0        0      461 2023-05-11 10:14:50.303432 material_zui-0.1.1/src/material_zui/image/index.py
--rw-r--r--   0        0        0     9945 2023-05-05 03:49:43.138352 material_zui-0.1.1/src/material_zui/image/model/colorization_deploy_v2.prototxt
--rw-r--r--   0        0        0     5088 2023-05-05 03:49:53.225773 material_zui-0.1.1/src/material_zui/image/model/pts_in_hull.npy
--rw-r--r--   0        0        0      782 2023-05-11 04:50:18.808963 material_zui-0.1.1/src/material_zui/image/remove_background.py
--rw-r--r--   0        0        0     6445 2023-05-06 08:59:41.215230 material_zui-0.1.1/src/material_zui/image/to_svg.py
--rw-r--r--   0        0        0      520 2023-05-11 09:48:54.829117 material_zui-0.1.1/src/material_zui/image/transparent_background.py
--rw-r--r--   0        0        0      249 2023-04-28 09:24:02.020353 material_zui-0.1.1/src/material_zui/image/type.py
--rw-r--r--   0        0        0     4779 2023-05-11 10:15:27.410813 material_zui-0.1.1/src/material_zui/image/upscale.py
--rw-r--r--   0        0        0       37 2023-04-30 11:48:06.179161 material_zui-0.1.1/src/material_zui/log/__init__.py
--rw-r--r--   0        0        0       83 2023-05-11 10:20:42.114888 material_zui-0.1.1/src/material_zui/log/index.py
--rw-r--r--   0        0        0      559 2023-05-11 10:19:34.415566 material_zui-0.1.1/src/material_zui/log/log.py
--rw-r--r--   0        0        0       36 2023-05-20 14:09:01.119097 material_zui-0.1.1/src/material_zui/os/__init__.py
--rw-r--r--   0        0        0       38 2023-05-20 14:09:01.031103 material_zui-0.1.1/src/material_zui/os/index.py
--rw-r--r--   0        0        0      188 2023-05-20 14:09:01.199091 material_zui-0.1.1/src/material_zui/os/os.py
--rw-r--r--   0        0        0     1140 2023-05-22 02:19:02.483823 material_zui-0.1.1/src/material_zui/readme.md
--rw-r--r--   0        0        0       39 2023-05-02 05:15:13.799596 material_zui-0.1.1/src/material_zui/regex/__init__.py
--rw-r--r--   0        0        0     5344 2023-05-02 05:18:47.668155 material_zui-0.1.1/src/material_zui/regex/index.py
--rw-r--r--   0        0        0       43 2023-04-30 11:47:27.662335 material_zui-0.1.1/src/material_zui/replicate/__init__.py
--rw-r--r--   0        0        0     2481 2023-05-01 15:33:18.205379 material_zui-0.1.1/src/material_zui/replicate/index.py
--rw-r--r--   0        0        0       42 2023-05-18 03:46:44.861073 material_zui-0.1.1/src/material_zui/selenium/__init__.py
--rw-r--r--   0        0        0     1726 2023-05-22 02:05:38.471188 material_zui-0.1.1/src/material_zui/selenium/chrome.py
--rw-r--r--   0        0        0      257 2023-05-22 02:03:22.582766 material_zui-0.1.1/src/material_zui/selenium/common.py
--rw-r--r--   0        0        0      120 2023-05-22 02:03:54.393486 material_zui-0.1.1/src/material_zui/selenium/index.py
--rw-r--r--   0        0        0      895 2023-05-11 10:31:29.010961 material_zui-0.1.1/src/material_zui/setup.py
--rw-r--r--   0        0        0       46 2023-05-02 13:44:38.645684 material_zui-0.1.1/src/material_zui/telegram_bot/__init__.py
--rw-r--r--   0        0        0      432 2023-05-07 05:43:32.880583 material_zui-0.1.1/src/material_zui/telegram_bot/index.py
--rw-r--r--   0        0        0       36 2023-04-30 11:48:06.223146 material_zui-0.1.1/src/material_zui/tmp/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 03:39:00.036364 material_zui-0.1.1/src/material_zui/tmp/index.py
--rw-r--r--   0        0        0       36 2023-05-01 14:11:23.375942 material_zui-0.1.1/src/material_zui/validate/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 14:11:23.379941 material_zui-0.1.1/src/material_zui/validate/index.py
--rw-r--r--   0        0        0     2491 1970-01-01 00:00:00.000000 material_zui-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-06-23 08:06:01.615959 material_zui-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-05-01 15:33:57.972869 material_zui-0.1.2/src/material_zui/.pypirc
+-rw-r--r--   0        0        0      555 2023-03-21 08:40:33.421115 material_zui-0.1.2/src/material_zui/ResizeImage.py
+-rw-r--r--   0        0        0     2405 2023-05-20 11:57:06.283965 material_zui-0.1.2/src/material_zui/automation/Constant.py
+-rw-r--r--   0        0        0       44 2023-05-21 02:36:24.004618 material_zui-0.1.2/src/material_zui/automation/__init__.py
+-rw-r--r--   0        0        0      175 2023-06-18 12:07:30.298939 material_zui-0.1.2/src/material_zui/automation/data.py
+-rw-r--r--   0        0        0      110 2023-05-21 04:26:37.532312 material_zui-0.1.2/src/material_zui/automation/index.py
+-rw-r--r--   0        0        0        0 2023-05-21 02:38:12.347239 material_zui-0.1.2/src/material_zui/automation/pinterest.py
+-rw-r--r--   0        0        0    10600 2023-06-19 01:47:01.519677 material_zui-0.1.2/src/material_zui/automation/tiktok.py
+-rw-r--r--   0        0        0      310 2023-05-21 14:22:10.812226 material_zui-0.1.2/src/material_zui/automation/type.py
+-rw-r--r--   0        0        0    13957 2023-06-23 02:26:53.960600 material_zui-0.1.2/src/material_zui/automation/youtube.py
+-rw-r--r--   0        0        0       38 2023-05-25 02:02:05.757233 material_zui-0.1.2/src/material_zui/bard/__init__.py
+-rw-r--r--   0        0        0      543 2023-05-25 02:04:14.001207 material_zui-0.1.2/src/material_zui/bard/google_bard.py
+-rw-r--r--   0        0        0       77 2023-05-25 02:02:05.757233 material_zui-0.1.2/src/material_zui/bard/index.py
+-rw-r--r--   0        0        0       41 2023-06-09 09:12:08.062573 material_zui-0.1.2/src/material_zui/bing_ai/__init__.py
+-rw-r--r--   0        0        0     2572 2023-06-14 10:38:43.733788 material_zui-0.1.2/src/material_zui/bing_ai/bing_ai.py
+-rw-r--r--   0        0        0       51 2023-06-09 09:12:20.262575 material_zui-0.1.2/src/material_zui/bing_ai/index.py
+-rw-r--r--   0        0        0      868 2023-06-14 08:51:22.816844 material_zui-0.1.2/src/material_zui/bing_ai/result.py
+-rw-r--r--   0        0        0       42 2023-05-07 05:09:56.400820 material_zui-0.1.2/src/material_zui/compress/__init__.py
+-rw-r--r--   0        0        0       74 2023-05-07 05:16:12.115224 material_zui-0.1.2/src/material_zui/compress/index.py
+-rw-r--r--   0        0        0     2131 2023-05-07 05:22:45.101162 material_zui-0.1.2/src/material_zui/compress/text.py
+-rw-r--r--   0        0        0       39 2023-05-22 10:20:44.145129 material_zui-0.1.2/src/material_zui/crawl/__init__.py
+-rw-r--r--   0        0        0     3282 2023-05-28 04:29:31.650227 material_zui-0.1.2/src/material_zui/crawl/image.py
+-rw-r--r--   0        0        0      171 2023-05-28 04:26:35.259642 material_zui-0.1.2/src/material_zui/crawl/index.py
+-rw-r--r--   0        0        0       41 2023-05-11 04:24:47.172982 material_zui-0.1.2/src/material_zui/crontab/__init__.py
+-rw-r--r--   0        0        0      638 2023-05-11 04:23:06.569200 material_zui-0.1.2/src/material_zui/crontab/index.py
+-rw-r--r--   0        0        0       21 2023-06-12 02:21:47.920504 material_zui-0.1.2/src/material_zui/date_time/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-12 02:56:34.237482 material_zui-0.1.2/src/material_zui/date_time/__init__.pyc
+-rw-r--r--   0        0        0      491 2023-06-18 06:24:16.415897 material_zui-0.1.2/src/material_zui/date_time/date_time.py
+-rw-r--r--   0        0        0       73 2023-06-13 08:55:03.914876 material_zui-0.1.2/src/material_zui/date_time/index.py
+-rw-r--r--   0        0        0      180 2023-06-12 02:58:53.334820 material_zui-0.1.2/src/material_zui/date_time/index.pyc
+-rw-r--r--   0        0        0      692 2023-05-07 14:16:10.888166 material_zui-0.1.2/src/material_zui/date_time/time.py
+-rw-r--r--   0        0        0       36 2023-05-21 13:41:44.819759 material_zui-0.1.2/src/material_zui/dict/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:45:02.045051 material_zui-0.1.2/src/material_zui/dict/common.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:41:44.819759 material_zui-0.1.2/src/material_zui/dict/index.py
+-rw-r--r--   0        0        0       37 2023-05-15 08:36:55.132989 material_zui-0.1.2/src/material_zui/env/__init__.py
+-rw-r--r--   0        0        0      183 2023-05-15 09:09:28.356336 material_zui-0.1.2/src/material_zui/env/env.py
+-rw-r--r--   0        0        0       52 2023-05-15 08:46:26.760087 material_zui-0.1.2/src/material_zui/env/index.py
+-rw-r--r--   0        0        0       38 2023-05-19 02:12:30.886319 material_zui-0.1.2/src/material_zui/fake/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-19 02:24:23.295278 material_zui-0.1.2/src/material_zui/fake/index.py
+-rw-r--r--   0        0        0      254 2023-05-21 05:39:54.079978 material_zui-0.1.2/src/material_zui/fake/number.py
+-rw-r--r--   0        0        0       38 2023-05-21 03:57:08.912678 material_zui-0.1.2/src/material_zui/file/__init__.py
+-rw-r--r--   0        0        0      551 2023-06-23 07:37:11.257875 material_zui-0.1.2/src/material_zui/file/check.py
+-rw-r--r--   0        0        0     2115 2023-06-15 03:25:12.103320 material_zui-0.1.2/src/material_zui/file/common.py
+-rw-r--r--   0        0        0      304 2023-06-15 03:25:12.271318 material_zui-0.1.2/src/material_zui/file/download.py
+-rw-r--r--   0        0        0      326 2023-06-23 08:03:00.554832 material_zui-0.1.2/src/material_zui/file/index.py
+-rw-r--r--   0        0        0     1042 2023-06-15 03:25:12.027320 material_zui-0.1.2/src/material_zui/file/read.py
+-rw-r--r--   0        0        0       77 2023-06-10 05:42:45.080334 material_zui-0.1.2/src/material_zui/file/type.py
+-rw-r--r--   0        0        0      992 2023-06-23 08:03:07.838708 material_zui-0.1.2/src/material_zui/file/write.py
+-rw-r--r--   0        0        0       37 2023-05-25 02:02:05.757233 material_zui-0.1.2/src/material_zui/gpt/__init__.py
+-rw-r--r--   0        0        0     1048 2023-05-25 02:22:20.028251 material_zui-0.1.2/src/material_zui/gpt/gpt_vietnam.py
+-rw-r--r--   0        0        0       63 2023-05-25 02:22:19.960250 material_zui-0.1.2/src/material_zui/gpt/index.py
+-rw-r--r--   0        0        0      216 2023-05-11 09:54:07.451440 material_zui-0.1.2/src/material_zui/image/__init__.py
+-rw-r--r--   0        0        0     2199 2023-05-05 09:48:58.874264 material_zui-0.1.2/src/material_zui/image/colorization.py
+-rw-r--r--   0        0        0     2921 2023-05-11 09:52:23.138728 material_zui-0.1.2/src/material_zui/image/combine.py
+-rw-r--r--   0        0        0     7057 2023-05-28 04:11:03.932782 material_zui-0.1.2/src/material_zui/image/common.py
+-rw-r--r--   0        0        0     2808 2023-05-11 10:13:26.444992 material_zui-0.1.2/src/material_zui/image/convert.py
+-rw-r--r--   0        0        0       78 2023-05-06 06:26:57.697131 material_zui-0.1.2/src/material_zui/image/data.py
+-rw-r--r--   0        0        0      490 2023-05-28 04:11:04.028780 material_zui-0.1.2/src/material_zui/image/index.py
+-rw-r--r--   0        0        0     9945 2023-05-05 03:49:43.138352 material_zui-0.1.2/src/material_zui/image/model/colorization_deploy_v2.prototxt
+-rw-r--r--   0        0        0     5088 2023-05-05 03:49:53.225773 material_zui-0.1.2/src/material_zui/image/model/pts_in_hull.npy
+-rw-r--r--   0        0        0      782 2023-05-11 04:50:18.808963 material_zui-0.1.2/src/material_zui/image/remove_background.py
+-rw-r--r--   0        0        0     6445 2023-05-06 08:59:41.215230 material_zui-0.1.2/src/material_zui/image/to_svg.py
+-rw-r--r--   0        0        0      520 2023-05-11 09:48:54.829117 material_zui-0.1.2/src/material_zui/image/transparent_background.py
+-rw-r--r--   0        0        0      249 2023-04-28 09:24:02.020353 material_zui-0.1.2/src/material_zui/image/type.py
+-rw-r--r--   0        0        0     4779 2023-05-11 10:15:27.410813 material_zui-0.1.2/src/material_zui/image/upscale.py
+-rw-r--r--   0        0        0       38 2023-05-22 04:09:03.922071 material_zui-0.1.2/src/material_zui/list/__init__.py
+-rw-r--r--   0        0        0     2916 2023-06-18 14:13:03.127264 material_zui-0.1.2/src/material_zui/list/common.py
+-rw-r--r--   0        0        0       92 2023-06-13 09:15:39.330734 material_zui-0.1.2/src/material_zui/list/index.py
+-rw-r--r--   0        0        0       37 2023-04-30 11:48:06.179161 material_zui-0.1.2/src/material_zui/log/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-11 10:20:42.114888 material_zui-0.1.2/src/material_zui/log/index.py
+-rw-r--r--   0        0        0      559 2023-05-11 10:19:34.415566 material_zui-0.1.2/src/material_zui/log/log.py
+-rw-r--r--   0        0        0       21 2023-06-13 09:33:05.320819 material_zui-0.1.2/src/material_zui/number/__init__.py
+-rw-r--r--   0        0        0      364 2023-06-13 10:11:32.006838 material_zui-0.1.2/src/material_zui/number/common.py
+-rw-r--r--   0        0        0       47 2023-06-13 09:40:32.023908 material_zui-0.1.2/src/material_zui/number/index.py
+-rw-r--r--   0        0        0       36 2023-05-20 14:09:01.119097 material_zui-0.1.2/src/material_zui/os/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-16 02:02:57.672095 material_zui-0.1.2/src/material_zui/os/index.py
+-rw-r--r--   0        0        0      840 2023-06-15 03:40:00.119319 material_zui-0.1.2/src/material_zui/os/os.py
+-rw-r--r--   0        0        0     1213 2023-06-23 08:04:27.953396 material_zui-0.1.2/src/material_zui/readme.md
+-rw-r--r--   0        0        0       39 2023-05-02 05:15:13.799596 material_zui-0.1.2/src/material_zui/regex/__init__.py
+-rw-r--r--   0        0        0     5344 2023-05-02 05:18:47.668155 material_zui-0.1.2/src/material_zui/regex/index.py
+-rw-r--r--   0        0        0       43 2023-04-30 11:47:27.662335 material_zui-0.1.2/src/material_zui/replicate/__init__.py
+-rw-r--r--   0        0        0     2481 2023-05-01 15:33:18.205379 material_zui-0.1.2/src/material_zui/replicate/index.py
+-rw-r--r--   0        0        0       42 2023-05-18 03:46:44.861073 material_zui-0.1.2/src/material_zui/selenium/__init__.py
+-rw-r--r--   0        0        0     5939 2023-06-18 11:54:12.858507 material_zui-0.1.2/src/material_zui/selenium/chrome.py
+-rw-r--r--   0        0        0      257 2023-05-22 02:03:22.582766 material_zui-0.1.2/src/material_zui/selenium/common.py
+-rw-r--r--   0        0        0      120 2023-05-22 02:03:54.393486 material_zui-0.1.2/src/material_zui/selenium/index.py
+-rw-r--r--   0        0        0      895 2023-05-11 10:31:29.010961 material_zui-0.1.2/src/material_zui/setup.py
+-rw-r--r--   0        0        0       40 2023-06-10 10:50:13.743103 material_zui-0.1.2/src/material_zui/string/__init__.py
+-rw-r--r--   0        0        0     2802 2023-06-18 14:03:40.774857 material_zui-0.1.2/src/material_zui/string/common.py
+-rw-r--r--   0        0        0      135 2023-06-14 08:12:20.153192 material_zui-0.1.2/src/material_zui/string/index.py
+-rw-r--r--   0        0        0       46 2023-05-02 13:44:38.645684 material_zui-0.1.2/src/material_zui/telegram_bot/__init__.py
+-rw-r--r--   0        0        0      432 2023-05-07 05:43:32.880583 material_zui-0.1.2/src/material_zui/telegram_bot/index.py
+-rw-r--r--   0        0        0       23 2023-06-12 02:21:47.852520 material_zui-0.1.2/src/material_zui/tmp/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-12 02:21:47.776537 material_zui-0.1.2/src/material_zui/tmp/index.py
+-rw-r--r--   0        0        0       41 2023-06-11 03:35:54.474267 material_zui-0.1.2/src/material_zui/utility/__init__.py
+-rw-r--r--   0        0        0      888 2023-06-11 04:23:19.200816 material_zui-0.1.2/src/material_zui/utility/common.py
+-rw-r--r--   0        0        0       56 2023-06-11 04:21:30.408379 material_zui-0.1.2/src/material_zui/utility/index.py
+-rw-r--r--   0        0        0       42 2023-05-25 02:32:34.010325 material_zui-0.1.2/src/material_zui/validate/__init__.py
+-rw-r--r--   0        0        0      308 2023-05-28 04:05:43.248601 material_zui-0.1.2/src/material_zui/validate/common.py
+-rw-r--r--   0        0        0       65 2023-05-27 14:15:24.849747 material_zui-0.1.2/src/material_zui/validate/index.py
+-rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 material_zui-0.1.2/PKG-INFO
```

### Comparing `material_zui-0.1.1/pyproject.toml` & `material_zui-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "material_zui"
-version = "0.1.1"
+version = "0.1.2"
 description = "Material Zui"
 authors = ["chauhmnguyen <chauhoangminhnguyen@gmail.com>"]
 readme = "src/material_zui/readme.md"
 keywords = [
 	"material",
 	"zui",
 	"material zui",
@@ -26,18 +26,23 @@
 pandas = "^2.0.1"
 pythonlangutil = "^0.1"
 python-crontab = "^2.7.1"
 rembg = "^2.0.36"
 pytelegrambotapi = "^4.11.0"
 bardapi = "^0.1.2"
 python-dotenv = "^1.0.0"
-youtube-uploader-selenium = "^0.1.0"
-selenium-firefox = "^2.0.7"
 selenium = "^4.9.1"
 selenium-browser = "^0.0.15"
-bot-studio = "^1.4.0"
 webdriver-manager = "^3.8.6"
 beautifulsoup4 = "^4.12.2"
+pytube = "^15.0.0"
+newspaper3k = "^0.2.8"
+validators = "^0.20.0"
+edgegpt = "^0.10.7"
+setuptools = "^67.8.0"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `material_zui-0.1.1/src/material_zui/ResizeImage.py` & `material_zui-0.1.2/src/material_zui/ResizeImage.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/automation/Constant.py` & `material_zui-0.1.2/src/material_zui/automation/Constant.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/automation/youtube.py` & `material_zui-0.1.2/src/material_zui/automation/youtube.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 import os
+from pyparsing import Any
 from selenium.webdriver.common.keys import Keys
 from time import sleep
 from selenium.webdriver.common.by import By
 from datetime import datetime
+from pytube import YouTube, Playlist
+from pytube.exceptions import VideoUnavailable
 
 from material_zui.automation.type import Video, Videos
 from material_zui.automation.Constant import Constant
-from material_zui.file import load_json_array
-from material_zui.selenium import safe_find_element, Zui_Selenium_Chrome
-from material_zui.array import is_not_last_index
+from material_zui.selenium import Zui_Selenium_Chrome
+from material_zui.file import get_files_info, write_json, load_json_array, ZuiFile
+from material_zui.date_time import add_days
+from material_zui.list import list_range, map_to, filter_to
+from material_zui.string import list_match, trim_space, remove_special_characters
+from material_zui.utility import pipe, pipe_list
 
 
 class Zui_Youtube(Zui_Selenium_Chrome):
     '''
-    - Automation base on the system UI, so it can be out updated in the future due to the update UI
     - Tested on `Ubuntu` platform, it might work on `Linux` (or `MacOS`), not sure for `Window`
+    - Upload video use `Selenium` to automation
+        - Automation base on the system UI, so it can be out updated in the future due to the update UI
+    - Download video base on `pytube`, detail here: https://pytube.io/en/latest/index.html
     '''
 
+    def __go_to_content_page(self) -> None:
+        self.driver.find_element(
+            By.XPATH, '//*[@id="menu-paper-icon-item-1"]').click()
+
     def get_account_info(self) -> str:
         '''
         Example result:
         ```txt
         Google Account: {Account name}
         ({username}@gmail.com)
         ```
@@ -57,42 +69,42 @@
         self.delay()
         file_input = self.driver.find_element(
             By.XPATH, '//*[@id="content"]/input')
         abs_path = os.path.abspath(str(path))
         file_input.send_keys(abs_path)
 
         # set title
-        print('Setting title')
+        print('Setting title:', title)
         sleep(7)
         title_element = self.driver.find_element(
             By.XPATH, '//*[@id="textbox"]')
         title_element.send_keys(Keys.CONTROL + 'a')
         title_element.send_keys(Keys.BACKSPACE)
         title_element.send_keys(title)
 
         # set description
-        print('Setting description')
+        print('Setting description:', description)
         self.delay()
         description_element = self.driver.find_element(
-            By.XPATH, '//*/ytcp-video-metadata-editor-basics/div[2]/ytcp-social-suggestions-textbox/ytcp-form-input-container/div[1]/div[2]/div/ytcp-social-suggestion-input/div')
+            By.XPATH, '//*/ytcp-video-description/div/ytcp-social-suggestions-textbox/ytcp-form-input-container/div[1]/div[2]/div/ytcp-social-suggestion-input/div')
         description_element.send_keys(description)
 
         # set playlist
         self.delay()
         if playlist:
-            print('Setting playlist')
+            print('Setting playlist:', playlist)
             # open playlist
             self.driver.find_element(
                 By.CLASS_NAME, Constant.PL_DROPDOWN_CLASS).click()
 
             # load playlist
             sleep(5)
             playlist_items_container = self.driver.find_element(
                 By.ID, Constant.PL_ITEMS_CONTAINER_ID)
-            playlist_item = self.find_element(
+            playlist_item = self.safe_find_element(
                 By.XPATH, Constant.PL_ITEM_CONTAINER.format(playlist), playlist_items_container)
             sleep(Constant.USER_WAITING_TIME)
             if playlist_item:
                 # choose playlist existed
                 playlist_item.click()
             else:
                 # new playlist
@@ -121,16 +133,15 @@
         # select kid option
         self.delay()
         self.driver.find_element(
             By.XPATH, '//*[@id="audience"]/ytkc-made-for-kids-select/div[4]/tp-yt-paper-radio-group/tp-yt-paper-radio-button[2]').click()
 
         # set tags
         if tags and len(tags):
-            print('Setting tags')
-            print(tags)
+            print('Setting tags:', tags)
 
             # open advance option
             self.delay()
             self.driver.find_element(
                 By.XPATH, '//*[@id="toggle-button"]/div').click()
 
             # click tags
@@ -144,28 +155,32 @@
                 tags_element.send_keys(tag)
                 tags_element.send_keys(Keys.ENTER)
 
         # click next 3 time
         self.delay()
         next_button = self.driver.find_element(
             By.XPATH, '//*[@id="next-button"]')
-        for i in range(3):
+        for _ in range(3):
             next_button.click()
-            self.delay(1)
+            self.delay(5)
 
         # publish or schedule
         self.delay()
         if is_publish:  # click public to direct publish
+            print('Setting publish')
             self.driver.find_element(
                 By.XPATH, '//*[@id="privacy-radios"]/tp-yt-paper-radio-button[3]').click()
         elif schedule:  # schedule
-            date_time = datetime.strptime(str(schedule), "%m/%d/%Y, %H:%M")
+            print('Setting schedule:', schedule)
+            date_time = datetime.strptime(schedule, "%m/%d/%Y, %H:%M")
             self.driver.find_element(
                 By.ID, Constant.SCHEDULE_CONTAINER_ID).click()
             self.driver.find_element(By.ID, Constant.SCHEDULE_DATE_ID).click()
+
+            self.delay()
             self.driver.find_element(
                 By.XPATH, Constant.SCHEDULE_DATE_TEXTBOX).clear()
             self.driver.find_element(By.XPATH, Constant.SCHEDULE_DATE_TEXTBOX).send_keys(
                 datetime.strftime(date_time, "%b %e, %Y"))
             self.driver.find_element(
                 By.XPATH, Constant.SCHEDULE_DATE_TEXTBOX).send_keys(Keys.ENTER)
             self.driver.find_element(By.XPATH, Constant.SCHEDULE_TIME).click()
@@ -181,42 +196,151 @@
         # 3. click schedule (for schedule video)
         print('Submit video')
         self.delay()
         self.driver.find_element(
             By.XPATH, '//*[@id="done-button"]').click()
         self.delay(10)
 
-        video_processing_element = self.find_element(
+        video_processing_element = self.safe_find_element(
             By.XPATH, '//*[@id="close-button"]/div')
         if video_processing_element:
             video_processing_element.click()
 
     def upload_videos(self, videos: Videos) -> None:
         '''
         Upload multiple videos to YouTube
         '''
         for index, video in enumerate(videos):
             self.upload_video(video)
-            if is_not_last_index(videos, index):
-                self.delay()
+            self.delay()
+            print('Uploaded video', index+1)
+        self.__go_to_content_page()
 
     def upload_videos_from_file_info(self, video_path: str, json_file_path: str) -> None:
         '''
         Upload multiple videos from json data file
         @video_path: video path including video to publish
         @json_file_path: json file path including video info
         '''
-        def map_item(video: dict) -> Video:
+        def map_item(video: dict[Any, Any], _: int) -> Video:  # type: ignore
             file_name = str(video['file_name'])
             path = f'{video_path}/{file_name}'
             return {
                 'title': video['title'],
                 'description': video['description'],
                 'path': path,
                 'playlist': video.get('playlist'),
                 'tags': video.get('tags'),
                 'is_publish': video.get('is_publish') or False,
                 'schedule': video.get('schedule')
             }
         items = load_json_array(json_file_path)
-        videos: Videos = list(map(map_item, items))
+        videos: Videos = map_to(items, map_item)
         self.upload_videos(videos)
+
+    def download_video(self, url: str, video_output_path: str) -> None:
+        '''
+        If error network, try again with VPN connected
+        '''
+        try:
+            youtube = YouTube(url)
+            video_stream = youtube.streams.get_highest_resolution()
+        except VideoUnavailable:
+            print(f'Video {url} is unavaialable, skipping.')
+        else:
+            print("Downloading:", youtube.title)
+            if video_stream:
+                video_stream.download(video_output_path)
+                print("Download complete")
+
+    # def download_video2(self, url: str, video_output_path: str) -> None:
+    #     '''
+    #     If error network, try again with VPN connected
+    #     '''
+    #     # video_list = ['https://www.youtube.com/watch?v=xTN2ktqKSBk',
+    #     #               'https://www.youtube.com/watch?v=w5Ji-VEnbmc']
+    #     # Looping through the list
+    #     try:
+    #         yt = YouTube(url)
+    #         print('Downloading Link: ')
+
+    #         # filters out all the files with "mp4" extension
+    #         stream = yt.streams.filter(res="360p").first()
+    #         if stream:
+    #             # print('Downloading video: ' + yt.streams[0].title)
+    #             stream.download(video_output_path)
+    #         print('Task Completed!')
+    #     except:
+    #         print("Connection Error")
+
+    def download_videos(self, urls: list[str], video_output_path: str) -> None:
+        '''
+        If error network, try again with VPN connected
+        '''
+        for url in urls:
+            self.download_video(url, video_output_path)
+
+    def get_playlist_videos(self, playlist_url: str) -> list[str]:
+        playlist = Playlist(playlist_url)
+        return list(playlist.video_urls)
+
+    def download_playlist_video(self, playlist_url: str, video_output_path: str, limit: int = 0, start_index: int = 0) -> None:
+        '''
+        If error network, try again with VPN connected
+        '''
+        # playlist = Playlist(playlist_url)
+        # urls = list(playlist.video_urls)
+        urls = self.get_playlist_videos(playlist_url)
+        download_urls: list[str] = list_range(urls, limit, start_index)
+        self.download_videos(download_urls, video_output_path)
+
+    def video_title_to_json(self, directory_path: str, json_path: str, playlist: str, start_day_schedule: str = "", time_schedules: list[str] = ["11:00", "19:00"]) -> None:
+        filenames = get_files_info(directory_path, 'mp4')
+
+        def handle(file: ZuiFile, index: int) -> dict[str, Any]:
+            index_schedule = index % len(time_schedules)
+            diff_day = int(index/len(time_schedules))
+
+            file_name = file['file_name']
+            name = file['name']
+            title = pipe(
+                remove_special_characters,
+                trim_space
+            )(name)
+
+            raw_tags = pipe_list(remove_special_characters, trim_space)(
+                list_match('(#)([^ ]+)', 2)(name.strip('#')))
+            tags = filter_to(raw_tags, lambda tag, _: len(tag) > 1)
+
+            start_day = datetime.strptime(
+                start_day_schedule, "%m/%d/%Y") if start_day_schedule else datetime.now()
+            day_schedule = add_days(start_day, diff_day)
+            time_schedule = time_schedules[index_schedule].split(
+                ':')
+            day_schedule = day_schedule.replace(
+                hour=int(time_schedule[0]), minute=int(time_schedule[1]))
+            schedule = datetime.strftime(day_schedule, "%m/%d/%Y, %H:%M")
+
+            result: dict[str, Any] = {
+                'file_name': file_name,
+                "title": title,
+                "description": title,
+                "playlist": playlist,
+                "tags": tags,
+                "is_publish": False,
+                "schedule": schedule
+            }
+            return result
+        file_info = map_to(filenames, handle)
+        write_json(file_info, json_path)
+
+    # def get_video_info(self, url: str):
+    #     youtube = YouTube(url)
+    #     video_stream = youtube.streams.get_highest_resolution()
+    #     print("Downloading video:", youtube.title,
+    #           youtube.description, youtube.thumbnail_url)
+    #     print(youtube.captions['en'])
+    #     print(youtube.channel_url)
+    #     print(youtube.channel_id)
+    #     print(youtube.keywords)
+    #     print(youtube.rating)
+        # print(youtube.vid_info)
```

### Comparing `material_zui-0.1.1/src/material_zui/bard/google_bard.py` & `material_zui-0.1.2/src/material_zui/bard/google_bard.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
-from bardapi import Bard  # type: ignore
+from bardapi import Bard
 
 
 def set_key(key: str):
     '''
     - set your `__Secure-1PSID` value to key
     - detail info: https://github.com/dsdanielpark/Bard-API
     - amazing prompt: https://github.com/dsdanielpark/amazing-bard-prompts
     '''
     os.environ['_BARD_API_KEY'] = key
 
 
 def get_response(
-    prompt: str) -> dict[{'content': str, 'choices': list[dict[{'id': str, 'content': list[str]}]]}]: return Bard().get_answer(prompt)
+    prompt: str) -> dict[{'content': str, 'choices': list[dict[{'id': str, 'content': list[str]}]]}]: return Bard().get_answer(prompt)  # type: ignore
 
 
 def get_content(prompt: str) -> str: return get_response(prompt)['content']
```

### Comparing `material_zui-0.1.1/src/material_zui/compress/text.py` & `material_zui-0.1.2/src/material_zui/compress/text.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/crontab/index.py` & `material_zui-0.1.2/src/material_zui/crontab/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/date_time/time.py` & `material_zui-0.1.2/src/material_zui/date_time/time.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/gpt/gpt_vietnam.py` & `material_zui-0.1.2/src/material_zui/gpt/gpt_vietnam.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,10 +24,10 @@
 
 def gpt_last_result(prompt: str) -> dict[{'text': str}] | None:
     data = gpt_call(prompt)
     last_value = value(data, '.+"finish_reason":"stop".+')
     return json.loads(last_value) if last_value else None
 
 
-def gpt_last_text_result(prompt: str) -> str:
+def get_content(prompt: str) -> str:
     data = gpt_last_result(prompt)
     return data['text'] if data else ''
```

### Comparing `material_zui-0.1.1/src/material_zui/image/colorization.py` & `material_zui-0.1.2/src/material_zui/image/colorization.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/image/combine.py` & `material_zui-0.1.2/src/material_zui/image/combine.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/image/convert.py` & `material_zui-0.1.2/src/material_zui/image/convert.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/image/model/colorization_deploy_v2.prototxt` & `material_zui-0.1.2/src/material_zui/image/model/colorization_deploy_v2.prototxt`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/image/model/pts_in_hull.npy` & `material_zui-0.1.2/src/material_zui/image/model/pts_in_hull.npy`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/image/remove_background.py` & `material_zui-0.1.2/src/material_zui/image/remove_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/image/to_svg.py` & `material_zui-0.1.2/src/material_zui/image/to_svg.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/image/transparent_background.py` & `material_zui-0.1.2/src/material_zui/image/transparent_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/image/upscale.py` & `material_zui-0.1.2/src/material_zui/image/upscale.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/log/log.py` & `material_zui-0.1.2/src/material_zui/log/log.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/readme.md` & `material_zui-0.1.2/src/material_zui/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Modules
 
 <ol>
-  <li>array</li>
-  <li>automation</li>
+  <!-- <li>automation</li> -->
   <li>bard</li>
+  <li>bing_ai</li>
   <li>compress</li>
   <li>crawl</li>
   <li>crontab</li>
   <li>date_time</li>
   <li>env</li>
   <li>fake</li>
   <li>file</li>
@@ -19,25 +19,28 @@
       <li>colorization</li>
       <li>sketch</li>
       <li>transparent background</li>
       <li>upscale</li>
       <li>convert to jpg/png</li>
     </ul>
   </li>
+  <li>list</li>
   <!-- <li><a href="#log">Log</a></li> -->
   <li>log</li>
   <li>os</li>
   <li>regex</li>
   <li>replicate: AI Platform API</li>
   <li>selenium</li>
+  <li>string</li>
   <li>telegram_bot</li>
+  <li>utility</li>
   <li>validate</li>
 </ol>
 
-# Log
+<!-- # Log
 
 - Example:
 
 ```py
 from material_zui.log import debug, info, warning, error, critical, printTable
 
 debug('This is a debug message')
@@ -47,15 +50,15 @@
 critical('This is a critical message')
 
 printTable({
     'Name': ['Alice', 'Bob', 'Charlie', 'Dave'],
     'Age': [25, 31, 35, 19],
     'Score': [85, 94, 76, 95]
 })
-```
+``` -->
 
 <!-- - Result:
   ![](../../static/img/doc/log1.png) -->
 
 # Package
 
 - https://pypi.org/project/material-zui
```

#### html2text {}

```diff
@@ -1,32 +1,29 @@
 # Modules
-   1. array
-   2. automation
-   3. bard
-   4. compress
-   5. crawl
-   6. crontab
-   7. date_time
-   8. env
-   9. fake
-  10. file
-  11. gpt
-  12. image
+   1. bard
+   2. bing_ai
+   3. compress
+   4. crawl
+   5. crontab
+   6. date_time
+   7. env
+   8. fake
+   9. file
+  10. gpt
+  11. image
           o grayscale
           o colorization
           o sketch
           o transparent background
           o upscale
           o convert to jpg/png
+  12. list
   13. log
   14. os
   15. regex
   16. replicate: AI Platform API
   17. selenium
-  18. telegram_bot
-  19. validate
-# Log - Example: ```py from material_zui.log import debug, info, warning,
-error, critical, printTable debug('This is a debug message') info('This is an
-info message') warning('This is a warning message') error('This is an error
-message') critical('This is a critical message') printTable({ 'Name': ['Alice',
-'Bob', 'Charlie', 'Dave'], 'Age': [25, 31, 35, 19], 'Score': [85, 94, 76, 95]
-}) ```  # Package - https://pypi.org/project/material-zui
+  18. string
+  19. telegram_bot
+  20. utility
+  21. validate
+  # Package - https://pypi.org/project/material-zui
```

### Comparing `material_zui-0.1.1/src/material_zui/regex/index.py` & `material_zui-0.1.2/src/material_zui/regex/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/replicate/index.py` & `material_zui-0.1.2/src/material_zui/replicate/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/src/material_zui/setup.py` & `material_zui-0.1.2/src/material_zui/setup.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.1/PKG-INFO` & `material_zui-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 Metadata-Version: 2.1
 Name: material-zui
-Version: 0.1.1
+Version: 0.1.2
 Summary: Material Zui
 Keywords: material,zui,material zui,zui material
 Author: chauhmnguyen
 Author-email: chauhoangminhnguyen@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: bardapi (>=0.1.2,<0.2.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: bot-studio (>=1.4.0,<2.0.0)
+Requires-Dist: edgegpt (>=0.10.7,<0.11.0)
 Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: multipledispatch (>=0.6.0,<0.7.0)
+Requires-Dist: newspaper3k (>=0.2.8,<0.3.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pytelegrambotapi (>=4.11.0,<5.0.0)
 Requires-Dist: python-crontab (>=2.7.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pythonlangutil (>=0.1,<0.2)
+Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Requires-Dist: rembg (>=2.0.36,<3.0.0)
 Requires-Dist: replicate (>=0.8.1,<0.9.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: selenium (>=4.9.1,<5.0.0)
 Requires-Dist: selenium-browser (>=0.0.15,<0.0.16)
-Requires-Dist: selenium-firefox (>=2.0.7,<3.0.0)
+Requires-Dist: setuptools (>=67.8.0,<68.0.0)
+Requires-Dist: validators (>=0.20.0,<0.21.0)
 Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0)
-Requires-Dist: youtube-uploader-selenium (>=0.1.0,<0.2.0)
 Description-Content-Type: text/markdown
 
 # Modules
 
 <ol>
-  <li>array</li>
-  <li>automation</li>
+  <!-- <li>automation</li> -->
   <li>bard</li>
+  <li>bing_ai</li>
   <li>compress</li>
   <li>crawl</li>
   <li>crontab</li>
   <li>date_time</li>
   <li>env</li>
   <li>fake</li>
   <li>file</li>
@@ -53,25 +55,28 @@
       <li>colorization</li>
       <li>sketch</li>
       <li>transparent background</li>
       <li>upscale</li>
       <li>convert to jpg/png</li>
     </ul>
   </li>
+  <li>list</li>
   <!-- <li><a href="#log">Log</a></li> -->
   <li>log</li>
   <li>os</li>
   <li>regex</li>
   <li>replicate: AI Platform API</li>
   <li>selenium</li>
+  <li>string</li>
   <li>telegram_bot</li>
+  <li>utility</li>
   <li>validate</li>
 </ol>
 
-# Log
+<!-- # Log
 
 - Example:
 
 ```py
 from material_zui.log import debug, info, warning, error, critical, printTable
 
 debug('This is a debug message')
@@ -81,15 +86,15 @@
 critical('This is a critical message')
 
 printTable({
     'Name': ['Alice', 'Bob', 'Charlie', 'Dave'],
     'Age': [25, 31, 35, 19],
     'Score': [85, 94, 76, 95]
 })
-```
+``` -->
 
 <!-- - Result:
   ![](../../static/img/doc/log1.png) -->
 
 # Package
 
 - https://pypi.org/project/material-zui
```

#### html2text {}

```diff
@@ -1,49 +1,48 @@
-Metadata-Version: 2.1 Name: material-zui Version: 0.1.1 Summary: Material Zui
+Metadata-Version: 2.1 Name: material-zui Version: 0.1.2 Summary: Material Zui
 Keywords: material,zui,material zui,zui material Author: chauhmnguyen Author-
 email: chauhoangminhnguyen@gmail.com Requires-Python: >=3.10,<3.11 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Requires-Dist: bardapi (>=0.1.2,<0.2.0) Requires-Dist: beautifulsoup4
-(>=4.12.2,<5.0.0) Requires-Dist: bot-studio (>=1.4.0,<2.0.0) Requires-Dist:
+(>=4.12.2,<5.0.0) Requires-Dist: edgegpt (>=0.10.7,<0.11.0) Requires-Dist:
 flask (>=2.3.2,<3.0.0) Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-
-Dist: multipledispatch (>=0.6.0,<0.7.0) Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0) Requires-Dist: pandas
-(>=2.0.1,<3.0.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) Requires-Dist:
-pytelegrambotapi (>=4.11.0,<5.0.0) Requires-Dist: python-crontab
-(>=2.7.1,<3.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0) Requires-Dist:
-pythonlangutil (>=0.1,<0.2) Requires-Dist: rembg (>=2.0.36,<3.0.0) Requires-
-Dist: replicate (>=0.8.1,<0.9.0) Requires-Dist: requests (>=2.30.0,<3.0.0)
-Requires-Dist: selenium (>=4.9.1,<5.0.0) Requires-Dist: selenium-browser
-(>=0.0.15,<0.0.16) Requires-Dist: selenium-firefox (>=2.0.7,<3.0.0) Requires-
-Dist: webdriver-manager (>=3.8.6,<4.0.0) Requires-Dist: youtube-uploader-
-selenium (>=0.1.0,<0.2.0) Description-Content-Type: text/markdown # Modules
-   1. array
-   2. automation
-   3. bard
-   4. compress
-   5. crawl
-   6. crontab
-   7. date_time
-   8. env
-   9. fake
-  10. file
-  11. gpt
-  12. image
+Dist: multipledispatch (>=0.6.0,<0.7.0) Requires-Dist: newspaper3k
+(>=0.2.8,<0.3.0) Requires-Dist: numpy (>=1.24.3,<2.0.0) Requires-Dist: opencv-
+python (>=4.7.0.72,<5.0.0.0) Requires-Dist: pandas (>=2.0.1,<3.0.0) Requires-
+Dist: pillow (>=9.5.0,<10.0.0) Requires-Dist: pytelegrambotapi
+(>=4.11.0,<5.0.0) Requires-Dist: python-crontab (>=2.7.1,<3.0.0) Requires-Dist:
+python-dotenv (>=1.0.0,<2.0.0) Requires-Dist: pythonlangutil (>=0.1,<0.2)
+Requires-Dist: pytube (>=15.0.0,<16.0.0) Requires-Dist: rembg (>=2.0.36,<3.0.0)
+Requires-Dist: replicate (>=0.8.1,<0.9.0) Requires-Dist: requests
+(>=2.30.0,<3.0.0) Requires-Dist: selenium (>=4.9.1,<5.0.0) Requires-Dist:
+selenium-browser (>=0.0.15,<0.0.16) Requires-Dist: setuptools
+(>=67.8.0,<68.0.0) Requires-Dist: validators (>=0.20.0,<0.21.0) Requires-Dist:
+webdriver-manager (>=3.8.6,<4.0.0) Description-Content-Type: text/markdown #
+Modules
+   1. bard
+   2. bing_ai
+   3. compress
+   4. crawl
+   5. crontab
+   6. date_time
+   7. env
+   8. fake
+   9. file
+  10. gpt
+  11. image
           o grayscale
           o colorization
           o sketch
           o transparent background
           o upscale
           o convert to jpg/png
+  12. list
   13. log
   14. os
   15. regex
   16. replicate: AI Platform API
   17. selenium
-  18. telegram_bot
-  19. validate
-# Log - Example: ```py from material_zui.log import debug, info, warning,
-error, critical, printTable debug('This is a debug message') info('This is an
-info message') warning('This is a warning message') error('This is an error
-message') critical('This is a critical message') printTable({ 'Name': ['Alice',
-'Bob', 'Charlie', 'Dave'], 'Age': [25, 31, 35, 19], 'Score': [85, 94, 76, 95]
-}) ```  # Package - https://pypi.org/project/material-zui
+  18. string
+  19. telegram_bot
+  20. utility
+  21. validate
+  # Package - https://pypi.org/project/material-zui
```

