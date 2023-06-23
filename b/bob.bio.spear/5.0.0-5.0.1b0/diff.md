# Comparing `tmp/bob.bio.spear-5.0.0.tar.gz` & `tmp/bob.bio.spear-5.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bob.bio.spear-5.0.0.tar", last modified: Thu Jun 22 16:44:40 2023, max compression
+gzip compressed data, was "bob.bio.spear-5.0.1b0.tar", last modified: Fri Jun 23 20:10:15 2023, max compression
```

## Comparing `bob.bio.spear-5.0.0.tar` & `bob.bio.spear-5.0.1b0.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.150073 bob.bio.spear-5.0.0/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2793 2023-06-22 16:44:40.146073 bob.bio.spear-5.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1831 2023-06-22 16:17:55.000000 bob.bio.spear-5.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.126073 bob.bio.spear-5.0.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)     8757 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/doc/baselines.rst
--rw-rw-rw-   0 root         (0) root         (0)     8085 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     3483 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/doc/implementation.rst
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/doc/implemented.rst
--rw-rw-rw-   0 root         (0) root         (0)     2205 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.130073 bob.bio.spear-5.0.0/doc/leaderboard/
--rw-rw-rw-   0 root         (0) root         (0)     1284 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/doc/leaderboard/leaderboard.rst
--rw-rw-rw-   0 root         (0) root         (0)     4474 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/doc/leaderboard/mobio_audio_female.rst
--rw-rw-rw-   0 root         (0) root         (0)     4469 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/doc/leaderboard/mobio_audio_male.rst
--rw-rw-rw-   0 root         (0) root         (0)     4496 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/doc/leaderboard/nist_sre04_16.rst
--rw-rw-rw-   0 root         (0) root         (0)     3728 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/doc/leaderboard/voxceleb.rst
--rw-rw-rw-   0 root         (0) root         (0)     5523 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/doc/leaderboard/voxforge.rst
--rw-rw-rw-   0 root         (0) root         (0)     1541 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/doc/links.rst
--rw-rw-rw-   0 root         (0) root         (0)      688 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/doc/references.rst
--rw-rw-rw-   0 root         (0) root         (0)     5755 2023-06-22 16:17:55.000000 bob.bio.spear-5.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 16:44:40.150073 bob.bio.spear-5.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.122073 bob.bio.spear-5.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.130073 bob.bio.spear-5.0.0/src/bob/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.130073 bob.bio.spear-5.0.0/src/bob/bio/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.130073 bob.bio.spear-5.0.0/src/bob/bio/spear/
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.134073 bob.bio.spear-5.0.0/src/bob/bio/spear/annotator/
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/annotator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6081 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/annotator/energy_2gauss.py
--rw-rw-rw-   0 root         (0) root         (0)     3912 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/annotator/energy_thr.py
--rw-rw-rw-   0 root         (0) root         (0)     9070 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/annotator/mod_4hz.py
--rw-rw-rw-   0 root         (0) root         (0)    18004 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/audio_processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.134073 bob.bio.spear-5.0.0/src/bob/bio/spear/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 16:44:17.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.134073 bob.bio.spear-5.0.0/src/bob/bio/spear/config/annotator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 16:44:17.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/annotator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/annotator/energy_2gauss.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/annotator/energy_thr.py
--rw-rw-rw-   0 root         (0) root         (0)      530 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/annotator/mod_4hz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.134073 bob.bio.spear-5.0.0/src/bob/bio/spear/config/database/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 16:44:17.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/database/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/database/asvspoof.py
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/database/avspoof.py
--rw-rw-rw-   0 root         (0) root         (0)     1209 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/database/mini_voxforge.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/database/mobio_audio_female.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/database/mobio_audio_male.py
--rw-rw-rw-   0 root         (0) root         (0)     1857 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/database/nist_sre04to16.py
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/database/timit.py
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/database/voicepa.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/database/voxceleb.py
--rw-rw-rw-   0 root         (0) root         (0)     1280 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/database/voxforge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.134073 bob.bio.spear-5.0.0/src/bob/bio/spear/config/extractor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 16:44:17.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/extractor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/extractor/mfcc60.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.138073 bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 16:44:17.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1840 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/mfcc60_gmm_default.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/mfcc60_gmm_mini.py
--rw-rw-rw-   0 root         (0) root         (0)     1799 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/mfcc60_gmm_mobio.py
--rw-rw-rw-   0 root         (0) root         (0)     1310 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/mfcc60_isv_default.py
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/mfcc60_isv_mini.py
--rw-rw-rw-   0 root         (0) root         (0)     1967 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/mfcc60_ivector.py
--rw-rw-rw-   0 root         (0) root         (0)     2698 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/mfcc60_ivector_postprocess.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/speechbrain_ecapa_voxceleb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.138073 bob.bio.spear-5.0.0/src/bob/bio/spear/config/preprocessor/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/config/preprocessor/mod_4hz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.138073 bob.bio.spear-5.0.0/src/bob/bio/spear/database/
--rw-rw-rw-   0 root         (0) root         (0)     1841 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/database/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/database/asvspoof.py
--rw-rw-rw-   0 root         (0) root         (0)     1623 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/database/asvspoof2017.py
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/database/avspoof.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/database/mobio.py
--rw-rw-rw-   0 root         (0) root         (0)      927 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/database/nist_sre04to16.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/database/timit.py
--rw-rw-rw-   0 root         (0) root         (0)     1844 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/database/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/database/voicepa.py
--rw-rw-rw-   0 root         (0) root         (0)      810 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/database/voxceleb.py
--rw-rw-rw-   0 root         (0) root         (0)     3385 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/database/voxforge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.142073 bob.bio.spear-5.0.0/src/bob/bio/spear/extractor/
--rw-rw-rw-   0 root         (0) root         (0)     5346 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/extractor/Cepstral.py
--rw-rw-rw-   0 root         (0) root         (0)     1491 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/extractor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1624 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/extractor/speechbrain_embeddings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.142073 bob.bio.spear-5.0.0/src/bob/bio/spear/transformer/
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/transformer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2943 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/transformer/path_to_audio.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/transformer/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/transformer/resample.py
--rw-rw-rw-   0 root         (0) root         (0)     2511 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/src/bob/bio/spear/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.130073 bob.bio.spear-5.0.0/src/bob.bio.spear.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2793 2023-06-22 16:44:40.000000 bob.bio.spear-5.0.0/src/bob.bio.spear.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3565 2023-06-22 16:44:40.000000 bob.bio.spear-5.0.0/src/bob.bio.spear.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 16:44:40.000000 bob.bio.spear-5.0.0/src/bob.bio.spear.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     2115 2023-06-22 16:44:40.000000 bob.bio.spear-5.0.0/src/bob.bio.spear.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 16:44:39.000000 bob.bio.spear-5.0.0/src/bob.bio.spear.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      450 2023-06-22 16:44:40.000000 bob.bio.spear-5.0.0/src/bob.bio.spear.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-22 16:44:40.000000 bob.bio.spear-5.0.0/src/bob.bio.spear.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.142073 bob.bio.spear-5.0.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:44:40.146073 bob.bio.spear-5.0.0/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)   179744 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/data/lfcc_60.hdf5
--rw-rw-rw-   0 root         (0) root         (0)   183008 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/data/mfcc_60.hdf5
--rw-rw-rw-   0 root         (0) root         (0)   313096 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/data/sample.hdf5
--rw-rw-rw-   0 root         (0) root         (0)   155564 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/data/sample.wav
--rw-rw-rw-   0 root         (0) root         (0)   244568 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/data/sample_cepstral.npy
--rw-rw-rw-   0 root         (0) root         (0)     4008 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/data/sample_energy.npy
--rw-rw-rw-   0 root         (0) root         (0)   997288 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/data/sample_spectrogram.npy
--rw-rw-rw-   0 root         (0) root         (0)   176480 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/data/silence.wav
--rw-rw-rw-   0 root         (0) root         (0)     5928 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/data/vad_energy_2gauss.hdf5
--rw-rw-rw-   0 root         (0) root         (0)     3018 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/data/vad_energy_thr.hdf5
--rw-rw-rw-   0 root         (0) root         (0)     3018 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/data/vad_mod_4hz.hdf5
--rw-rw-rw-   0 root         (0) root         (0)     5111 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/test_annotators.py
--rw-rw-rw-   0 root         (0) root         (0)     2869 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/test_audio_processing.py
--rw-rw-rw-   0 root         (0) root         (0)    10638 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/test_databases.py
--rw-rw-rw-   0 root         (0) root         (0)     2631 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/test_extractors.py
--rw-rw-rw-   0 root         (0) root         (0)     4872 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/test_pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     1740 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.0/tests/test_transformers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.365531 bob.bio.spear-5.0.1b0/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2795 2023-06-23 20:10:15.365531 bob.bio.spear-5.0.1b0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2023-06-23 19:39:18.000000 bob.bio.spear-5.0.1b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.337531 bob.bio.spear-5.0.1b0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     8757 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/doc/baselines.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8085 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3483 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/doc/implementation.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/doc/implemented.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2205 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.341531 bob.bio.spear-5.0.1b0/doc/leaderboard/
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/doc/leaderboard/leaderboard.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4474 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/doc/leaderboard/mobio_audio_female.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4469 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/doc/leaderboard/mobio_audio_male.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4496 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/doc/leaderboard/nist_sre04_16.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3728 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/doc/leaderboard/voxceleb.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5523 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/doc/leaderboard/voxforge.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/doc/links.rst
+-rw-rw-rw-   0 root         (0) root         (0)      688 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/doc/references.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5468 2023-06-23 19:39:18.000000 bob.bio.spear-5.0.1b0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 20:10:15.365531 bob.bio.spear-5.0.1b0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.333531 bob.bio.spear-5.0.1b0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.341531 bob.bio.spear-5.0.1b0/src/bob/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.345531 bob.bio.spear-5.0.1b0/src/bob/bio/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.345531 bob.bio.spear-5.0.1b0/src/bob/bio/spear/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.345531 bob.bio.spear-5.0.1b0/src/bob/bio/spear/annotator/
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/annotator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6081 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/annotator/energy_2gauss.py
+-rw-rw-rw-   0 root         (0) root         (0)     3912 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/annotator/energy_thr.py
+-rw-rw-rw-   0 root         (0) root         (0)     9070 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/annotator/mod_4hz.py
+-rw-rw-rw-   0 root         (0) root         (0)    18004 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/audio_processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.345531 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 20:09:49.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.345531 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/annotator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 20:09:49.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/annotator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/annotator/energy_2gauss.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/annotator/energy_thr.py
+-rw-rw-rw-   0 root         (0) root         (0)      530 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/annotator/mod_4hz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.349531 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/database/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 20:09:49.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/database/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/database/asvspoof.py
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/database/avspoof.py
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/database/mini_voxforge.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/database/mobio_audio_female.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/database/mobio_audio_male.py
+-rw-rw-rw-   0 root         (0) root         (0)     1857 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/database/nist_sre04to16.py
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/database/timit.py
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/database/voicepa.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/database/voxceleb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1280 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/database/voxforge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.349531 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/extractor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 20:09:49.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/extractor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/extractor/mfcc60.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.349531 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 20:09:49.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/mfcc60_gmm_default.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/mfcc60_gmm_mini.py
+-rw-rw-rw-   0 root         (0) root         (0)     1799 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/mfcc60_gmm_mobio.py
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/mfcc60_isv_default.py
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/mfcc60_isv_mini.py
+-rw-rw-rw-   0 root         (0) root         (0)     1967 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/mfcc60_ivector.py
+-rw-rw-rw-   0 root         (0) root         (0)     2698 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/mfcc60_ivector_postprocess.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/speechbrain_ecapa_voxceleb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.349531 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/preprocessor/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/preprocessor/mod_4hz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.353531 bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/
+-rw-rw-rw-   0 root         (0) root         (0)     1841 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/asvspoof.py
+-rw-rw-rw-   0 root         (0) root         (0)     1623 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/asvspoof2017.py
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/avspoof.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/mobio.py
+-rw-rw-rw-   0 root         (0) root         (0)      927 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/nist_sre04to16.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/timit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1844 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/voicepa.py
+-rw-rw-rw-   0 root         (0) root         (0)      810 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/voxceleb.py
+-rw-rw-rw-   0 root         (0) root         (0)     3385 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/voxforge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.353531 bob.bio.spear-5.0.1b0/src/bob/bio/spear/extractor/
+-rw-rw-rw-   0 root         (0) root         (0)     5346 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/extractor/Cepstral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/extractor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/extractor/speechbrain_embeddings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.353531 bob.bio.spear-5.0.1b0/src/bob/bio/spear/transformer/
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/transformer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2943 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/transformer/path_to_audio.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/transformer/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/transformer/resample.py
+-rw-rw-rw-   0 root         (0) root         (0)     2511 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/src/bob/bio/spear/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.341531 bob.bio.spear-5.0.1b0/src/bob.bio.spear.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2795 2023-06-23 20:10:15.000000 bob.bio.spear-5.0.1b0/src/bob.bio.spear.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-06-23 20:10:15.000000 bob.bio.spear-5.0.1b0/src/bob.bio.spear.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 20:10:15.000000 bob.bio.spear-5.0.1b0/src/bob.bio.spear.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     2115 2023-06-23 20:10:15.000000 bob.bio.spear-5.0.1b0/src/bob.bio.spear.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 20:10:15.000000 bob.bio.spear-5.0.1b0/src/bob.bio.spear.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-23 20:10:15.000000 bob.bio.spear-5.0.1b0/src/bob.bio.spear.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-23 20:10:15.000000 bob.bio.spear-5.0.1b0/src/bob.bio.spear.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.357531 bob.bio.spear-5.0.1b0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:10:15.365531 bob.bio.spear-5.0.1b0/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)   179744 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/data/lfcc_60.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)   183008 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/data/mfcc_60.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)   313096 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/data/sample.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)   155564 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/data/sample.wav
+-rw-rw-rw-   0 root         (0) root         (0)   244568 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/data/sample_cepstral.npy
+-rw-rw-rw-   0 root         (0) root         (0)     4008 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/data/sample_energy.npy
+-rw-rw-rw-   0 root         (0) root         (0)   997288 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/data/sample_spectrogram.npy
+-rw-rw-rw-   0 root         (0) root         (0)   176480 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/data/silence.wav
+-rw-rw-rw-   0 root         (0) root         (0)     5928 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/data/vad_energy_2gauss.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)     3018 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/data/vad_energy_thr.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)     3018 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/data/vad_mod_4hz.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)     5111 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/test_annotators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2869 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/test_audio_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)    10638 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/test_databases.py
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/test_extractors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4872 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/test_pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     1740 2023-06-22 15:33:05.000000 bob.bio.spear-5.0.1b0/tests/test_transformers.py
```

### Comparing `bob.bio.spear-5.0.0/COPYING` & `bob.bio.spear-5.0.1b0/COPYING`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/PKG-INFO` & `bob.bio.spear-5.0.1b0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bob.bio.spear
-Version: 5.0.0
+Version: 5.0.1b0
 Author-email: Andre Anjos <andre.anjos@idiap.ch>
 License: GPLv3
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/v5.0.0/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/stable/
 Project-URL: homepage, https://pypi.org/project/bob.bio.spear/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.bio.spear
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.bio.spear/-/releases
 Keywords: bob,biometric recognition,evaluation
 Classifier: Framework :: Bob
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,17 +18,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: COPYING
 
-[![badge doc](https://img.shields.io/badge/docs-v5.0.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/v5.0.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.spear/badges/v5.0.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.spear/commits/v5.0.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.spear/badges/v5.0.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/v5.0.0/coverage/index.html)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.spear/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.spear/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.spear/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/master/coverage/index.html)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.bio.spear)
 
 # Run speaker recognition algorithms
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob).
 This package is part of the `bob.bio` packages, which allow to run comparable
```

