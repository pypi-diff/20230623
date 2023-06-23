# Comparing `tmp/python-rtmidi-1.5.2.tar.gz` & `tmp/python_rtmidi-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-rtmidi-1.5.2.tar", last modified: Wed Jun 14 06:50:52 2023, max compression
+gzip compressed data, was "python_rtmidi-1.5.3.tar", last modified: Fri Jun 23 06:48:00 2023, max compression
```

## Comparing `python-rtmidi-1.5.2.tar` & `python_rtmidi-1.5.3.tar`

### file list

```diff
@@ -1,178 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:47.066178 python-rtmidi-1.5.2/
--rw-rw-r--   0 runner    (1001) docker     (123)       94 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.flake8
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.github/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (123)     1393 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.github/workflows/pr_to_master.yml
--rw-rw-r--   0 runner    (1001) docker     (123)     2338 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.github/workflows/push_to_master.yml
--rw-rw-r--   0 runner    (1001) docker     (123)     2277 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.github/workflows/release.yml
--rw-rw-r--   0 runner    (1001) docker     (123)      571 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (123)      118 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.gitmodules
--rw-rw-r--   0 runner    (1001) docker     (123)      300 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/AUTHORS.md
--rw-rw-r--   0 runner    (1001) docker     (123)    21704 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (123)     3849 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/INSTALL-windows.md
--rw-rw-r--   0 runner    (1001) docker     (123)     8352 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/INSTALL.md
--rw-rw-r--   0 runner    (1001) docker     (123)     2771 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/LICENSE.md
--rw-rw-r--   0 runner    (1001) docker     (123)      393 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/MANIFEST.in
--rw-rw-r--   0 runner    (1001) docker     (123)     2497 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/Makefile
--rw-rw-r--   0 runner    (1001) docker     (123)     2802 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/README.md
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/
--rw-rw-r--   0 runner    (1001) docker     (123)     6778 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/Makefile
--rw-rw-r--   0 runner    (1001) docker     (123)      759 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/api.rst.inc
--rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/authors.md
--rwxrwxr-x   0 runner    (1001) docker     (123)     8521 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/conf.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3257 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/contributing.rst
--rw-rw-r--   0 runner    (1001) docker     (123)       33 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/history.md
--rw-rw-r--   0 runner    (1001) docker     (123)      478 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (123)       39 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/install-windows.md
--rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/installation.md
--rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/license.md
--rw-rw-r--   0 runner    (1001) docker     (123)     6467 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/make.bat
--rw-rw-r--   0 runner    (1001) docker     (123)       55 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/modules.rst
--rw-rw-r--   0 runner    (1001) docker     (123)       30 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/readme.md
--rw-rw-r--   0 runner    (1001) docker     (123)     1337 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/rtmidi.rst
--rw-rw-r--   0 runner    (1001) docker     (123)     1129 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/usage.rst
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/advanced/
--rw-rw-r--   0 runner    (1001) docker     (123)     1687 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/advanced/ccstore.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2398 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/advanced/midiclock.py
--rw-rw-r--   0 runner    (1001) docker     (123)     8741 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/advanced/midioutwrapper.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2585 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/advanced/recvrpn.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/
--rw-rw-r--   0 runner    (1001) docker     (123)      545 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/contextmanager.py
--rwxrwxr-x   0 runner    (1001) docker     (123)     1359 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/midiin_callback.py
--rwxrwxr-x   0 runner    (1001) docker     (123)     1050 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/midiin_poll.py
--rwxrwxr-x   0 runner    (1001) docker     (123)      991 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/midiout.py
--rw-rw-r--   0 runner    (1001) docker     (123)     1012 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/noteon2osc.py
--rw-rw-r--   0 runner    (1001) docker     (123)      765 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/panic.py
--rwxrwxr-x   0 runner    (1001) docker     (123)     1571 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/probe_ports.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/
--rw-rw-r--   0 runner    (1001) docker     (123)     2195 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/README.rst
--rw-rw-r--   0 runner    (1001) docker     (123)      275 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/break-on-through.txt
--rwxrwxr-x   0 runner    (1001) docker     (123)     6485 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/drumseq.py
--rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_01.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_02.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      255 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_03.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      206 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_04.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      294 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_05.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_06.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      302 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_07.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      302 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_08.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      434 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_09.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      435 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_10.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      299 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_11.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      347 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_12.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      157 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/funkydrummer.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      205 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/rosanna-shuffle.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      477 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/template.txt
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midi2command/
--rw-rw-r--   0 runner    (1001) docker     (123)    45974 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midi2command/000-playback.mp3
--rw-rw-r--   0 runner    (1001) docker     (123)     2506 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midi2command/000-sheet.pdf
--rw-rw-r--   0 runner    (1001) docker     (123)     5624 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midi2command/README.rst
--rw-rw-r--   0 runner    (1001) docker     (123)      522 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midi2command/example.cfg
--rw-rw-r--   0 runner    (1001) docker     (123)     7132 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midi2command/midi2command.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midifilter/
--rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midifilter/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3667 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midifilter/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3119 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midifilter/filters.py
--rwxrwxr-x   0 runner    (1001) docker     (123)     5328 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sendsysex.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sequencer/
--rw-rw-r--   0 runner    (1001) docker     (123)     7155 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sequencer/sequencer.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysex/
--rwxrwxr-x   0 runner    (1001) docker     (123)      745 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysex/send_sysex.py
--rwxrwxr-x   0 runner    (1001) docker     (123)     1067 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysex/send_sysex_file.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysexsaver/
--rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysexsaver/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     7022 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysexsaver/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (123)    11493 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysexsaver/manufacturers.csv
--rw-rw-r--   0 runner    (1001) docker     (123)    12337 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysexsaver/manufacturers.py
--rw-rw-r--   0 runner    (1001) docker     (123)    12147 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysexsaver/models.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3247 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/wavetablemodstep.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3224 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/meson.build
--rw-rw-r--   0 runner    (1001) docker     (123)      801 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/meson_options.txt
--rwxrwxr-x   0 runner    (1001) docker     (123)      462 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/meson_postinstall.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3109 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (123)       91 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/requirements-dev.in
--rw-rw-r--   0 runner    (1001) docker     (123)     2686 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/requirements-dev.txt
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/rtmidi/
--rw-rw-r--   0 runner    (1001) docker     (123)      165 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/rtmidi/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     1744 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/rtmidi/meson.build
--rw-rw-r--   0 runner    (1001) docker     (123)     7533 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/rtmidi/midiconstants.py
--rw-rw-r--   0 runner    (1001) docker     (123)     9261 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/rtmidi/midiutil.py
--rw-rw-r--   0 runner    (1001) docker     (123)       30 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/rtmidi/version.py.in
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:47.706187 python-rtmidi-1.5.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)   737312 2023-06-14 06:50:47.706187 python-rtmidi-1.5.2/src/_rtmidi.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)    39588 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/src/_rtmidi.pyx
--rw-rw-r--   0 runner    (1001) docker     (123)      857 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/src/meson.build
--rwxrwxr-x   0 runner    (1001) docker     (123)     1261 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/src/meson_dist_cython.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/
--rw-rw-r--   0 runner    (1001) docker     (123)     9806 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (123)     1349 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (123)      533 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/Makefile.am
--rw-rw-r--   0 runner    (1001) docker     (123)     2396 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/README.md
--rw-rw-r--   0 runner    (1001) docker     (123)   126845 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/RtMidi.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)    27079 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/RtMidi.h
--rwxrwxr-x   0 runner    (1001) docker     (123)     2884 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/autogen.sh
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/cmake/
--rw-rw-r--   0 runner    (1001) docker     (123)      940 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in
--rw-rw-r--   0 runner    (1001) docker     (123)      277 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/cmake/rtmidi-config.cmake.in
--rw-rw-r--   0 runner    (1001) docker     (123)     9307 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/configure.ac
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/go/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/
--rw-rw-r--   0 runner    (1001) docker     (123)       59 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/go.mod
--rw-rw-r--   0 runner    (1001) docker     (123)    10504 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/rtmidi.go
--rw-rw-r--   0 runner    (1001) docker     (123)      125 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.h
--rw-rw-r--   0 runner    (1001) docker     (123)      758 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/
--rw-rw-r--   0 runner    (1001) docker     (123)      682 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/Makefile.am
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/
--rw-rw-r--   0 runner    (1001) docker     (123)    81155 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/Doxyfile.in
--rw-rw-r--   0 runner    (1001) docker     (123)      254 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/footer.html
--rw-rw-r--   0 runner    (1001) docker     (123)      494 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/header.html
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/samples/
--rw-rw-r--   0 runner    (1001) docker     (123)      173 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/samples/getting_started.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)    21717 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/tutorial.txt
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/images/
--rw-rw-r--   0 runner    (1001) docker     (123)     3527 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/images/ccrma.gif
--rw-rw-r--   0 runner    (1001) docker     (123)     4614 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/images/mcgill.gif
--rw-rw-r--   0 runner    (1001) docker     (123)     7130 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/release.txt
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/m4/
--rw-rw-r--   0 runner    (1001) docker     (123)    19367 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/msw/
--rw-rw-r--   0 runner    (1001) docker     (123)      171 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/msw/readme
--rwxrwxr-x   0 runner    (1001) docker     (123)      883 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/msw/rtmidilib.sln
--rwxrwxr-x   0 runner    (1001) docker     (123)     3734 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/msw/rtmidilib.vcproj
--rw-rw-r--   0 runner    (1001) docker     (123)      388 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/rtmidi-config.in
--rw-rw-r--   0 runner    (1001) docker     (123)      369 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/rtmidi.pc.in
--rw-rw-r--   0 runner    (1001) docker     (123)    10218 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/rtmidi_c.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     9532 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/rtmidi_c.h
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/Debug/
--rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/Debug/.placeholder
--rw-rw-r--   0 runner    (1001) docker     (123)     1018 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/Makefile.am
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/Release/
--rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/Release/.placeholder
--rw-rw-r--   0 runner    (1001) docker     (123)     1311 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/RtMidi.dsw
--rw-rw-r--   0 runner    (1001) docker     (123)     5284 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/apinames.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     2873 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/cmidiin.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/cmidiin.dsp
--rw-rw-r--   0 runner    (1001) docker     (123)     5541 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/midiclock.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     3147 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/midiout.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/midiout.dsp
--rw-rw-r--   0 runner    (1001) docker     (123)     2138 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/midiprobe.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     4356 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/midiprobe.dsp
--rw-rw-r--   0 runner    (1001) docker     (123)     2361 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/qmidiin.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/qmidiin.dsp
--rw-rw-r--   0 runner    (1001) docker     (123)     3926 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/sysextest.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     4360 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/sysextest.dsp
--rw-rw-r--   0 runner    (1001) docker     (123)      667 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/testcapi.c
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/tests/
--rw-rw-r--   0 runner    (1001) docker     (123)     2922 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/tests/test_basic.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2484 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/tests/test_delete.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2100 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/tests/test_errorcallback.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2299 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/tests/test_errors.py
--rw-rw-r--   0 runner    (1001) docker     (123)     9256 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/tests/test_rtmidi.py
--rw-rw-r--   0 runner    (1001) docker     (123)      298 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/tox.ini
--rwxrwxr-x   0 runner    (1001) docker     (123)      346 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/update-docs.sh
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-14 06:50:52.266248 python-rtmidi-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0       94 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/.flake8
+-rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/.github/workflows/pr_to_master.yml
+-rw-r--r--   0        0        0     2603 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/.github/workflows/push_to_master.yml
+-rw-r--r--   0        0        0     2539 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/.gitignore
+-rw-r--r--   0        0        0      118 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/.gitmodules
+-rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/AUTHORS.md
+-rw-r--r--   0        0        0    22683 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/CHANGELOG.md
+-rw-r--r--   0        0        0     3849 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/INSTALL-windows.md
+-rw-r--r--   0        0        0     8891 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/INSTALL.md
+-rw-r--r--   0        0        0     2771 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/LICENSE.md
+-rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/MANIFEST.in
+-rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/Makefile
+-rw-r--r--   0        0        0     2802 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/README.md
+-rw-r--r--   0        0        0     6778 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/Makefile
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/api.rst.inc
+-rw-r--r--   0        0        0       31 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/authors.md
+-rwxr-xr-x   0        0        0     8521 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/conf.py
+-rw-r--r--   0        0        0     3436 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/contributing.rst
+-rw-r--r--   0        0        0       33 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/history.md
+-rw-r--r--   0        0        0      257 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/index.rst
+-rw-r--r--   0        0        0       39 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/install-windows.md
+-rw-r--r--   0        0        0       31 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/installation.md
+-rw-r--r--   0        0        0       31 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/license.md
+-rw-r--r--   0        0        0     6467 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/make.bat
+-rw-r--r--   0        0        0       55 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/modules.rst
+-rw-r--r--   0        0        0       30 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/readme.md
+-rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/rtmidi.rst
+-rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/usage.rst
+-rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/advanced/ccstore.py
+-rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/advanced/midiclock.py
+-rw-r--r--   0        0        0     8741 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/advanced/midioutwrapper.py
+-rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/advanced/recvrpn.py
+-rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/basic/contextmanager.py
+-rwxr-xr-x   0        0        0     1359 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/basic/midiin_callback.py
+-rwxr-xr-x   0        0        0     1050 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/basic/midiin_poll.py
+-rwxr-xr-x   0        0        0      991 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/basic/midiout.py
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/basic/noteon2osc.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/basic/panic.py
+-rwxr-xr-x   0        0        0     1571 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/basic/probe_ports.py
+-rw-r--r--   0        0        0     2195 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/README.rst
+-rw-r--r--   0        0        0      275 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/break-on-through.txt
+-rwxr-xr-x   0        0        0     6485 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/drumseq.py
+-rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_01.txt
+-rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_02.txt
+-rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_03.txt
+-rw-r--r--   0        0        0      206 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_04.txt
+-rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_05.txt
+-rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_06.txt
+-rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_07.txt
+-rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_08.txt
+-rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_09.txt
+-rw-r--r--   0        0        0      435 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_10.txt
+-rw-r--r--   0        0        0      299 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_11.txt
+-rw-r--r--   0        0        0      347 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_12.txt
+-rw-r--r--   0        0        0      157 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/funkydrummer.txt
+-rw-r--r--   0        0        0      205 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/rosanna-shuffle.txt
+-rw-r--r--   0        0        0      477 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/template.txt
+-rw-r--r--   0        0        0    45974 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midi2command/000-playback.mp3
+-rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midi2command/000-sheet.pdf
+-rw-r--r--   0        0        0     5624 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midi2command/README.rst
+-rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midi2command/example.cfg
+-rw-r--r--   0        0        0     7132 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midi2command/midi2command.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midifilter/__init__.py
+-rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midifilter/__main__.py
+-rw-r--r--   0        0        0     3119 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midifilter/filters.py
+-rwxr-xr-x   0        0        0     5328 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sendsysex.py
+-rw-r--r--   0        0        0     7155 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sequencer/sequencer.py
+-rwxr-xr-x   0        0        0      745 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sysex/send_sysex.py
+-rwxr-xr-x   0        0        0     1067 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sysex/send_sysex_file.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sysexsaver/__init__.py
+-rw-r--r--   0        0        0     7022 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sysexsaver/__main__.py
+-rw-r--r--   0        0        0    11493 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sysexsaver/manufacturers.csv
+-rw-r--r--   0        0        0    12337 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sysexsaver/manufacturers.py
+-rw-r--r--   0        0        0    12147 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sysexsaver/models.py
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/wavetablemodstep.py
+-rw-r--r--   0        0        0     3305 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/meson.build
+-rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/meson_options.txt
+-rwxr-xr-x   0        0        0      462 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/meson_postinstall.py
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0       91 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/requirements-dev.in
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/requirements-dev.txt
+-rw-r--r--   0        0        0      165 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/rtmidi/__init__.py
+-rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/rtmidi/meson.build
+-rw-r--r--   0        0        0     7533 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/rtmidi/midiconstants.py
+-rw-r--r--   0        0        0     9261 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/rtmidi/midiutil.py
+-rw-r--r--   0        0        0       30 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/rtmidi/version.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)   737312 2023-06-23 06:48:00.492697 python_rtmidi-1.5.3/src/_rtmidi.cpp
+-rw-r--r--   0        0        0    39588 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/_rtmidi.pyx
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/meson.build
+-rwxr-xr-x   0        0        0     1261 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/meson_dist_cython.py
+-rw-r--r--   0        0        0     9806 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/CMakeLists.txt
+-rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/LICENSE
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/Makefile.am
+-rw-r--r--   0        0        0     2396 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/README.md
+-rw-r--r--   0        0        0   126845 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/RtMidi.cpp
+-rw-r--r--   0        0        0    27079 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/RtMidi.h
+-rwxr-xr-x   0        0        0     2884 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/autogen.sh
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in
+-rw-r--r--   0        0        0      277 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/cmake/rtmidi-config.cmake.in
+-rw-r--r--   0        0        0     9307 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/configure.ac
+-rw-r--r--   0        0        0       59 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/contrib/go/rtmidi/go.mod
+-rw-r--r--   0        0        0    10504 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/contrib/go/rtmidi/rtmidi.go
+-rw-r--r--   0        0        0      125 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.cpp
+-rw-r--r--   0        0        0       31 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.h
+-rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/Makefile.am
+-rw-r--r--   0        0        0    81155 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/doxygen/Doxyfile.in
+-rw-r--r--   0        0        0      254 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/doxygen/footer.html
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/doxygen/header.html
+-rw-r--r--   0        0        0      173 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/doxygen/samples/getting_started.cpp
+-rw-r--r--   0        0        0    21717 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/doxygen/tutorial.txt
+-rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/images/ccrma.gif
+-rw-r--r--   0        0        0     4614 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/images/mcgill.gif
+-rw-r--r--   0        0        0     7130 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/release.txt
+-rw-r--r--   0        0        0    19367 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4
+-rw-r--r--   0        0        0      171 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/msw/readme
+-rwxr-xr-x   0        0        0      883 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/msw/rtmidilib.sln
+-rwxr-xr-x   0        0        0     3734 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/msw/rtmidilib.vcproj
+-rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/rtmidi-config.in
+-rw-r--r--   0        0        0      369 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/rtmidi.pc.in
+-rw-r--r--   0        0        0    10218 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/rtmidi_c.cpp
+-rw-r--r--   0        0        0     9532 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/rtmidi_c.h
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/Debug/.placeholder
+-rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/Makefile.am
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/Release/.placeholder
+-rw-r--r--   0        0        0     1311 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/RtMidi.dsw
+-rw-r--r--   0        0        0     5284 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/apinames.cpp
+-rw-r--r--   0        0        0     2873 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/cmidiin.cpp
+-rw-r--r--   0        0        0     4320 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/cmidiin.dsp
+-rw-r--r--   0        0        0     5541 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/midiclock.cpp
+-rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/midiout.cpp
+-rw-r--r--   0        0        0     4320 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/midiout.dsp
+-rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/midiprobe.cpp
+-rw-r--r--   0        0        0     4356 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/midiprobe.dsp
+-rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/qmidiin.cpp
+-rw-r--r--   0        0        0     4320 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/qmidiin.dsp
+-rw-r--r--   0        0        0     3926 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/sysextest.cpp
+-rw-r--r--   0        0        0     4360 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/sysextest.dsp
+-rw-r--r--   0        0        0      667 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/testcapi.c
+-rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/tests/test_basic.py
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/tests/test_ci_wheels.py
+-rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/tests/test_delete.py
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/tests/test_errorcallback.py
+-rw-r--r--   0        0        0     2276 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/tests/test_errors.py
+-rw-r--r--   0        0        0     7000 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/tests/test_rtmidi.py
+-rw-r--r--   0        0        0      298 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/tox.ini
+-rwxr-xr-x   0        0        0      346 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/update-docs.sh
+-rw-r--r--   0        0        0     7498 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/PKG-INFO
```

### Comparing `python-rtmidi-1.5.2/.github/workflows/pr_to_master.yml` & `python_rtmidi-1.5.3/.github/workflows/pr_to_master.yml`

 * *Files 21% similar despite different names*

```diff
@@ -3,33 +3,38 @@
 on:
   pull_request:
     branches:
       - master
 
 jobs:
   build_sdist:
