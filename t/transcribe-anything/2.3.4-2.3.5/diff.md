# Comparing `tmp/transcribe-anything-2.3.4.tar.gz` & `tmp/transcribe-anything-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transcribe-anything-2.3.4.tar", last modified: Mon May  8 10:09:37 2023, max compression
+gzip compressed data, was "transcribe-anything-2.3.5.tar", last modified: Fri Jun 23 18:19:39 2023, max compression
```

## Comparing `transcribe-anything-2.3.4.tar` & `transcribe-anything-2.3.5.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 10:09:37.277005 transcribe-anything-2.3.4/
--rw-rw-rw-   0        0        0     1064 2022-12-01 20:48:45.000000 transcribe-anything-2.3.4/LICENSE
--rw-rw-rw-   0        0        0       57 2022-12-01 20:48:45.000000 transcribe-anything-2.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     9256 2023-05-08 10:09:37.277005 transcribe-anything-2.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     8231 2023-05-08 07:32:22.000000 transcribe-anything-2.3.4/README.md
--rw-rw-rw-   0        0        0       24 2022-12-01 20:48:45.000000 transcribe-anything-2.3.4/requirements.testing.txt
--rw-rw-rw-   0        0        0       71 2023-05-05 22:22:57.000000 transcribe-anything-2.3.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 10:09:37.278002 transcribe-anything-2.3.4/setup.cfg
--rw-rw-rw-   0        0        0     3109 2023-05-08 07:31:13.000000 transcribe-anything-2.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:09:37.243003 transcribe-anything-2.3.4/tests/
--rw-rw-rw-   0        0        0      808 2023-05-08 09:56:56.000000 transcribe-anything-2.3.4/tests/test_local_file_cmd.py
--rw-rw-rw-   0        0        0     2813 2023-05-08 09:15:57.000000 transcribe-anything-2.3.4/tests/test_transcribe_anything.py
--rw-rw-rw-   0        0        0     2110 2023-05-08 09:47:26.000000 transcribe-anything-2.3.4/tests/test_transcribe_anything_api.py
--rw-rw-rw-   0        0        0      449 2023-05-08 09:15:57.000000 transcribe-anything-2.3.4/tests/test_whisper.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:09:37.250008 transcribe-anything-2.3.4/transcribe_anything/
--rw-rw-rw-   0        0        0        0 2022-12-08 07:42:26.000000 transcribe-anything-2.3.4/transcribe_anything/__init__.py
--rw-rw-rw-   0        0        0     6003 2023-05-08 09:49:04.000000 transcribe-anything-2.3.4/transcribe_anything/api.py
--rw-rw-rw-   0        0        0     3740 2023-05-08 09:06:47.000000 transcribe-anything-2.3.4/transcribe_anything/audio.py
--rw-rw-rw-   0        0        0     2598 2023-05-08 07:34:00.000000 transcribe-anything-2.3.4/transcribe_anything/cmd.py
--rw-rw-rw-   0        0        0      613 2022-12-03 03:51:42.000000 transcribe-anything-2.3.4/transcribe_anything/logger.py
--rw-rw-rw-   0        0        0     1210 2022-12-03 03:51:42.000000 transcribe-anything-2.3.4/transcribe_anything/parse_whisper_options.py
--rw-rw-rw-   0        0        0     1536 2023-05-05 23:48:52.000000 transcribe-anything-2.3.4/transcribe_anything/util.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:09:37.276004 transcribe-anything-2.3.4/transcribe_anything.egg-info/
--rw-rw-rw-   0        0        0     9256 2023-05-08 10:09:37.000000 transcribe-anything-2.3.4/transcribe_anything.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      681 2023-05-08 10:09:37.000000 transcribe-anything-2.3.4/transcribe_anything.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 10:09:37.000000 transcribe-anything-2.3.4/transcribe_anything.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2023-05-08 10:09:37.000000 transcribe-anything-2.3.4/transcribe_anything.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       71 2023-05-08 10:09:37.000000 transcribe-anything-2.3.4/transcribe_anything.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-08 10:09:37.000000 transcribe-anything-2.3.4/transcribe_anything.egg-info/top_level.txt
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-23 18:19:39.381072 transcribe-anything-2.3.5/
+-rw-r--r--   0 niteris    (501) staff       (20)     1064 2022-12-15 00:53:40.000000 transcribe-anything-2.3.5/LICENSE
+-rw-r--r--   0 niteris    (501) staff       (20)       57 2022-12-15 00:53:40.000000 transcribe-anything-2.3.5/MANIFEST.in
+-rw-r--r--   0 niteris    (501) staff       (20)     9183 2023-06-23 18:19:39.379815 transcribe-anything-2.3.5/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)     8350 2023-06-23 18:19:08.000000 transcribe-anything-2.3.5/README.md
+-rw-r--r--   0 niteris    (501) staff       (20)       24 2022-12-15 00:53:40.000000 transcribe-anything-2.3.5/requirements.testing.txt
+-rw-r--r--   0 niteris    (501) staff       (20)      100 2023-06-23 18:13:58.000000 transcribe-anything-2.3.5/requirements.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       38 2023-06-23 18:19:39.381167 transcribe-anything-2.3.5/setup.cfg
+-rw-r--r--   0 niteris    (501) staff       (20)     3109 2023-06-23 18:18:29.000000 transcribe-anything-2.3.5/setup.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-23 18:19:39.375794 transcribe-anything-2.3.5/tests/
+-rw-r--r--   0 niteris    (501) staff       (20)     1338 2023-06-22 21:56:45.000000 transcribe-anything-2.3.5/tests/test_embed_transcript.py
+-rw-r--r--   0 niteris    (501) staff       (20)      808 2023-06-22 20:03:20.000000 transcribe-anything-2.3.5/tests/test_local_file_cmd.py
+-rw-r--r--   0 niteris    (501) staff       (20)     2813 2023-06-22 20:03:20.000000 transcribe-anything-2.3.5/tests/test_transcribe_anything.py
+-rw-r--r--   0 niteris    (501) staff       (20)     2110 2023-06-22 20:03:20.000000 transcribe-anything-2.3.5/tests/test_transcribe_anything_api.py
+-rw-r--r--   0 niteris    (501) staff       (20)      449 2023-06-22 20:03:20.000000 transcribe-anything-2.3.5/tests/test_whisper.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-23 18:19:39.378106 transcribe-anything-2.3.5/transcribe_anything/
+-rw-r--r--   0 niteris    (501) staff       (20)        0 2022-12-15 00:53:40.000000 transcribe-anything-2.3.5/transcribe_anything/__init__.py
+-rw-r--r--   0 niteris    (501) staff       (20)     7702 2023-06-23 18:10:55.000000 transcribe-anything-2.3.5/transcribe_anything/api.py
+-rw-r--r--   0 niteris    (501) staff       (20)     3047 2023-06-22 22:57:04.000000 transcribe-anything-2.3.5/transcribe_anything/audio.py
+-rw-r--r--   0 niteris    (501) staff       (20)     2782 2023-06-22 21:54:49.000000 transcribe-anything-2.3.5/transcribe_anything/cmd.py
+-rw-r--r--   0 niteris    (501) staff       (20)      613 2022-12-15 00:53:40.000000 transcribe-anything-2.3.5/transcribe_anything/logger.py
+-rw-r--r--   0 niteris    (501) staff       (20)     1210 2022-12-15 00:53:40.000000 transcribe-anything-2.3.5/transcribe_anything/parse_whisper_options.py
+-rw-r--r--   0 niteris    (501) staff       (20)     1568 2023-06-22 22:57:04.000000 transcribe-anything-2.3.5/transcribe_anything/util.py
+-rw-r--r--   0 niteris    (501) staff       (20)      935 2023-06-22 22:57:04.000000 transcribe-anything-2.3.5/transcribe_anything/ytldp_download.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-23 18:19:39.379574 transcribe-anything-2.3.5/transcribe_anything.egg-info/
+-rw-r--r--   0 niteris    (501) staff       (20)     9183 2023-06-23 18:19:39.000000 transcribe-anything-2.3.5/transcribe_anything.egg-info/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)      750 2023-06-23 18:19:39.000000 transcribe-anything-2.3.5/transcribe_anything.egg-info/SOURCES.txt
+-rw-r--r--   0 niteris    (501) staff       (20)        1 2023-06-23 18:19:39.000000 transcribe-anything-2.3.5/transcribe_anything.egg-info/dependency_links.txt
+-rw-r--r--   0 niteris    (501) staff       (20)      120 2023-06-23 18:19:39.000000 transcribe-anything-2.3.5/transcribe_anything.egg-info/entry_points.txt
+-rw-r--r--   0 niteris    (501) staff       (20)      101 2023-06-23 18:19:39.000000 transcribe-anything-2.3.5/transcribe_anything.egg-info/requires.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       20 2023-06-23 18:19:39.000000 transcribe-anything-2.3.5/transcribe_anything.egg-info/top_level.txt
```

### Comparing `transcribe-anything-2.3.4/LICENSE` & `transcribe-anything-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.4/PKG-INFO` & `transcribe-anything-2.3.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,192 +1,173 @@
-Metadata-Version: 2.1
-Name: transcribe-anything
-Version: 2.3.4
-Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
-Home-page: https://github.com/zackees/transcribe-anything
-Author: Zach Vorhies
-Author-email: dont@email.me
-License: MIT
-Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Environment :: Console
-Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# transcribe-anything
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_macos.yml)
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Win_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_win.yml)
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_ubuntu.yml)
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Lint/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/lint.yml)
-
-### USES WHISPER AI
-
-Input a local file or url and this tool will transcribe it using Whisper AI into subtitle files and raw text.
-
-Uses whisper AI so this is state of the art translation service - completely free. 🤯🤯🤯
-
-Your data stays private and is not uploaded to any service.
-
-# Usage (CPU Version)
-
-```bash
-> pip install transcribe-anything
-# Outputs the srt, vtt and txt files in title/out.vtt
-> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
-```
-
-# Usage (GPU Accelerated Version) (works on Python 3.10.X)
-
-```bash
-> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
-# Outputs the srt, vtt and txt files in title/out.vtt
-> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
-```
-
-Will output:
-
-```
-Detecting language using up to the first 30 seconds. Use `--language` to specify the language
-Detected language: English
-[00:00.000 --> 00:27.000]  We're no strangers to love, you know the rules, and so do I
-[00:27.000 --> 00:31.000]  I've built commitments while I'm thinking of
-[00:31.000 --> 00:35.000]  You wouldn't get this from any other guy
-[00:35.000 --> 00:40.000]  I just wanna tell you how I'm feeling
-[00:40.000 --> 00:43.000]  Gotta make you understand
-[00:43.000 --> 00:45.000]  Never gonna give you up
-[00:45.000 --> 00:47.000]  Never gonna let you down
-[00:47.000 --> 00:51.000]  Never gonna run around and desert you
-[00:51.000 --> 00:53.000]  Never gonna make you cry
-[00:53.000 --> 00:55.000]  Never gonna say goodbye
-[00:55.000 --> 00:58.000]  Never gonna tell a lie
-[00:58.000 --> 01:00.000]  And hurt you
-[01:00.000 --> 01:04.000]  We've known each other for so long
-[01:04.000 --> 01:09.000]  Your heart's been aching but you're too shy to say it
-[01:09.000 --> 01:13.000]  Inside we both know what's been going on
-[01:13.000 --> 01:17.000]  We know the game and we're gonna play it
-[01:17.000 --> 01:22.000]  And if you ask me how I'm feeling
-[01:22.000 --> 01:25.000]  Don't tell me you're too much to see
-[01:25.000 --> 01:27.000]  Never gonna give you up
-[01:27.000 --> 01:29.000]  Never gonna let you down
-[01:29.000 --> 01:33.000]  Never gonna run around and desert you
-[01:33.000 --> 01:35.000]  Never gonna make you cry
-[01:35.000 --> 01:38.000]  Never gonna say goodbye
-[01:38.000 --> 01:40.000]  Never gonna tell a lie
-[01:40.000 --> 01:42.000]  And hurt you
-[01:42.000 --> 01:44.000]  Never gonna give you up
-[01:44.000 --> 01:46.000]  Never gonna let you down
-[01:46.000 --> 01:50.000]  Never gonna run around and desert you
-[01:50.000 --> 01:52.000]  Never gonna make you cry
-[01:52.000 --> 01:54.000]  Never gonna say goodbye
-[01:54.000 --> 01:57.000]  Never gonna tell a lie
-[01:57.000 --> 01:59.000]  And hurt you
-[02:08.000 --> 02:10.000]  Never gonna give
-[02:12.000 --> 02:14.000]  Never gonna give
-[02:16.000 --> 02:19.000]  We've known each other for so long
-[02:19.000 --> 02:24.000]  Your heart's been aching but you're too shy to say it
-[02:24.000 --> 02:28.000]  Inside we both know what's been going on
-[02:28.000 --> 02:32.000]  We know the game and we're gonna play it
-[02:32.000 --> 02:37.000]  I just wanna tell you how I'm feeling
-[02:37.000 --> 02:40.000]  Gotta make you understand
-[02:40.000 --> 02:42.000]  Never gonna give you up
-[02:42.000 --> 02:44.000]  Never gonna let you down
-[02:44.000 --> 02:48.000]  Never gonna run around and desert you
-[02:48.000 --> 02:50.000]  Never gonna make you cry
-[02:50.000 --> 02:53.000]  Never gonna say goodbye
-[02:53.000 --> 02:55.000]  Never gonna tell a lie
-[02:55.000 --> 02:57.000]  And hurt you
-[02:57.000 --> 02:59.000]  Never gonna give you up
-[02:59.000 --> 03:01.000]  Never gonna let you down
-[03:01.000 --> 03:05.000]  Never gonna run around and desert you
-[03:05.000 --> 03:08.000]  Never gonna make you cry
-[03:08.000 --> 03:10.000]  Never gonna say goodbye
-[03:10.000 --> 03:12.000]  Never gonna tell a lie
-[03:12.000 --> 03:14.000]  And hurt you
-[03:14.000 --> 03:16.000]  Never gonna give you up
-[03:16.000 --> 03:23.000]  If you want, never gonna let you down Never gonna run around and desert you
-[03:23.000 --> 03:28.000]  Never gonna make you hide Never gonna say goodbye
-[03:28.000 --> 03:42.000]  Never gonna tell you I ain't ready
-```
-
-## Api
-
-```python
-from transcribe_anyting.api import transcribe
-
-transcribe(
-    url_or_file="https://www.youtube.com/watch?v=dQw4w9WgXcQ",
-    output_dir="output_dir",
-)
-```
-
-## Install GPU/CUDA Accelerated version
-
-GPU acceleration is *much* faster than the CPU version. Install it using the following:
-
-```bash
-> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
-# transcribe-anything should now be installed
-> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
-```
-
-## Develop
-
-Works for Ubuntu/MacOS/Win32(in git-bash)
-This will create a virtual environment
-
-```bash
-> cd transcribe_anything
-> ./install_dev.sh
-# Enter the environment:
-> source activate.sh
-```
-
-The environment is now active and the next step will only install to the local python. If the terminal
-is closed then to get back into the environment `cd transcribe_anything` and execute `source activate.sh`
-
-## Required: Install to current python environment
-  * `pip install transcribe-anything`
-    * The command `transcribe_anything` will magically become available.
-  * `transcribe_anything <YOUTUBE_URL>`
-
-
-# Tech Stack
-  * OpenAI whisper
-  * yt-dlp: https://github.com/yt-dlp/yt-dlp
-  * static-ffmpeg
-    * github: https://github.com/zackees/static_ffmpeg
-    * pypi: https://pypi.org/project/static-ffmpeg/
-
-# Testing
-  * All tests are run by `tox`, simply go to the project directory root and run it.
-
-# Versions
-  * 2.3.4: Removed `out.mp3` and instead use a temporary wav file, as that is faster to process. --no-keep-audio has now been removed.
-  * 2.3.3: Fix case where there spaces in name (happens on windows)
-  * 2.3.2: Fix windows transcoding error
-  * 2.3.1: static-ffmpeg >= 2.5 now specified
-  * 2.3.0: Now uses the official version of whisper ai
-  * 2.2.1: "test_" is now prepended to all the different output folder names.
-  * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
-  * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
-  * 2.1.1: Updates keywords for easier pypi finding.
-  * 2.1.0: Unknown args are now assumed to be for whisper and passed to it as-is. Fixes https://github.com/zackees/transcribe-anything/issues/3
-  * 2.0.13: Now works with python 3.9
-  * 2.0.12: Adds --device to argument parameters. This will default to CUDA if available, else CPU.
-  * 2.0.11: Automatically deletes files in the out directory if they already exist.
-  * 2.0.10: fixes local file issue https://github.com/zackees/transcribe-anything/issues/2
-  * 2.0.9: fixes sanitization of path names for some youtube videos
-  * 2.0.8: fix `--output_dir` not being respected.
-  * 2.0.7: `install_cuda.sh` -> `install_cuda.py`
-  * 2.0.6: Fixes twitter video fetching. --keep-audio -> --no-keep-audio
-  * 2.0.5: Fix bad filename on trailing urls ending with /, adds --keep-audio
-  * 2.0.3: GPU support is now added. Run the `install_cuda.sh` script to enable.
-  * 2.0.2: Minor cleanup of file names (no more out.mp3.txt, it's now out.txt)
-  * 2.0.1: Fixes missing dependencies and adds whisper option.
-  * 2.0.0: New! Now a front end for Whisper ai!
+
+# transcribe-anything
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_macos.yml)
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Win_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_win.yml)
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_ubuntu.yml)
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Lint/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/lint.yml)
+
+### USES WHISPER AI
+
+Input a local file or url and this tool will transcribe it using Whisper AI into subtitle files and raw text.
+
+Uses whisper AI so this is state of the art translation service - completely free. 🤯🤯🤯
+
+Your data stays private and is not uploaded to any service.
+
+# Usage (CPU Version)
+
+```bash
+> pip install transcribe-anything
+# Outputs the srt, vtt and txt files in title/out.vtt
+> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
+```
+
+# Usage (GPU Accelerated Version) (works on Python 3.10.X)
+
+```bash
+> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
+# Outputs the srt, vtt and txt files in title/out.vtt
+> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
+```
+
+Will output:
+
+```
+Detecting language using up to the first 30 seconds. Use `--language` to specify the language
+Detected language: English
+[00:00.000 --> 00:27.000]  We're no strangers to love, you know the rules, and so do I
+[00:27.000 --> 00:31.000]  I've built commitments while I'm thinking of
+[00:31.000 --> 00:35.000]  You wouldn't get this from any other guy
+[00:35.000 --> 00:40.000]  I just wanna tell you how I'm feeling
+[00:40.000 --> 00:43.000]  Gotta make you understand
+[00:43.000 --> 00:45.000]  Never gonna give you up
+[00:45.000 --> 00:47.000]  Never gonna let you down
+[00:47.000 --> 00:51.000]  Never gonna run around and desert you
+[00:51.000 --> 00:53.000]  Never gonna make you cry
+[00:53.000 --> 00:55.000]  Never gonna say goodbye
+[00:55.000 --> 00:58.000]  Never gonna tell a lie
+[00:58.000 --> 01:00.000]  And hurt you
+[01:00.000 --> 01:04.000]  We've known each other for so long
+[01:04.000 --> 01:09.000]  Your heart's been aching but you're too shy to say it
+[01:09.000 --> 01:13.000]  Inside we both know what's been going on
+[01:13.000 --> 01:17.000]  We know the game and we're gonna play it
+[01:17.000 --> 01:22.000]  And if you ask me how I'm feeling
+[01:22.000 --> 01:25.000]  Don't tell me you're too much to see
+[01:25.000 --> 01:27.000]  Never gonna give you up
+[01:27.000 --> 01:29.000]  Never gonna let you down
+[01:29.000 --> 01:33.000]  Never gonna run around and desert you
+[01:33.000 --> 01:35.000]  Never gonna make you cry
+[01:35.000 --> 01:38.000]  Never gonna say goodbye
+[01:38.000 --> 01:40.000]  Never gonna tell a lie
+[01:40.000 --> 01:42.000]  And hurt you
+[01:42.000 --> 01:44.000]  Never gonna give you up
+[01:44.000 --> 01:46.000]  Never gonna let you down
+[01:46.000 --> 01:50.000]  Never gonna run around and desert you
+[01:50.000 --> 01:52.000]  Never gonna make you cry
+[01:52.000 --> 01:54.000]  Never gonna say goodbye
+[01:54.000 --> 01:57.000]  Never gonna tell a lie
+[01:57.000 --> 01:59.000]  And hurt you
+[02:08.000 --> 02:10.000]  Never gonna give
+[02:12.000 --> 02:14.000]  Never gonna give
+[02:16.000 --> 02:19.000]  We've known each other for so long
+[02:19.000 --> 02:24.000]  Your heart's been aching but you're too shy to say it
+[02:24.000 --> 02:28.000]  Inside we both know what's been going on
+[02:28.000 --> 02:32.000]  We know the game and we're gonna play it
+[02:32.000 --> 02:37.000]  I just wanna tell you how I'm feeling
+[02:37.000 --> 02:40.000]  Gotta make you understand
+[02:40.000 --> 02:42.000]  Never gonna give you up
+[02:42.000 --> 02:44.000]  Never gonna let you down
+[02:44.000 --> 02:48.000]  Never gonna run around and desert you
+[02:48.000 --> 02:50.000]  Never gonna make you cry
+[02:50.000 --> 02:53.000]  Never gonna say goodbye
+[02:53.000 --> 02:55.000]  Never gonna tell a lie
+[02:55.000 --> 02:57.000]  And hurt you
+[02:57.000 --> 02:59.000]  Never gonna give you up
+[02:59.000 --> 03:01.000]  Never gonna let you down
+[03:01.000 --> 03:05.000]  Never gonna run around and desert you
+[03:05.000 --> 03:08.000]  Never gonna make you cry
+[03:08.000 --> 03:10.000]  Never gonna say goodbye
+[03:10.000 --> 03:12.000]  Never gonna tell a lie
+[03:12.000 --> 03:14.000]  And hurt you
+[03:14.000 --> 03:16.000]  Never gonna give you up
+[03:16.000 --> 03:23.000]  If you want, never gonna let you down Never gonna run around and desert you
+[03:23.000 --> 03:28.000]  Never gonna make you hide Never gonna say goodbye
+[03:28.000 --> 03:42.000]  Never gonna tell you I ain't ready
+```
+
+## Api
+
+```python
+from transcribe_anyting.api import transcribe
+
+transcribe(
+    url_or_file="https://www.youtube.com/watch?v=dQw4w9WgXcQ",
+    output_dir="output_dir",
+)
+```
+
+## Install GPU/CUDA Accelerated version
+
+GPU acceleration is *much* faster than the CPU version. Install it using the following:
+
+```bash
+> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
+# transcribe-anything should now be installed
+> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
+```
+
+## Develop
+
+Works for Ubuntu/MacOS/Win32(in git-bash)
+This will create a virtual environment
+
+```bash
+> cd transcribe_anything
+> ./install_dev.sh
+# Enter the environment:
+> source activate.sh
+```
+
+The environment is now active and the next step will only install to the local python. If the terminal
+is closed then to get back into the environment `cd transcribe_anything` and execute `source activate.sh`
+
+## Required: Install to current python environment
+  * `pip install transcribe-anything`
+    * The command `transcribe_anything` will magically become available.
+  * `transcribe_anything <YOUTUBE_URL>`
+
+
+# Tech Stack
+  * OpenAI whisper
+  * yt-dlp: https://github.com/yt-dlp/yt-dlp
+  * static-ffmpeg
+    * github: https://github.com/zackees/static_ffmpeg
+    * pypi: https://pypi.org/project/static-ffmpeg/
+
+# Testing
+  * All tests are run by `tox`, simply go to the project directory root and run it.
+
+# Versions
+  * 2.3.5: Now has `--embed` to burn the subtitles into the video itself. Only works on local mp4 files at the moment.
+  * 2.3.4: Removed `out.mp3` and instead use a temporary wav file, as that is faster to process. --no-keep-audio has now been removed.
+  * 2.3.3: Fix case where there spaces in name (happens on windows)
+  * 2.3.2: Fix windows transcoding error
+  * 2.3.1: static-ffmpeg >= 2.5 now specified
+  * 2.3.0: Now uses the official version of whisper ai
+  * 2.2.1: "test_" is now prepended to all the different output folder names.
+  * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
+  * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
+  * 2.1.1: Updates keywords for easier pypi finding.
+  * 2.1.0: Unknown args are now assumed to be for whisper and passed to it as-is. Fixes https://github.com/zackees/transcribe-anything/issues/3
+  * 2.0.13: Now works with python 3.9
+  * 2.0.12: Adds --device to argument parameters. This will default to CUDA if available, else CPU.
+  * 2.0.11: Automatically deletes files in the out directory if they already exist.
+  * 2.0.10: fixes local file issue https://github.com/zackees/transcribe-anything/issues/2
+  * 2.0.9: fixes sanitization of path names for some youtube videos
+  * 2.0.8: fix `--output_dir` not being respected.
+  * 2.0.7: `install_cuda.sh` -> `install_cuda.py`
+  * 2.0.6: Fixes twitter video fetching. --keep-audio -> --no-keep-audio
+  * 2.0.5: Fix bad filename on trailing urls ending with /, adds --keep-audio
+  * 2.0.3: GPU support is now added. Run the `install_cuda.sh` script to enable.
+  * 2.0.2: Minor cleanup of file names (no more out.mp3.txt, it's now out.txt)
+  * 2.0.1: Fixes missing dependencies and adds whisper option.
+  * 2.0.0: New! Now a front end for Whisper ai!
```

### Comparing `transcribe-anything-2.3.4/README.md` & `transcribe-anything-2.3.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: transcribe-anything
+Version: 2.3.5
+Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
+Home-page: https://github.com/zackees/transcribe-anything
+Author: Zach Vorhies
+Author-email: dont@email.me
+License: MIT
+Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Environment :: Console
+Requires-Python: >=3.9.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 # transcribe-anything
 [![Actions Status](https://github.com/zackees/transcribe-anything/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_macos.yml)
 [![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Win_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_win.yml)
 [![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_ubuntu.yml)
 [![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Lint/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/lint.yml)
 
@@ -143,14 +163,15 @@
     * github: https://github.com/zackees/static_ffmpeg
     * pypi: https://pypi.org/project/static-ffmpeg/
 
 # Testing
   * All tests are run by `tox`, simply go to the project directory root and run it.
 
 # Versions
+  * 2.3.5: Now has `--embed` to burn the subtitles into the video itself. Only works on local mp4 files at the moment.
   * 2.3.4: Removed `out.mp3` and instead use a temporary wav file, as that is faster to process. --no-keep-audio has now been removed.
   * 2.3.3: Fix case where there spaces in name (happens on windows)
   * 2.3.2: Fix windows transcoding error
   * 2.3.1: static-ffmpeg >= 2.5 now specified
   * 2.3.0: Now uses the official version of whisper ai
   * 2.2.1: "test_" is now prepended to all the different output folder names.
   * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
```

### Comparing `transcribe-anything-2.3.4/setup.py` & `transcribe-anything-2.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "Uses whisper AI to transcribe speach from video and audio files. "
     "Also accepts urls for youtube, rumble, bitchute, clear file, etc."
 )
 URL = "https://github.com/zackees/transcribe-anything"
 EMAIL = "dont@email.me"
 AUTHOR = "Zach Vorhies"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "2.3.4"
+VERSION = "2.3.5"
 
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), encoding="utf-8", mode="r") as fd:
     README = fd.read()
 
 
 def parse_requirements(filename):
```

### Comparing `transcribe-anything-2.3.4/tests/test_local_file_cmd.py` & `transcribe-anything-2.3.5/tests/test_local_file_cmd.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.4/tests/test_transcribe_anything.py` & `transcribe-anything-2.3.5/tests/test_transcribe_anything.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.4/tests/test_transcribe_anything_api.py` & `transcribe-anything-2.3.5/tests/test_transcribe_anything_api.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.4/transcribe_anything/api.py` & `transcribe-anything-2.3.5/transcribe_anything/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,51 @@
 """
     Api for using transcribe_anything from python. Allows bulk processing.
 """
 
-# pylint: disable=too-many-arguments,broad-except,too-many-locals,unsupported-binary-operation,too-many-branches,too-many-statements
+# pylint: disable=too-many-arguments,broad-except,too-many-locals,unsupported-binary-operation,too-many-branches,too-many-statements,disable=notimplemented-raised,unused-variable
+
+# flake8: noqa F401,E303,F821
 
 import atexit
 import os
 import stat
 import sys
 import time
 import subprocess
 from typing import Optional
 import tempfile
 import shutil
+from hashlib import md5  # pylint: disable=unused-import
+
+from appdirs import user_config_dir  # type: ignore
+from disklru import DiskLRUCache  # type: ignore  # pylint: disable=unused-import
 
 from static_ffmpeg import add_paths as ffmpeg_add_paths  # type: ignore
 
 from transcribe_anything.audio import fetch_audio
 from transcribe_anything.util import (
     get_computing_device,
     sanitize_filename,
     chop_double_extension,
 )
 from transcribe_anything.logger import log_error
 
-PERMS = stat.S_IRUSR | stat.S_IRGRP | stat.S_IROTH | stat.S_IWOTH | stat.S_IWUSR | stat.S_IWGRP
+
+
+CACHE_FILE = os.path.join(user_config_dir("transcript-anything", "cache", roaming=True))
+
+PERMS = (
+    stat.S_IRUSR
+    | stat.S_IRGRP
+    | stat.S_IROTH
+    | stat.S_IWOTH
+    | stat.S_IWUSR
+    | stat.S_IWGRP
+)
 
 ffmpeg_add_paths()
 
 
 def make_temp_wav() -> str:
     """
     Makes a temporary mp3 file and returns the path to it.
@@ -50,19 +67,26 @@
 def transcribe(
     url_or_file: str,
     output_dir: Optional[str] = None,
     model: Optional[str] = None,
     task: Optional[str] = None,
     language: Optional[str] = None,
     device: Optional[str] = None,
+    embed: bool = False,
     other_args: Optional[list[str]] = None,
 ) -> str:
     """
     Runs the program.
     """
+    if not os.path.isfile(url_or_file) and embed:
+        raise NotImplementedError(
+            "Embedding is only supported for local files. "
+            "Please download the file first."
+        )
+    # cache = DiskLRUCache(CACHE_FILE, 16)
     basename = os.path.basename(url_or_file)
     if not basename or basename == ".":  # if url_or_file is a directory
         # Defense against paths with a trailing /, for example:
         # https://example.com/, which will yield a basename of "".
         basename = os.path.basename(os.path.dirname(url_or_file))
         basename = sanitize_filename(basename)
     output_dir_was_generated = False
@@ -86,18 +110,24 @@
         else:
             output_dir = "text_" + os.path.splitext(basename)[0]
     if output_dir_was_generated and language is not None:
         output_dir = os.path.join(output_dir, language)
     print(f"making dir {output_dir}")
     os.makedirs(output_dir, exist_ok=True)
     tmp_wav = make_temp_wav()
-    assert os.path.isdir(output_dir), f"Path {output_dir} is not found or not a directory."
+    assert os.path.isdir(
+        output_dir
+    ), f"Path {output_dir} is not found or not a directory."
     # tmp_mp3 = os.path.join(output_dir, "out.mp3")
     fetch_audio(url_or_file, tmp_wav)
     assert os.path.exists(tmp_wav), f"Path {tmp_wav} doesn't exist."
+    #filemd5 = md5(file.encode("utf-8")).hexdigest()
+    #key = f"{file}-{filemd5}-{model}"
+    #cached_data = cache.get_json(key)
+    # print(f"Todo: cached data: {cached_data}")å
     device = device or get_computing_device()
     if device == "cuda":
         print("#####################################")
         print("######### GPU ACCELERATED! ##########")
         print("#####################################")
     elif device == "cpu":
         print("WARNING: NOT using GPU acceleration, using 10x slower CPU instead.")
@@ -108,14 +138,15 @@
     task_str = f" --task {task}" if task else ""
     language_str = f" --language {language}" if language else ""
     cmd_list = []
     if sys.platform == "win32":
         # Set the text mode to UTF-8 on Windows.
         cmd_list.extend(["chcp", "65001", "&&"])
 
+    print(f"Running whisper on {tmp_wav} (will install models on first run)")
     with tempfile.TemporaryDirectory() as tmpdir:
         cmd_list.extend(
             [
                 "whisper",
                 f'"{tmp_wav}"',
                 "--device",
                 device,
@@ -140,30 +171,45 @@
                 time.sleep(0.25)
                 continue
             if rtn != 0:
                 msg = f"Failed to execute {cmd}\n "
                 raise OSError(msg)
             break
         files = [os.path.join(tmpdir, name) for name in os.listdir(tmpdir)]
+        srt_file: Optional[str] = None
         for file in files:
             # Change the filename to remove the double extension
             file_name = os.path.basename(file)
             base_path = os.path.dirname(file)
             new_file = os.path.join(base_path, chop_double_extension(file_name))
             _, ext = os.path.splitext(new_file)
             outfile = os.path.join(output_dir, f"out{ext}")
             if os.path.exists(outfile):
                 os.remove(outfile)
             assert os.path.isfile(file), f"Path {file} doesn't exist."
             assert not os.path.exists(outfile), f"Path {outfile} already exists."
             shutil.move(file, outfile)
+            if ext == ".srt":
+                srt_file = outfile
+        assert srt_file is not None, "No srt file found."
+        if embed:
+            assert os.path.isfile(url_or_file), f"Path {url_or_file} doesn't exist."
+            # embed_srt(srt_file, url_or_file)
+            #print("Embedding not implemented yet.")
+            out_mp4 = os.path.join(output_dir, "out.mp4")
+            #ffmpeg -i input.mp4 -c copy -vf "subtitles=subtitle.srt" output.mp4
+            embed_ffmpeg_cmd = f'ffmpeg -i "{url_or_file}" -i "{srt_file}" -vf "subtitles={srt_file}" "{out_mp4}"'  # pylint: disable=line-too-long
+            print(f"Running:\n  {embed_ffmpeg_cmd}")
+            os.system(embed_ffmpeg_cmd)
     return output_dir
 
 
 if __name__ == "__main__":
     # test case for twitter video
     # transcribe(url_or_file="https://twitter.com/wlctv_ca/status/1598895698870951943")
     try:
-        transcribe(url_or_file="https://www.youtube.com/watch?v=DWtpNPZ4tb4", output_dir="test")
+        transcribe(
+            url_or_file="https://www.youtube.com/watch?v=DWtpNPZ4tb4", output_dir="test"
+        )
     except KeyboardInterrupt:
         print("Keyboard interrupt")
         sys.exit(1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `transcribe-anything-2.3.4/transcribe_anything/audio.py` & `transcribe-anything-2.3.5/transcribe_anything/audio.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,55 +6,37 @@
 import sys
 import tempfile
 import subprocess
 import os
 import shutil
 import static_ffmpeg  # type: ignore
 
-_PROCESS_TIMEOUT = 4 * 60 * 60
+from transcribe_anything.util import PROCESS_TIMEOUT
+from transcribe_anything.ytldp_download import ytdlp_download
 
 
-def _ytdlp_download(url: str, outdir: str) -> str:
-    """Downloads a file using ytdlp."""
-    os.makedirs(outdir, exist_ok=True)
-    # remove all files in the directory
-    for file in os.listdir(outdir):
-        os.remove(os.path.join(outdir, file))
-    cmd = f'yt-dlp --no-check-certificate {url} -o "out.%(ext)s"'
-    print(f"Running:\n  {cmd}")
-    subprocess.run(
-        cmd,
-        shell=True,
-        cwd=outdir,
-        check=True,
-        timeout=_PROCESS_TIMEOUT,
-        universal_newlines=True,
-    )
-    new_files = os.listdir(outdir)
-    assert len(new_files) == 1, f"Expected 1 file, got {new_files}"
-    downloaded_file = os.path.join(outdir, new_files[0])
-    assert os.path.exists(downloaded_file), f"The expected file {downloaded_file} doesn't exist"
-    return downloaded_file
-
-
-def _convert_to_wav(inpath: str, outpath: str, speech_normalization: bool = False) -> None:
+def _convert_to_wav(
+    inpath: str, outpath: str, speech_normalization: bool = False
+) -> None:
     """Converts a file to wav."""
     cmd_audio_filter = ""
     if speech_normalization:
         cmd_audio_filter = "-filter:a speechnorm=e=12.5:r=0.00001:l=1"
     tmpwav = tempfile.NamedTemporaryFile(  # pylint: disable=consider-using-with
         suffix=".wav", delete=False
     )
     tmpwav.close()
     tmpwavepath = tmpwav.name
     audio_encoder = "-acodec pcm_s16le -ar 44100 -ac 1"
     cmd = f'ffmpeg -y -i "{inpath}" {cmd_audio_filter} {audio_encoder} "{tmpwavepath}"'
     print(f"Running:\n  {cmd}")
     try:
-        subprocess.run(cmd, shell=True, check=True, capture_output=True, timeout=_PROCESS_TIMEOUT)
+        subprocess.run(
+            cmd, shell=True, check=True, capture_output=True, timeout=PROCESS_TIMEOUT
+        )
     except subprocess.CalledProcessError as exc:
         print(f"Failed to run {cmd} with error {exc}")
         print(f"stdout: {exc.stdout}")
         print(f"stderr: {exc.stderr}")
         raise
     os.remove(outpath)
     os.rename(tmpwavepath, outpath)
@@ -64,15 +46,15 @@
 def fetch_audio(url_or_file: str, out_wav: str) -> None:
     """Fetches from the internet or from a local file and outputs a wav file."""
     assert out_wav.endswith(".wav")
     static_ffmpeg.add_paths()  # pylint: disable=no-member
     if url_or_file.startswith("http") or url_or_file.startswith("ftp"):
         with tempfile.TemporaryDirectory() as tmpdir:
             print(f"Using temporary directory {tmpdir}")
-            downloaded_file = _ytdlp_download(url_or_file, os.path.abspath(tmpdir))
+            downloaded_file = ytdlp_download(url_or_file, os.path.abspath(tmpdir))
             print("Downloaded file: ", downloaded_file)
             _convert_to_wav(downloaded_file, out_wav, speech_normalization=True)
         sys.stderr.write("Downloading complete.\n")
         assert os.path.exists(out_wav), f"The expected file {out_wav} doesn't exist"
     else:
         assert os.path.isfile(url_or_file)
         abspath = os.path.abspath(url_or_file)
@@ -82,15 +64,15 @@
             sys.stderr.write(f"Running:\n  {cmd}\n")
             subprocess.run(
                 cmd,
                 cwd=tmpdir,
                 shell=True,
                 check=True,
                 capture_output=True,
-                timeout=_PROCESS_TIMEOUT,
+                timeout=PROCESS_TIMEOUT,
             )
             shutil.copyfile(os.path.join(tmpdir, "out.wav"), out_wav_abs)
         assert os.path.exists(out_wav), f"The expected file {out_wav} doesn't exist"
 
 
 def unit_test() -> None:
     """Runs the program."""
```

### Comparing `transcribe-anything-2.3.4/transcribe_anything/cmd.py` & `transcribe-anything-2.3.5/transcribe_anything/cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,26 +49,32 @@
     )
     parser.add_argument(
         "--device",
         help="device to use for processing, None will auto select CUDA if available or else CPU",
         default=None,
         choices=[None, "cpu", "cuda"],
     )
+    parser.add_argument(
+        "--embed",
+        help="whether to embed the translation file into the output file",
+        action="store_true",
+    )
     # add extra options that are passed into the transcribe function
     args, unknown = parser.parse_known_args()
     print(f"Unknown args: {unknown}")
     print(f"Running transcribe_audio on {args.url_or_file}")
     try:
         transcribe(
             url_or_file=args.url_or_file,
             output_dir=args.output_dir,
             model=args.model if args.model != "None" else None,
             task=args.task,
             language=args.language if args.language != "None" else None,
             device=args.device,
+            embed=args.embed,
             other_args=unknown,
         )
     except KeyboardInterrupt:
         print("KeyboardInterrupt")
         return 1
     return 0
```

### Comparing `transcribe-anything-2.3.4/transcribe_anything/logger.py` & `transcribe-anything-2.3.5/transcribe_anything/logger.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.4/transcribe_anything/parse_whisper_options.py` & `transcribe-anything-2.3.5/transcribe_anything/parse_whisper_options.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.4/transcribe_anything/util.py` & `transcribe-anything-2.3.5/transcribe_anything/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 import re
 from html import unescape
 from urllib.parse import unquote
 import torch  # pylint: disable=import-outside-toplevel
 
 
+PROCESS_TIMEOUT = 4 * 60 * 60
+
+
 def get_computing_device() -> str:
     """Get the computing device."""
     try:
         if torch.cuda.is_available():
             return "cuda"
         return "cpu"
     except ImportError:
```

### Comparing `transcribe-anything-2.3.4/transcribe_anything.egg-info/PKG-INFO` & `transcribe-anything-2.3.5/transcribe_anything.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,192 +1,193 @@
-Metadata-Version: 2.1
-Name: transcribe-anything
-Version: 2.3.4
-Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
-Home-page: https://github.com/zackees/transcribe-anything
-Author: Zach Vorhies
-Author-email: dont@email.me
-License: MIT
-Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Environment :: Console
-Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# transcribe-anything
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_macos.yml)
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Win_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_win.yml)
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_ubuntu.yml)
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Lint/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/lint.yml)
-
-### USES WHISPER AI
-
-Input a local file or url and this tool will transcribe it using Whisper AI into subtitle files and raw text.
-
-Uses whisper AI so this is state of the art translation service - completely free. 🤯🤯🤯
-
-Your data stays private and is not uploaded to any service.
-
-# Usage (CPU Version)
-
-```bash
-> pip install transcribe-anything
-# Outputs the srt, vtt and txt files in title/out.vtt
-> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
-```
-
-# Usage (GPU Accelerated Version) (works on Python 3.10.X)
-
-```bash
-> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
-# Outputs the srt, vtt and txt files in title/out.vtt
-> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
-```
-
-Will output:
-
-```
-Detecting language using up to the first 30 seconds. Use `--language` to specify the language
-Detected language: English
-[00:00.000 --> 00:27.000]  We're no strangers to love, you know the rules, and so do I
-[00:27.000 --> 00:31.000]  I've built commitments while I'm thinking of
-[00:31.000 --> 00:35.000]  You wouldn't get this from any other guy
-[00:35.000 --> 00:40.000]  I just wanna tell you how I'm feeling
-[00:40.000 --> 00:43.000]  Gotta make you understand
-[00:43.000 --> 00:45.000]  Never gonna give you up
-[00:45.000 --> 00:47.000]  Never gonna let you down
-[00:47.000 --> 00:51.000]  Never gonna run around and desert you
-[00:51.000 --> 00:53.000]  Never gonna make you cry
-[00:53.000 --> 00:55.000]  Never gonna say goodbye
-[00:55.000 --> 00:58.000]  Never gonna tell a lie
-[00:58.000 --> 01:00.000]  And hurt you
-[01:00.000 --> 01:04.000]  We've known each other for so long
-[01:04.000 --> 01:09.000]  Your heart's been aching but you're too shy to say it
-[01:09.000 --> 01:13.000]  Inside we both know what's been going on
-[01:13.000 --> 01:17.000]  We know the game and we're gonna play it
-[01:17.000 --> 01:22.000]  And if you ask me how I'm feeling
-[01:22.000 --> 01:25.000]  Don't tell me you're too much to see
-[01:25.000 --> 01:27.000]  Never gonna give you up
-[01:27.000 --> 01:29.000]  Never gonna let you down
-[01:29.000 --> 01:33.000]  Never gonna run around and desert you
-[01:33.000 --> 01:35.000]  Never gonna make you cry
-[01:35.000 --> 01:38.000]  Never gonna say goodbye
-[01:38.000 --> 01:40.000]  Never gonna tell a lie
-[01:40.000 --> 01:42.000]  And hurt you
-[01:42.000 --> 01:44.000]  Never gonna give you up
-[01:44.000 --> 01:46.000]  Never gonna let you down
-[01:46.000 --> 01:50.000]  Never gonna run around and desert you
-[01:50.000 --> 01:52.000]  Never gonna make you cry
-[01:52.000 --> 01:54.000]  Never gonna say goodbye
-[01:54.000 --> 01:57.000]  Never gonna tell a lie
-[01:57.000 --> 01:59.000]  And hurt you
-[02:08.000 --> 02:10.000]  Never gonna give
-[02:12.000 --> 02:14.000]  Never gonna give
-[02:16.000 --> 02:19.000]  We've known each other for so long
-[02:19.000 --> 02:24.000]  Your heart's been aching but you're too shy to say it
-[02:24.000 --> 02:28.000]  Inside we both know what's been going on
-[02:28.000 --> 02:32.000]  We know the game and we're gonna play it
-[02:32.000 --> 02:37.000]  I just wanna tell you how I'm feeling
-[02:37.000 --> 02:40.000]  Gotta make you understand
-[02:40.000 --> 02:42.000]  Never gonna give you up
-[02:42.000 --> 02:44.000]  Never gonna let you down
-[02:44.000 --> 02:48.000]  Never gonna run around and desert you
-[02:48.000 --> 02:50.000]  Never gonna make you cry
-[02:50.000 --> 02:53.000]  Never gonna say goodbye
-[02:53.000 --> 02:55.000]  Never gonna tell a lie
-[02:55.000 --> 02:57.000]  And hurt you
-[02:57.000 --> 02:59.000]  Never gonna give you up
-[02:59.000 --> 03:01.000]  Never gonna let you down
-[03:01.000 --> 03:05.000]  Never gonna run around and desert you
-[03:05.000 --> 03:08.000]  Never gonna make you cry
-[03:08.000 --> 03:10.000]  Never gonna say goodbye
-[03:10.000 --> 03:12.000]  Never gonna tell a lie
-[03:12.000 --> 03:14.000]  And hurt you
-[03:14.000 --> 03:16.000]  Never gonna give you up
-[03:16.000 --> 03:23.000]  If you want, never gonna let you down Never gonna run around and desert you
-[03:23.000 --> 03:28.000]  Never gonna make you hide Never gonna say goodbye
-[03:28.000 --> 03:42.000]  Never gonna tell you I ain't ready
-```
-
-## Api
-
-```python
-from transcribe_anyting.api import transcribe
-
-transcribe(
-    url_or_file="https://www.youtube.com/watch?v=dQw4w9WgXcQ",
-    output_dir="output_dir",
-)
-```
-
-## Install GPU/CUDA Accelerated version
-
-GPU acceleration is *much* faster than the CPU version. Install it using the following:
-
-```bash
-> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
-# transcribe-anything should now be installed
-> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
-```
-
-## Develop
-
-Works for Ubuntu/MacOS/Win32(in git-bash)
-This will create a virtual environment
-
-```bash
-> cd transcribe_anything
-> ./install_dev.sh
-# Enter the environment:
-> source activate.sh
-```
-
-The environment is now active and the next step will only install to the local python. If the terminal
-is closed then to get back into the environment `cd transcribe_anything` and execute `source activate.sh`
-
-## Required: Install to current python environment
-  * `pip install transcribe-anything`
-    * The command `transcribe_anything` will magically become available.
-  * `transcribe_anything <YOUTUBE_URL>`
-
-
-# Tech Stack
-  * OpenAI whisper
-  * yt-dlp: https://github.com/yt-dlp/yt-dlp
-  * static-ffmpeg
-    * github: https://github.com/zackees/static_ffmpeg
-    * pypi: https://pypi.org/project/static-ffmpeg/
-
-# Testing
-  * All tests are run by `tox`, simply go to the project directory root and run it.
-
-# Versions
-  * 2.3.4: Removed `out.mp3` and instead use a temporary wav file, as that is faster to process. --no-keep-audio has now been removed.
-  * 2.3.3: Fix case where there spaces in name (happens on windows)
-  * 2.3.2: Fix windows transcoding error
-  * 2.3.1: static-ffmpeg >= 2.5 now specified
-  * 2.3.0: Now uses the official version of whisper ai
-  * 2.2.1: "test_" is now prepended to all the different output folder names.
-  * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
-  * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
-  * 2.1.1: Updates keywords for easier pypi finding.
-  * 2.1.0: Unknown args are now assumed to be for whisper and passed to it as-is. Fixes https://github.com/zackees/transcribe-anything/issues/3
-  * 2.0.13: Now works with python 3.9
-  * 2.0.12: Adds --device to argument parameters. This will default to CUDA if available, else CPU.
-  * 2.0.11: Automatically deletes files in the out directory if they already exist.
-  * 2.0.10: fixes local file issue https://github.com/zackees/transcribe-anything/issues/2
-  * 2.0.9: fixes sanitization of path names for some youtube videos
-  * 2.0.8: fix `--output_dir` not being respected.
-  * 2.0.7: `install_cuda.sh` -> `install_cuda.py`
-  * 2.0.6: Fixes twitter video fetching. --keep-audio -> --no-keep-audio
-  * 2.0.5: Fix bad filename on trailing urls ending with /, adds --keep-audio
-  * 2.0.3: GPU support is now added. Run the `install_cuda.sh` script to enable.
-  * 2.0.2: Minor cleanup of file names (no more out.mp3.txt, it's now out.txt)
-  * 2.0.1: Fixes missing dependencies and adds whisper option.
-  * 2.0.0: New! Now a front end for Whisper ai!
+Metadata-Version: 2.1
+Name: transcribe-anything
+Version: 2.3.5
+Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
+Home-page: https://github.com/zackees/transcribe-anything
+Author: Zach Vorhies
+Author-email: dont@email.me
+License: MIT
+Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Environment :: Console
+Requires-Python: >=3.9.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# transcribe-anything
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_macos.yml)
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Win_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_win.yml)
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_ubuntu.yml)
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Lint/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/lint.yml)
+
+### USES WHISPER AI
+
+Input a local file or url and this tool will transcribe it using Whisper AI into subtitle files and raw text.
+
+Uses whisper AI so this is state of the art translation service - completely free. 🤯🤯🤯
+
+Your data stays private and is not uploaded to any service.
+
+# Usage (CPU Version)
+
+```bash
+> pip install transcribe-anything
+# Outputs the srt, vtt and txt files in title/out.vtt
+> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
+```
+
+# Usage (GPU Accelerated Version) (works on Python 3.10.X)
+
+```bash
+> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
+# Outputs the srt, vtt and txt files in title/out.vtt
+> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
+```
+
+Will output:
+
+```
+Detecting language using up to the first 30 seconds. Use `--language` to specify the language
+Detected language: English
+[00:00.000 --> 00:27.000]  We're no strangers to love, you know the rules, and so do I
+[00:27.000 --> 00:31.000]  I've built commitments while I'm thinking of
+[00:31.000 --> 00:35.000]  You wouldn't get this from any other guy
+[00:35.000 --> 00:40.000]  I just wanna tell you how I'm feeling
+[00:40.000 --> 00:43.000]  Gotta make you understand
+[00:43.000 --> 00:45.000]  Never gonna give you up
+[00:45.000 --> 00:47.000]  Never gonna let you down
+[00:47.000 --> 00:51.000]  Never gonna run around and desert you
+[00:51.000 --> 00:53.000]  Never gonna make you cry
+[00:53.000 --> 00:55.000]  Never gonna say goodbye
+[00:55.000 --> 00:58.000]  Never gonna tell a lie
+[00:58.000 --> 01:00.000]  And hurt you
+[01:00.000 --> 01:04.000]  We've known each other for so long
+[01:04.000 --> 01:09.000]  Your heart's been aching but you're too shy to say it
+[01:09.000 --> 01:13.000]  Inside we both know what's been going on
+[01:13.000 --> 01:17.000]  We know the game and we're gonna play it
+[01:17.000 --> 01:22.000]  And if you ask me how I'm feeling
+[01:22.000 --> 01:25.000]  Don't tell me you're too much to see
+[01:25.000 --> 01:27.000]  Never gonna give you up
+[01:27.000 --> 01:29.000]  Never gonna let you down
+[01:29.000 --> 01:33.000]  Never gonna run around and desert you
+[01:33.000 --> 01:35.000]  Never gonna make you cry
+[01:35.000 --> 01:38.000]  Never gonna say goodbye
+[01:38.000 --> 01:40.000]  Never gonna tell a lie
+[01:40.000 --> 01:42.000]  And hurt you
+[01:42.000 --> 01:44.000]  Never gonna give you up
+[01:44.000 --> 01:46.000]  Never gonna let you down
+[01:46.000 --> 01:50.000]  Never gonna run around and desert you
+[01:50.000 --> 01:52.000]  Never gonna make you cry
+[01:52.000 --> 01:54.000]  Never gonna say goodbye
+[01:54.000 --> 01:57.000]  Never gonna tell a lie
+[01:57.000 --> 01:59.000]  And hurt you
+[02:08.000 --> 02:10.000]  Never gonna give
+[02:12.000 --> 02:14.000]  Never gonna give
+[02:16.000 --> 02:19.000]  We've known each other for so long
+[02:19.000 --> 02:24.000]  Your heart's been aching but you're too shy to say it
+[02:24.000 --> 02:28.000]  Inside we both know what's been going on
+[02:28.000 --> 02:32.000]  We know the game and we're gonna play it
+[02:32.000 --> 02:37.000]  I just wanna tell you how I'm feeling
+[02:37.000 --> 02:40.000]  Gotta make you understand
+[02:40.000 --> 02:42.000]  Never gonna give you up
+[02:42.000 --> 02:44.000]  Never gonna let you down
+[02:44.000 --> 02:48.000]  Never gonna run around and desert you
+[02:48.000 --> 02:50.000]  Never gonna make you cry
+[02:50.000 --> 02:53.000]  Never gonna say goodbye
+[02:53.000 --> 02:55.000]  Never gonna tell a lie
+[02:55.000 --> 02:57.000]  And hurt you
+[02:57.000 --> 02:59.000]  Never gonna give you up
+[02:59.000 --> 03:01.000]  Never gonna let you down
+[03:01.000 --> 03:05.000]  Never gonna run around and desert you
+[03:05.000 --> 03:08.000]  Never gonna make you cry
+[03:08.000 --> 03:10.000]  Never gonna say goodbye
+[03:10.000 --> 03:12.000]  Never gonna tell a lie
+[03:12.000 --> 03:14.000]  And hurt you
+[03:14.000 --> 03:16.000]  Never gonna give you up
+[03:16.000 --> 03:23.000]  If you want, never gonna let you down Never gonna run around and desert you
+[03:23.000 --> 03:28.000]  Never gonna make you hide Never gonna say goodbye
+[03:28.000 --> 03:42.000]  Never gonna tell you I ain't ready
+```
+
+## Api
+
+```python
+from transcribe_anyting.api import transcribe
+
+transcribe(
+    url_or_file="https://www.youtube.com/watch?v=dQw4w9WgXcQ",
+    output_dir="output_dir",
+)
+```
+
+## Install GPU/CUDA Accelerated version
+
+GPU acceleration is *much* faster than the CPU version. Install it using the following:
+
+```bash
+> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
+# transcribe-anything should now be installed
+> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
+```
+
+## Develop
+
+Works for Ubuntu/MacOS/Win32(in git-bash)
+This will create a virtual environment
+
+```bash
+> cd transcribe_anything
+> ./install_dev.sh
+# Enter the environment:
+> source activate.sh
+```
+
+The environment is now active and the next step will only install to the local python. If the terminal
+is closed then to get back into the environment `cd transcribe_anything` and execute `source activate.sh`
+
+## Required: Install to current python environment
+  * `pip install transcribe-anything`
+    * The command `transcribe_anything` will magically become available.
+  * `transcribe_anything <YOUTUBE_URL>`
+
+
+# Tech Stack
+  * OpenAI whisper
+  * yt-dlp: https://github.com/yt-dlp/yt-dlp
+  * static-ffmpeg
+    * github: https://github.com/zackees/static_ffmpeg
+    * pypi: https://pypi.org/project/static-ffmpeg/
+
+# Testing
+  * All tests are run by `tox`, simply go to the project directory root and run it.
+
+# Versions
+  * 2.3.5: Now has `--embed` to burn the subtitles into the video itself. Only works on local mp4 files at the moment.
+  * 2.3.4: Removed `out.mp3` and instead use a temporary wav file, as that is faster to process. --no-keep-audio has now been removed.
+  * 2.3.3: Fix case where there spaces in name (happens on windows)
+  * 2.3.2: Fix windows transcoding error
+  * 2.3.1: static-ffmpeg >= 2.5 now specified
+  * 2.3.0: Now uses the official version of whisper ai
+  * 2.2.1: "test_" is now prepended to all the different output folder names.
+  * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
+  * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
+  * 2.1.1: Updates keywords for easier pypi finding.
+  * 2.1.0: Unknown args are now assumed to be for whisper and passed to it as-is. Fixes https://github.com/zackees/transcribe-anything/issues/3
+  * 2.0.13: Now works with python 3.9
+  * 2.0.12: Adds --device to argument parameters. This will default to CUDA if available, else CPU.
+  * 2.0.11: Automatically deletes files in the out directory if they already exist.
+  * 2.0.10: fixes local file issue https://github.com/zackees/transcribe-anything/issues/2
+  * 2.0.9: fixes sanitization of path names for some youtube videos
+  * 2.0.8: fix `--output_dir` not being respected.
+  * 2.0.7: `install_cuda.sh` -> `install_cuda.py`
+  * 2.0.6: Fixes twitter video fetching. --keep-audio -> --no-keep-audio
+  * 2.0.5: Fix bad filename on trailing urls ending with /, adds --keep-audio
+  * 2.0.3: GPU support is now added. Run the `install_cuda.sh` script to enable.
+  * 2.0.2: Minor cleanup of file names (no more out.mp3.txt, it's now out.txt)
+  * 2.0.1: Fixes missing dependencies and adds whisper option.
+  * 2.0.0: New! Now a front end for Whisper ai!
```

### Comparing `transcribe-anything-2.3.4/transcribe_anything.egg-info/SOURCES.txt` & `transcribe-anything-2.3.5/transcribe_anything.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.testing.txt
 requirements.txt
 setup.py
+tests/test_embed_transcript.py
 tests/test_local_file_cmd.py
 tests/test_transcribe_anything.py
 tests/test_transcribe_anything_api.py
 tests/test_whisper.py
 transcribe_anything/__init__.py
 transcribe_anything/api.py
 transcribe_anything/audio.py
 transcribe_anything/cmd.py
 transcribe_anything/logger.py
 transcribe_anything/parse_whisper_options.py
 transcribe_anything/util.py
+transcribe_anything/ytldp_download.py
 transcribe_anything.egg-info/PKG-INFO
 transcribe_anything.egg-info/SOURCES.txt
 transcribe_anything.egg-info/dependency_links.txt
 transcribe_anything.egg-info/entry_points.txt
 transcribe_anything.egg-info/requires.txt
 transcribe_anything.egg-info/top_level.txt
```