### Comparing `bob.bio.spear-5.0.0/README.md` & `bob.bio.spear-5.0.1b0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-[![badge doc](https://img.shields.io/badge/docs-v5.0.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/v5.0.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.spear/badges/v5.0.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.spear/commits/v5.0.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.spear/badges/v5.0.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/v5.0.0/coverage/index.html)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.spear/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.spear/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.spear/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/master/coverage/index.html)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.bio.spear)
 
 # Run speaker recognition algorithms
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob).
 This package is part of the `bob.bio` packages, which allow to run comparable
```

### Comparing `bob.bio.spear-5.0.0/doc/baselines.rst` & `bob.bio.spear-5.0.1b0/doc/baselines.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/doc/conf.py` & `bob.bio.spear-5.0.1b0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/doc/implementation.rst` & `bob.bio.spear-5.0.1b0/doc/implementation.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/doc/implemented.rst` & `bob.bio.spear-5.0.1b0/doc/implemented.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/doc/index.rst` & `bob.bio.spear-5.0.1b0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/doc/leaderboard/leaderboard.rst` & `bob.bio.spear-5.0.1b0/doc/leaderboard/leaderboard.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/doc/leaderboard/mobio_audio_female.rst` & `bob.bio.spear-5.0.1b0/doc/leaderboard/mobio_audio_female.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/doc/leaderboard/mobio_audio_male.rst` & `bob.bio.spear-5.0.1b0/doc/leaderboard/mobio_audio_male.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/doc/leaderboard/nist_sre04_16.rst` & `bob.bio.spear-5.0.1b0/doc/leaderboard/nist_sre04_16.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/doc/leaderboard/voxceleb.rst` & `bob.bio.spear-5.0.1b0/doc/leaderboard/voxceleb.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/doc/leaderboard/voxforge.rst` & `bob.bio.spear-5.0.1b0/doc/leaderboard/voxforge.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/doc/links.rst` & `bob.bio.spear-5.0.1b0/doc/links.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/doc/references.rst` & `bob.bio.spear-5.0.1b0/doc/references.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/pyproject.toml` & `bob.bio.spear-5.0.1b0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires      = ["setuptools>=61.0.0", "wheel"]
     build-backend = "setuptools.build_meta"
 
 [project]
     name            = "bob.bio.spear"