-   name: Build sdist
-   runs-on: ubuntu-latest
-   steps:
+    name: Build sdist
+    runs-on: ubuntu-latest
+    steps:
+
+    - uses: actions/checkout@v3
+      with:
+        submodules: true
 
-   - uses: actions/checkout@v3
-     with:
-       submodules: true
+    - name: Install ninja
+      run: pipx install ninja
 
-   - name: Install ninja
-     run: pipx install ninja
+    - name: Install alsa deps
+      run: sudo apt-get install libasound2-dev
 
-   - name: Install alsa deps
-     run: sudo apt-get install libasound2-dev
+    - name: Build sdist
+      run: pipx run build --sdist
 
-   - name: Build sdist
-     run: pipx run build --sdist
+    - name: Check metadata
+      run: pipx run twine check --strict dist/*
 
-   - name: Check metadata
-     run: pipx run twine check --strict dist/*
+    - name: Upload sdist
+      uses: actions/upload-artifact@v3
+      with:
+        path: dist/*.tar.gz
 
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: true
       matrix:
@@ -40,33 +45,46 @@
       with:
         submodules: true
 
     - uses: ilammy/msvc-dev-cmd@v1
       if: matrix.os == 'windows-latest'
 
     - name: Build wheels
-      uses: pypa/cibuildwheel@v2.12.3
+      uses: pypa/cibuildwheel@v2.13
+      env:
+        # Skip trying to test arm64 builds on Intel Macs
+        CIBW_TEST_SKIP: "*-macosx_arm64 *-macosx_universal2:arm64"
+
+    - name: Upload wheels
+      uses: actions/upload-artifact@v3
+      with:
+        path: wheelhouse/*.whl
 
   build_arch_wheels:
-   name: Build wheels on Linux ${{ matrix.arch }}
-   runs-on: ubuntu-20.04
-   strategy:
-     matrix:
-       arch: [aarch64]
-   steps:
-
-   - uses: actions/checkout@v3
-     with:
-       submodules: true
-
-   - uses: docker/setup-qemu-action@v2
-     with:
-       platforms: all
-
-   - uses: pypa/cibuildwheel@v2.12.3
-     env:
-       CIBW_ARCHS: ${{ matrix.arch }}
-
-   - name: Verify clean directory
-     run: git diff --exit-code
-     shell: bash
+    name: Build wheels on Linux ${{ matrix.arch }}
+    runs-on: ubuntu-20.04
+    strategy:
+      matrix:
+        arch: [aarch64]
+    steps:
+
+    - uses: actions/checkout@v3
+      with:
+        submodules: true
 
+    - uses: docker/setup-qemu-action@v2
+      with:
+        platforms: all
+
+    - name: Build wheels
+      uses: pypa/cibuildwheel@v2.13
+      env:
+        CIBW_ARCHS: ${{ matrix.arch }}
+
+    - name: Verify clean directory
+      run: git diff --exit-code
+      shell: bash
+
+    - name: Upload wheels
+      uses: actions/upload-artifact@v3
+      with:
+        path: wheelhouse/*.whl
```

### Comparing `python-rtmidi-1.5.2/.github/workflows/push_to_master.yml` & `python_rtmidi-1.5.3/.github/workflows/release.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,107 +1,112 @@
-name: Build sdist and wheels and publish to TestPyPI
+name: Build sdist and wheels and publish to PyPI
 
 on:
-  push:
-    branches:
-      - master
+  release:
+    types:
+      - published
+  workflow_dispatch:
+
+permissions:
+  id-token: write # This is required for requesting the JWT
 
 jobs:
   build_sdist:
-   name: Build sdist
-   runs-on: ubuntu-latest
-   steps:
+    name: Build sdist
+    runs-on: ubuntu-latest
+    steps:
 
-   - uses: actions/checkout@v3
-     with:
-       submodules: true
+    - uses: actions/checkout@v3
+      with:
+        submodules: true
 
-   - name: Install ninja
-     run: pipx install ninja
+    - name: Install ninja
+      run: pipx install ninja
 
-   - name: Install alsa deps
-     run: sudo apt-get install libasound2-dev
+    - name: Install alsa deps
+      run: sudo apt-get install libasound2-dev
 
-   - name: Build sdist
-     run: pipx run build --sdist
+    - name: Build sdist
+      run: pipx run build --sdist
 
-   - name: Check metadata
-     run: pipx run twine check --strict dist/*
+    - name: Check metadata
+      run: pipx run twine check --strict dist/*
 
-   - uses: actions/upload-artifact@v3
-     with:
-       path: dist/*.tar.gz
+    - name: Upload sdist
+      uses: actions/upload-artifact@v3
+      with:
+        path: dist/*.tar.gz
 
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
-      fail-fast: true
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
     steps:
 
     - uses: actions/checkout@v3
       with:
         submodules: true
 
     - uses: ilammy/msvc-dev-cmd@v1
       if: matrix.os == 'windows-latest'
 
     - name: Build wheels
-      uses: pypa/cibuildwheel@v2.12.3
+      uses: pypa/cibuildwheel@v2.13
+      env:
+        # Skip trying to test arm64 builds on Intel Macs
+        CIBW_TEST_SKIP: "*-macosx_arm64 *-macosx_universal2:arm64"
 
-    - uses: actions/upload-artifact@v3
+    - name: Upload wheels
+      uses: actions/upload-artifact@v3
       with:
         path: wheelhouse/*.whl
 
   build_arch_wheels:
-   name: Build wheels on Linux ${{ matrix.arch }}
-   runs-on: ubuntu-20.04
-   strategy:
-     matrix:
-       arch: [aarch64]
-   steps:
-
-   - uses: actions/checkout@v3
-     with:
-       submodules: true
-
-   - uses: docker/setup-qemu-action@v2
-     with:
-       platforms: all
-
-   - uses: pypa/cibuildwheel@v2.12.3
-     env:
-       CIBW_ARCHS: ${{ matrix.arch }}
-
-   - name: Verify clean directory
-     run: git diff --exit-code
-     shell: bash
-
-   - name: Upload wheels
-     uses: actions/upload-artifact@v3
-     with:
-       path: wheelhouse/*.whl
+    name: Build wheels on Linux ${{ matrix.arch }}
+    runs-on: ubuntu-20.04
+    strategy:
+      matrix:
+        arch: [aarch64]
+    steps:
+
+    - uses: actions/checkout@v3
+      with:
+        submodules: true
+
+    - uses: docker/setup-qemu-action@v2
+      with:
+        platforms: all
+
+    - name: Build wheels
+      uses: pypa/cibuildwheel@v2.13
+      env:
+        CIBW_ARCHS: ${{ matrix.arch }}
+
+    - name: Verify clean directory
+      run: git diff --exit-code
+      shell: bash
+
+    - name: Upload wheels
+      uses: actions/upload-artifact@v3
+      with:
+        path: wheelhouse/*.whl
 
   upload_pypi:
-   needs: [build_arch_wheels, build_wheels, build_sdist]
-   runs-on: ubuntu-latest
-   environment: PyPI release
-   if: github.ref == 'refs/heads/develop'
-   steps:
-   - uses: actions/download-artifact@v3
-     with:
-       # unpacks default artifact into dist/
-       # if `name: artifact` is omitted, the action will create extra parent dir
-       name: artifact
-       path: dist
-
-   - name: Publish distribution to Test PyPI
-     uses: pypa/gh-action-pypi-publish@v1.8.6
-     with:
-       skip_existing: true
-       user: __token__
-       password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-       repository_url: https://test.pypi.org/legacy/
-       verify-metadata: false
+    needs: [build_arch_wheels, build_wheels, build_sdist]
+    runs-on: ubuntu-latest
+    environment: PyPI release
+    steps:
+    - uses: actions/download-artifact@v3
+      with:
+        # unpacks default artifact into dist/
+        # if `name: artifact` is omitted, the action will create extra parent dir
+        name: artifact
+        path: dist
 
+    - name: Publish distribution to PyPI
+      uses: pypa/gh-action-pypi-publish@v1.8.6
+      with:
+        user: __token__
+        password: ${{ secrets.PYPI_API_TOKEN }}
+        verify-metadata: false
```

### Comparing `python-rtmidi-1.5.2/.github/workflows/release.yml` & `python_rtmidi-1.5.3/.github/workflows/push_to_master.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,106 +1,113 @@
-name: Build sdist and wheels and publish to PyPI
+name: Build sdist and wheels and publish to TestPyPI
 
 on:
-  release:
-    types:
-      - published
-  workflow_dispatch:
-
-permissions:
-  id-token: write # This is required for requesting the JWT
+  push:
+    branches:
+      - master
 
 jobs:
   build_sdist:
-   name: Build sdist
-   runs-on: ubuntu-latest
-   steps:
+    name: Build sdist
+    runs-on: ubuntu-latest
+    steps:
 
-   - uses: actions/checkout@v3
-     with:
-       submodules: true
+    - uses: actions/checkout@v3
+      with:
+        submodules: true
 
-   - name: Install ninja
-     run: pipx install ninja
+    - name: Install ninja
+      run: pipx install ninja
 
-   - name: Install alsa deps
-     run: sudo apt-get install libasound2-dev
+    - name: Install alsa deps
+      run: sudo apt-get install libasound2-dev
 
-   - name: Build sdist
-     run: pipx run build --sdist
+    - name: Build sdist
+      run: pipx run build --sdist
 
-   - name: Check metadata
-     run: pipx run twine check --strict dist/*
+    - name: Check metadata
+      run: pipx run twine check --strict dist/*
 
-   - uses: actions/upload-artifact@v3
-     with:
-       path: dist/*.tar.gz
+    - name: Upload sdist
+      uses: actions/upload-artifact@v3
+      with:
+        path: dist/*.tar.gz
 
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
+      fail-fast: true
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
     steps:
 
     - uses: actions/checkout@v3
       with:
         submodules: true
 
     - uses: ilammy/msvc-dev-cmd@v1
       if: matrix.os == 'windows-latest'
 
     - name: Build wheels
-      uses: pypa/cibuildwheel@v2.12.3
+      uses: pypa/cibuildwheel@v2.13
+      env:
+        # Skip trying to test arm64 builds on Intel Macs
+        CIBW_TEST_SKIP: "*-macosx_arm64 *-macosx_universal2:arm64"
 
-    - uses: actions/upload-artifact@v3
+    - name: Upload wheels
+      uses: actions/upload-artifact@v3
       with:
         path: wheelhouse/*.whl
 
   build_arch_wheels:
-   name: Build wheels on Linux ${{ matrix.arch }}
-   runs-on: ubuntu-20.04
-   strategy:
-     matrix:
-       arch: [aarch64]
-   steps:
-
-   - uses: actions/checkout@v3
-     with:
-       submodules: true
-
-   - uses: docker/setup-qemu-action@v2
-     with:
-       platforms: all
-
-   - uses: pypa/cibuildwheel@v2.12.3
-     env:
-       CIBW_ARCHS: ${{ matrix.arch }}
-
-   - name: Verify clean directory
-     run: git diff --exit-code
-     shell: bash
-
-   - name: Upload wheels
-     uses: actions/upload-artifact@v3
-     with:
-       path: wheelhouse/*.whl
+    name: Build wheels on Linux ${{ matrix.arch }}
+    runs-on: ubuntu-20.04
+    strategy:
+      matrix:
+        arch: [aarch64]
+    steps:
+
+    - uses: actions/checkout@v3
+      with:
+        submodules: true
+
+    - uses: docker/setup-qemu-action@v2
+      with:
+        platforms: all
+
+    - name: Build wheels
+      uses: pypa/cibuildwheel@v2.13
+      env:
+        CIBW_ARCHS: ${{ matrix.arch }}
+
+    - name: Verify clean directory
+      run: git diff --exit-code
+      shell: bash
+
+    - name: Upload wheels
+      uses: actions/upload-artifact@v3
+      with:
+        path: wheelhouse/*.whl
 
   upload_pypi:
-   needs: [build_arch_wheels, build_wheels, build_sdist]
-   runs-on: ubuntu-latest
-   environment: PyPI release
-   steps:
-   - uses: actions/download-artifact@v3
-     with:
-       # unpacks default artifact into dist/
-       # if `name: artifact` is omitted, the action will create extra parent dir
-       name: artifact
-       path: dist
-
-   - name: Publish distribution to PyPI
-     uses: pypa/gh-action-pypi-publish@v1.8.6
-     with:
-       user: __token__
-       password: ${{ secrets.PYPI_API_TOKEN }}
-       verify-metadata: false
+    needs: [build_arch_wheels, build_wheels, build_sdist]
+    runs-on: ubuntu-latest
+    environment: PyPI release
+    if: github.ref == 'refs/heads/develop'
+    steps:
+
+    - uses: actions/download-artifact@v3
+      with:
+        # unpacks default artifact into dist/
+        # if `name: artifact` is omitted, the action will create extra parent dir
+        name: artifact
+        path: dist
+
+    - name: Publish distribution to Test PyPI
+      uses: pypa/gh-action-pypi-publish@v1.8.6
+      with:
+        skip_existing: true
+        user: __token__
+        password: ${{ secrets.TEST_PYPI_API_TOKEN }}
+        repository_url: https://test.pypi.org/legacy/
+        verify-metadata: false
```

### Comparing `python-rtmidi-1.5.2/.gitignore` & `python_rtmidi-1.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/CHANGELOG.md` & `python_rtmidi-1.5.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,47 @@
 # Changelog
 
 For details and minor changes, please see the [version control log
 messages](https://github.com/SpotlightKid/python-rtmidi/commits/master).
 
+## Development
+
+Changes:
+
+-   Updated `rtmidi` submodule (#156).
+
+Documentation:
+
+-   Updated installation documentation (#165).
+-   Updated contributing guide (#165).
+-   Removed Python 3.7 from meta-data classifiers in `pyproject.toml`(dfb3800).
+
+Project infrastructure:
+
+-   Changed the build back-end to meson-python (#161).
+-   Fixed broken macOS arm64 binary wheels built by CI (#161).
+-   Fixed missing JACK backend API support in Linux aarch64 binary wheels built
+    by CI (#161).
+-   Improved tests for binary wheels built by CI (#162).
+-   Cleaned up GitHub actions workflow definitions (#163).
+-   Fixed test coverage report target in Makefile (#164).
+
+
+## 1.5.2 (2023-06-14)
+
+Changes:
+
+-   Updated `rtmidi` submodule (#156).
+
+Project infrastructure:
+
+-   Updated `requirements-dev.txt` with `pip-compile` (#153).
+-   Changed CI to build separate wheels for both macOS architectures (18bbc74, 20f5cdd).
+-   Improved build dependency selection in meson config (#156).
+
 
 ## 1.5.1 (2023-06-12)
 
 Project infrastructure:
 
 -   Fixed broken windows binary wheels built by CI.
 
@@ -40,15 +75,15 @@
 
 -   Fixed Windows build for 64-bit Python 3.9 on AppVeyor CI.
 
 Changes:
 
 -   The SysEx reception buffer size for the Windows MM backend was
     changed from 8096 to 8196.
-s-   Synced with upstream [RtMidi](https://github.com/thestk/rtmidi)
+-   Synced with upstream [RtMidi](https://github.com/thestk/rtmidi)
     (3dc525baf3cac345cdd3511316571c20b47f30b5, fixes #89).
 
 
 ## 1.4.8 (2021-04-26)
 
 Fixes:
```

### Comparing `python-rtmidi-1.5.2/INSTALL-windows.md` & `python_rtmidi-1.5.3/INSTALL-windows.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # How to install python-rtmidi from source on Windows
 
 These instructions should work for installing `python-rtmidi` from source with
-Python 3.7+ in the 64-bit or 32-bit versions (you can run the latter on Windows
+Python 3.8+ in the 64-bit or 32-bit versions (you can run the latter on Windows
 64-bit versions with no problems).
 
 Please follow all the steps below in the exact order.
 
 ## Installing required software
 
 You probably need administrator rights for some or all of the following steps.
 
 1.  Install the latest release of Python (3.11 at the time of writing, at least
-    3.7+) from <https://www.python.org/downloads/windows/> to the default
+    3.8+) from <https://www.python.org/downloads/windows/> to the default
     location (e.g. `C:\Python311`). You can install either or both the 32-bit
     and the 64-bit version.
 
     In the installer, enable the option to install [pip]. Optionally, *for only
     one of the chosen Python versions*, enable the options to add the
     installation directory to your `PATH` and set it as the system's default
     version. Also enable the option to install the `py` helper script (only
```

### Comparing `python-rtmidi-1.5.2/INSTALL.md` & `python_rtmidi-1.5.3/INSTALL.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Installation
 
 **python-rtmidi** uses a modern [PEP 517] compliant Python build system based
-on [meson] and [mesonpep517] and can be installed from the Python Package Index
+on [meson] and [meson-python] and can be installed from the Python Package Index
 via [pip]. Since it is a Python C(++)-extension, a C++ compiler and build
 environment as well as some system-dependent libraries are needed to install,
 unless wheel packages with pre-compiled binaries are available for your system.
 See the [Requirements] section below for details.
 
 
 ## From PyPI
@@ -36,122 +36,152 @@
 If you want to pass options to the build process, you need to compile
 python-rtmidi from source manually. See the [From Source](#from-source) section
 below for moe information.
 
 
 ## Pre-compiled Binaries
 
-Pre-compiled binary wheels of the latest python-rtmidi version for Windows and
-macOS / OS X are available on PyPI for several major Python versions. If you
+Pre-compiled binary wheels of the latest python-rtmidi version for Windows,
+macOS and Linux are available on PyPI for all supported Python versions. If you
 install python-rtmidi via pip (see above), these wheels will be selected by pip
-automatically, if you have a compatible Python and Windows or macOS version.
+automatically, if you have a compatible Python and OS version and processor
+architecture.
 
-The Windows binary wheels are compiled with Windows MultiMedia API support and
-are available in 32-bit and 64-bit versions. The macOS / OS X binary wheels are
-compiled with CoreMIDI support and are only available in 64-bit versions for OS
-X 10.6 and later. If you need JACK support on OS X, you need to compile
-python-rtmidi yourself (see the [macOS] section below for details).
+* Windows binary wheels are compiled with Windows MultiMedia API support and
+  are available for x86_64 (aka amd64).
 
+* macOS / OS X binary wheels are compiled with CoreMIDI support and are
+  available for OS X intel (10.9+) and arm64 (aka M1/M2/Apple silicon, 11.0+).
 
-## From Source
-
-To compile python-rtmidi from source and install it manually without pip, you
-can either download a source distribution archive or check out the sources from
-the Git repository.
-
-While the steps to get the sources differ, the actual compilation and
-installation steps consist of the same standard meson commands in both cases:
+  If you need JACK support on OS X, you need to compile python-rtmidi yourself
+  (see the [macOS] section below for details).
 
-```console
-meson setup --prefix=/usr --buildtype=plain builddir
-meson compile -C builddir
-meson install -C builddir
-```
+* Linux binary wheels are available for x64_64 and aarch64,
 
-The `meson setup` command recognizes several options to control which
-OS-dependent MIDI backends will be supported by the python-rtmidi extension
-binary it produces, plus other options to control compilation of the RtMidi C++
-library:
 
-|  Option            | Linux | macOS | Windows | Note                                                     |
-| ------------------ | ----- | ----- | ------- | -------------------------------------------------------- |
-| `-Dalsa=false`     | x     | n/a   | n/a     | Don't compile in support for ALSA backend.               |
-| `-Djack=false`     | x     | x     | n/a     | Don't compile in support for JACK backend.               |
-| `-Dcoremidi=false` | n/a   | x     | n/a     | Don't compile in support for CoreMIDI backend.           |
-| `-Dwinmm=false`    | n/a   | n/a   | x       | Don't compile in support for Windows MultiMedia backend. |
-| `-Dverbose=true`   | x     | x     | x       | Don't suppress RtMidi warnings to stderr.                |
+## From Source
 
-Support for each OS dependent MIDI backend is only enabled when the required
-library and header files are actually present on the system.
+To compile python-rtmidi from source and install it manually without pip, you
+can either download a source distribution archive or check out the sources from
+the Git repository. While the steps to get the sources differ, the actual
+compilation and installation steps consist of the same commands in both cases.
 
 
 ### From the Source Distribution
 
 To download the python-rtmidi source distribution archive for the current
-version, extract and install it, use the following commands:
+version and extract it, use the following commands:
 
 ```console
 pip download python-rtmidi
 tar -xzf python-rtmidi-1.X.Y.tar.gz
 cd python-rtmidi-1.X.Y
-meson setup --prefix=/usr --buildtype=plain builddir
-meson compile -C builddir
-meson install -C builddir
 ```
 
-On Linux or macOS / OS X, if you want to install python-rtmidi into the
-system-wide Python library directory, you may have to prefix the last command
-with `sudo`, e.g.:
+Then follow the commands shown in the section [buildinstall].
+
+
+### From the Source Code Repository
+
+Alternatively, you can check out the python-rtmidi source code from the Git
+repository and then install it from your working copy.
 
 ```console
-sudo meson install -C builddir
+(rtmidi)$ git clone --recursive https://github.com/SpotlightKid/python-rtmidi.git
+(rtmidi)$ cd python-rtmidi
 ```
 
-The recommended way, though, is to install python-rtmidi only for your current
-user (which `installer` does by default) or into a virtual environment:
+Then follow the commands shown in the section [buildinstall].
+
+
+(buildinstall)=
+### Build and Install
+
+#### Using the PEP 517 build method (recommended)
+
+The recommended way is to build python-rtmidi via the standard PEP 517 build
+method and install it only for your current user (which `installer` does by
+default) or into a virtual environment.
+
+If you don't already have the `build` and `installer` Python packages
+installed, install them with:
 
 ```console
+pip install build installer
+```
+
+Then build and install python-rtmidi:
+
+```console
+python -m build --wheel
 python -m installer dist/*.whl
 ```
 
+This will download all the required build tools, install them in a temporary
+virtual environment, build a wheel, and install it.
 
-### From the Source Code Repository
 
-Alternatively, you can check out the python-rtmidi source code from the Git
-repository and then install it from your working copy. Since the repository
-does not include the C++ module source code pre-compiled from the Cython
-source, you'll also need to install Cython >= 0.28, either via pip or from its
-Git repository. Using virtualenv / virtualenvwrapper is strongly recommended in
-this scenario:
+### Using meson directly
+
+If you can't or don't want to use the standard PEP 517 build method, you can
+also use meson directly, but then you'll need to make sure all the required
+build tools are installed.
+
+If you are installing from a Git repository checkout, since this does not
+include the C++ module source code pre-compiled from the Cython source, you'll
+also need to install Cython >= 0.29, either via pip or from its Git repository.
+Using virtualenv / virtualenvwrapper is strongly recommended in this scenario:
 
 Make a virtual environment:
 
 ```console
 mkvirtualenv rtmidi
 (rtmidi)$ cdvirtualenv
 ```
 
-Install Cython from PyPI:
+Install meson and ninja and, if neccessary, Cython from PyPI:
+
+```console
+(rtmidi)$ pip install Cython meson ninja
+```
 
 ```console
-(rtmidi)$ pip install Cython meson ninja wheel
+meson setup --prefix=/usr -Dbuildtype=plain builddir
+meson compile -C builddir
+meson install -C builddir
 ```
 
-Then install python-rtmidi:
+On Linux or macOS, if you want to install python-rtmidi into the system-wide
+Python library directory, you may have to prefix the last command with `sudo`,
+e.g.:
 
 ```console
-(rtmidi)$ git clone --recursive https://github.com/SpotlightKid/python-rtmidi.git
-(rtmidi)$ cd python-rtmidi
-(rtmidi)$ meson setup --prefix=/usr --buildtype=plain builddir
-(rtmidi)$ meson compile -C builddir
-(rtmidi)$ meson install -C builddir
+sudo meson install -C builddir
 ```
 
+The `meson setup` command recognizes several options to control which
+OS-dependent MIDI backends will be supported by the python-rtmidi extension
+binary it produces, plus other options to control compilation of the RtMidi C++
+library:
+
+|  Option            | Linux | macOS | Windows | Note                                                     |
+| ------------------ | ----- | ----- | ------- | -------------------------------------------------------- |
+| `-Dalsa=false`     | x     | n/a   | n/a     | Don't compile in support for ALSA backend.               |
+| `-Djack=false`     | x     | x     | n/a     | Don't compile in support for JACK backend.               |
+| `-Dcoremidi=false` | n/a   | x     | n/a     | Don't compile in support for CoreMIDI backend.           |
+| `-Dwinmm=false`    | n/a   | n/a   | x       | Don't compile in support for Windows MultiMedia backend. |
+| `-Dverbose=true`   | x     | x     | x       | Don't suppress RtMidi warnings to stderr.                |
+| `-Dpython=python3` | x     | x     | x       | Set name (or path) of Python interpreter.                |
+
+Support for each OS dependent MIDI backend is only enabled when the required
+library and header files are actually present on the system.
+
+
 (requirements)=
-#### Requirements
+## Requirements
 
 Naturally, you'll need a C++ compiler and a build environment. See the
 platform-specific hints below.
 
 If you want to change the Cython source file `_rtmidi.pyx` or want to recompile
 `_rtmidi.cpp` with a newer Cython version, you'll need to install Cython.
 
@@ -162,15 +192,15 @@
 appropriate compilations flags automatically.
 
 -   Linux: ALSA, JACK
 -   macOS (OS X): CoreMIDI, JACK
 -   Windows: MultiMedia (MM)
 
 
-## Linux
+### Linux
 
 First you need a C++ compiler and the pthread library. Install the
 `build-essential` package on debian-based systems to get these.
 
 Then you'll need Python development headers and libraries. On debian-based
 systems, install the `python-dev` package. If you use the official installers
 from python.org you should already have these.
@@ -178,47 +208,38 @@
 To get ALSA support, you must install development files for the `libasound2`
 library (debian package: `libasound2-dev`). For JACK support, install the
 `libjack` development files (if you are using Jack1, install `libjack-dev`, if
 you are using Jack2, install `libjack-jackd2-dev`).
 
 
 (macos)=
-## macOS (OS X)
+### macOS (OS X)
 
 Install the latest Xcode version or `g++` from MacPorts or homebrew (untested).
-CoreMIDI support comes with installing Xcode. For JACK support, install
-[JackOSX] with the installer or build JACK from source.
-
-**Note:**
-
-*If you have a very old version of OS X and Xcode which still supports building
-binaries for PPC, you'll have to tell distribute to build the package only for
-i386 and x86_64 architectures:*
-
-```console
-env ARCHFLAGS=\"-arch i386 -arch x86_64\" python setup.py install
-```
+CoreMIDI support comes with installing Xcode. For JACK support, install JACK
+with the [macOS installer] provided on the JACK web site or build JACK from
+source.
 
 
-## Windows
+### Windows
 
 Please see the detailed instructions for Windows in `install-windows`.
 
 
 ## User Contributed Documentation
 
 The python-rtmidi wiki on GitHub contains some [user contributed documentation]
 for additional installation scenarios. Please check these, if you have trouble
 installing python-rtmidi in an uncommon or not-yet-covered environment.
 
 
 [Cython]: http://cython.org/
-[JackOSX]: http://jackaudio.org/downloads/
+[macOS installer]: http://jackaudio.org/downloads/
 [meson]: https://mesonbuild.com/
-[mesonpep517]: https://thiblahute.gitlab.io/mesonpep517/
+[meson-python]: https://github.com/mesonbuild/meson-python
 [pep 517]: https://peps.python.org/pep-0517/
 [pip]: https://pypi.python.org/pypi/pip
 [PyPI page]: http://python.org/pypi/python-rtmidi#downloads
 [setuptools]: https://pypi.python.org/pypi/setuptools
 [user contributed documentation]: https://github.com/SpotlightKid/python-rtmidi/wiki/User-contributed-documentation
 [virtualenv]: https://pypi.python.org/pypi/virtualenv
 [virtualenvwrapper]: http://www.doughellmann.com/projects/virtualenvwrapper/
```

### Comparing `python-rtmidi-1.5.2/LICENSE.md` & `python_rtmidi-1.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/Makefile` & `python_rtmidi-1.5.3/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 	@echo "release - package a release"
 	@echo "release_upload - package a release and upload it to PyPI"
 	@echo "requirements - generate 'requirement-dev.txt' from 'requirements-dev.in'"
 	@echo "test - run tests on every supported Python version with tox"
 
 build: $(SOURCES)
 	if [[ -d "$(BUILDDIR)" ]]; then \
-		meson setup --reconfigure "--prefix=$(PREFIX)" --buildtype=plain $(BUILDDIR); \
+		meson setup --reconfigure "--prefix=$(PREFIX)" -Dbuildtype=plain $(BUILDDIR); \
 	else \
-		meson setup "--prefix=$(PREFIX)" --buildtype=plain $(BUILDDIR); \
+		meson setup "--prefix=$(PREFIX)" -Dbuildtype=plain $(BUILDDIR); \
 	fi
 	meson compile -C $(BUILDDIR)
 
 check-docs:
 	$(PYTHON) -m pydocstyle rtmidi
 
 clean: clean-build clean-docs clean-pyc
@@ -45,18 +45,21 @@
 
 clean-pyc:
 	find . -name '*.pyc' -exec rm -f {} +
 	find . -name '*.pyo' -exec rm -f {} +
 	find . -name '*~' -exec rm -f {} +
 	find . -name __pycache__ -type d -exec rm -rf {} +
 
-coverage:
-	$(PYTHON) -mcoverage run --source rtmidi test
-	$(PYTHON) -mcoverage report -m
-	$(PYTHON) -mcoverage html
+coverage: build
+	cp -f $(BUILDDIR)/rtmidi/_rtmidi.*.so rtmidi/
+	cp -f $(BUILDDIR)/rtmidi/version.py rtmidi/
+	$(PYTHON) -m coverage run --source rtmidi -m pytest tests
+	$(PYTHON) -m coverage report -m
+	$(PYTHON) -m coverage html
+	-rm -f rtmidi/*.so rtmidi/version.py
 	-xdg-open htmlcov/index.html
 
 dist: clean release
 	ls -l dist
 
 docs: build
 	cp -f $(BUILDDIR)/rtmidi/_rtmidi.*.so rtmidi/
```

### Comparing `python-rtmidi-1.5.2/README.md` & `python_rtmidi-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/docs/Makefile` & `python_rtmidi-1.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/docs/api.rst.inc` & `python_rtmidi-1.5.3/docs/api.rst.inc`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/docs/conf.py` & `python_rtmidi-1.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/docs/contributing.rst` & `python_rtmidi-1.5.3/docs/contributing.rst`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 * Detailed steps to reproduce the bug.
 
 
 Fix Bugs
 ~~~~~~~~
 
 Look through the GitHub issues for bugs. Anything tagged with "bug" is open to
-whoever wants to implement it.
+whoever wants to fix it.
 
 
 Implement Features
 ~~~~~~~~~~~~~~~~~~
 
 Look through the GitHub issues for features. Anything tagged with "feature" is
 open to whoever wants to implement it.
@@ -68,35 +68,38 @@
 
 1. Fork the ``python-rtmidi`` repo on GitHub.
 2. Clone your fork locally::
 
     $ git clone --recursive git@github.com:your_name_here/python-rtmidi.git
 
 3. Install your local copy into a virtualenv. Assuming you have
-   virtualenvwrapper installed, this is how you set up your fork for local
+   ``virtualenvwrapper`` installed, this is how you set up your fork for local
    development::
 
     $ mkvirtualenv python-rtmidi
     $ cd python-rtmidi/
     $ pip install -r requirements-dev.txt
-    $ python setup.py develop
+    $ python -m pip install .
 
 4. Create a branch for local development::
 
     $ git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
-5. When you're done making changes, check that your changes pass flake8 and the
-   tests, including testing other Python versions with tox::
+5. When you're done making changes, make sure that your changes pass the
+   ``flake8`` checks and the unit tests, also testing other Python versions
+   with ``tox``::
 
     $ make lint
     $ make test
 
-   To get flake8 and tox, just ``pip install`` them into your virtualenv.
+   ``flake8`` and ``tox`` shoudl have been installed via the requirements
+   file used in the instructions above. Should you use a different setup, make
+   sure you ``pip install`` them into your current Python environment.
 
 6. Commit your changes and push your branch to GitHub::
 
     $ git add .
     $ git commit -m "Detailed description of your changes."
     $ git push -u origin name-of-your-bugfix-or-feature
 
@@ -109,15 +112,15 @@
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the release notes in ``CHANGELOG.rst``.
 3. The pull request should work for all supported Python 3 versions (see
-   classifiers in ``setup.cfg``)
+   classifiers in ``pyproject.toml``)
 
    Run ``tox`` to make sure that the tests pass for all supported Python
    versions.
 
 
 Tips
 ----
```

### Comparing `python-rtmidi-1.5.2/docs/make.bat` & `python_rtmidi-1.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/docs/rtmidi.rst` & `python_rtmidi-1.5.3/docs/rtmidi.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/docs/usage.rst` & `python_rtmidi-1.5.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/advanced/ccstore.py` & `python_rtmidi-1.5.3/examples/advanced/ccstore.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/advanced/midiclock.py` & `python_rtmidi-1.5.3/examples/advanced/midiclock.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/advanced/midioutwrapper.py` & `python_rtmidi-1.5.3/examples/advanced/midioutwrapper.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/advanced/recvrpn.py` & `python_rtmidi-1.5.3/examples/advanced/recvrpn.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/basic/contextmanager.py` & `python_rtmidi-1.5.3/examples/basic/contextmanager.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/basic/midiin_callback.py` & `python_rtmidi-1.5.3/examples/basic/midiin_callback.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/basic/midiin_poll.py` & `python_rtmidi-1.5.3/examples/basic/midiin_poll.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/basic/midiout.py` & `python_rtmidi-1.5.3/examples/basic/midiout.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/basic/noteon2osc.py` & `python_rtmidi-1.5.3/examples/basic/noteon2osc.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/basic/panic.py` & `python_rtmidi-1.5.3/examples/basic/panic.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/basic/probe_ports.py` & `python_rtmidi-1.5.3/examples/basic/probe_ports.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/drumseq/README.rst` & `python_rtmidi-1.5.3/examples/drumseq/README.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/drumseq/drumseq.py` & `python_rtmidi-1.5.3/examples/drumseq/drumseq.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/midi2command/000-playback.mp3` & `python_rtmidi-1.5.3/examples/midi2command/000-playback.mp3`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/midi2command/000-sheet.pdf` & `python_rtmidi-1.5.3/examples/midi2command/000-sheet.pdf`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/midi2command/README.rst` & `python_rtmidi-1.5.3/examples/midi2command/README.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/midi2command/example.cfg` & `python_rtmidi-1.5.3/examples/midi2command/example.cfg`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/midi2command/midi2command.py` & `python_rtmidi-1.5.3/examples/midi2command/midi2command.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/midifilter/__main__.py` & `python_rtmidi-1.5.3/examples/midifilter/__main__.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/midifilter/filters.py` & `python_rtmidi-1.5.3/examples/midifilter/filters.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/sendsysex.py` & `python_rtmidi-1.5.3/examples/sendsysex.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/sequencer/sequencer.py` & `python_rtmidi-1.5.3/examples/sequencer/sequencer.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/sysex/send_sysex.py` & `python_rtmidi-1.5.3/examples/sysex/send_sysex.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/sysex/send_sysex_file.py` & `python_rtmidi-1.5.3/examples/sysex/send_sysex_file.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/sysexsaver/__main__.py` & `python_rtmidi-1.5.3/examples/sysexsaver/__main__.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/sysexsaver/manufacturers.csv` & `python_rtmidi-1.5.3/examples/sysexsaver/manufacturers.csv`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/sysexsaver/manufacturers.py` & `python_rtmidi-1.5.3/examples/sysexsaver/manufacturers.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/sysexsaver/models.py` & `python_rtmidi-1.5.3/examples/sysexsaver/models.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/examples/wavetablemodstep.py` & `python_rtmidi-1.5.3/examples/wavetablemodstep.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/meson.build` & `python_rtmidi-1.5.3/meson.build`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 project(
     'python-rtmidi',
     'cpp',
-    version: '1.5.2',
+    version: '1.5.3',
     license: 'MIT',
     default_options: [
-        'warning_level=2'
+        'warning_level=2',
+        'cpp_std=c++11'
     ],
-    meson_version: '>=0.63.0'
+    meson_version: '>=0.64.0'
 )
 
+message('Host machine system:', host_machine.system())
+
 cpp = meson.get_compiler('cpp')
 
 # Jack API (portable)
 jack2_dep = dependency('jack', version: '>=1.9.11', required: false)
 jack1_dep = dependency('jack', version: ['>=0.125.0', '<1.0'], required: false)
 
 if not jack2_dep.found() and jack1_dep.found()
@@ -24,15 +27,15 @@
     jack_dep = disabler()
 endif
 
 jack_not_found = jack_dep.found() ? false : true
 
 ## From https://github.com/numpy/numpy/blob/main/numpy/meson.build
 # Platform dependent config
-if host_machine.system() == 'windows'
+if host_machine.system().to_lower() == 'windows'
     # WINDOWS
     if cpp.get_id() == 'gcc'
         # For mingw-w64, link statically against the UCRT.
         gcc_link_args = ['-lucrtbase', '-static']
         add_project_link_arguments(gcc_link_args, language: ['c', 'cpp'])
         # Make fprintf("%zd") work (see https://github.com/rgommers/scipy/issues/118)
         add_project_arguments('-D__USE_MINGW_ANSI_STDIO=1', language: ['c', 'cpp'])
@@ -43,26 +46,25 @@
         # Force gcc to float64 long doubles for compatibility with MSVC
         # builds, for C only.
         add_project_arguments('-mlong-double-64', language: 'c')
     endif
 
     # API
     winmm_dep = cpp.find_library('winmm', required: jack_not_found)
-elif host_machine.system() == 'darwin'
+    alsa_dep = disabler()
+elif host_machine.system().to_lower() == 'darwin'
     # OSX
 
-    # Enable c++11 support
-    add_project_arguments('-std=c++11', language: ['cpp'])
-
     # API
     coremidi_dep = dependency(
         'appleframeworks',
         modules: ['coreaudio', 'coremidi', 'foundation'],
         required: jack_not_found
     )
+    alsa_dep = disabler()
 else
     # LINUX
 
     # API
     alsa_dep = dependency('alsa', required: jack_not_found)
 endif # Platform detection
 
@@ -71,15 +73,15 @@
 coremidi_support = host_machine.system() == 'darwin' and coremidi_dep.found() and get_option('coremidi')
 winmm_support = host_machine.system() == 'windows' and winmm_dep.found() and get_option('winmm')
 
 threads_dep = dependency('threads', required: alsa_support or jack_support)
 have_semaphore = cpp.has_header('semaphore.h')
 
 pymod = import('python')
-python = pymod.find_installation(get_option('python'), required: true)
+python = pymod.find_installation(get_option('python'), required: true, pure: false)
 
 # Generate _rtmidi extension source
 subdir('src')
 
 # Build & install C++ extension module and Python package
 subdir('rtmidi')
```

### Comparing `python-rtmidi-1.5.2/meson_options.txt` & `python_rtmidi-1.5.3/meson_options.txt`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/pyproject.toml` & `python_rtmidi-1.5.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
-# https://thiblahute.gitlab.io/mesonpep517/
-build-backend = "mesonpep517.buildapi"
+build-backend = "mesonpy"
 requires = [
     "cython",
     "wheel",
-    "mesonpep517 @ git+https://gitlab.com/SpotlightKid/mesonpep517.git@rtmidi",
+    "meson-python",
     "ninja"
 ]
 
 [project]
+name = "python-rtmidi"
 description = "A Python binding for the RtMidi C++ library implemented using Cython."
 authors = [
     { name="Christopher Arndt", email="info@chrisarndt.de" },
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -23,33 +23,33 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
     "Operating System :: MacOS :: MacOS X",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Multimedia :: Sound/Audio :: MIDI",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = [
     "MIDI",
     "multimedia",
     "music",
     "rtmidi",
 ]
-meson-python-option-name = "python"
-meson-options = [
+
+[tool.meson-python.args]
+setup = [
     "-Dwheel=true",
     "-Dverbose=false",
-    "--buildtype=plain"
+    "-Dbuildtype=plain"
 ]
 
 [project.license]
 file = "LICENSE.md"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/SpotlightKid/python-rtmidi/issues"
@@ -74,45 +74,46 @@
 [tool.pydocstyle]
 match = '(?!test_).*\.pyx?'
 match_dir = '(src|rtmidi)'
 add_ignore = [
     "D412"
 ]
 
+[tool.pytest.ini_options]
+markers = [
+    "ci: marks tests to run as part of the CI builds",
+    "jack: marks tests requiring a running JACK server",
+]
+
 [tool.cibuildwheel]
 # Switch to using build
 build-frontend = "build"
 skip = "pp*"
 manylinux-x86_64-image = "manylinux_2_28"
 manylinux-aarch64-image = "manylinux_2_28"
-
 # Run the package tests using `pytest`
-test-command = "pytest {package}/tests/test_basic.py"
 test-requires = "pytest"
 
 # Install system library
 [tool.cibuildwheel.linux]
 build = "cp3{8,9,10,11}-manylinux*"
 archs = ["auto64"]
 before-all = [
     "dnf -y install alsa-lib-devel alsa-utils",
-    "pipx install ninja",
-    "curl -o jack2-1.9.21.tar.gz https://codeload.github.com/jackaudio/jack2/tar.gz/refs/tags/v1.9.21",
-    "tar -xzf jack2-1.9.21.tar.gz",
-    "cd jack2-1.9.21",
-    "python3 waf configure --prefix=/usr --autostart=none --classic",
+    "curl -o jack2-1.9.22.tar.gz https://codeload.github.com/jackaudio/jack2/tar.gz/refs/tags/v1.9.22",
+    "tar -xzf jack2-1.9.22.tar.gz",
+    "cd jack2-1.9.22",
+    "python3 waf configure --prefix=/usr --autostart=none --classic --pkgconfigdir=/usr/lib64/pkgconfig",
     "python3 waf build",
     "python3 waf install",
 ]
+test-command = "pytest -v -m ci {package}/tests"
 
 [tool.cibuildwheel.macos]
 build = "cp3{8,9,10,11}-macosx*"
 archs = ["x86_64", "arm64"]
-environment = { MACOSX_DEPLOYMENT_TARGET = "10.14" }
-before-all = [
-    "pipx install ninja",
-]
+test-command = "pytest -v -m ci {package}/tests"
 
 [tool.cibuildwheel.windows]
 build = "cp3{8,9,10,11}-win*"
 archs = ["AMD64"]
-
+test-command = "pytest -v -m ci {package}/tests"
```

### Comparing `python-rtmidi-1.5.2/requirements-dev.txt` & `python_rtmidi-1.5.3/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/rtmidi/meson.build` & `python_rtmidi-1.5.3/rtmidi/meson.build`

 * *Files 2% similar despite different names*

```diff
@@ -77,10 +77,9 @@
 ])
 
 
 # Install pure Python modules
 python.install_sources(
     python_sources,
     version_py,
-    pure: true,
     subdir: 'rtmidi',
 )
```

### Comparing `python-rtmidi-1.5.2/rtmidi/midiconstants.py` & `python_rtmidi-1.5.3/rtmidi/midiconstants.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/rtmidi/midiutil.py` & `python_rtmidi-1.5.3/rtmidi/midiutil.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/_rtmidi.cpp` & `python_rtmidi-1.5.3/src/_rtmidi.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/_rtmidi.pyx` & `python_rtmidi-1.5.3/src/_rtmidi.pyx`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/meson.build` & `python_rtmidi-1.5.3/src/meson.build`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/meson_dist_cython.py` & `python_rtmidi-1.5.3/src/meson_dist_cython.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/CMakeLists.txt` & `python_rtmidi-1.5.3/src/rtmidi/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/LICENSE` & `python_rtmidi-1.5.3/src/rtmidi/LICENSE`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/Makefile.am` & `python_rtmidi-1.5.3/src/rtmidi/Makefile.am`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/README.md` & `python_rtmidi-1.5.3/src/rtmidi/README.md`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/RtMidi.cpp` & `python_rtmidi-1.5.3/src/rtmidi/RtMidi.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/RtMidi.h` & `python_rtmidi-1.5.3/src/rtmidi/RtMidi.h`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/autogen.sh` & `python_rtmidi-1.5.3/src/rtmidi/autogen.sh`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in` & `python_rtmidi-1.5.3/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/configure.ac` & `python_rtmidi-1.5.3/src/rtmidi/configure.ac`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/rtmidi.go` & `python_rtmidi-1.5.3/src/rtmidi/contrib/go/rtmidi/rtmidi.go`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go` & `python_rtmidi-1.5.3/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/doc/Makefile.am` & `python_rtmidi-1.5.3/src/rtmidi/doc/Makefile.am`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/Doxyfile.in` & `python_rtmidi-1.5.3/src/rtmidi/doc/doxygen/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/tutorial.txt` & `python_rtmidi-1.5.3/src/rtmidi/doc/doxygen/tutorial.txt`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/doc/images/ccrma.gif` & `python_rtmidi-1.5.3/src/rtmidi/doc/images/ccrma.gif`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/doc/images/mcgill.gif` & `python_rtmidi-1.5.3/src/rtmidi/doc/images/mcgill.gif`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/doc/release.txt` & `python_rtmidi-1.5.3/src/rtmidi/doc/release.txt`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4` & `python_rtmidi-1.5.3/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/msw/rtmidilib.sln` & `python_rtmidi-1.5.3/src/rtmidi/msw/rtmidilib.sln`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/msw/rtmidilib.vcproj` & `python_rtmidi-1.5.3/src/rtmidi/msw/rtmidilib.vcproj`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/rtmidi_c.cpp` & `python_rtmidi-1.5.3/src/rtmidi/rtmidi_c.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/rtmidi_c.h` & `python_rtmidi-1.5.3/src/rtmidi/rtmidi_c.h`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/tests/Makefile.am` & `python_rtmidi-1.5.3/src/rtmidi/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/tests/RtMidi.dsw` & `python_rtmidi-1.5.3/src/rtmidi/tests/RtMidi.dsw`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/tests/apinames.cpp` & `python_rtmidi-1.5.3/src/rtmidi/tests/apinames.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/tests/cmidiin.cpp` & `python_rtmidi-1.5.3/src/rtmidi/tests/cmidiin.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/tests/cmidiin.dsp` & `python_rtmidi-1.5.3/src/rtmidi/tests/cmidiin.dsp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/tests/midiclock.cpp` & `python_rtmidi-1.5.3/src/rtmidi/tests/midiclock.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/tests/midiout.cpp` & `python_rtmidi-1.5.3/src/rtmidi/tests/midiout.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/tests/midiout.dsp` & `python_rtmidi-1.5.3/src/rtmidi/tests/midiout.dsp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/tests/midiprobe.cpp` & `python_rtmidi-1.5.3/src/rtmidi/tests/midiprobe.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/tests/midiprobe.dsp` & `python_rtmidi-1.5.3/src/rtmidi/tests/midiprobe.dsp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/tests/qmidiin.cpp` & `python_rtmidi-1.5.3/src/rtmidi/tests/qmidiin.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/tests/qmidiin.dsp` & `python_rtmidi-1.5.3/src/rtmidi/tests/qmidiin.dsp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/tests/sysextest.cpp` & `python_rtmidi-1.5.3/src/rtmidi/tests/sysextest.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/tests/sysextest.dsp` & `python_rtmidi-1.5.3/src/rtmidi/tests/sysextest.dsp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/src/rtmidi/tests/testcapi.c` & `python_rtmidi-1.5.3/src/rtmidi/tests/testcapi.c`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.2/tests/test_basic.py` & `python_rtmidi-1.5.3/tests/test_basic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
-""" Basic tests that don't need midi ports"""
+"""Basic tests that don't need midi ports."""
 
 import unittest
 import rtmidi
 
-
-if bytes is str:
-    string_types = (str, unicode)  # noqa:F821
-else:
-    string_types = (str,)
+import pytest
 
 
+@pytest.mark.ci
 class BasicTest(unittest.TestCase):
     def test_get_api_display_name(self):
         self.assertEqual(rtmidi.get_api_display_name(rtmidi.API_LINUX_ALSA), 'ALSA')
         self.assertEqual(rtmidi.get_api_display_name(rtmidi.API_MACOSX_CORE), 'CoreMidi')
         self.assertEqual(rtmidi.get_api_display_name(rtmidi.API_RTMIDI_DUMMY), 'Dummy')
         self.assertEqual(rtmidi.get_api_display_name(rtmidi.API_UNIX_JACK), 'Jack')
         self.assertEqual(rtmidi.get_api_display_name(rtmidi.API_UNSPECIFIED), 'Unknown')
@@ -52,21 +48,22 @@
             if api in rtmidi.get_compiled_api():
                 self.assertEqual(res, api)
             else:
                 self.assertEqual(res, rtmidi.API_UNSPECIFIED)
 
     def test_get_rtmidi_version(self):
         version = rtmidi.get_rtmidi_version()
-        self.assertTrue(isinstance(version, string_types))
+        self.assertTrue(isinstance(version, str))
         self.assertEqual(version, '5.0.0')
 
     def test_nondummy_api_present(self):
         # Make sure at least one actual API has been compiled
         apilist = rtmidi.get_compiled_api()
         apiFound = False
         for api in apilist:
             if api != rtmidi.API_RTMIDI_DUMMY:
                 apiFound = True
         self.assertTrue(apiFound)
 
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `python-rtmidi-1.5.2/tests/test_delete.py` & `python_rtmidi-1.5.3/tests/test_delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """Unit tests for the rtmidi module."""
 
 import gc
 import unittest
 
 import rtmidi
```

### Comparing `python-rtmidi-1.5.2/tests/test_errorcallback.py` & `python_rtmidi-1.5.3/tests/test_errorcallback.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """Tests for the error callback"""
 
 import unittest
-try:
-    from unittest import mock
-except ImportError:
-    import mock
+from unittest import mock
 
 import rtmidi
 
 
 class TestErrorCallback(unittest.TestCase):
 
     INVALID_PORT_NUMBER = 9999
```

### Comparing `python-rtmidi-1.5.2/tests/test_errors.py` & `python_rtmidi-1.5.3/tests/test_errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""Tests for the error conditions"""
+"""Tests for the error conditions."""
 
 import unittest
 
 import rtmidi
 from rtmidi import InvalidPortError, InvalidUseError
```

### Comparing `python-rtmidi-1.5.2/PKG-INFO` & `python_rtmidi-1.5.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,93 @@
 Metadata-Version: 2.1
 Name: python-rtmidi
-Version: 1.5.2
+Version: 1.5.3
 Summary: A Python binding for the RtMidi C++ library implemented using Cython.
-Keywords: MIDI, multimedia, music, rtmidi
-Author: Christopher Arndt
-Author-email: info@chrisarndt.de
+Keywords: MIDI multimedia music rtmidi
+Author-Email: Christopher Arndt <info@chrisarndt.de>
+License: Copyright & License
+        ===================
+        
+        python-rtmidi was written by Christopher Arndt, 2012 - 2023.
+        
+        The software is released unter the MIT License:
+        
+        Copyright (c) 2012 - 2023 Christopher Arndt
+        
+            Permission is hereby granted, free of charge, to any person obtaining a
+            copy of this software and associated documentation files (the "Software"),
+            to deal in the Software without restriction, including without limitation
+            the rights to use, copy, modify, merge, publish, distribute, sublicense,
+            and/or sell copies of the Software, and to permit persons to whom the
+            Software is furnished to do so, subject to the following conditions:
+        
+            The above copyright notice and this permission notice shall be included
+            in all copies or substantial portions of the Software.
+        
+            THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+            OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+            FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+            AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+            LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+            FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+            DEALINGS IN THE SOFTWARE.
+        
+        
+        RtMidi is distributed under a modified MIT License:
+        
+            RtMidi: realtime MIDI i/o C++ classes
+            Copyright (c) 2003-2019 Gary P. Scavone
+        
+            Permission is hereby granted, free of charge, to any person
+            obtaining a copy of this software and associated documentation files
+            (the "Software"), to deal in the Software without restriction,
+            including without limitation the rights to use, copy, modify, merge,
+            publish, distribute, sublicense, and/or sell copies of the Software,
+            and to permit persons to whom the Software is furnished to do so,
+            subject to the following conditions:
+        
+            The above copyright notice and this permission notice shall be
+            included in all copies or substantial portions of the Software.
+        
+            Any person wishing to distribute modifications to the Software is
+            asked to send the modifications to the original developer so that
+            they can be incorporated into the canonical version.  This is,
+            however, not a binding provision of this license.
+        
+            THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+            EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+            MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+            IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR
+            ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+            CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+            WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Bug tracker, https://github.com/SpotlightKid/python-rtmidi/issues
 Project-URL: Documentation, https://spotlightkid.github.io/python-rtmidi/
 Project-URL: Download, https://pypi.python.org/pypi/python-rtmidi
 Project-URL: Homepage, https://github.com/SpotlightKid/python-rtmidi
 Project-URL: Source, https://gitlab.com/SpotlightKid/python-rtmidi/
-License:
-       |Copyright & License
-       |===================
-       |
-       |python-rtmidi was written by Christopher Arndt, 2012 - 2023.
-       |
-       |The software is released unter the MIT License:
-       |
-       |Copyright (c) 2012 - 2023 Christopher Arndt
-       |
-       |    Permission is hereby granted, free of charge, to any person obtaining a
-       |    copy of this software and associated documentation files (the "Software"),
-       |    to deal in the Software without restriction, including without limitation
-       |    the rights to use, copy, modify, merge, publish, distribute, sublicense,
-       |    and/or sell copies of the Software, and to permit persons to whom the
-       |    Software is furnished to do so, subject to the following conditions:
-       |
-       |    The above copyright notice and this permission notice shall be included
-       |    in all copies or substantial portions of the Software.
-       |
-       |    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-       |    OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-       |    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-       |    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-       |    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-       |    FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-       |    DEALINGS IN THE SOFTWARE.
-       |
-       |
-       |RtMidi is distributed under a modified MIT License:
-       |
-       |    RtMidi: realtime MIDI i/o C++ classes
-       |    Copyright (c) 2003-2019 Gary P. Scavone
-       |
-       |    Permission is hereby granted, free of charge, to any person
-       |    obtaining a copy of this software and associated documentation files
-       |    (the "Software"), to deal in the Software without restriction,
-       |    including without limitation the rights to use, copy, modify, merge,
-       |    publish, distribute, sublicense, and/or sell copies of the Software,
-       |    and to permit persons to whom the Software is furnished to do so,
-       |    subject to the following conditions:
-       |
-       |    The above copyright notice and this permission notice shall be
-       |    included in all copies or substantial portions of the Software.
-       |
-       |    Any person wishing to distribute modifications to the Software is
-       |    asked to send the modifications to the original developer so that
-       |    they can be incorporated into the canonical version.  This is,
-       |    however, not a binding provision of this license.
-       |
-       |    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-       |    EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-       |    MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-       |    IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR
-       |    ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-       |    CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-       |    WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-       |
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Description:
 
 # Welcome to python-rtmidi!
 
 A Python binding for the RtMidi C++ library implemented using Cython.
 
 [![Latest version](https://shields.io/pypi/v/python-rtmidi)](https://pypi.org/project/python-rtmidi)
 ![Project status](https://shields.io/pypi/status/python-rtmidi)
```

