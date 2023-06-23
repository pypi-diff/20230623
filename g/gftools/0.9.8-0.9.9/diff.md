# Comparing `tmp/gftools-0.9.8.tar.gz` & `tmp/gftools-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gftools-0.9.8.tar", last modified: Thu Apr 14 09:43:36 2022, max compression
+gzip compressed data, was "gftools-0.9.9.tar", last modified: Wed Apr 20 14:54:50 2022, max compression
```

## Comparing `gftools-0.9.8.tar` & `gftools-0.9.9.tar`

### file list

```diff
@@ -1,220 +1,231 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.779890 gftools-0.9.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.735887 gftools-0.9.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.739887 gftools-0.9.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-04-14 09:43:19.000000 gftools-0.9.8/.github/workflows/publish-release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      930 2022-04-14 09:43:19.000000 gftools-0.9.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-04-14 09:43:19.000000 gftools-0.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-04-14 09:43:19.000000 gftools-0.9.8/.gitmodules
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.739887 gftools-0.9.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-04-14 09:43:19.000000 gftools-0.9.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-14 09:43:19.000000 gftools-0.9.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.735887 gftools-0.9.8/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.747888 gftools-0.9.8/Lib/gftools/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-04-14 09:43:34.000000 gftools-0.9.8/Lib/gftools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.751888 gftools-0.9.8/Lib/gftools/actions/
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/actions/checkgooglefonts.py
--rw-r--r--   0 runner    (1001) docker     (121)     3473 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/actions/checkversionbump.py
--rw-r--r--   0 runner    (1001) docker     (121)     9019 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/actions/notobuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1998 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/actions/qa2issue.py
--rw-r--r--   0 runner    (1001) docker     (121)     4187 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/actions/updateupstream.py
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/axes.proto
--rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/axes_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.751888 gftools-0.9.8/Lib/gftools/builder/
--rw-r--r--   0 runner    (1001) docker     (121)    21351 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/builder/autohint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2477 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/builder/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/designers.proto
--rw-r--r--   0 runner    (1001) docker     (121)     3980 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/designers_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.751888 gftools-0.9.8/Lib/gftools/encodings/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.751888 gftools-0.9.8/Lib/gftools/encodings/GF Glyph Sets/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/encodings/GF Glyph Sets/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/encodings/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    28567 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/fix.py
--rw-r--r--   0 runner    (1001) docker     (121)     4149 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/fonts_public.proto
--rw-r--r--   0 runner    (1001) docker     (121)    12018 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/fonts_public_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/github.py
--rw-r--r--   0 runner    (1001) docker     (121)    27187 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/html.py
--rw-r--r--   0 runner    (1001) docker     (121)     1997 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/instancer.py
--rw-r--r--   0 runner    (1001) docker     (121)    78976 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/packager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.751888 gftools-0.9.8/Lib/gftools/push-templates/
--rw-r--r--   0 runner    (1001) docker     (121)    14356 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/push-templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     3920 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/push.py
--rw-r--r--   0 runner    (1001) docker     (121)     9550 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/qa.py
--rw-r--r--   0 runner    (1001) docker     (121)    17486 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/stat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/template.upstream.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.751888 gftools-0.9.8/Lib/gftools/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2690 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/templates/_base.html
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/templates/glyphs.html
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/templates/text.html
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/templates/waterfall.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.751888 gftools-0.9.8/Lib/gftools/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)    12735 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/tests/test_fix.py
--rw-r--r--   0 runner    (1001) docker     (121)    12134 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (121)     2669 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/tests/test_instancer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/tests/test_qa.py
--rw-r--r--   0 runner    (1001) docker     (121)    15241 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/tests/test_stat.py
--rw-r--r--   0 runner    (1001) docker     (121)    11027 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/tests/test_usage.py
--rw-r--r--   0 runner    (1001) docker     (121)  6150714 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/udhr_all.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7338 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/ufomerge.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.751888 gftools-0.9.8/Lib/gftools/util/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.759889 gftools-0.9.8/Lib/gftools/util/GlyphsInfo/
--rw-r--r--   0 runner    (1001) docker     (121)  4102534 2022-04-14 09:43:20.000000 gftools-0.9.8/Lib/gftools/util/GlyphsInfo/GlyphData.xml
--rw-r--r--   0 runner    (1001) docker     (121)  2264108 2022-04-14 09:43:20.000000 gftools-0.9.8/Lib/gftools/util/GlyphsInfo/GlyphData_Ideographs.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.759889 gftools-0.9.8/Lib/gftools/util/UnicodeSections/
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/util/UnicodeSections/README.md
--rw-r--r--   0 runner    (1001) docker     (121)   665510 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/util/UnicodeSections/UnicodeSections.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15735 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/util/filter_lists.py
--rw-r--r--   0 runner    (1001) docker     (121)     2508 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/util/glyphdata.py
--rw-r--r--   0 runner    (1001) docker     (121)    15432 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/util/google_fonts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/util/styles.py
--rw-r--r--   0 runner    (1001) docker     (121)     8619 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/util/udhr.py
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/util/unicode_sections.py
--rw-r--r--   0 runner    (1001) docker     (121)    16287 2022-04-14 09:43:19.000000 gftools-0.9.8/Lib/gftools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.751888 gftools-0.9.8/Lib/gftools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4420 2022-04-14 09:43:35.000000 gftools-0.9.8/Lib/gftools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5662 2022-04-14 09:43:36.000000 gftools-0.9.8/Lib/gftools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-14 09:43:35.000000 gftools-0.9.8/Lib/gftools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-14 09:43:35.000000 gftools-0.9.8/Lib/gftools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-04-14 09:43:36.000000 gftools-0.9.8/Lib/gftools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-04-14 09:43:36.000000 gftools-0.9.8/Lib/gftools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4420 2022-04-14 09:43:36.779890 gftools-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3612 2022-04-14 09:43:19.000000 gftools-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.771890 gftools-0.9.8/bin/
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/bash_completion
--rwxr-xr-x   0 runner    (1001) docker     (121)     2963 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/fonts-subset-support.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4057 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools
--rwxr-xr-x   0 runner    (1001) docker     (121)     5864 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-add-axis.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6008 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-add-designer.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9636 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-add-font.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7196 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-build-ofl.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2476 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-builder.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4258 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-check-bbox.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3561 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-check-category.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2465 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-check-copyright-notices.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3259 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-check-font-version.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2277 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-check-name.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3758 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-check-sandbox-family.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6859 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-check-vertical-extents.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3603 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-check-vtt-compatibility.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1526 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-check-vtt-compile.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8651 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-cldr.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7500 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-compare-font.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1885 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-drop-hints.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6090 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-family-html-snippet.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1914 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-find-features.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1212 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-ascii-fontmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2410 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-cmap.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2077 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-family.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4758 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-familymetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1040 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-font.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2728 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-fsselection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1527 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-fstype.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1523 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-gasp.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1730 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-glyph-private-encoding.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2020 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-glyphs.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1461 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-hinting.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1704 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-isfixedpitch.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3601 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-nameids.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3394 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-nonhinting.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1644 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-ttfautohint.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1471 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-unwanted-tables.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2553 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-vendorid.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13840 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-vertical-metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1153 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-fix-weightclass.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3692 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-font-diff.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1935 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-font-weights-coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3393 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-gen-html.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4031 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-gen-push-lists.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3579 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-gen-stat.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9367 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-lang-sample-text.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6620 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-lang-support.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    30500 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-lang.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1404 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-list-italicangle.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1648 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-list-panose.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2271 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-list-variable-source.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1484 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-list-weightclass.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3356 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-list-widthclass.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9431 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-metadata-vs-api.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7649 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-namelist.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7889 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-nametable-from-filename.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1520 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-ots.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7317 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-packager.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4075 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-push-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1744 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-push-status.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8879 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-qa.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1433 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-rangify.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      880 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-rename-font.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16579 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-sanity-check.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3704 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-space-check.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1433 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-tag-noto.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1569 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-test-gf-coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1817 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-ttf2cp.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7394 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-udhr.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2104 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-ufo-fix-instances.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3772 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-ufo-merge.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1415 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-ufo-set-order.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2196 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-ufo-setter.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3781 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-ufo-transfer-data.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1401 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-unicode-names.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3072 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-update-families.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3533 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-update-nameids.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2440 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-update-version.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2116 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-varfont-info.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1453 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/gftools-what-subsets.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2503 2022-04-14 09:43:19.000000 gftools-0.9.8/bin/test_args.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.735887 gftools-0.9.8/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.775890 gftools-0.9.8/data/test/
--rw-r--r--   0 runner    (1001) docker     (121)   763532 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/Inconsolata[wdth,wght].ttf
--rw-r--r--   0 runner    (1001) docker     (121)   120556 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/Lora-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   120580 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/Lora-Regular.ttf-old
--rw-r--r--   0 runner    (1001) docker     (121)   274156 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/Lora-Roman-VF.ttf
--rw-r--r--   0 runner    (1001) docker     (121)  1179872 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/Lora.glyphs
--rw-r--r--   0 runner    (1001) docker     (121)    86920 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/MavenPro[wght].ttf
--rw-r--r--   0 runner    (1001) docker     (121)   263192 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/Montserrat-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   318476 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/Raleway-Italic[wght].ttf
--rw-r--r--   0 runner    (1001) docker     (121)   312352 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/Raleway[wght].ttf
--rw-r--r--   0 runner    (1001) docker     (121)    15758 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/arabic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/builder_test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.775890 gftools-0.9.8/data/test/cabin/
--rw-r--r--   0 runner    (1001) docker     (121)   104644 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/cabin/Cabin-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   104644 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/cabin/Cabin-Regular.ttf-old
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.775890 gftools-0.9.8/data/test/cabin_multi/
--rw-r--r--   0 runner    (1001) docker     (121)   155412 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/cabin_multi/Cabin-Italic[wdth,wght].ttf
--rw-r--r--   0 runner    (1001) docker     (121)   165468 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/cabin_multi/Cabin[wdth,wght].ttf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.775890 gftools-0.9.8/data/test/cabin_split/
--rw-r--r--   0 runner    (1001) docker     (121)   110176 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/cabin_split/Cabin-Italic[wght].ttf
--rw-r--r--   0 runner    (1001) docker     (121)   110996 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/cabin_split/CabinCondensed-Italic[wght].ttf
--rw-r--r--   0 runner    (1001) docker     (121)   121692 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/cabin_split/CabinCondensed[wght].ttf
--rw-r--r--   0 runner    (1001) docker     (121)   122632 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/cabin_split/Cabin[wght].ttf
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/lora_stat.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.779890 gftools-0.9.8/data/test/mavenpro/
--rw-r--r--   0 runner    (1001) docker     (121)    58672 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/mavenpro/MavenPro-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    58628 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/mavenpro/MavenPro-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    58780 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/mavenpro/MavenPro-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    58192 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/mavenpro/MavenPro-Regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.739887 gftools-0.9.8/data/test/mock_googlefonts/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.739887 gftools-0.9.8/data/test/mock_googlefonts/ofl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.779890 gftools-0.9.8/data/test/mock_googlefonts/ofl/abel/
--rw-r--r--   0 runner    (1001) docker     (121)    35220 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/mock_googlefonts/ofl/abel/Abel-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/mock_googlefonts/ofl/abel/DESCRIPTION.en_us.html
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/mock_googlefonts/ofl/abel/FONTLOG.txt
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/mock_googlefonts/ofl/abel/METADATA.pb
--rw-r--r--   0 runner    (1001) docker     (121)     4418 2022-04-14 09:43:19.000000 gftools-0.9.8/data/test/mock_googlefonts/ofl/abel/OFL.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.739887 gftools-0.9.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.779890 gftools-0.9.8/docs/gftools-gen-html/
--rw-r--r--   0 runner    (1001) docker     (121)     3592 2022-04-14 09:43:19.000000 gftools-0.9.8/docs/gftools-gen-html/README.md
--rw-r--r--   0 runner    (1001) docker     (121)   409993 2022-04-14 09:43:19.000000 gftools-0.9.8/docs/gftools-gen-html/genned_result.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.779890 gftools-0.9.8/docs/gftools-packager/
--rw-r--r--   0 runner    (1001) docker     (121)    17226 2022-04-14 09:43:19.000000 gftools-0.9.8/docs/gftools-packager/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 09:43:36.779890 gftools-0.9.8/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)     2652 2022-04-14 09:43:19.000000 gftools-0.9.8/experimental/make_kit.py
--rw-r--r--   0 runner    (1001) docker     (121)    54359 2022-04-14 09:43:19.000000 gftools-0.9.8/font-metadata.csv
--rw-r--r--   0 runner    (1001) docker     (121)    33342 2022-04-14 09:43:19.000000 gftools-0.9.8/nametest.nam
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-04-14 09:43:19.000000 gftools-0.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-14 09:43:36.779890 gftools-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3763 2022-04-14 09:43:19.000000 gftools-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.731542 gftools-0.9.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.695541 gftools-0.9.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.695541 gftools-0.9.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-04-20 14:54:39.000000 gftools-0.9.9/.github/workflows/publish-release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      930 2022-04-20 14:54:39.000000 gftools-0.9.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2022-04-20 14:54:39.000000 gftools-0.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2022-04-20 14:54:39.000000 gftools-0.9.9/.gitmodules
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.695541 gftools-0.9.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-04-20 14:54:39.000000 gftools-0.9.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-20 14:54:39.000000 gftools-0.9.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.695541 gftools-0.9.9/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.703542 gftools-0.9.9/Lib/gftools/
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-04-20 14:54:49.000000 gftools-0.9.9/Lib/gftools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.703542 gftools-0.9.9/Lib/gftools/actions/
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/actions/checkgooglefonts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3473 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/actions/checkversionbump.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9019 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/actions/notobuilder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1998 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/actions/qa2issue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4502 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/actions/updateupstream.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/axes.proto
+-rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/axes_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.703542 gftools-0.9.9/Lib/gftools/builder/
+-rw-r--r--   0 runner    (1001) docker     (121)    21464 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/builder/autohint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2641 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/builder/schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/designers.proto
+-rw-r--r--   0 runner    (1001) docker     (121)     3980 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/designers_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.703542 gftools-0.9.9/Lib/gftools/encodings/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.703542 gftools-0.9.9/Lib/gftools/encodings/GF Glyph Sets/
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/encodings/GF Glyph Sets/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/encodings/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)    28567 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/fix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4149 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/fonts_public.proto
+-rw-r--r--   0 runner    (1001) docker     (121)    12018 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/fonts_public_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/github.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27187 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/html.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1997 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/instancer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    79121 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/packager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.703542 gftools-0.9.9/Lib/gftools/push-templates/
+-rw-r--r--   0 runner    (1001) docker     (121)    14356 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/push-templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3920 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/push.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9550 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/qa.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17486 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/stat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/template.upstream.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.707542 gftools-0.9.9/Lib/gftools/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     2690 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/templates/_base.html
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/templates/glyphs.html
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/templates/text.html
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/templates/waterfall.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.707542 gftools-0.9.9/Lib/gftools/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12735 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/tests/test_fix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12134 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2669 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/tests/test_instancer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/tests/test_qa.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15241 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/tests/test_stat.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11292 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/tests/test_usage.py
+-rw-r--r--   0 runner    (1001) docker     (121)  6150714 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/udhr_all.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7338 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/ufomerge.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.707542 gftools-0.9.9/Lib/gftools/util/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.711542 gftools-0.9.9/Lib/gftools/util/GlyphsInfo/
+-rw-r--r--   0 runner    (1001) docker     (121)  4102534 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/util/GlyphsInfo/GlyphData.xml
+-rw-r--r--   0 runner    (1001) docker     (121)  2264108 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/util/GlyphsInfo/GlyphData_Ideographs.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.711542 gftools-0.9.9/Lib/gftools/util/UnicodeSections/
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/util/UnicodeSections/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)   665510 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/util/UnicodeSections/UnicodeSections.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15735 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/util/filter_lists.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2508 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/util/glyphdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15432 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/util/google_fonts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/util/styles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8619 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/util/udhr.py
+-rw-r--r--   0 runner    (1001) docker     (121)      955 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/util/unicode_sections.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16447 2022-04-20 14:54:39.000000 gftools-0.9.9/Lib/gftools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.703542 gftools-0.9.9/Lib/gftools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4420 2022-04-20 14:54:50.000000 gftools-0.9.9/Lib/gftools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6026 2022-04-20 14:54:50.000000 gftools-0.9.9/Lib/gftools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 14:54:50.000000 gftools-0.9.9/Lib/gftools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 14:54:50.000000 gftools-0.9.9/Lib/gftools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2022-04-20 14:54:50.000000 gftools-0.9.9/Lib/gftools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-04-20 14:54:50.000000 gftools-0.9.9/Lib/gftools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4420 2022-04-20 14:54:50.731542 gftools-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3612 2022-04-20 14:54:39.000000 gftools-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.719542 gftools-0.9.9/bin/
+-rw-r--r--   0 runner    (1001) docker     (121)      377 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/bash_completion
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2963 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/fonts-subset-support.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4057 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5864 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-add-axis.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6008 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-add-designer.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9636 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-add-font.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7196 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-build-ofl.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2476 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-builder.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4258 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-check-bbox.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3561 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-check-category.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2465 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-check-copyright-notices.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3259 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-check-font-version.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2277 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-check-name.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3758 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-check-sandbox-family.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6859 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-check-vertical-extents.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3603 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-check-vtt-compatibility.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1526 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-check-vtt-compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8651 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-cldr.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7500 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-compare-font.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1885 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-drop-hints.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6090 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-family-html-snippet.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1914 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-find-features.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1212 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-ascii-fontmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2410 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-cmap.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2077 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-family.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4758 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-familymetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1040 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-font.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2728 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-fsselection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1527 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-fstype.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1523 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-gasp.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1730 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-glyph-private-encoding.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2020 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-glyphs.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1461 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-hinting.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1704 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-isfixedpitch.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3601 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-nameids.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3394 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-nonhinting.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1644 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-ttfautohint.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1471 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-unwanted-tables.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2553 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-vendorid.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    13840 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-vertical-metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1153 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-fix-weightclass.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3692 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-font-diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1935 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-font-weights-coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3393 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-gen-html.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4031 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-gen-push-lists.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3579 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-gen-stat.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9367 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-lang-sample-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6620 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-lang-support.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    30500 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-lang.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1404 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-list-italicangle.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1648 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-list-panose.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2271 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-list-variable-source.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1484 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-list-weightclass.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3356 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-list-widthclass.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9431 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-metadata-vs-api.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7649 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-namelist.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7889 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-nametable-from-filename.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1520 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-ots.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7317 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-packager.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4075 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-push-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1744 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-push-status.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9391 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-qa.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1433 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-rangify.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      880 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-rename-font.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    16579 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-sanity-check.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3704 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-space-check.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1433 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-tag-noto.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1569 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-test-gf-coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1817 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-ttf2cp.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7394 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-udhr.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2104 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-ufo-fix-instances.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3772 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-ufo-merge.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1415 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-ufo-set-order.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2196 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-ufo-setter.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3781 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-ufo-transfer-data.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1401 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-unicode-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3072 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-update-families.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3533 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-update-nameids.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2440 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-update-version.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2116 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-varfont-info.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1453 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/gftools-what-subsets.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2503 2022-04-20 14:54:39.000000 gftools-0.9.9/bin/test_args.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.695541 gftools-0.9.9/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.723542 gftools-0.9.9/data/test/
+-rw-r--r--   0 runner    (1001) docker     (121)   763532 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Inconsolata[wdth,wght].ttf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.727542 gftools-0.9.9/data/test/Libre-Bodoni/
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Libre-Bodoni/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      548 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Libre-Bodoni/CONTRIBUTORS.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1438 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Libre-Bodoni/FONTLOG.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4492 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Libre-Bodoni/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Libre-Bodoni/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Libre-Bodoni/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.727542 gftools-0.9.9/data/test/Libre-Bodoni/sources/
+-rw-r--r--   0 runner    (1001) docker     (121)   557974 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Libre-Bodoni/sources/LibreBodoni-Italic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (121)   847168 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Libre-Bodoni/sources/LibreBodoni.glyphs
+-rw-r--r--   0 runner    (1001) docker     (121)      932 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Libre-Bodoni/sources/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)   120556 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Lora-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   120580 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Lora-Regular.ttf-old
+-rw-r--r--   0 runner    (1001) docker     (121)   274156 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Lora-Roman-VF.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)  1179872 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Lora.glyphs
+-rw-r--r--   0 runner    (1001) docker     (121)    86920 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/MavenPro[wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   263192 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Montserrat-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   318476 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Raleway-Italic[wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   312352 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/Raleway[wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (121)    15758 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/arabic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/builder_test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.727542 gftools-0.9.9/data/test/cabin/
+-rw-r--r--   0 runner    (1001) docker     (121)   104644 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/cabin/Cabin-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   104644 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/cabin/Cabin-Regular.ttf-old
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.727542 gftools-0.9.9/data/test/cabin_multi/
+-rw-r--r--   0 runner    (1001) docker     (121)   155412 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/cabin_multi/Cabin-Italic[wdth,wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   165468 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/cabin_multi/Cabin[wdth,wght].ttf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.727542 gftools-0.9.9/data/test/cabin_split/
+-rw-r--r--   0 runner    (1001) docker     (121)   110176 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/cabin_split/Cabin-Italic[wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   110996 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/cabin_split/CabinCondensed-Italic[wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   121692 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/cabin_split/CabinCondensed[wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   122632 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/cabin_split/Cabin[wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/lora_stat.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.727542 gftools-0.9.9/data/test/mavenpro/
+-rw-r--r--   0 runner    (1001) docker     (121)    58672 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/mavenpro/MavenPro-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)    58628 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/mavenpro/MavenPro-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)    58780 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/mavenpro/MavenPro-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)    58192 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/mavenpro/MavenPro-Regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.695541 gftools-0.9.9/data/test/mock_googlefonts/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.695541 gftools-0.9.9/data/test/mock_googlefonts/ofl/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.731542 gftools-0.9.9/data/test/mock_googlefonts/ofl/abel/
+-rw-r--r--   0 runner    (1001) docker     (121)    35220 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/mock_googlefonts/ofl/abel/Abel-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)      547 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/mock_googlefonts/ofl/abel/DESCRIPTION.en_us.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/mock_googlefonts/ofl/abel/FONTLOG.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/mock_googlefonts/ofl/abel/METADATA.pb
+-rw-r--r--   0 runner    (1001) docker     (121)     4418 2022-04-20 14:54:39.000000 gftools-0.9.9/data/test/mock_googlefonts/ofl/abel/OFL.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.695541 gftools-0.9.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.731542 gftools-0.9.9/docs/gftools-gen-html/
+-rw-r--r--   0 runner    (1001) docker     (121)     3592 2022-04-20 14:54:39.000000 gftools-0.9.9/docs/gftools-gen-html/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)   409993 2022-04-20 14:54:39.000000 gftools-0.9.9/docs/gftools-gen-html/genned_result.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.731542 gftools-0.9.9/docs/gftools-packager/
+-rw-r--r--   0 runner    (1001) docker     (121)    17226 2022-04-20 14:54:39.000000 gftools-0.9.9/docs/gftools-packager/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 14:54:50.731542 gftools-0.9.9/experimental/
+-rw-r--r--   0 runner    (1001) docker     (121)     2652 2022-04-20 14:54:39.000000 gftools-0.9.9/experimental/make_kit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54359 2022-04-20 14:54:39.000000 gftools-0.9.9/font-metadata.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    33342 2022-04-20 14:54:39.000000 gftools-0.9.9/nametest.nam
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-04-20 14:54:39.000000 gftools-0.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-20 14:54:50.731542 gftools-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3763 2022-04-20 14:54:39.000000 gftools-0.9.9/setup.py
```

### Comparing `gftools-0.9.8/.github/workflows/publish-release.yml` & `gftools-0.9.9/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/.github/workflows/test.yml` & `gftools-0.9.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/.gitignore` & `gftools-0.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/LICENSE` & `gftools-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/actions/checkgooglefonts.py` & `gftools-0.9.9/Lib/gftools/actions/checkgooglefonts.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/actions/checkversionbump.py` & `gftools-0.9.9/Lib/gftools/actions/checkversionbump.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/actions/notobuilder.py` & `gftools-0.9.9/Lib/gftools/actions/notobuilder.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/actions/qa2issue.py` & `gftools-0.9.9/Lib/gftools/actions/qa2issue.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/actions/updateupstream.py` & `gftools-0.9.9/Lib/gftools/actions/updateupstream.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,35 +12,37 @@
 from strictyaml import as_document
 from gftools.utils import download_file
 from fontTools.ttLib import TTFont
 
 
 parser = argparse.ArgumentParser(description="Process some integers.")
 parser.add_argument("url", help="URL of GitHub release")
+parser.add_argument("--family", help="Family name", required=False)
+parser.add_argument("--config", help="Config file", default="sources/config.yaml", required=False)
 
 
 def get_family_name(config):
     if "familyName" in config:
         return config["familyName"]
     return GFBuilder(config).get_family_name()
 
 
 def generate_upstream(config, url):
     repo = os.environ.get("GITHUB_REPOSITORY")
     if not repo:
         raise ValueError("Not being run from a GitHub action?")
+    if "category" not in config:
+        config["category"] = ["SANS_SERIF"]
 
     upstream = {
         "name": get_family_name(config),
         "repository_url": os.environ["GITHUB_SERVER_URL"] + "/" + repo + ".git",
         "archive": url,
         "branch": "main",
-        "category": [
-            "SANS_SERIF"
-        ],  # One man's rigged demo is another man's proof of concept
+        "category": config["category"],
         "build": "",
         "files": {},
         "designer": "Will be filled in",
     }
     return upstream
 
 
@@ -76,29 +78,34 @@
                         # Add statics
                         upstream["files"][relpath] = file
                         a_font = fullpath
         if not license_found:
             raise ValueError(
                 "No license file was found. Ensure OFL.txt is added the the release"
             )
-        if not description_found:
+        if not description_found and "Noto" not in upstream["name"]:
             raise ValueError(
                 "No description file was found. Ensure DESCRIPTION.en_us.html is added the the release"
             )
         if not a_font:
             raise ValueError("No font files were found. Is the release broken?")
 
-        upstream["designer"] = TTFont(a_font)["name"].getDebugName(9)
+        designer = TTFont(a_font)["name"].getDebugName(9)
+        if designer:
+            upstream["designer"] = designer
 
 
 if __name__ == "__main__":
-    config = yaml.load(
-        open(os.path.join("sources", "config.yaml")), Loader=yaml.FullLoader
-    )
     args = parser.parse_args()
+    if args.family:
+        config = {"familyName": args.family}
+    else:
+        config = yaml.load(
+            open(args.config, Loader=yaml.FullLoader)
+        )
 
     if os.path.isfile("upstream.yaml"):
         try:
             upstream = gftools.packager._upstream_conf_from_file(
                 "upstream.yaml", yes=True, quiet=True
             )
         except Exception as e:
```

### Comparing `gftools-0.9.8/Lib/gftools/axes.proto` & `gftools-0.9.9/Lib/gftools/axes.proto`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/axes_pb2.py` & `gftools-0.9.9/Lib/gftools/axes_pb2.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/builder/__init__.py` & `gftools-0.9.9/Lib/gftools/builder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 * ``autohintTTF``: Whether or not to autohint TTF files. Defaults to ``true``.
 * ``ttfaUseScript``: Whether or not to detect a font's primary script and add a ``-D<script>`` flag to ttfautohint. Defaults to ``false``.
 * ``axisOrder``: STAT table axis order. Defaults to fvar order.
 * ``familyName``: Family name for variable fonts. Defaults to family name of first source file.
 * ``flattenComponents``: Whether to flatten components on export. Defaults to ``true``.
 * ``decomposeTransformedComponents``: Whether to decompose transformed components on export. Defaults to ``true``.
 * ``googleFonts``: Whether this font is destined for release on Google Fonts. Used by GitHub Actions. Defaults to ``false``.
+* ``category``: If this font is destined for release on Google Fonts, a list of the categories it should be catalogued under. Used by GitHub Actions. Must be set if ``googleFonts`` is set.
 
 """
 
 from fontmake.font_project import FontProject
 from fontTools import designspaceLib
 from fontTools.otlLib.builder import buildStatTable
 from fontTools.ttLib import TTFont, newTable
@@ -275,17 +276,17 @@
         if "flattenComponents" not in self.config:
             self.config["flattenComponents"] = True
         if "decomposeTransformedComponents" not in self.config:
             self.config["decomposeTransformedComponents"] = True
 
     def build_variable(self):
         self.mkdir(self.config["vfDir"], clean=True)
-        args = {"output": ["variable"], "family_name": self.config["familyName"]}
         ttFonts = []
         for source in self.config["sources"]:
+            args = {"output": ["variable"], "family_name": self.config["familyName"]}
             if not source.endswith(".designspace") and not source.endswith("glyphs"):
                 continue
             self.logger.info("Creating variable fonts from %s" % source)
             sourcebase = os.path.splitext(os.path.basename(source))[0]
             args["output_path"] = os.path.join(
                 self.config["vfDir"], sourcebase + "-VF.ttf",
             )
@@ -445,24 +446,21 @@
                     )
                     static_font.save(dst)
                     postprocessor(dst)
                     self.outputs.add(dst)
 
     def build_a_static_format(self, format, directory, postprocessor):
         self.mkdir(directory, clean=True)
-        args = {
-            "output": [format],
-            "output_dir": directory,
-            "optimize_cff": CFFOptimization.SUBROUTINIZE,
-        }
         for source in self.config["sources"]:
-            if source.endswith("ufo"):
-                if "interpolate" in args:
-                    del args["interpolate"]
-            else:
+            args = {
+                "output": [format],
+                "output_dir": directory,
+                "optimize_cff": CFFOptimization.SUBROUTINIZE,
+            }
+            if not source.endswith("ufo"):
                 args["interpolate"] = True
             self.logger.info("Creating static fonts from %s" % source)
             for fontfile in self.run_fontmake(source, args):
                 self.logger.info("Created static font %s" % fontfile)
                 postprocessor(fontfile)
                 self.outputs.add(fontfile)
```

### Comparing `gftools-0.9.8/Lib/gftools/builder/autohint.py` & `gftools-0.9.9/Lib/gftools/builder/autohint.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/builder/schema.py` & `gftools-0.9.9/Lib/gftools/builder/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,19 @@
                         Map,
                         MapPattern,
                         Str,
                         Int,
                         Float,
                         Seq,
                         Optional,
-                        Bool
+                        Bool,
+                        UniqueSeq,
+                        Enum
                         )
+from gftools.packager import CATEGORIES
 
 
 stat_schema = Seq(
     Map({
         "name": Str(),
         "tag": Str(),
         "values": Seq(
@@ -72,9 +75,10 @@
         Optional("cleanUp"): Bool(),
         Optional("autohintTTF"): Bool(),
         Optional("axisOrder"): Seq(Str()),
         Optional("flattenComponents"): Bool(),
         Optional("decomposeTransformedComponents"): Bool(),
         Optional("ttfaUseScript"): Bool(),
         Optional("googleFonts"): Bool(),
+        Optional("category"): UniqueSeq(Enum(CATEGORIES)),
     }
 )
```

### Comparing `gftools-0.9.8/Lib/gftools/constants.py` & `gftools-0.9.9/Lib/gftools/constants.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/designers_pb2.py` & `gftools-0.9.9/Lib/gftools/designers_pb2.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/fix.py` & `gftools-0.9.9/Lib/gftools/fix.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/fonts_public.proto` & `gftools-0.9.9/Lib/gftools/fonts_public.proto`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/fonts_public_pb2.py` & `gftools-0.9.9/Lib/gftools/fonts_public_pb2.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/github.py` & `gftools-0.9.9/Lib/gftools/github.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/html.py` & `gftools-0.9.9/Lib/gftools/html.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/instancer.py` & `gftools-0.9.9/Lib/gftools/instancer.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/packager.py` & `gftools-0.9.9/Lib/gftools/packager.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 with open(resource_filename('gftools', 'template.upstream.yaml')) as f:
   upstream_yaml_template = f.read()
   # string.format fails if we use other instances of {variables}
   # without adding them to the call to format (KeyError).
   upstream_yaml_template = upstream_yaml_template.replace('{CATEGORIES}', ', '.join(CATEGORIES))
 
 
+NOTO_GITHUB_URL = "https://github.com/notofonts/"
 GIT_NEW_BRANCH_PREFIX = 'gftools_packager_'
 # Using object(expression:$rev), we query all three license folders
 # for family_name, but only the entry that exists will return a tree (directory).
 # Non existing directories will be null (i.e. None).
 # Hence, we can send one query to know the family exists or not, in which
 # directory (license) and have a (flat) directory listing.
 # I queried "rateLimit{cost}" and this had a cost of 1!
@@ -889,14 +890,17 @@
 
   metadata.source.repository_url = upstream_conf['repository_url']
   if upstream_commit_sha:
     metadata.source.commit = upstream_commit_sha
   if upstream_archive_url:
     metadata.source.archive_url = upstream_archive_url
 
+  if upstream_conf['repository_url'].startswith(NOTO_GITHUB_URL):
+    metadata.is_noto = True
+
   language_comments = fonts.LanguageComments(LoadLanguages())
   fonts.WriteProto(metadata, metadata_file_name, comments=language_comments)
 
 def _create_package_content(package_target_dir: str, repos_dir: str,
         upstream_conf_yaml: YAML, license_dir: str, gf_dir_content:dict,
         allow_build: bool, yes: bool, quiet: bool,
         no_allowlist: bool = False) -> str:
```

### Comparing `gftools-0.9.8/Lib/gftools/push-templates/index.html` & `gftools-0.9.9/Lib/gftools/push-templates/index.html`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/push.py` & `gftools-0.9.9/Lib/gftools/push.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/qa.py` & `gftools-0.9.9/Lib/gftools/qa.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/stat.py` & `gftools-0.9.9/Lib/gftools/stat.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/template.upstream.yaml` & `gftools-0.9.9/Lib/gftools/template.upstream.yaml`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/templates/_base.html` & `gftools-0.9.9/Lib/gftools/templates/_base.html`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/templates/glyphs.html` & `gftools-0.9.9/Lib/gftools/templates/glyphs.html`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/templates/waterfall.html` & `gftools-0.9.9/Lib/gftools/templates/waterfall.html`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/tests/test_builder.py` & `gftools-0.9.9/Lib/gftools/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/tests/test_fix.py` & `gftools-0.9.9/Lib/gftools/tests/test_fix.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/tests/test_html.py` & `gftools-0.9.9/Lib/gftools/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/tests/test_instancer.py` & `gftools-0.9.9/Lib/gftools/tests/test_instancer.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/tests/test_qa.py` & `gftools-0.9.9/Lib/gftools/tests/test_qa.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/tests/test_stat.py` & `gftools-0.9.9/Lib/gftools/tests/test_stat.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/tests/test_usage.py` & `gftools-0.9.9/Lib/gftools/tests/test_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         self.get_path = lambda name: os.path.join('bin', 'gftools-' + name + '.py')
         self.example_dir = os.path.join('data', 'test', 'cabin')
         self.example_font = os.path.join(self.example_dir, 'Cabin-Regular.ttf')
         self.example_family = glob(os.path.join("data", "test", "mavenpro", "*.ttf"))
         self.example_vf_font = os.path.join("data", "test", 'Lora-Roman-VF.ttf')
         self.example_vf_stat = os.path.join("data", "test", 'lora_stat.yaml')
         self.example_builder_config = os.path.join("data", "test", 'builder_test.yaml')
+        self.example_builder_config_2_sources = os.path.join("data", "test", "Libre-Bodoni", "sources", "config.yaml")
         self.src_vtt_font = os.path.join("data", "test", "Inconsolata[wdth,wght].ttf")
         self.gf_family_dir = os.path.join('data', 'test', 'mock_googlefonts', 'ofl', 'abel')
         self.nam_file = os.path.join('data', 'test', 'arabic_unique-glyphs.nam')
         self.blacklisted_scripts = [
           ['python', self.get_path('build-contributors')],  # requires source folder of git commits
           ['python', self.get_path('check-category')],  # Requires GF key
           ['python', self.get_path('check-gf-github')],  # Requires github credentials
@@ -233,11 +234,14 @@
     def test_gen_stat2(self):
         self.check_script(
             ['python', self.get_path('gen-stat'), self.example_vf_font, "--src", self.example_vf_stat]
         )
 
     def test_builder(self):
         self.check_script(['python', self.get_path('builder'), self.example_builder_config])
+    
+    def test_builder_2_sources(self):
+        self.check_script(["python", self.get_path("builder"), self.example_builder_config_2_sources])
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `gftools-0.9.8/Lib/gftools/udhr_all.txt` & `gftools-0.9.9/Lib/gftools/udhr_all.txt`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/ufomerge.py` & `gftools-0.9.9/Lib/gftools/ufomerge.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/util/GlyphsInfo/GlyphData.xml` & `gftools-0.9.9/Lib/gftools/util/GlyphsInfo/GlyphData.xml`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/util/GlyphsInfo/GlyphData_Ideographs.xml` & `gftools-0.9.9/Lib/gftools/util/GlyphsInfo/GlyphData_Ideographs.xml`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/util/UnicodeSections/UnicodeSections.json` & `gftools-0.9.9/Lib/gftools/util/UnicodeSections/UnicodeSections.json`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/util/filter_lists.py` & `gftools-0.9.9/Lib/gftools/util/filter_lists.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/util/glyphdata.py` & `gftools-0.9.9/Lib/gftools/util/glyphdata.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/util/google_fonts.py` & `gftools-0.9.9/Lib/gftools/util/google_fonts.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/util/styles.py` & `gftools-0.9.9/Lib/gftools/util/styles.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/util/udhr.py` & `gftools-0.9.9/Lib/gftools/util/udhr.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/util/unicode_sections.py` & `gftools-0.9.9/Lib/gftools/util/unicode_sections.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/Lib/gftools/utils.py` & `gftools-0.9.9/Lib/gftools/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,14 +193,20 @@
         dst_ = os.path.dirname(filename)
         mkdir(dst_, overwrite=False)
         download_file(f.download_url, filename)
         results.append(filename)
     return results
 
 
+def download_files_from_archive(url, dst):
+    zip_io = download_file(url)
+    with ZipFile(zip_io) as zip_file:
+        return fonts_from_zip(zip_file, dst)
+
+
 def download_file(url, dst_path=None):
     """Download a file from a url. If no dst_path is specified, store the file
     as a BytesIO object"""
     request = requests.get(url, stream=True)
     if not dst_path:
         return BytesIO(request.content)
     with open(dst_path, 'wb') as downloaded_file:
```

### Comparing `gftools-0.9.8/Lib/gftools.egg-info/PKG-INFO` & `gftools-0.9.9/Lib/gftools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gftools
-Version: 0.9.8
+Version: 0.9.9
 Summary: Google Fonts Tools is a set of command-line tools for testing font projects
 Home-page: https://github.com/googlefonts/tools/
 Author: Google Fonts Tools Authors: Dave Crossland, Felipe Sanches, Lasse Fister, Marc Foley, Eli Heuer, Roderick Sheeter
 Author-email: dave@lab6.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `gftools-0.9.8/Lib/gftools.egg-info/SOURCES.txt` & `gftools-0.9.9/Lib/gftools.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -160,14 +160,23 @@
 data/test/MavenPro[wght].ttf
 data/test/Montserrat-Regular.ttf
 data/test/Raleway-Italic[wght].ttf
 data/test/Raleway[wght].ttf
 data/test/arabic_unique-glyphs.nam
 data/test/builder_test.yaml
 data/test/lora_stat.yaml
+data/test/Libre-Bodoni/AUTHORS.txt
+data/test/Libre-Bodoni/CONTRIBUTORS.txt
+data/test/Libre-Bodoni/FONTLOG.txt
+data/test/Libre-Bodoni/OFL.txt
+data/test/Libre-Bodoni/README.md
+data/test/Libre-Bodoni/requirements.txt
+data/test/Libre-Bodoni/sources/LibreBodoni-Italic.glyphs
+data/test/Libre-Bodoni/sources/LibreBodoni.glyphs
+data/test/Libre-Bodoni/sources/config.yaml
 data/test/cabin/Cabin-Regular.ttf
 data/test/cabin/Cabin-Regular.ttf-old
 data/test/cabin_multi/Cabin-Italic[wdth,wght].ttf
 data/test/cabin_multi/Cabin[wdth,wght].ttf
 data/test/cabin_split/Cabin-Italic[wght].ttf
 data/test/cabin_split/CabinCondensed-Italic[wght].ttf
 data/test/cabin_split/CabinCondensed[wght].ttf
```

### Comparing `gftools-0.9.8/PKG-INFO` & `gftools-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gftools
-Version: 0.9.8
+Version: 0.9.9
 Summary: Google Fonts Tools is a set of command-line tools for testing font projects
 Home-page: https://github.com/googlefonts/tools/
 Author: Google Fonts Tools Authors: Dave Crossland, Felipe Sanches, Lasse Fister, Marc Foley, Eli Heuer, Roderick Sheeter
 Author-email: dave@lab6.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `gftools-0.9.8/README.md` & `gftools-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/fonts-subset-support.py` & `gftools-0.9.9/bin/fonts-subset-support.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools` & `gftools-0.9.9/bin/gftools`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-add-axis.py` & `gftools-0.9.9/bin/gftools-add-axis.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-add-designer.py` & `gftools-0.9.9/bin/gftools-add-designer.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-add-font.py` & `gftools-0.9.9/bin/gftools-add-font.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-build-ofl.py` & `gftools-0.9.9/bin/gftools-build-ofl.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-builder.py` & `gftools-0.9.9/bin/gftools-builder.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-check-bbox.py` & `gftools-0.9.9/bin/gftools-check-bbox.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-check-category.py` & `gftools-0.9.9/bin/gftools-check-category.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-check-copyright-notices.py` & `gftools-0.9.9/bin/gftools-check-copyright-notices.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-check-font-version.py` & `gftools-0.9.9/bin/gftools-check-font-version.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-check-name.py` & `gftools-0.9.9/bin/gftools-check-name.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-check-sandbox-family.py` & `gftools-0.9.9/bin/gftools-check-sandbox-family.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-check-vertical-extents.py` & `gftools-0.9.9/bin/gftools-check-vertical-extents.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-check-vtt-compatibility.py` & `gftools-0.9.9/bin/gftools-check-vtt-compatibility.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-check-vtt-compile.py` & `gftools-0.9.9/bin/gftools-check-vtt-compile.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-cldr.py` & `gftools-0.9.9/bin/gftools-cldr.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-compare-font.py` & `gftools-0.9.9/bin/gftools-compare-font.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-drop-hints.py` & `gftools-0.9.9/bin/gftools-drop-hints.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-family-html-snippet.py` & `gftools-0.9.9/bin/gftools-family-html-snippet.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-find-features.py` & `gftools-0.9.9/bin/gftools-find-features.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-ascii-fontmetadata.py` & `gftools-0.9.9/bin/gftools-fix-ascii-fontmetadata.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-cmap.py` & `gftools-0.9.9/bin/gftools-fix-cmap.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-family.py` & `gftools-0.9.9/bin/gftools-fix-family.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-familymetadata.py` & `gftools-0.9.9/bin/gftools-fix-familymetadata.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-font.py` & `gftools-0.9.9/bin/gftools-fix-font.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-fsselection.py` & `gftools-0.9.9/bin/gftools-fix-fsselection.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-fstype.py` & `gftools-0.9.9/bin/gftools-fix-fstype.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-gasp.py` & `gftools-0.9.9/bin/gftools-fix-gasp.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-glyph-private-encoding.py` & `gftools-0.9.9/bin/gftools-fix-glyph-private-encoding.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-glyphs.py` & `gftools-0.9.9/bin/gftools-fix-glyphs.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-hinting.py` & `gftools-0.9.9/bin/gftools-fix-hinting.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-isfixedpitch.py` & `gftools-0.9.9/bin/gftools-fix-isfixedpitch.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-nameids.py` & `gftools-0.9.9/bin/gftools-fix-nameids.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-nonhinting.py` & `gftools-0.9.9/bin/gftools-fix-nonhinting.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-ttfautohint.py` & `gftools-0.9.9/bin/gftools-fix-ttfautohint.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-unwanted-tables.py` & `gftools-0.9.9/bin/gftools-fix-unwanted-tables.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-vendorid.py` & `gftools-0.9.9/bin/gftools-fix-vendorid.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-vertical-metrics.py` & `gftools-0.9.9/bin/gftools-fix-vertical-metrics.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-fix-weightclass.py` & `gftools-0.9.9/bin/gftools-fix-weightclass.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-font-diff.py` & `gftools-0.9.9/bin/gftools-font-diff.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-font-weights-coverage.py` & `gftools-0.9.9/bin/gftools-font-weights-coverage.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-gen-html.py` & `gftools-0.9.9/bin/gftools-gen-html.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-gen-push-lists.py` & `gftools-0.9.9/bin/gftools-gen-push-lists.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-gen-stat.py` & `gftools-0.9.9/bin/gftools-gen-stat.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-lang-sample-text.py` & `gftools-0.9.9/bin/gftools-lang-sample-text.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-lang-support.py` & `gftools-0.9.9/bin/gftools-lang-support.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-lang.py` & `gftools-0.9.9/bin/gftools-lang.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-list-italicangle.py` & `gftools-0.9.9/bin/gftools-list-italicangle.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-list-panose.py` & `gftools-0.9.9/bin/gftools-list-panose.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-list-variable-source.py` & `gftools-0.9.9/bin/gftools-list-variable-source.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-list-weightclass.py` & `gftools-0.9.9/bin/gftools-list-weightclass.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-list-widthclass.py` & `gftools-0.9.9/bin/gftools-list-widthclass.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-metadata-vs-api.py` & `gftools-0.9.9/bin/gftools-metadata-vs-api.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-namelist.py` & `gftools-0.9.9/bin/gftools-namelist.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-nametable-from-filename.py` & `gftools-0.9.9/bin/gftools-nametable-from-filename.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-ots.py` & `gftools-0.9.9/bin/gftools-ots.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-packager.py` & `gftools-0.9.9/bin/gftools-packager.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-push-stats.py` & `gftools-0.9.9/bin/gftools-push-stats.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-push-status.py` & `gftools-0.9.9/bin/gftools-push-status.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-qa.py` & `gftools-0.9.9/bin/gftools-qa.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import os
 import shutil
 import logging
 from gftools.utils import (
     download_family_from_Google_Fonts,
     download_files_in_github_pr,
     download_files_in_github_dir,
+    download_files_from_archive,
     Google_Fonts_has_family,
     mkdir,
 )
 from gftools.qa import FontQA
 
 __version__ = "2.2.0"
 logger = logging.getLogger(__name__)
@@ -70,27 +71,31 @@
         help="Paths to fonts")
     font_input_group.add_argument("-pr", "--pull-request",
         help="Get fonts from a Github pull request")
     font_input_group.add_argument("-gh", "--github-dir",
         help="Get fonts from a Github directory")
     font_input_group.add_argument("-gf", "--googlefonts",
         help="Get fonts from Google Fonts")
+    font_input_group.add_argument("-ar", "--archive",
+        help="Get fonts from a zip file URL")
 
     font_before_group = parser.add_argument_group(title="Fonts before input")
     font_before_input_group = font_before_group.add_mutually_exclusive_group(
         required=False
     )
     font_before_input_group.add_argument(
         "-fb", "--fonts-before", nargs="+",
         help="Paths to previous fonts"
     )
     font_before_input_group.add_argument("-prb", "--pull-request-before",
         help="Get previous fonts from a Github pull request")
     font_before_input_group.add_argument("-ghb", "--github-dir-before",
         help="Get previous fonts from a Github dir")
+    font_before_input_group.add_argument("-arb", "--archive-before",
+        help="Get previous fonts from a zip file URL")
     font_before_input_group.add_argument(
         "-gfb",
         "--googlefonts-before",
         action="store_true",
         help="Get previous fonts from Google Fonts",
     )
 
@@ -178,29 +183,31 @@
             logger.info("No fonts found in pull request. Skipping")
             return
     elif args.github_dir:
         fonts = download_files_in_github_dir(args.github_dir, fonts_dir)
         if not fonts:
             logger.info("No fonts found in github dir. Skipping")
             return
+    elif args.archive:
+        fonts = download_files_from_archive(args.archive, fonts_dir)
     elif args.googlefonts:
         fonts = download_family_from_Google_Fonts(args.googlefonts, fonts_dir)
 
     if args.filter_fonts:
         re_filter = re.compile(args.filter_fonts)
         fonts = [f for f in fonts if re_filter.search(f)]
 
     ttfonts = [TTFont(f) for f in fonts if f.endswith((".ttf", ".otf"))
                and "static" not in f]
     family_name = family_name_from_fonts(ttfonts)
     family_on_gf = Google_Fonts_has_family(family_name)
 
     # Retrieve fonts_before and store in out dir
     fonts_before = None
-    if any([args.fonts_before, args.pull_request_before, args.github_dir_before]) or \
+    if any([args.fonts_before, args.pull_request_before, args.github_dir_before, args.archive_before]) or \
            (args.googlefonts_before and family_on_gf):
         fonts_before_dir = os.path.join(args.out, "fonts_before")
         mkdir(fonts_before_dir, overwrite=False)
     if args.fonts_before:
         [shutil.copy(f, fonts_before_dir) for f in args.fonts_before]
         fonts_before = args.fonts_before
     elif args.pull_request_before:
@@ -209,14 +216,18 @@
             fonts_before_dir,
             ignore_static_dir=False
         )
     elif args.github_dir_before:
         fonts_before = download_files_in_github_dir(
             args.github_dir_before, fonts_before_dir
         )
+    elif args.archive_before:
+        fonts_before = download_files_from_archive(
+            args.archive_before, fonts_before_dir
+        )
     elif args.googlefonts_before and family_on_gf:
         fonts_before = download_family_from_Google_Fonts(
             family_name, fonts_before_dir
         )
 
     if fonts_before:
         ttfonts_before = [TTFont(f) for f in fonts_before if f.endswith((".ttf", ".otf"))
```

### Comparing `gftools-0.9.8/bin/gftools-rangify.py` & `gftools-0.9.9/bin/gftools-rangify.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-rename-font.py` & `gftools-0.9.9/bin/gftools-rename-font.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-sanity-check.py` & `gftools-0.9.9/bin/gftools-sanity-check.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-space-check.py` & `gftools-0.9.9/bin/gftools-space-check.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-tag-noto.py` & `gftools-0.9.9/bin/gftools-tag-noto.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-test-gf-coverage.py` & `gftools-0.9.9/bin/gftools-test-gf-coverage.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-ttf2cp.py` & `gftools-0.9.9/bin/gftools-ttf2cp.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-udhr.py` & `gftools-0.9.9/bin/gftools-udhr.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-ufo-fix-instances.py` & `gftools-0.9.9/bin/gftools-ufo-fix-instances.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-ufo-merge.py` & `gftools-0.9.9/bin/gftools-ufo-merge.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-ufo-set-order.py` & `gftools-0.9.9/bin/gftools-ufo-set-order.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-ufo-setter.py` & `gftools-0.9.9/bin/gftools-ufo-setter.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-ufo-transfer-data.py` & `gftools-0.9.9/bin/gftools-ufo-transfer-data.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-unicode-names.py` & `gftools-0.9.9/bin/gftools-unicode-names.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-update-families.py` & `gftools-0.9.9/bin/gftools-update-families.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-update-nameids.py` & `gftools-0.9.9/bin/gftools-update-nameids.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-update-version.py` & `gftools-0.9.9/bin/gftools-update-version.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-varfont-info.py` & `gftools-0.9.9/bin/gftools-varfont-info.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/gftools-what-subsets.py` & `gftools-0.9.9/bin/gftools-what-subsets.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/bin/test_args.py` & `gftools-0.9.9/bin/test_args.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/Inconsolata[wdth,wght].ttf` & `gftools-0.9.9/data/test/Inconsolata[wdth,wght].ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/Lora-Regular.ttf` & `gftools-0.9.9/data/test/Lora-Regular.ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/Lora-Regular.ttf-old` & `gftools-0.9.9/data/test/Lora-Regular.ttf-old`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/Lora-Roman-VF.ttf` & `gftools-0.9.9/data/test/Lora-Roman-VF.ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/Lora.glyphs` & `gftools-0.9.9/data/test/Lora.glyphs`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/MavenPro[wght].ttf` & `gftools-0.9.9/data/test/MavenPro[wght].ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/Montserrat-Regular.ttf` & `gftools-0.9.9/data/test/Montserrat-Regular.ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/Raleway-Italic[wght].ttf` & `gftools-0.9.9/data/test/Raleway-Italic[wght].ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/Raleway[wght].ttf` & `gftools-0.9.9/data/test/Raleway[wght].ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/arabic_unique-glyphs.nam` & `gftools-0.9.9/data/test/arabic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/cabin/Cabin-Regular.ttf` & `gftools-0.9.9/data/test/cabin/Cabin-Regular.ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/cabin/Cabin-Regular.ttf-old` & `gftools-0.9.9/data/test/cabin/Cabin-Regular.ttf-old`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/cabin_multi/Cabin-Italic[wdth,wght].ttf` & `gftools-0.9.9/data/test/cabin_multi/Cabin-Italic[wdth,wght].ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/cabin_multi/Cabin[wdth,wght].ttf` & `gftools-0.9.9/data/test/cabin_multi/Cabin[wdth,wght].ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/cabin_split/Cabin-Italic[wght].ttf` & `gftools-0.9.9/data/test/cabin_split/Cabin-Italic[wght].ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/cabin_split/CabinCondensed-Italic[wght].ttf` & `gftools-0.9.9/data/test/cabin_split/CabinCondensed-Italic[wght].ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/cabin_split/CabinCondensed[wght].ttf` & `gftools-0.9.9/data/test/cabin_split/CabinCondensed[wght].ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/cabin_split/Cabin[wght].ttf` & `gftools-0.9.9/data/test/cabin_split/Cabin[wght].ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/mavenpro/MavenPro-Black.ttf` & `gftools-0.9.9/data/test/mavenpro/MavenPro-Black.ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/mavenpro/MavenPro-Bold.ttf` & `gftools-0.9.9/data/test/mavenpro/MavenPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/mavenpro/MavenPro-Medium.ttf` & `gftools-0.9.9/data/test/mavenpro/MavenPro-Medium.ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/mavenpro/MavenPro-Regular.ttf` & `gftools-0.9.9/data/test/mavenpro/MavenPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/mock_googlefonts/ofl/abel/Abel-Regular.ttf` & `gftools-0.9.9/data/test/mock_googlefonts/ofl/abel/Abel-Regular.ttf`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/mock_googlefonts/ofl/abel/DESCRIPTION.en_us.html` & `gftools-0.9.9/data/test/mock_googlefonts/ofl/abel/DESCRIPTION.en_us.html`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/mock_googlefonts/ofl/abel/FONTLOG.txt` & `gftools-0.9.9/data/test/mock_googlefonts/ofl/abel/FONTLOG.txt`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/data/test/mock_googlefonts/ofl/abel/OFL.txt` & `gftools-0.9.9/data/test/mock_googlefonts/ofl/abel/OFL.txt`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/docs/gftools-gen-html/README.md` & `gftools-0.9.9/docs/gftools-gen-html/README.md`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/docs/gftools-gen-html/genned_result.png` & `gftools-0.9.9/docs/gftools-gen-html/genned_result.png`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/docs/gftools-packager/README.md` & `gftools-0.9.9/docs/gftools-packager/README.md`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/experimental/make_kit.py` & `gftools-0.9.9/experimental/make_kit.py`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/font-metadata.csv` & `gftools-0.9.9/font-metadata.csv`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/nametest.nam` & `gftools-0.9.9/nametest.nam`

 * *Files identical despite different names*

### Comparing `gftools-0.9.8/setup.py` & `gftools-0.9.9/setup.py`

 * *Files identical despite different names*