-    version         = "5.0.0"
+    version         = "5.0.1b0"
     requires-python = ">=3.9"
     description     = ""
     dynamic         = ["readme"]
     license         = {text = "GPLv3"}
     authors         = [
     {name = "Andre Anjos", email = "andre.anjos@idiap.ch"},
     ]
@@ -20,50 +20,50 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ]
     dependencies = [
-        "bob==12.0.0",
-        "bob.io.base==5.1.0",
-        "bob.measure==6.1.0",
-        "bob.pipelines==4.0.0",
-        "bob.learn.em==3.3.0",
-        "bob.bio.base==8.0.0",
-        "clapper==1.0.1",
+        "bob",
+        "bob.io.base",
+        "bob.measure",
+        "bob.pipelines",
+        "bob.learn.em",
+        "bob.bio.base",
+        "clapper",
         "pysoundfile",
-        "scikit-learn==1.1.2",
-        "six==1.16.0",
-        "torch==1.13.0",
+        "scikit-learn",
+        "six",
+        "torch",
         "torchaudio",
-        "tqdm==4.64.1",
+        "tqdm",
     ]
 
 [project.urls]
-    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/v5.0.0/"
+    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/stable/"
     homepage      = "https://pypi.org/project/bob.bio.spear/"
     repository    = "https://gitlab.idiap.ch/bob/bob.bio.spear"
     changelog     = "https://gitlab.idiap.ch/bob/bob.bio.spear/-/releases"
 
 [project.optional-dependencies]
     qa  = ["pre-commit"]
     doc = [
-        "sphinx==5.3.0",
-        "sphinx-rtd-theme==1.1.1",
-        "sphinx-autodoc-typehints==1.21.8",
-        "auto-intersphinx==1.0.2",
-        "sphinxcontrib-programoutput==0.17",
-        "matplotlib==3.6.2",
+        "sphinx",
+        "sphinx_rtd_theme",
+        "sphinx-autodoc-typehints",
+        "auto-intersphinx",
+        "sphinxcontrib-programoutput",
+        "matplotlib",
         ]
     test = [
-        "pytest==7.2.1",
-        "pytest-cov==4.0.0",
-        "coverage==7.0.5",
-        "dask==2023.1.0",
+        "pytest",
+        "pytest-cov",
+        "coverage",
+        "dask",
         ]
 
 [tool.setuptools]
     zip-safe    = false
     package-dir = {"" = "src"}
 
 [tool.setuptools.dynamic]
@@ -135,11 +135,7 @@
         "--cov=bob.bio.spear",
     ]
     markers = [
         "slow: marks tests as slow (deselect with '-m \"not slow\"')",
     ]
     junit_logging           = "all"
     junit_log_passing_tests = false
-
-[profile]
-    repository_url = "git@gitlab.idiap.ch:bob/dev-profile.git"
-    commit_hash = "ade723be1f11feddb7bece235de32cc98953dc07"
```

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/annotator/__init__.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/annotator/energy_2gauss.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/annotator/energy_2gauss.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/annotator/energy_thr.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/annotator/energy_thr.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/annotator/mod_4hz.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/annotator/mod_4hz.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/audio_processing.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/audio_processing.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/config/annotator/energy_2gauss.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/annotator/energy_2gauss.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/config/annotator/energy_thr.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/annotator/energy_thr.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/config/annotator/mod_4hz.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/annotator/mod_4hz.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/config/database/mini_voxforge.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/database/mini_voxforge.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/config/database/nist_sre04to16.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/database/nist_sre04to16.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/config/database/voxforge.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/database/voxforge.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/mfcc60_gmm_default.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/mfcc60_gmm_default.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/mfcc60_gmm_mini.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/mfcc60_gmm_mini.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/mfcc60_gmm_mobio.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/mfcc60_gmm_mobio.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/mfcc60_isv_default.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/mfcc60_isv_default.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/mfcc60_isv_mini.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/mfcc60_isv_mini.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/mfcc60_ivector.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/mfcc60_ivector.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/mfcc60_ivector_postprocess.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/mfcc60_ivector_postprocess.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/config/pipeline/speechbrain_ecapa_voxceleb.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/config/pipeline/speechbrain_ecapa_voxceleb.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/database/__init__.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/database/asvspoof.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/asvspoof.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/database/asvspoof2017.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/asvspoof2017.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/database/avspoof.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/avspoof.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/database/mobio.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/mobio.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/database/nist_sre04to16.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/nist_sre04to16.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/database/timit.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/timit.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/database/utils.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/utils.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/database/voicepa.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/voicepa.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/database/voxceleb.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/voxceleb.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/database/voxforge.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/database/voxforge.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/extractor/Cepstral.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/extractor/Cepstral.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/extractor/__init__.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/extractor/speechbrain_embeddings.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/extractor/speechbrain_embeddings.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/transformer/__init__.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/transformer/path_to_audio.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/transformer/path_to_audio.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/transformer/preprocessing.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/transformer/preprocessing.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/transformer/resample.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/transformer/resample.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob/bio/spear/utils.py` & `bob.bio.spear-5.0.1b0/src/bob/bio/spear/utils.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob.bio.spear.egg-info/PKG-INFO` & `bob.bio.spear-5.0.1b0/src/bob.bio.spear.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bob.bio.spear
-Version: 5.0.0
+Version: 5.0.1b0
 Author-email: Andre Anjos <andre.anjos@idiap.ch>
 License: GPLv3
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/v5.0.0/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/stable/
 Project-URL: homepage, https://pypi.org/project/bob.bio.spear/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.bio.spear
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.bio.spear/-/releases
 Keywords: bob,biometric recognition,evaluation
 Classifier: Framework :: Bob
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,17 +18,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: COPYING
 
-[![badge doc](https://img.shields.io/badge/docs-v5.0.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/v5.0.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.spear/badges/v5.0.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.spear/commits/v5.0.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.spear/badges/v5.0.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/v5.0.0/coverage/index.html)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.spear/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.spear/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.spear/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.spear/master/coverage/index.html)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.bio.spear)
 
 # Run speaker recognition algorithms
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob).
 This package is part of the `bob.bio` packages, which allow to run comparable
```

### Comparing `bob.bio.spear-5.0.0/src/bob.bio.spear.egg-info/SOURCES.txt` & `bob.bio.spear-5.0.1b0/src/bob.bio.spear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/src/bob.bio.spear.egg-info/entry_points.txt` & `bob.bio.spear-5.0.1b0/src/bob.bio.spear.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/data/lfcc_60.hdf5` & `bob.bio.spear-5.0.1b0/tests/data/lfcc_60.hdf5`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/data/mfcc_60.hdf5` & `bob.bio.spear-5.0.1b0/tests/data/mfcc_60.hdf5`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/data/sample.hdf5` & `bob.bio.spear-5.0.1b0/tests/data/sample.hdf5`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/data/sample.wav` & `bob.bio.spear-5.0.1b0/tests/data/sample.wav`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/data/sample_cepstral.npy` & `bob.bio.spear-5.0.1b0/tests/data/sample_cepstral.npy`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/data/sample_energy.npy` & `bob.bio.spear-5.0.1b0/tests/data/sample_energy.npy`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/data/sample_spectrogram.npy` & `bob.bio.spear-5.0.1b0/tests/data/sample_spectrogram.npy`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/data/silence.wav` & `bob.bio.spear-5.0.1b0/tests/data/silence.wav`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/data/vad_energy_2gauss.hdf5` & `bob.bio.spear-5.0.1b0/tests/data/vad_energy_2gauss.hdf5`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/data/vad_energy_thr.hdf5` & `bob.bio.spear-5.0.1b0/tests/data/vad_energy_thr.hdf5`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/data/vad_mod_4hz.hdf5` & `bob.bio.spear-5.0.1b0/tests/data/vad_mod_4hz.hdf5`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/test_annotators.py` & `bob.bio.spear-5.0.1b0/tests/test_annotators.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/test_audio_processing.py` & `bob.bio.spear-5.0.1b0/tests/test_audio_processing.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/test_databases.py` & `bob.bio.spear-5.0.1b0/tests/test_databases.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/test_extractors.py` & `bob.bio.spear-5.0.1b0/tests/test_extractors.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/test_pipelines.py` & `bob.bio.spear-5.0.1b0/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `bob.bio.spear-5.0.0/tests/test_transformers.py` & `bob.bio.spear-5.0.1b0/tests/test_transformers.py`

 * *Files identical despite different names*

