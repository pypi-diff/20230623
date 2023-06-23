# Comparing `tmp/diffoscope-98.tar.gz` & `tmp/diffoscope-99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/diffoscope-98.tar", last modified: Fri Jun 29 07:20:57 2018, max compression
+gzip compressed data, was "dist/diffoscope-99.tar", last modified: Sun Jul  8 18:21:59 2018, max compression
```

## Comparing `diffoscope-98.tar` & `diffoscope-99.tar`

### file list

```diff
@@ -1,482 +1,522 @@
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/diffoscope/
--rw-r--r--   0 lamby     (1000) lamby     (1000)      805 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/__init__.py
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/diffoscope/comparators/
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1432 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/tar.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1331 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/sqlite.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     6913 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/image.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1422 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/fonts.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1449 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/docx.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     7458 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/deb.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4231 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/__init__.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3451 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/rpm.py
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/diffoscope/comparators/utils/
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3250 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/utils/command.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2254 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/utils/specialize.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/utils/__init__.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)    10198 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/utils/libarchive.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4273 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/utils/archive.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4952 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/utils/compare.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     7134 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/utils/container.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)    15897 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/utils/file.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2027 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/utils/fuzzy.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2528 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/android.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2437 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/rust.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2748 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/ar.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     9291 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/directory.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     8708 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/debian.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1620 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/pcap.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1746 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/berkeley_db.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1316 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/pdf.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)    18332 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/elf.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     6537 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/apk.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2720 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/fontconfig.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1342 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/icc.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2414 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/png.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     8933 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/squashfs.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1625 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/pgp.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3185 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/missing_file.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1936 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/debian_fallback.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1344 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/openssh.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2784 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/device.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1801 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/dex.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3638 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/ppu.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3319 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/iso9660.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1706 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/ps.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3021 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/json.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1215 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/rpm_fallback.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4958 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/haskell.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1414 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/cpio.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2107 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/symlink.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2663 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/git.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2826 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/text.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1313 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/javascript.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1408 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/dtb.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1925 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/gnumeric.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1482 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/xsb.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3602 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/xml.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1909 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/xz.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1890 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/llvm.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1387 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/mono.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     5145 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/cbfs.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3096 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/rdata.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2338 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/gettext.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3326 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/binwalk.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1379 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/ogg.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1893 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/gzip.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1450 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/odt.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1351 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/binary.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2932 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/java.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3139 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/fsimage.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3152 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/gif.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     5859 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/zip.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)      982 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/ipk.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1772 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/bzip2.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4625 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/comparators/macho.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3865 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/tools.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3322 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/feeders.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     6727 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/external_tools.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2918 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/profiling.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1417 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/exc.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1624 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/logging.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2735 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/tempfiles.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     7939 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/progress.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3173 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/config.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1600 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/excludes.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)    12215 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/difference.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1507 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/locale.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)    11361 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/changes.py
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/diffoscope/presenters/
--rw-r--r--   0 lamby     (1000) lamby     (1000)    13562 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/presenters/utils.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/presenters/__init__.py
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/diffoscope/presenters/html/
--rw-r--r--   0 lamby     (1000) lamby     (1000)    30572 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/presenters/html/html.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)      875 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/presenters/html/__init__.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     6640 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/presenters/html/templates.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1638 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/presenters/markdown.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1874 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/presenters/restructuredtext.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1369 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/presenters/icon.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2141 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/presenters/json.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3022 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/presenters/text.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3661 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/presenters/formats.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1030 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/path.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)    24044 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/main.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)    20465 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/diff.py
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/diffoscope/readers/
--rw-r--r--   0 lamby     (1000) lamby     (1000)      835 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/readers/utils.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1025 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/readers/__init__.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1815 2018-06-29 07:18:58.000000 diffoscope-98/diffoscope/readers/json.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1910 2018-06-29 07:18:58.000000 diffoscope-98/setup.py
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/diffoscope.egg-info/
--rw-r--r--   0 lamby     (1000) lamby     (1000)    13933 2018-06-29 07:20:57.000000 diffoscope-98/diffoscope.egg-info/SOURCES.txt
--rw-r--r--   0 lamby     (1000) lamby     (1000)       53 2018-06-29 07:20:57.000000 diffoscope-98/diffoscope.egg-info/entry_points.txt
--rw-r--r--   0 lamby     (1000) lamby     (1000)       53 2018-06-29 07:20:57.000000 diffoscope-98/diffoscope.egg-info/requires.txt
--rw-r--r--   0 lamby     (1000) lamby     (1000)     6068 2018-06-29 07:20:57.000000 diffoscope-98/diffoscope.egg-info/PKG-INFO
--rw-r--r--   0 lamby     (1000) lamby     (1000)       11 2018-06-29 07:20:57.000000 diffoscope-98/diffoscope.egg-info/top_level.txt
--rw-r--r--   0 lamby     (1000) lamby     (1000)        1 2018-06-29 07:20:57.000000 diffoscope-98/diffoscope.egg-info/dependency_links.txt
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4332 2018-06-29 07:18:59.000000 diffoscope-98/README.rst
--rw-r--r--   0 lamby     (1000) lamby     (1000)     6068 2018-06-29 07:20:57.000000 diffoscope-98/PKG-INFO
--rw-r--r--   0 lamby     (1000) lamby     (1000)       47 2018-06-29 07:18:59.000000 diffoscope-98/MANIFEST.in
--rw-r--r--   0 lamby     (1000) lamby     (1000)    35147 2018-06-29 07:18:59.000000 diffoscope-98/COPYING
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/tests/
--rw-r--r--   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:18:59.000000 diffoscope-98/tests/__init__.py
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/tests/comparators/
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2517 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_ppu.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2211 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_android.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3647 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_directory.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1661 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_docx.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/__init__.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1739 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_gnumeric.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2818 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_squashfs.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1640 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_ogg.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2443 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_bzip2.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3371 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_rpm.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3520 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_fsimage.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3224 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_jpeg_image.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1501 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_git.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2704 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_tar.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2989 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_dex.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1426 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_fontconfig.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2370 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_openssh_pub_key.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1855 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_fonts.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1685 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_rdata.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2145 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_device.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2529 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_dtb.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1640 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_odt.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1655 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_berkeley_db.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2517 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_gif.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1640 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_xsb.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2900 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_ico_image.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2555 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_binwalk.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3108 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_text.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3046 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_java.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2123 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_ipk.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1958 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_pdf.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1187 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_archive.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3258 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_gzip.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     8346 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_binary.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2974 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_iso9660.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2350 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_macho.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2004 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_icc.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1477 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_xml.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3446 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_zip.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3666 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_rlib.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1963 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_javascript.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1917 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_json.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1307 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_symlink.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2013 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_mono.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4226 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_utils.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3503 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_apk.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2247 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_cpio.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)    11439 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_debian.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1640 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_pgp.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2009 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_ps.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2310 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_epub.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3046 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_containers.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1659 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_pcap.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2374 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_xz.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     6154 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_elf.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2242 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_gettext.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1768 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_haskell.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3727 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_cbfs.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1852 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_sqlite.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4789 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_deb.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2123 2018-06-29 07:18:59.000000 diffoscope-98/tests/comparators/test_png.py
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/tests/utils/
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1664 2018-06-29 07:18:59.000000 diffoscope-98/tests/utils/__init__.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4734 2018-06-29 07:18:59.000000 diffoscope-98/tests/utils/tools.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2177 2018-06-29 07:18:59.000000 diffoscope-98/tests/utils/data.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1396 2018-06-29 07:18:59.000000 diffoscope-98/tests/utils/nonexisting.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2245 2018-06-29 07:18:59.000000 diffoscope-98/tests/test_quines.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4037 2018-06-29 07:18:59.000000 diffoscope-98/tests/test_difference.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2546 2018-06-29 07:18:59.000000 diffoscope-98/tests/test_progress.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1893 2018-06-29 07:18:59.000000 diffoscope-98/tests/conftest.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1227 2018-06-29 07:18:59.000000 diffoscope-98/tests/test_tools.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1066 2018-06-29 07:18:59.000000 diffoscope-98/tests/test_source.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2292 2018-06-29 07:18:59.000000 diffoscope-98/tests/test_excludes.py
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/tests/data/
--rw-r--r--   0 lamby     (1000) lamby     (1000)     9734 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.rlib
--rw-r--r--   0 lamby     (1000) lamby     (1000)     7767 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/rpm_fallback_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1216 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.o
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2218 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/text_unicode_binary_fallback
--rw-r--r--   0 lamby     (1000) lamby     (1000)      362 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/pe_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)    46408 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/Samyak-Malayalam1.ttf
--rw-r--r--   0 lamby     (1000) lamby     (1000)      287 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.gz
--rw-r--r--   0 lamby     (1000) lamby     (1000)      400 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/ico_image_meta_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      671 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/text_ascii2
--rw-r--r--   0 lamby     (1000) lamby     (1000)      637 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/rds_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      493 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/iso9660_content_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      672 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/text_unicode1
--rw-r--r--   0 lamby     (1000) lamby     (1000)     5975 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.rpm
--rw-r--r--   0 lamby     (1000) lamby     (1000)   286518 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test_weird_non_unicode_chars2.pdf
--rw-r--r--   0 lamby     (1000) lamby     (1000)       29 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/order1a.json
--rw-r--r--   0 lamby     (1000) lamby     (1000)      458 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test_iso8859-1.mo
--rw-r--r--   0 lamby     (1000) lamby     (1000)      150 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/binary_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      580 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/iso9660_rockridge_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      854 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test3.gif
--rw-r--r--   0 lamby     (1000) lamby     (1000)     5952 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/rpm_header_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1216 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.o
--rw-r--r--   0 lamby     (1000) lamby     (1000)      516 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/mo_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      440 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/quine.zip
--rw-r--r--   0 lamby     (1000) lamby     (1000)    10240 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/no-perms.tar
--rw-r--r--   0 lamby     (1000) lamby     (1000)      865 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.pdf
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1643 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/berkeley_db_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)    10240 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.tar
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1646 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/bug881937_1.deb
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1546 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.xsb
--rw-r--r--   0 lamby     (1000) lamby     (1000)      430 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.gz
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1354 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.a
--rw-r--r--   0 lamby     (1000) lamby     (1000)      298 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/dot_changes_identical_contents_and_different_files_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3270 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2_meta.ico
--rw-r--r--   0 lamby     (1000) lamby     (1000)      314 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/elf_lib_metadata_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3346 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/epub_expected_diffs
--rw-r--r--   0 lamby     (1000) lamby     (1000)      215 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/gzip_metadata_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     8932 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/ttf_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      523 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/ext4_expected_diffs
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1743 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/output.md
--rw-r--r--   0 lamby     (1000) lamby     (1000)      731 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test_openssh_pub_key2.pub
--rw-r--r--   0 lamby     (1000) lamby     (1000)       80 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/binary_hexdump_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      767 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/mozzip_zipinfo_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)    10240 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/archive2.tar
--rw-r--r--   0 lamby     (1000) lamby     (1000)      662 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1_meta.jpg
--rw-r--r--   0 lamby     (1000) lamby     (1000)      228 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/dot_changes_different_contents_and_identical_files_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      846 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/apk_manifest_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)       92 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/ps_text_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      284 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.xml
--rw-r--r--   0 lamby     (1000) lamby     (1000)       35 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/text_order1
--rw-r--r--   0 lamby     (1000) lamby     (1000)      793 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.gif
--rw-r--r--   0 lamby     (1000) lamby     (1000)      135 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/procyon_class_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)   627936 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/pcap_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      129 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.git-index
--rw-r--r--   0 lamby     (1000) lamby     (1000)    14437 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/gif_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)       35 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/text_order2
--rw-r--r--   0 lamby     (1000) lamby     (1000)     7922 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.odt
--rw-r--r--   0 lamby     (1000) lamby     (1000)       69 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.png
--rw-r--r--   0 lamby     (1000) lamby     (1000)    14208 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1-le64.cache-4
--rw-r--r--   0 lamby     (1000) lamby     (1000)      457 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/iso9660_content_expected_diff_cdrtools
--rw-r--r--   0 lamby     (1000) lamby     (1000)       46 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/symlink_expected_destination_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4567 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.ogg
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4322 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.hi
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1757 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/output.txt
--rw-r--r--   0 lamby     (1000) lamby     (1000)       22 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.json
--rw-r--r--   0 lamby     (1000) lamby     (1000)     7745 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/haskell_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)    46408 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/Samyak-Malayalam2.ttf
--rw-r--r--   0 lamby     (1000) lamby     (1000)      819 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test4.changes
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2142 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/device_expected_diff_freebsd
--rw-r--r--   0 lamby     (1000) lamby     (1000)      276 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.rdx
--rw-r--r--   0 lamby     (1000) lamby     (1000)      150 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/openssh_pub_key_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     6926 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1_meta.ico
--rw-r--r--   0 lamby     (1000) lamby     (1000)      387 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/javap_class_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)    68323 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/devicetree2.dtb
--rw-r--r--   0 lamby     (1000) lamby     (1000)      651 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/binwalk_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      202 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/ipk_metadata_expected_diff
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/tests/data/containers/
--rw-r--r--   0 lamby     (1000) lamby     (1000)      616 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/containers/b.tar.xz
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1112 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/containers/different_files_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      348 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/containers/a.tar.bz2
--rw-r--r--   0 lamby     (1000) lamby     (1000)       19 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/containers/magic_xz
--rw-r--r--   0 lamby     (1000) lamby     (1000)      525 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/containers/b.tar.bz2
--rw-r--r--   0 lamby     (1000) lamby     (1000)      404 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/containers/a.tar.xz
--rw-r--r--   0 lamby     (1000) lamby     (1000)       41 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/containers/magic_bzip2
--rw-r--r--   0 lamby     (1000) lamby     (1000)      532 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/containers/b.tar.gz
--rw-r--r--   0 lamby     (1000) lamby     (1000)       94 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/containers/magic_gzip
--rw-r--r--   0 lamby     (1000) lamby     (1000)      335 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/containers/a.tar.gz
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2142 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/device_expected_diff_reverse_freebsd
--rw-r--r--   0 lamby     (1000) lamby     (1000)    35903 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/ogg_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      607 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/ppu_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      595 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test_openssh_pub_key1.pub
--rw-r--r--   0 lamby     (1000) lamby     (1000)     7931 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.odt
--rw-r--r--   0 lamby     (1000) lamby     (1000)      450 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.dsc
--rw-r--r--   0 lamby     (1000) lamby     (1000)      634 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/archive12.diff.txt
--rw-r--r--   0 lamby     (1000) lamby     (1000)    15384 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2-le64.cache-4
--rw-r--r--   0 lamby     (1000) lamby     (1000)       16 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/binary2
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3072 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.binwalk
--rw-r--r--   0 lamby     (1000) lamby     (1000)      349 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/quine_deb_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)    10240 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.tar
--rw-r--r--   0 lamby     (1000) lamby     (1000)      869 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/bug881937_control_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)    10240 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/fuzzy1.tar
--rw-r--r--   0 lamby     (1000) lamby     (1000)      450 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.dsc
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2048 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.sqlite3
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2141 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/device_expected_diff_reverse
--rw-r--r--   0 lamby     (1000) lamby     (1000)       29 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/order1b.json
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1803 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.gnumeric
--rw-r--r--   0 lamby     (1000) lamby     (1000)      220 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/javascript_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2094 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test4.gif
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1864 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/output.rst
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1024 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.cpio
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1716 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/bug881937_2.deb
--rw-r--r--   0 lamby     (1000) lamby     (1000)      293 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.xml
--rw-r--r--   0 lamby     (1000) lamby     (1000)       29 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/macho_expected_diff_arch
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3320 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.epub
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1316 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/macho_expected_diff_disassembly
--rw-r--r--   0 lamby     (1000) lamby     (1000)   286703 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test_weird_non_unicode_chars1.pdf
--rw-r--r--   0 lamby     (1000) lamby     (1000)      644 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/quine_a.deb
--rw-r--r--   0 lamby     (1000) lamby     (1000)       16 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/binary1
--rw-r--r--   0 lamby     (1000) lamby     (1000)      318 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.ico
--rw-r--r--   0 lamby     (1000) lamby     (1000)    10240 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/fuzzy3.tar
--rw-r--r--   0 lamby     (1000) lamby     (1000)     7808 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/xsb_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     6020 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.jpg
--rw-r--r--   0 lamby     (1000) lamby     (1000)      826 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.changes
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4046 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.docx
--rw-r--r--   0 lamby     (1000) lamby     (1000)      409 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.mozzip
--rw-r--r--   0 lamby     (1000) lamby     (1000)    68260 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/devicetree1.dtb
--rw-r--r--   0 lamby     (1000) lamby     (1000)      518 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/deb_metadata_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)    41435 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.ppu
--rw-r--r--   0 lamby     (1000) lamby     (1000)    22251 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/ps_internal_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)   256000 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.ext4
--rw-r--r--   0 lamby     (1000) lamby     (1000)      586 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/cpio_listing_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)    10240 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/fuzzy2.tar
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2400 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.hi
--rw-r--r--   0 lamby     (1000) lamby     (1000)   360448 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.iso
--rw-r--r--   0 lamby     (1000) lamby     (1000)      397 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.mo
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2086 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.debsrc.tar.gz
--rw-r--r--   0 lamby     (1000) lamby     (1000)    14684 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.icc
--rwxr-xr-x   0 lamby     (1000) lamby     (1000)     3072 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.exe
--rw-r--r--   0 lamby     (1000) lamby     (1000)      193 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.git-index
--rw-r--r--   0 lamby     (1000) lamby     (1000)    49504 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/base-files_157-r45918_ar71xx.ipk
--rw-r--r--   0 lamby     (1000) lamby     (1000)      516 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/icc_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)       72 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/json_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      347 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/elf_obj_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      409 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/git_expected_diff_freebsd
--rw-r--r--   0 lamby     (1000) lamby     (1000)       44 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test_directory_symlink_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      423 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/zip_zipinfo_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      759 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/dot_buildinfo_fallback_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1546 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.xsb
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1908 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/rlib_llvm_dis_expected_diff_5
--rw-r--r--   0 lamby     (1000) lamby     (1000)    20480 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/fuzzy-tar-in-tar1.tar
--rw-r--r--   0 lamby     (1000) lamby     (1000)      532 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.xz
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2116 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.dex
--rw-r--r--   0 lamby     (1000) lamby     (1000)       75 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/dot_changes_description_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      266 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/macho_expected_diff_headers
--rw-r--r--   0 lamby     (1000) lamby     (1000)      644 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/quine_b.deb
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4482 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/ico_image_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      538 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/iso9660_rockridge_expected_diff_cdrtools
--rw-r--r--   0 lamby     (1000) lamby     (1000)       26 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/odt_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1791 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.gif
--rw-r--r--   0 lamby     (1000) lamby     (1000)     5265 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.jpg
--rw-r--r--   0 lamby     (1000) lamby     (1000)      744 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/text_iso8859_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1262 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/dot_changes_fallback_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      163 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/png_expected_diff
--rwxr-xr-x   0 lamby     (1000) lamby     (1000)     3072 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.exe
--rw-r--r--   0 lamby     (1000) lamby     (1000)      398 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/ico_image_meta_expected_diff_v2
--rw-r--r--   0 lamby     (1000) lamby     (1000)      714 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.zip
--rw-r--r--   0 lamby     (1000) lamby     (1000)       92 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.js
--rw-r--r--   0 lamby     (1000) lamby     (1000)       22 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.json
--rw-r--r--   0 lamby     (1000) lamby     (1000)      571 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test3.zip
--rw-r--r--   0 lamby     (1000) lamby     (1000)   256000 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.ext4
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3317 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.epub
--rw-r--r--   0 lamby     (1000) lamby     (1000)       69 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.png
--rwxr-xr-x   0 lamby     (1000) lamby     (1000)     8432 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.macho
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1354 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.a
--rw-r--r--   0 lamby     (1000) lamby     (1000)      305 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.bz2
--rw-r--r--   0 lamby     (1000) lamby     (1000)      602 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/debian-bug-876316-control.tar.gz
--rw-r--r--   0 lamby     (1000) lamby     (1000)  4208640 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/android1.img
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2141 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/device_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3636 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/pgp_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      866 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.pgp
--rw-r--r--   0 lamby     (1000) lamby     (1000)      439 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/squashfs_superblock_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)       18 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/docx_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      864 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.apk
--rw-r--r--   0 lamby     (1000) lamby     (1000)      571 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.zip
--rw-r--r--   0 lamby     (1000) lamby     (1000)    14684 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.icc
--rw-r--r--   0 lamby     (1000) lamby     (1000)      395 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/rlib_armap_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2116 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.dex
--rw-r--r--   0 lamby     (1000) lamby     (1000)      414 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/cbfs_listing_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      276 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.rdx
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2262 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.deb
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2048 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.sqlite3
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1880 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/dex_expected_diffs
--rw-r--r--   0 lamby     (1000) lamby     (1000)      717 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/rlib_elf_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      446 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/text_ascii1
--rw-r--r--   0 lamby     (1000) lamby     (1000)    41435 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.ppu
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3765 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.buildinfo
--rw-r--r--   0 lamby     (1000) lamby     (1000)      388 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.xz
--rw-r--r--   0 lamby     (1000) lamby     (1000)      466 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.bz2
--rw-r--r--   0 lamby     (1000) lamby     (1000)      571 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/gnu_debuglink_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2050 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/output.json
--rw-r--r--   0 lamby     (1000) lamby     (1000)    29922 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.ps
--rw-r--r--   0 lamby     (1000) lamby     (1000)      186 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/zip_bsdtar_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      174 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/rpm_listing_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2388 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.deb
--rw-r--r--   0 lamby     (1000) lamby     (1000)  4210688 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/android2.img
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1024 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.cpio
--rw-r--r--   0 lamby     (1000) lamby     (1000)       41 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test_directory_file_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)       43 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test_directory_device_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      250 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/quine.gz
--rw-r--r--   0 lamby     (1000) lamby     (1000)      182 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/macho_expected_diff_loadcommands
--rw-r--r--   0 lamby     (1000) lamby     (1000)    84442 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.pcap
--rw-r--r--   0 lamby     (1000) lamby     (1000)      321 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/cbfs_listing_no_legacy_header_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      154 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/quine_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)   360448 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.iso
--rw-r--r--   0 lamby     (1000) lamby     (1000)      795 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/tar_listing_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)       58 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/pdf_text_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)    85965 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.pcap
--rw-r--r--   0 lamby     (1000) lamby     (1000)     9734 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.rlib
--rw-r--r--   0 lamby     (1000) lamby     (1000)    29784 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.ps
--rw-r--r--   0 lamby     (1000) lamby     (1000)      749 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/text_unicode_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3203 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/devicetree_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4046 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.docx
--rw-r--r--   0 lamby     (1000) lamby     (1000)      428 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test_no_charset.mo
--rw-r--r--   0 lamby     (1000) lamby     (1000)    20480 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/fuzzy-tar-in-tar2.tar
--rw-r--r--   0 lamby     (1000) lamby     (1000)       13 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test_invalid.json
--rw-r--r--   0 lamby     (1000) lamby     (1000)       97 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.js
--rw-r--r--   0 lamby     (1000) lamby     (1000)      819 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test3.changes
--rw-r--r--   0 lamby     (1000) lamby     (1000)    49226 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/base-files_157-r45695_ar71xx.ipk
--rw-r--r--   0 lamby     (1000) lamby     (1000)      312 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/apk_zipinfo_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)   362501 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/debian-bug-875281.collapsed-diff.json
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/tests/data/dbgsym/
--rw-r--r--   0 lamby     (1000) lamby     (1000)      729 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/dbgsym/test-dbgsym_1.tar.gz
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/tests/data/dbgsym/add/
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2356 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/dbgsym/add/test-dbgsym_1_amd64.deb
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2628 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/dbgsym/add/test-dbgsym-dbgsym_1_amd64.deb
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-06-29 07:20:57.000000 diffoscope-98/tests/data/dbgsym/mult/
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2364 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/dbgsym/mult/test-dbgsym_1_amd64.deb
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2632 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/dbgsym/mult/test-dbgsym-dbgsym_1_amd64.deb
--rw-r--r--   0 lamby     (1000) lamby     (1000)      453 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/dbgsym/test-dbgsym_1.dsc
--rw-r--r--   0 lamby     (1000) lamby     (1000)      608 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/mo_charsets_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      533 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/jpeg_image_meta_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      627 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2_meta.jpg
--rw-r--r--   0 lamby     (1000) lamby     (1000)       92 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/order1.diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     6114 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.rpm
--rw-r--r--   0 lamby     (1000) lamby     (1000)      254 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/Test2.class
--rw-r--r--   0 lamby     (1000) lamby     (1000)     5660 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/jpeg_image_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4096 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.squashfs
--rwxr-xr-x   0 lamby     (1000) lamby     (1000)    24840 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.macho
--rw-r--r--   0 lamby     (1000) lamby     (1000)      443 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.mo
--rw-r--r--   0 lamby     (1000) lamby     (1000)       61 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/symlink_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      866 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.apk
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1150 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.ico
--rw-r--r--   0 lamby     (1000) lamby     (1000)      417 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test_xml_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      866 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.pgp
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1084 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/fontconfig_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      255 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/Test1.class
--rw-r--r--   0 lamby     (1000) lamby     (1000)      671 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/text_iso8859
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3072 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.binwalk
--rw-r--r--   0 lamby     (1000) lamby     (1000)      840 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.pdf
--rw-r--r--   0 lamby     (1000) lamby     (1000)    32768 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.db
--rw-r--r--   0 lamby     (1000) lamby     (1000)      706 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/android_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)       22 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/gnumeric_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      678 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/text_unicode2
--rw-r--r--   0 lamby     (1000) lamby     (1000)      700 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/text_ascii_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     5940 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.ogg
--rw-r--r--   0 lamby     (1000) lamby     (1000)    10240 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/archive1.tar
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1934 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/output.colored.txt
--rw-r--r--   0 lamby     (1000) lamby     (1000)     2193 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.debsrc.tar.gz
--rw-r--r--   0 lamby     (1000) lamby     (1000)    16384 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.db
--rw-r--r--   0 lamby     (1000) lamby     (1000)      626 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/dot_dsc_fallback_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      403 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/git_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1803 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.gnumeric
--rw-r--r--   0 lamby     (1000) lamby     (1000)       77 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/text_order_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1898 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/rlib_llvm_dis_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      552 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test2.mozzip
--rw-r--r--   0 lamby     (1000) lamby     (1000)      283 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test_invalid.xml
--rw-r--r--   0 lamby     (1000) lamby     (1000)      347 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/elf_lib_objdump_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)      571 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test3.apk
--rw-r--r--   0 lamby     (1000) lamby     (1000)      819 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.changes
--rw-r--r--   0 lamby     (1000) lamby     (1000)      165 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/sqlite3_expected_diff
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4096 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.squashfs
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3780 2018-06-29 07:18:59.000000 diffoscope-98/tests/data/test1.buildinfo
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1603 2018-06-29 07:18:59.000000 diffoscope-98/tests/test_readers.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     7752 2018-06-29 07:18:59.000000 diffoscope-98/tests/test_presenters.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     4697 2018-06-29 07:18:59.000000 diffoscope-98/tests/test_main.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)       38 2018-06-29 07:20:57.000000 diffoscope-98/setup.cfg
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       60 2018-01-29 11:36:33.000000 diffoscope-99/.coveragerc
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    35147 2016-12-25 23:50:38.000000 diffoscope-99/COPYING
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/tests/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1066 2018-03-09 19:00:00.000000 diffoscope-99/tests/test_source.py
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/tests/data/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      174 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/rpm_listing_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      865 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.pdf
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       46 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/symlink_expected_destination_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    15384 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test2-le64.cache-4
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    29784 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.ps
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3203 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/devicetree_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      586 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/cpio_listing_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      457 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/iso9660_content_expected_diff_cdrtools
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1546 2018-03-08 10:52:14.000000 diffoscope-99/tests/data/test1.xsb
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      362 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/pe_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      671 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/text_ascii2
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      532 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.xz
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      571 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.zip
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       92 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/order1.diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3765 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.buildinfo
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       18 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/docx_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     9734 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.rlib
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     5952 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/rpm_header_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      443 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.mo
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      744 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/text_iso8859_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      819 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test4.changes
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      403 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/git_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    85965 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test2.pcap
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      347 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/elf_lib_objdump_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     6926 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test1_meta.ico
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     6114 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.rpm
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2400 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.hi
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1803 2018-03-18 14:41:33.000000 diffoscope-99/tests/data/test1.gnumeric
+-rw-r--r--   0 mattia    (1000) mattia    (1000)  4208640 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/android1.img
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1546 2018-03-08 10:52:14.000000 diffoscope-99/tests/data/test2.xsb
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      450 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.dsc
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      293 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test1.xml
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      671 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/text_iso8859
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      634 2018-05-10 09:01:54.000000 diffoscope-99/tests/data/archive12.diff.txt
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       75 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/dot_changes_description_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       58 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/pdf_text_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      717 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/rlib_elf_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      398 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/ico_image_meta_expected_diff_v2
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      228 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/dot_changes_different_contents_and_identical_files_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    10240 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/fuzzy3.tar
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     7922 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test1.odt
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1803 2018-03-18 14:41:33.000000 diffoscope-99/tests/data/test2.gnumeric
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    14684 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.icc
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1354 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.a
+-rw-r--r--   0 mattia    (1000) mattia    (1000)   256000 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.ext4
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       92 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/ps_text_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      440 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/quine.zip
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      700 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/text_ascii_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      595 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test_openssh_pub_key1.pub
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      866 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test1.apk
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       80 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/binary_hexdump_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      767 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/mozzip_zipinfo_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      826 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.changes
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       16 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/binary2
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    68260 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/devicetree1.dtb
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      580 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/iso9660_rockridge_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      318 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test1.ico
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1354 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.a
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      154 2018-05-10 09:01:54.000000 diffoscope-99/tests/data/quine_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      312 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/apk_zipinfo_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      552 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.mozzip
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4322 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.hi
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2193 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.debsrc.tar.gz
+-rw-r--r--   0 mattia    (1000) mattia    (1000)   627936 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/pcap_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      443 2018-07-08 16:22:26.000000 diffoscope-99/tests/data/test1.lz4
+-rw-r--r--   0 mattia    (1000) mattia    (1000)   360448 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.iso
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/tests/data/containers/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      532 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/containers/b.tar.gz
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1112 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/containers/different_files_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      348 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/containers/a.tar.bz2
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       19 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/containers/magic_xz
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      404 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/containers/a.tar.xz
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      525 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/containers/b.tar.bz2
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       94 2018-05-10 09:01:54.000000 diffoscope-99/tests/data/containers/magic_gzip
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      616 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/containers/b.tar.xz
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      335 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/containers/a.tar.gz
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       41 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/containers/magic_bzip2
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      651 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/binwalk_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      254 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/Test2.class
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      706 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/android_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      644 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/quine_b.deb
+-rwxr-xr-x   0 mattia    (1000) mattia    (1000)     3072 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.exe
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1880 2018-03-18 14:41:33.000000 diffoscope-99/tests/data/dex_expected_diffs
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1262 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/dot_changes_fallback_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      163 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/png_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     9734 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.rlib
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       92 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.js
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       69 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.png
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      866 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test2.pgp
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      749 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/text_unicode_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      533 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/jpeg_image_meta_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      409 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.mozzip
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    68323 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/devicetree2.dtb
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    10240 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/no-perms.tar
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      409 2018-05-20 16:27:59.000000 diffoscope-99/tests/data/git_expected_diff_freebsd
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4567 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test2.ogg
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    84442 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test1.pcap
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    32768 2018-03-08 10:52:14.000000 diffoscope-99/tests/data/test1.db
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       43 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test_directory_device_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1757 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/output.txt
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      759 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/dot_buildinfo_fallback_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1024 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.cpio
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      298 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/dot_changes_identical_contents_and_different_files_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      731 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test_openssh_pub_key2.pub
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      493 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/iso9660_content_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)   286518 2018-05-20 16:27:59.000000 diffoscope-99/tests/data/test_weird_non_unicode_chars2.pdf
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2388 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.deb
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2116 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.dex
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      305 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.bz2
+-rwxr-xr-x   0 mattia    (1000) mattia    (1000)    24840 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.macho
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       26 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/odt_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4046 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test1.docx
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      193 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.git-index
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       22 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.json
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       29 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/order1b.json
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      714 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.zip
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4096 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.squashfs
+-rw-r--r--   0 mattia    (1000) mattia    (1000)   256000 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.ext4
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       35 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/text_order1
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       72 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/json_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3320 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.epub
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       41 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test_directory_file_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      202 2018-05-10 09:01:54.000000 diffoscope-99/tests/data/ipk_metadata_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    10240 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/fuzzy2.tar
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2094 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test4.gif
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      150 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/openssh_pub_key_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2086 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.debsrc.tar.gz
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     7767 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/rpm_fallback_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     5265 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.jpg
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      428 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test_no_charset.mo
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1898 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/rlib_llvm_dis_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3636 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/pgp_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       13 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test_invalid.json
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       77 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/text_order_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      458 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test_iso8859-1.mo
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     7745 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/haskell_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    49226 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/base-files_157-r45695_ar71xx.ipk
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      602 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/debian-bug-876316-control.tar.gz
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      250 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/quine.gz
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      637 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/rds_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1743 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/output.md
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    41435 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.ppu
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2141 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/device_expected_diff_reverse
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      864 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test2.apk
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       22 2018-03-18 14:41:33.000000 diffoscope-99/tests/data/gnumeric_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1084 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/fontconfig_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      644 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/quine_a.deb
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      283 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test_invalid.xml
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       35 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/text_order2
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       22 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.json
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4096 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.squashfs
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      793 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test2.gif
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      400 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/ico_image_meta_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1908 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/rlib_llvm_dis_expected_diff_5
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    14684 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.icc
+-rwxr-xr-x   0 mattia    (1000) mattia    (1000)     8432 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.macho
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      287 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.gz
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      571 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test3.zip
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      414 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/cbfs_listing_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3317 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.epub
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      819 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test3.changes
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    14208 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test1-le64.cache-4
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      538 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/iso9660_rockridge_expected_diff_cdrtools
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3072 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test2.binwalk
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3270 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test2_meta.ico
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2142 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/device_expected_diff_reverse_freebsd
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      795 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/tar_listing_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      450 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.dsc
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     6020 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.jpg
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      439 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/squashfs_superblock_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       97 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.js
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2218 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/text_unicode_binary_fallback
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1643 2018-03-08 10:52:14.000000 diffoscope-99/tests/data/berkeley_db_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    20480 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/fuzzy-tar-in-tar2.tar
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       61 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/symlink_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      631 2018-07-08 16:22:26.000000 diffoscope-99/tests/data/test2.lz4
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3346 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/epub_expected_diffs
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       29 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/order1a.json
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     7931 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test2.odt
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      284 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test2.xml
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      854 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test3.gif
+-rwxr-xr-x   0 mattia    (1000) mattia    (1000)     3072 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.exe
+-rw-r--r--   0 mattia    (1000) mattia    (1000)  4210688 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/android2.img
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    22251 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/ps_internal_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2141 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/device_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    16384 2018-03-08 10:52:14.000000 diffoscope-99/tests/data/test2.db
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      446 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/text_ascii1
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1716 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/bug881937_2.deb
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       69 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.png
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    10240 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/archive2.tar
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      417 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test_xml_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      571 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test3.apk
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      523 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/ext4_expected_diffs
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    49504 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/base-files_157-r45918_ar71xx.ipk
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    35903 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/ogg_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      186 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/zip_bsdtar_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      387 2018-03-18 14:41:33.000000 diffoscope-99/tests/data/javap_class_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      607 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/ppu_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      129 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.git-index
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4046 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test2.docx
+-rw-r--r--   0 mattia    (1000) mattia    (1000)   360448 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.iso
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1791 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test1.gif
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      627 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test2_meta.jpg
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4482 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/ico_image_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      672 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/text_unicode1
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    10240 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.tar
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      516 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/mo_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2048 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.sqlite3
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      397 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.mo
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    10240 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/fuzzy1.tar
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      430 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.gz
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    29922 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.ps
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1316 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/macho_expected_diff_disassembly
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    10240 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/archive1.tar
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      276 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test1.rdx
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      608 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/mo_charsets_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    46408 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/Samyak-Malayalam1.ttf
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     5975 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.rpm
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      846 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/apk_manifest_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       29 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/macho_expected_diff_arch
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      321 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/cbfs_listing_no_legacy_header_expected_diff
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/tests/data/dbgsym/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      453 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/dbgsym/test-dbgsym_1.dsc
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      729 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/dbgsym/test-dbgsym_1.tar.gz
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/tests/data/dbgsym/mult/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2632 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/dbgsym/mult/test-dbgsym-dbgsym_1_amd64.deb
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2364 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/dbgsym/mult/test-dbgsym_1_amd64.deb
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/tests/data/dbgsym/add/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2628 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/dbgsym/add/test-dbgsym-dbgsym_1_amd64.deb
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2356 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/dbgsym/add/test-dbgsym_1_amd64.deb
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1934 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/output.colored.txt
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      165 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/sqlite3_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)   286703 2018-05-20 16:27:59.000000 diffoscope-99/tests/data/test_weird_non_unicode_chars1.pdf
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      314 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/elf_lib_metadata_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      347 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/elf_obj_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     8932 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/ttf_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    14437 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/gif_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      388 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.xz
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2050 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/output.json
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     5940 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test1.ogg
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      866 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test1.pgp
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      626 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/dot_dsc_fallback_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)   362501 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/debian-bug-875281.collapsed-diff.json
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2262 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.deb
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      255 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/Test1.class
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2116 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.dex
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      215 2018-05-10 09:01:54.000000 diffoscope-99/tests/data/gzip_metadata_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      518 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/deb_metadata_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       16 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/binary1
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      349 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/quine_deb_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      662 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test1_meta.jpg
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    20480 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/fuzzy-tar-in-tar1.tar
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1216 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.o
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       44 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test_directory_symlink_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      276 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test2.rdx
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3072 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test1.binwalk
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3780 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.buildinfo
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     7808 2018-03-08 10:52:14.000000 diffoscope-99/tests/data/xsb_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      135 2018-03-08 10:52:14.000000 diffoscope-99/tests/data/procyon_class_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      840 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.pdf
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      150 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/binary_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      182 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/macho_expected_diff_loadcommands
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1646 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/bug881937_1.deb
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     5660 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/jpeg_image_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      395 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/rlib_armap_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      266 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/macho_expected_diff_headers
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      869 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/bug881937_control_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1024 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.cpio
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      516 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/icc_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2048 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.sqlite3
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      571 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/gnu_debuglink_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    10240 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test1.tar
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1864 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/output.rst
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      466 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.bz2
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      220 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/javascript_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      678 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/text_unicode2
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1216 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/test2.o
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1150 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/test2.ico
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2142 2018-01-29 11:36:33.000000 diffoscope-99/tests/data/device_expected_diff_freebsd
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    41435 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test2.ppu
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      423 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/zip_zipinfo_expected_diff
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    46408 2016-12-25 23:50:38.000000 diffoscope-99/tests/data/Samyak-Malayalam2.ttf
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      819 2017-01-14 10:59:14.000000 diffoscope-99/tests/data/test1.changes
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2546 2018-03-08 10:52:14.000000 diffoscope-99/tests/test_progress.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)        0 2018-01-29 11:36:33.000000 diffoscope-99/tests/__init__.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1603 2018-01-29 11:36:33.000000 diffoscope-99/tests/test_readers.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2292 2018-01-29 11:36:33.000000 diffoscope-99/tests/test_excludes.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     7752 2018-05-23 10:59:17.000000 diffoscope-99/tests/test_presenters.py
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/tests/comparators/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2145 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_device.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4789 2018-05-23 10:59:17.000000 diffoscope-99/tests/comparators/test_deb.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3503 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_apk.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2443 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_bzip2.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1659 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_pcap.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2310 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_epub.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3108 2018-05-23 10:59:17.000000 diffoscope-99/tests/comparators/test_text.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1477 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_xml.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2247 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_cpio.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4226 2018-05-23 10:59:17.000000 diffoscope-99/tests/comparators/test_utils.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1501 2018-05-20 16:27:59.000000 diffoscope-99/tests/comparators/test_git.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1640 2018-03-08 10:52:14.000000 diffoscope-99/tests/comparators/test_xsb.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3666 2018-05-23 10:59:17.000000 diffoscope-99/tests/comparators/test_rlib.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2009 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_ps.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2974 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_iso9660.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1917 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_json.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2374 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_xz.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2517 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_gif.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2123 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_png.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1187 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_archive.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2350 2018-03-08 11:27:07.000000 diffoscope-99/tests/comparators/test_macho.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1768 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_haskell.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2013 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_mono.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2989 2018-03-18 14:41:33.000000 diffoscope-99/tests/comparators/test_dex.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)        0 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/__init__.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2004 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_icc.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1655 2018-03-08 10:52:14.000000 diffoscope-99/tests/comparators/test_berkeley_db.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3371 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_rpm.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    11439 2018-05-23 10:59:17.000000 diffoscope-99/tests/comparators/test_debian.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2211 2018-05-23 10:59:17.000000 diffoscope-99/tests/comparators/test_android.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3727 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_cbfs.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3258 2018-05-10 09:01:54.000000 diffoscope-99/tests/comparators/test_gzip.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2242 2018-05-23 10:59:17.000000 diffoscope-99/tests/comparators/test_gettext.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1661 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_docx.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1855 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_fonts.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1640 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_odt.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2123 2018-05-10 09:01:54.000000 diffoscope-99/tests/comparators/test_ipk.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1640 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_ogg.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     6154 2018-05-23 10:59:17.000000 diffoscope-99/tests/comparators/test_elf.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1739 2018-03-18 14:41:33.000000 diffoscope-99/tests/comparators/test_gnumeric.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2517 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_ppu.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3046 2018-05-23 10:59:17.000000 diffoscope-99/tests/comparators/test_containers.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1852 2018-05-23 10:59:17.000000 diffoscope-99/tests/comparators/test_sqlite.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3224 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_jpeg_image.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2529 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_dtb.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2555 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_binwalk.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1958 2018-07-08 09:00:43.000000 diffoscope-99/tests/comparators/test_pdf.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2818 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_squashfs.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1426 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_fontconfig.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1685 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_rdata.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3647 2018-05-23 10:59:17.000000 diffoscope-99/tests/comparators/test_directory.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2370 2018-05-23 10:59:17.000000 diffoscope-99/tests/comparators/test_openssh_pub_key.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3446 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_zip.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3046 2018-03-18 14:41:33.000000 diffoscope-99/tests/comparators/test_java.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2408 2018-07-08 16:22:26.000000 diffoscope-99/tests/comparators/test_lz4.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1640 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_pgp.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1307 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_symlink.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3520 2018-05-23 10:59:17.000000 diffoscope-99/tests/comparators/test_fsimage.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     8346 2018-05-23 10:59:17.000000 diffoscope-99/tests/comparators/test_binary.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1963 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_javascript.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2704 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_tar.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2900 2018-01-29 11:36:33.000000 diffoscope-99/tests/comparators/test_ico_image.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2245 2018-05-10 09:01:54.000000 diffoscope-99/tests/test_quines.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1266 2018-07-08 16:22:26.000000 diffoscope-99/tests/test_tools.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4037 2018-05-23 10:59:17.000000 diffoscope-99/tests/test_difference.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4697 2018-05-23 10:59:17.000000 diffoscope-99/tests/test_main.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1893 2018-07-08 09:00:43.000000 diffoscope-99/tests/conftest.py
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/tests/utils/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1664 2018-05-23 10:59:17.000000 diffoscope-99/tests/utils/__init__.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1396 2018-01-29 11:36:33.000000 diffoscope-99/tests/utils/nonexisting.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4734 2018-05-23 10:59:17.000000 diffoscope-99/tests/utils/tools.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2177 2018-01-29 11:36:33.000000 diffoscope-99/tests/utils/data.py
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/diffoscope/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    12215 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/difference.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1030 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/path.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3173 2018-03-08 10:52:14.000000 diffoscope-99/diffoscope/config.py
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/diffoscope/presenters/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3661 2018-07-08 09:00:43.000000 diffoscope-99/diffoscope/presenters/formats.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3022 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/presenters/text.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    13562 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/presenters/utils.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)        0 2017-09-09 20:38:24.000000 diffoscope-99/diffoscope/presenters/__init__.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1874 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/presenters/restructuredtext.py
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/diffoscope/presenters/html/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    30572 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/presenters/html/html.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      875 2018-03-08 10:52:14.000000 diffoscope-99/diffoscope/presenters/html/__init__.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     6640 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/presenters/html/templates.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1638 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/presenters/markdown.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1369 2017-09-09 20:38:24.000000 diffoscope-99/diffoscope/presenters/icon.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2141 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/presenters/json.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2747 2018-07-08 13:41:44.000000 diffoscope-99/diffoscope/tempfiles.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      805 2018-07-08 18:15:03.000000 diffoscope-99/diffoscope/__init__.py
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/diffoscope/comparators/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1387 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/mono.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1379 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/ogg.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2414 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/png.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2107 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/symlink.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1909 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/xz.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    18332 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/elf.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3139 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/fsimage.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     8933 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/squashfs.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2932 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/java.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1746 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/berkeley_db.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3326 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/comparators/binwalk.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2826 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/text.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1316 2018-07-08 09:00:43.000000 diffoscope-99/diffoscope/comparators/pdf.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1772 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/bzip2.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     6537 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/apk.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4651 2018-07-08 16:22:26.000000 diffoscope-99/diffoscope/comparators/__init__.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1890 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/llvm.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1344 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/openssh.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3602 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/xml.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2784 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/device.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1706 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/ps.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1936 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/debian_fallback.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1801 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/dex.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      982 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/ipk.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1313 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/javascript.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1914 2018-07-08 16:22:26.000000 diffoscope-99/diffoscope/comparators/lz4.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2720 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/fontconfig.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2748 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/ar.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2663 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/git.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1449 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/docx.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     5859 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/zip.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1620 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/pcap.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1331 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/sqlite.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1432 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/tar.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1893 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/gzip.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2437 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/rust.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1925 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/gnumeric.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3096 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/rdata.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1482 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/xsb.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2528 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/android.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1422 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/fonts.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1408 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/dtb.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4625 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/macho.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3638 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/ppu.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     8708 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/debian.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1625 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/pgp.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     9291 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/directory.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1450 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/odt.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3185 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/comparators/missing_file.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2338 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/gettext.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3451 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/rpm.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     5145 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/cbfs.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1351 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/comparators/binary.py
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/diffoscope/comparators/utils/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    10630 2018-07-08 16:22:26.000000 diffoscope-99/diffoscope/comparators/utils/libarchive.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)        0 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/comparators/utils/__init__.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4273 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/utils/archive.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     7134 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/utils/container.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3250 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/utils/command.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2254 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/utils/specialize.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2027 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/utils/fuzzy.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4952 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/utils/compare.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    15897 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/utils/file.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1215 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/rpm_fallback.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4958 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/haskell.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3021 2018-07-08 09:00:43.000000 diffoscope-99/diffoscope/comparators/json.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1342 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/icc.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     7458 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/comparators/deb.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3319 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/iso9660.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1414 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/cpio.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     6913 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/image.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3152 2018-03-29 09:43:55.000000 diffoscope-99/diffoscope/comparators/gif.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     8515 2018-07-08 16:22:26.000000 diffoscope-99/diffoscope/progress.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1417 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/exc.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    20465 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/diff.py
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/diffoscope/readers/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      835 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/readers/utils.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1025 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/readers/__init__.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1815 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/readers/json.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2195 2018-07-08 16:22:26.000000 diffoscope-99/diffoscope/logging.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3322 2018-03-08 10:52:14.000000 diffoscope-99/diffoscope/feeders.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3865 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/tools.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1600 2018-05-23 10:59:17.000000 diffoscope-99/diffoscope/excludes.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    24105 2018-07-08 16:25:49.000000 diffoscope-99/diffoscope/main.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     6798 2018-07-08 17:37:29.000000 diffoscope-99/diffoscope/external_tools.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    11361 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/changes.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     2918 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/profiling.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1507 2018-01-29 11:36:33.000000 diffoscope-99/diffoscope/locale.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3883 2017-01-14 10:59:14.000000 diffoscope-99/logo.svg
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3196 2018-06-15 07:25:49.000000 diffoscope-99/CONTRIBUTING.rst
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     4332 2018-01-29 11:36:33.000000 diffoscope-99/README.rst
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/diffoscope.egg-info/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)        1 2018-07-08 18:21:59.000000 diffoscope-99/diffoscope.egg-info/dependency_links.txt
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    14640 2018-07-08 18:21:59.000000 diffoscope-99/diffoscope.egg-info/SOURCES.txt
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       53 2018-07-08 18:21:59.000000 diffoscope-99/diffoscope.egg-info/requires.txt
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       11 2018-07-08 18:21:59.000000 diffoscope-99/diffoscope.egg-info/top_level.txt
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       53 2018-07-08 18:21:59.000000 diffoscope-99/diffoscope.egg-info/entry_points.txt
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     6068 2018-07-08 18:21:59.000000 diffoscope-99/diffoscope.egg-info/PKG-INFO
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/debian/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3103 2018-07-08 17:34:20.000000 diffoscope-99/debian/control
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/debian/tests/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      817 2018-07-08 17:38:25.000000 diffoscope-99/debian/tests/control
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      226 2018-07-08 16:58:44.000000 diffoscope-99/debian/tests/control.in
+-rwxr-xr-x   0 mattia    (1000) mattia    (1000)     1386 2017-01-14 10:59:14.000000 diffoscope-99/debian/tests/basic-command-line
+-rwxr-xr-x   0 mattia    (1000) mattia    (1000)      174 2018-01-29 11:36:33.000000 diffoscope-99/debian/tests/pytest-with-recommends
+-rwxr-xr-x   0 mattia    (1000) mattia    (1000)      174 2018-01-29 11:36:33.000000 diffoscope-99/debian/tests/pytest
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/debian/upstream/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    15660 2018-01-29 11:36:33.000000 diffoscope-99/debian/upstream/signing-key.asc
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      304 2018-01-29 11:36:33.000000 diffoscope-99/debian/README.source
+-rw-r--r--   0 mattia    (1000) mattia    (1000)    98006 2018-07-08 18:15:03.000000 diffoscope-99/debian/changelog
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      220 2018-01-29 11:36:33.000000 diffoscope-99/debian/gbp.conf
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     5134 2018-05-20 16:27:59.000000 diffoscope-99/debian/copyright
+-rwxr-xr-x   0 mattia    (1000) mattia    (1000)     3220 2018-07-08 18:14:29.000000 diffoscope-99/debian/rules
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       83 2018-03-08 10:52:14.000000 diffoscope-99/debian/clean
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       11 2017-01-14 10:59:14.000000 diffoscope-99/debian/diffoscope.docs
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/debian/source/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      299 2017-01-14 10:59:14.000000 diffoscope-99/debian/source/options
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      137 2018-01-29 11:36:33.000000 diffoscope-99/debian/source/lintian-overrides
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       13 2016-12-25 23:50:38.000000 diffoscope-99/debian/source/format
+-rw-r--r--   0 mattia    (1000) mattia    (1000)        3 2018-01-29 11:36:33.000000 diffoscope-99/debian/compat
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       23 2017-01-14 10:59:14.000000 diffoscope-99/debian/diffoscope.install
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       17 2018-01-29 11:36:33.000000 diffoscope-99/debian/diffoscope.manpages
+-rwxr-xr-x   0 mattia    (1000) mattia    (1000)      377 2017-01-14 10:59:14.000000 diffoscope-99/debian/check-dep-sizes.sh
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       95 2018-05-20 16:27:59.000000 diffoscope-99/debian/watch
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       80 2017-01-14 10:59:14.000000 diffoscope-99/debian/py3dist-overrides
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/bin/
+-rwxr-xr-x   0 mattia    (1000) mattia    (1000)     1269 2017-09-09 20:38:26.000000 diffoscope-99/bin/diffoscope
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      174 2018-01-29 11:36:33.000000 diffoscope-99/.travis.yml
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     6068 2018-07-08 18:21:59.000000 diffoscope-99/PKG-INFO
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2018-07-08 18:21:59.000000 diffoscope-99/doc/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)      280 2018-01-29 11:36:33.000000 diffoscope-99/doc/diffoscope.h2m.0
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1044 2018-04-05 22:05:45.000000 diffoscope-99/doc/Makefile
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       47 2017-01-14 10:59:14.000000 diffoscope-99/MANIFEST.in
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     1910 2018-05-23 10:59:17.000000 diffoscope-99/setup.py
+-rw-r--r--   0 mattia    (1000) mattia    (1000)       38 2018-07-08 18:21:59.000000 diffoscope-99/setup.cfg
```

### Comparing `diffoscope-98/diffoscope/__init__.py` & `diffoscope-99/diffoscope/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffoscope.  If not, see <https://www.gnu.org/licenses/>.
 
-VERSION = "98"
+VERSION = "99"
```

### Comparing `diffoscope-98/diffoscope/comparators/tar.py` & `diffoscope-99/diffoscope/comparators/tar.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/sqlite.py` & `diffoscope-99/diffoscope/comparators/sqlite.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/image.py` & `diffoscope-99/diffoscope/comparators/image.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/fonts.py` & `diffoscope-99/diffoscope/comparators/fonts.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/docx.py` & `diffoscope-99/diffoscope/comparators/docx.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/deb.py` & `diffoscope-99/diffoscope/comparators/deb.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/__init__.py` & `diffoscope-99/diffoscope/comparators/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,21 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffoscope.  If not, see <https://www.gnu.org/licenses/>.
 
+import sys
 import logging
 import importlib
+import traceback
+
+from ..logging import line_ereser
+
 
 logger = logging.getLogger(__name__)
 
 
 class ComparatorManager(object):
     COMPARATORS = (
         ('directory.Directory',),
@@ -60,14 +65,15 @@
         ('rust.RustObjectFile',),
         ('gnumeric.GnumericFile',),
         ('gzip.GzipFile',),
         ('haskell.HiFile',),
         ('icc.IccFile',),
         ('iso9660.Iso9660File',),
         ('java.ClassFile',),
+        ('lz4.Lz4File',),
         ('mono.MonoExeFile',),
         ('pdf.PdfFile',),
         ('png.PngFile',),
         ('ppu.PpuFile',),
         ('rdata.RdbFile',),
         ('rdata.RdsFile',),
         ('rpm.RpmFile', 'rpm_fallback.RpmFile'),
@@ -103,31 +109,38 @@
         if not self._singleton:
             self.reload()
 
     def reload(self):
         self.classes = []
 
         for xs in self.COMPARATORS:
+            errors = []
             for x in xs:
                 package, klass_name = x.rsplit('.', 1)
 
                 try:
                     mod = importlib.import_module(
                         'diffoscope.comparators.{}'.format(package)
                     )
-                except ImportError:
+                except ImportError as e:
+                    errors.append((x, e))
                     continue
 
                 self.classes.append(getattr(mod, klass_name))
                 break
             else:  # noqa
-                raise ImportError("Could not import {}{}".format(
-                    "any of" if len(xs) > 1 else '',
+                logger.error("Could not import {}{}".format(
+                    "any of " if len(xs) > 1 else '',
                     ', '.join(xs)
                 ))
+                for x in errors:
+                    logger.error("Original error for %s:", x[0])
+                    sys.stderr.buffer.write(line_ereser())
+                    traceback.print_exception(None, x[1], x[1].__traceback__)
+                sys.exit(2)
 
         logger.debug("Loaded %d comparator classes", len(self.classes))
 
     def get_descriptions(self):
         for x in self.classes:
             try:
                 yield x.DESCRIPTION
```

### Comparing `diffoscope-98/diffoscope/comparators/rpm.py` & `diffoscope-99/diffoscope/comparators/rpm.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/utils/command.py` & `diffoscope-99/diffoscope/comparators/utils/command.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/utils/specialize.py` & `diffoscope-99/diffoscope/comparators/utils/specialize.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/utils/libarchive.py` & `diffoscope-99/diffoscope/comparators/utils/libarchive.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,14 +76,22 @@
     libarchive.ArchiveEntry.uname = property(
         lambda self: libarchive.ffi.entry_uname(self._entry_p))
 if not hasattr(libarchive.ffi, 'entry_gname'):
     libarchive.ffi.ffi(
         'entry_gname', [libarchive.ffi.c_archive_entry_p], ctypes.c_char_p)
     libarchive.ArchiveEntry.gname = property(
         lambda self: libarchive.ffi.entry_gname(self._entry_p))
+# Monkeypatch libarchive-c (>= 2.8)
+# Wire mtime_nsec attribute as some libarchive versions (>=2.8) don't expose it
+# for ArchiveEntry. Doing this allows a unified API no matter which version is
+# available.
+if not hasattr(libarchive.ArchiveEntry, 'mtime_nsec') and hasattr(libarchive.ffi, 'entry_mtime_nsec'):
+    libarchive.ArchiveEntry.mtime_nsec = property(
+        lambda self: libarchive.ffi.entry_mtime_nsec(self._entry_p))
+
 
 # Monkeypatch libarchive-c so we always get pathname as (Unicode) str
 # Otherwise, we'll get sometimes str and sometimes bytes and always pain.
 libarchive.ArchiveEntry.pathname = property(lambda self: libarchive.ffi.entry_pathname(
     self._entry_p).decode('utf-8', errors='surrogateescape'))
```

### Comparing `diffoscope-98/diffoscope/comparators/utils/archive.py` & `diffoscope-99/diffoscope/comparators/utils/archive.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/utils/compare.py` & `diffoscope-99/diffoscope/comparators/utils/compare.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/utils/container.py` & `diffoscope-99/diffoscope/comparators/utils/container.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/utils/file.py` & `diffoscope-99/diffoscope/comparators/utils/file.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/utils/fuzzy.py` & `diffoscope-99/diffoscope/comparators/utils/fuzzy.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/android.py` & `diffoscope-99/diffoscope/comparators/android.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/rust.py` & `diffoscope-99/diffoscope/comparators/rust.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/ar.py` & `diffoscope-99/diffoscope/comparators/ar.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/directory.py` & `diffoscope-99/diffoscope/comparators/directory.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/debian.py` & `diffoscope-99/diffoscope/comparators/debian.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/pcap.py` & `diffoscope-99/diffoscope/comparators/pcap.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/berkeley_db.py` & `diffoscope-99/diffoscope/comparators/berkeley_db.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/pdf.py` & `diffoscope-99/diffoscope/comparators/pdf.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/elf.py` & `diffoscope-99/diffoscope/comparators/elf.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/apk.py` & `diffoscope-99/diffoscope/comparators/apk.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/fontconfig.py` & `diffoscope-99/diffoscope/comparators/fontconfig.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/icc.py` & `diffoscope-99/diffoscope/comparators/icc.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/png.py` & `diffoscope-99/diffoscope/comparators/png.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/squashfs.py` & `diffoscope-99/diffoscope/comparators/squashfs.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/pgp.py` & `diffoscope-99/diffoscope/comparators/pgp.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/missing_file.py` & `diffoscope-99/diffoscope/comparators/missing_file.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/debian_fallback.py` & `diffoscope-99/diffoscope/comparators/debian_fallback.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/openssh.py` & `diffoscope-99/diffoscope/comparators/openssh.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/device.py` & `diffoscope-99/diffoscope/comparators/device.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/dex.py` & `diffoscope-99/diffoscope/comparators/dex.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/ppu.py` & `diffoscope-99/diffoscope/comparators/ppu.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/iso9660.py` & `diffoscope-99/diffoscope/comparators/iso9660.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/ps.py` & `diffoscope-99/diffoscope/comparators/ps.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/json.py` & `diffoscope-99/diffoscope/comparators/json.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/rpm_fallback.py` & `diffoscope-99/diffoscope/comparators/rpm_fallback.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/haskell.py` & `diffoscope-99/diffoscope/comparators/haskell.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/cpio.py` & `diffoscope-99/diffoscope/comparators/cpio.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/symlink.py` & `diffoscope-99/diffoscope/comparators/symlink.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/git.py` & `diffoscope-99/diffoscope/comparators/git.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/text.py` & `diffoscope-99/diffoscope/comparators/text.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/javascript.py` & `diffoscope-99/diffoscope/comparators/javascript.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/dtb.py` & `diffoscope-99/diffoscope/comparators/dtb.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/gnumeric.py` & `diffoscope-99/diffoscope/comparators/gnumeric.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/xsb.py` & `diffoscope-99/diffoscope/comparators/xsb.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/xml.py` & `diffoscope-99/diffoscope/comparators/xml.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/xz.py` & `diffoscope-99/diffoscope/comparators/xz.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/llvm.py` & `diffoscope-99/diffoscope/comparators/llvm.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/mono.py` & `diffoscope-99/diffoscope/comparators/mono.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/cbfs.py` & `diffoscope-99/diffoscope/comparators/cbfs.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/rdata.py` & `diffoscope-99/diffoscope/comparators/rdata.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/gettext.py` & `diffoscope-99/diffoscope/comparators/gettext.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/binwalk.py` & `diffoscope-99/diffoscope/comparators/binwalk.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/ogg.py` & `diffoscope-99/diffoscope/comparators/ogg.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/gzip.py` & `diffoscope-99/diffoscope/comparators/gzip.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/odt.py` & `diffoscope-99/diffoscope/comparators/odt.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/binary.py` & `diffoscope-99/diffoscope/comparators/binary.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/java.py` & `diffoscope-99/diffoscope/comparators/java.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/fsimage.py` & `diffoscope-99/diffoscope/comparators/fsimage.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/gif.py` & `diffoscope-99/diffoscope/comparators/gif.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/zip.py` & `diffoscope-99/diffoscope/comparators/zip.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/ipk.py` & `diffoscope-99/diffoscope/comparators/ipk.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/bzip2.py` & `diffoscope-99/diffoscope/comparators/bzip2.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/comparators/macho.py` & `diffoscope-99/diffoscope/comparators/macho.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/tools.py` & `diffoscope-99/diffoscope/tools.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/feeders.py` & `diffoscope-99/diffoscope/feeders.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/external_tools.py` & `diffoscope-99/diffoscope/external_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,18 @@
         'arch': 'coreutils',
     },
     'lsattr': {
         'debian': 'e2fsprogs',
         'arch': 'e2fsprogs',
         'FreeBSD': 'e2fsprogs',
     },
+    'lz4': {
+        'debian': 'lz4',
+        'FreeBSD': 'lz4',
+    },
     'msgunfmt': {
         'debian': 'gettext',
         'arch': 'gettext',
         'FreeBSD': 'gettext-tools',
     },
     'convert': {
         'debian': 'imagemagick',
@@ -260,15 +264,15 @@
         'arch': 'unzip',
         'FreeBSD': 'unzip',
     },
     'procyon-decompiler': {
         'debian': 'procyon-decompiler',
     },
     'dumpxsb': {
-        'debian': 'xmlutils',
+        'debian': 'xmlbeans',
     },
 }
 
 # May be populated at runtime by remapped names like
 # readelf -> arm-none-eabi-readelf, etc
 # diff -> gdiff, etc
 REMAPPED_TOOL_NAMES = {}
```

### Comparing `diffoscope-98/diffoscope/profiling.py` & `diffoscope-99/diffoscope/profiling.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/exc.py` & `diffoscope-99/diffoscope/exc.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/logging.py` & `diffoscope-99/diffoscope/logging.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,29 +13,47 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffoscope.  If not, see <https://www.gnu.org/licenses/>.
 
+import sys
 import contextlib
 import logging
 
 
+def line_ereser(fd=sys.stderr) -> bytes:
+    ereser = b''  # avoid None to avoid 'NoneType + str/bytes' failures
+    if fd.isatty():
+        from curses import tigetstr, setupterm
+        setupterm(fd=fd.fileno())
+        ereser = tigetstr('el')
+
+    if not ereser and fd.isatty():
+        # is a tty, but doesn't support the proper scape code, so let's fake it
+        from shutil import get_terminal_size
+        width = get_terminal_size().columns
+        ereser = b'\r{}\r'.format(b' ' * width)
+
+    return ereser
+
+
 @contextlib.contextmanager
 def setup_logging(debug, log_handler):
     logger = logging.getLogger()
     old_level = logger.getEffectiveLevel()
     logger.setLevel(logging.DEBUG if debug else logging.WARNING)
 
     ch = log_handler or logging.StreamHandler()
     ch.setLevel(logging.DEBUG)
     logger.addHandler(ch)
 
     formatter = logging.Formatter(
+        line_ereser().decode('ascii') +
         '%(asctime)s %(levelname).1s: %(name)s: %(message)s',
         '%Y-%m-%d %H:%M:%S',
     )
     ch.setFormatter(formatter)
     try:
         yield logger
     finally:
```

### Comparing `diffoscope-98/diffoscope/tempfiles.py` & `diffoscope-99/diffoscope/tempfiles.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # diffoscope: in-depth comparison of files, archives, and directories
 #
 # Copyright © 2016 Chris Lamb <lamby@debian.org>
+#           © 2018 Mattia Rizzolo <mattia@debian.org>
 #
 # diffoscope is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # diffoscope is distributed in the hope that it will be useful,
@@ -23,26 +24,24 @@
 
 _DIRS, _FILES = [], []
 
 logger = logging.getLogger(__name__)
 
 
 def get_named_temporary_file(*args, **kwargs):
-    kwargs['dir'] = _get_base_temporary_directory()
-    kwargs['suffix'] = kwargs.pop('suffix', '_diffoscope')
+    kwargs['dir'] = kwargs.pop('dir', _get_base_temporary_directory())
 
     f = tempfile.NamedTemporaryFile(*args, **kwargs)
     _FILES.append(f.name)
 
     return f
 
 
 def get_temporary_directory(*args, **kwargs):
-    kwargs['dir'] = _get_base_temporary_directory()
-    kwargs['suffix'] = kwargs.pop('suffix', '_diffoscope')
+    kwargs['dir'] = kwargs.pop('dir', _get_base_temporary_directory())
 
     d = tempfile.TemporaryDirectory(*args, **kwargs)
     _DIRS.append(d)
 
     return d
 
 
@@ -52,14 +51,15 @@
     for x in _FILES:
         try:
             os.unlink(x)
         except FileNotFoundError:
             pass
         except:
             logger.exception("Unable to delete %s", x)
+    _FILES.clear()
 
     logger.debug("Cleaning %d temporary directories", len(_DIRS))
 
     # Reverse so we delete the top-level directory last.
     for x in reversed(_DIRS):
         try:
             x.cleanup()
@@ -72,21 +72,22 @@
                     os.chmod(os.path.join(dirpath, y), 0o777)
             # try removing it again now
             x.cleanup()
         except FileNotFoundError:
             pass
         except:
             logger.exception("Unable to delete %s", x)
+    _DIRS.clear()
 
 
 def _get_base_temporary_directory():
     if not _DIRS:
         d = tempfile.TemporaryDirectory(
             dir=tempfile.gettempdir(),
-            prefix='diffoscope-',
+            prefix='diffoscope_',
         )
 
         logger.debug("Created top-level temporary directory: %s", d.name)
 
         _DIRS.append(d)
 
     return _DIRS[0].name
```

### Comparing `diffoscope-98/diffoscope/progress.py` & `diffoscope-99/diffoscope/progress.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # diffoscope: in-depth comparison of files, archives, and directories
 #
 # Copyright © 2016 Chris Lamb <lamby@debian.org>
+# Copyright © 2018 Paul Wise <pabs@debian.org>
 #
 # diffoscope is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # diffoscope is distributed in the hope that it will be useful,
@@ -16,29 +17,30 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with diffoscope.  If not, see <https://www.gnu.org/licenses/>.
 
 import os
 import sys
 import json
+import signal
 import logging
 
+from .logging import line_ereser
+
+
 logger = logging.getLogger(__name__)
 
 
 class ProgressLoggingHandler(logging.StreamHandler):
     def __init__(self, progressbar):
         self.progressbar = progressbar
         super().__init__()
 
     def emit(self, record):
         try:
-            # Delete the current line (i.e. the progress bar)
-            self.stream.write("\r\033[K")
-            self.flush()
             super().emit(record)
             if not self.progressbar.bar.finished:
                 self.progressbar.bar.update()
         except Exception:
             # Wrap otherwise tests fail due to test_progress.py call main()
             # several times. This mirrors the super() implementation.
             self.handleError(record)
@@ -211,18 +213,33 @@
                 return '…{}'.format(msg[-width + 1:])
 
         class OurProgressBar(progressbar.ProgressBar):
             def __init__(self, *args, **kwargs):
                 # Remove after https://github.com/niltonvolpato/python-progressbar/pull/57 is fixed.
                 kwargs.setdefault('fd', sys.stderr)
                 super().__init__(*args, **kwargs)
+                # Terminal handling after parent init since that sets self.fd
+                self.erase_to_eol = line_ereser(self.fd)
 
             def _need_update(self):
                 return True
 
+            def erase_line(self):
+                if self.erase_to_eol:
+                    self.fd.buffer.write(self.erase_to_eol)
+                    self.fd.flush()
+
+            def finish(self):
+                self.finished = True
+                self.update(self.maxval)
+                # Clear the progress bar after completion
+                self.erase_line()
+                if self.signal_set:
+                    signal.signal(signal.SIGWINCH, signal.SIG_DFL)
+
         self.bar = OurProgressBar(widgets=(
             ' ',
             progressbar.Bar(),
             '  ',
             progressbar.Percentage(),
             '  ',
             Message(),
```

### Comparing `diffoscope-98/diffoscope/config.py` & `diffoscope-99/diffoscope/config.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/excludes.py` & `diffoscope-99/diffoscope/excludes.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/difference.py` & `diffoscope-99/diffoscope/difference.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/locale.py` & `diffoscope-99/diffoscope/locale.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/changes.py` & `diffoscope-99/diffoscope/changes.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/presenters/utils.py` & `diffoscope-99/diffoscope/presenters/utils.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/presenters/html/html.py` & `diffoscope-99/diffoscope/presenters/html/html.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/presenters/html/__init__.py` & `diffoscope-99/diffoscope/presenters/html/__init__.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/presenters/html/templates.py` & `diffoscope-99/diffoscope/presenters/html/templates.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/presenters/markdown.py` & `diffoscope-99/diffoscope/presenters/markdown.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/presenters/restructuredtext.py` & `diffoscope-99/diffoscope/presenters/restructuredtext.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/presenters/icon.py` & `diffoscope-99/diffoscope/presenters/icon.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/presenters/json.py` & `diffoscope-99/diffoscope/presenters/json.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/presenters/text.py` & `diffoscope-99/diffoscope/presenters/text.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/presenters/formats.py` & `diffoscope-99/diffoscope/presenters/formats.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/path.py` & `diffoscope-99/diffoscope/path.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/main.py` & `diffoscope-99/diffoscope/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import traceback
 
 from . import VERSION
 from .path import set_path
 from .tools import tool_prepend_prefix, tool_required, OS_NAMES, get_current_os
 from .config import Config
 from .locale import set_locale
-from .logging import setup_logging
+from .logging import line_ereser, setup_logging
 from .progress import ProgressManager, Progress
 from .profiling import ProfileManager, profile
 from .tempfiles import clean_all_temp_files
 from .difference import Difference
 from .comparators import ComparatorManager
 from .external_tools import EXTERNAL_TOOLS
 from .presenters.html import JQUERY_SYSTEM_LOCATIONS
@@ -455,19 +455,20 @@
             parser, post_parse = create_parser()
             parsed_args = parser.parse_args(args)
         log_handler = ProgressManager().setup(parsed_args)
         with setup_logging(parsed_args.debug, log_handler) as logger:
             post_parse(parsed_args)
             sys.exit(run_diffoscope(parsed_args))
     except KeyboardInterrupt:
-        logger.info('Keyboard Interrupt')
+        logger.error('Keyboard Interrupt')
         sys.exit(2)
     except BrokenPipeError:
         sys.exit(2)
     except Exception:
+        sys.stderr.buffer.write(line_ereser())
         traceback.print_exc()
         if parsed_args and parsed_args.debugger:
             import pdb
             pdb.post_mortem()
         sys.exit(2)
     finally:
         # Helps our tests run more predictably - some of them call main()
```

### Comparing `diffoscope-98/diffoscope/diff.py` & `diffoscope-99/diffoscope/diff.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/readers/utils.py` & `diffoscope-99/diffoscope/readers/utils.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/readers/__init__.py` & `diffoscope-99/diffoscope/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope/readers/json.py` & `diffoscope-99/diffoscope/readers/json.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/setup.py` & `diffoscope-99/setup.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/diffoscope.egg-info/SOURCES.txt` & `diffoscope-99/diffoscope.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,39 @@
+.coveragerc
+.travis.yml
+CONTRIBUTING.rst
 COPYING
 MANIFEST.in
 README.rst
+logo.svg
 setup.py
+bin/diffoscope
+debian/README.source
+debian/changelog
+debian/check-dep-sizes.sh
+debian/clean
+debian/compat
+debian/control
+debian/copyright
+debian/diffoscope.docs
+debian/diffoscope.install
+debian/diffoscope.manpages
+debian/gbp.conf
+debian/py3dist-overrides
+debian/rules
+debian/watch
+debian/source/format
+debian/source/lintian-overrides
+debian/source/options
+debian/tests/basic-command-line
+debian/tests/control
+debian/tests/control.in
+debian/tests/pytest
+debian/tests/pytest-with-recommends
+debian/upstream/signing-key.asc
 diffoscope/__init__.py
 diffoscope/changes.py
 diffoscope/config.py
 diffoscope/diff.py
 diffoscope/difference.py
 diffoscope/exc.py
 diffoscope/excludes.py
@@ -57,14 +85,15 @@
 diffoscope/comparators/image.py
 diffoscope/comparators/ipk.py
 diffoscope/comparators/iso9660.py
 diffoscope/comparators/java.py
 diffoscope/comparators/javascript.py
 diffoscope/comparators/json.py
 diffoscope/comparators/llvm.py
+diffoscope/comparators/lz4.py
 diffoscope/comparators/macho.py
 diffoscope/comparators/missing_file.py
 diffoscope/comparators/mono.py
 diffoscope/comparators/odt.py
 diffoscope/comparators/ogg.py
 diffoscope/comparators/openssh.py
 diffoscope/comparators/pcap.py
@@ -105,14 +134,16 @@
 diffoscope/presenters/utils.py
 diffoscope/presenters/html/__init__.py
 diffoscope/presenters/html/html.py
 diffoscope/presenters/html/templates.py
 diffoscope/readers/__init__.py
 diffoscope/readers/json.py
 diffoscope/readers/utils.py
+doc/Makefile
+doc/diffoscope.h2m.0
 tests/__init__.py
 tests/conftest.py
 tests/test_difference.py
 tests/test_excludes.py
 tests/test_main.py
 tests/test_presenters.py
 tests/test_progress.py
@@ -153,14 +184,15 @@
 tests/comparators/test_ico_image.py
 tests/comparators/test_ipk.py
 tests/comparators/test_iso9660.py
 tests/comparators/test_java.py
 tests/comparators/test_javascript.py
 tests/comparators/test_jpeg_image.py
 tests/comparators/test_json.py
+tests/comparators/test_lz4.py
 tests/comparators/test_macho.py
 tests/comparators/test_mono.py
 tests/comparators/test_odt.py
 tests/comparators/test_ogg.py
 tests/comparators/test_openssh_pub_key.py
 tests/comparators/test_pcap.py
 tests/comparators/test_pdf.py
@@ -328,14 +360,15 @@
 tests/data/test1.hi
 tests/data/test1.icc
 tests/data/test1.ico
 tests/data/test1.iso
 tests/data/test1.jpg
 tests/data/test1.js
 tests/data/test1.json
+tests/data/test1.lz4
 tests/data/test1.macho
 tests/data/test1.mo
 tests/data/test1.mozzip
 tests/data/test1.o
 tests/data/test1.odt
 tests/data/test1.ogg
 tests/data/test1.pcap
@@ -380,14 +413,15 @@
 tests/data/test2.hi
 tests/data/test2.icc
 tests/data/test2.ico
 tests/data/test2.iso
 tests/data/test2.jpg
 tests/data/test2.js
 tests/data/test2.json
+tests/data/test2.lz4
 tests/data/test2.macho
 tests/data/test2.mo
 tests/data/test2.mozzip
 tests/data/test2.o
 tests/data/test2.odt
 tests/data/test2.ogg
 tests/data/test2.pcap
```

### Comparing `diffoscope-98/diffoscope.egg-info/PKG-INFO` & `diffoscope-99/diffoscope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffoscope
-Version: 98
+Version: 99
 Summary: in-depth comparison of files, archives, and directories
 Home-page: https://diffoscope.org/
 Author: Lunar
 Author-email: lunar@debian.org
 License: GPL-3+
 Description: diffoscope
         ==========
```

### Comparing `diffoscope-98/README.rst` & `diffoscope-99/README.rst`

 * *Files identical despite different names*

### Comparing `diffoscope-98/PKG-INFO` & `diffoscope-99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffoscope
-Version: 98
+Version: 99
 Summary: in-depth comparison of files, archives, and directories
 Home-page: https://diffoscope.org/
 Author: Lunar
 Author-email: lunar@debian.org
 License: GPL-3+
 Description: diffoscope
         ==========
```

### Comparing `diffoscope-98/COPYING` & `diffoscope-99/COPYING`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_ppu.py` & `diffoscope-99/tests/comparators/test_ppu.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_android.py` & `diffoscope-99/tests/comparators/test_android.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_directory.py` & `diffoscope-99/tests/comparators/test_directory.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_docx.py` & `diffoscope-99/tests/comparators/test_docx.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_gnumeric.py` & `diffoscope-99/tests/comparators/test_gnumeric.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_squashfs.py` & `diffoscope-99/tests/comparators/test_squashfs.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_ogg.py` & `diffoscope-99/tests/comparators/test_ogg.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_bzip2.py` & `diffoscope-99/tests/comparators/test_bzip2.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_rpm.py` & `diffoscope-99/tests/comparators/test_rpm.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_fsimage.py` & `diffoscope-99/tests/comparators/test_fsimage.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_jpeg_image.py` & `diffoscope-99/tests/comparators/test_jpeg_image.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_git.py` & `diffoscope-99/tests/comparators/test_git.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_tar.py` & `diffoscope-99/tests/comparators/test_tar.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_dex.py` & `diffoscope-99/tests/comparators/test_dex.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_fontconfig.py` & `diffoscope-99/tests/comparators/test_fontconfig.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_openssh_pub_key.py` & `diffoscope-99/tests/comparators/test_openssh_pub_key.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_fonts.py` & `diffoscope-99/tests/comparators/test_fonts.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_rdata.py` & `diffoscope-99/tests/comparators/test_rdata.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_device.py` & `diffoscope-99/tests/comparators/test_device.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_dtb.py` & `diffoscope-99/tests/comparators/test_dtb.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_odt.py` & `diffoscope-99/tests/comparators/test_odt.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_berkeley_db.py` & `diffoscope-99/tests/comparators/test_berkeley_db.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_gif.py` & `diffoscope-99/tests/comparators/test_gif.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_xsb.py` & `diffoscope-99/tests/comparators/test_xsb.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_ico_image.py` & `diffoscope-99/tests/comparators/test_ico_image.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_binwalk.py` & `diffoscope-99/tests/comparators/test_binwalk.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_text.py` & `diffoscope-99/tests/comparators/test_text.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_java.py` & `diffoscope-99/tests/comparators/test_java.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_ipk.py` & `diffoscope-99/tests/comparators/test_ipk.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_pdf.py` & `diffoscope-99/tests/comparators/test_pdf.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_archive.py` & `diffoscope-99/tests/comparators/test_archive.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_gzip.py` & `diffoscope-99/tests/comparators/test_gzip.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_binary.py` & `diffoscope-99/tests/comparators/test_binary.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_iso9660.py` & `diffoscope-99/tests/comparators/test_iso9660.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_macho.py` & `diffoscope-99/tests/comparators/test_macho.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_icc.py` & `diffoscope-99/tests/comparators/test_icc.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_xml.py` & `diffoscope-99/tests/comparators/test_xml.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_zip.py` & `diffoscope-99/tests/comparators/test_zip.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_rlib.py` & `diffoscope-99/tests/comparators/test_rlib.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_javascript.py` & `diffoscope-99/tests/comparators/test_javascript.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_json.py` & `diffoscope-99/tests/comparators/test_json.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_symlink.py` & `diffoscope-99/tests/comparators/test_symlink.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_mono.py` & `diffoscope-99/tests/comparators/test_mono.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_utils.py` & `diffoscope-99/tests/comparators/test_utils.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_apk.py` & `diffoscope-99/tests/comparators/test_apk.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_cpio.py` & `diffoscope-99/tests/comparators/test_cpio.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_debian.py` & `diffoscope-99/tests/comparators/test_debian.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_pgp.py` & `diffoscope-99/tests/comparators/test_pgp.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_ps.py` & `diffoscope-99/tests/comparators/test_ps.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_epub.py` & `diffoscope-99/tests/comparators/test_epub.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_containers.py` & `diffoscope-99/tests/comparators/test_containers.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_pcap.py` & `diffoscope-99/tests/comparators/test_pcap.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_xz.py` & `diffoscope-99/tests/comparators/test_xz.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_elf.py` & `diffoscope-99/tests/comparators/test_elf.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_gettext.py` & `diffoscope-99/tests/comparators/test_gettext.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_haskell.py` & `diffoscope-99/tests/comparators/test_haskell.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_cbfs.py` & `diffoscope-99/tests/comparators/test_cbfs.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_sqlite.py` & `diffoscope-99/tests/comparators/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_deb.py` & `diffoscope-99/tests/comparators/test_deb.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/comparators/test_png.py` & `diffoscope-99/tests/comparators/test_png.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/utils/__init__.py` & `diffoscope-99/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/utils/tools.py` & `diffoscope-99/tests/utils/tools.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/utils/data.py` & `diffoscope-99/tests/utils/data.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/utils/nonexisting.py` & `diffoscope-99/tests/utils/nonexisting.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/test_quines.py` & `diffoscope-99/tests/test_quines.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/test_difference.py` & `diffoscope-99/tests/test_difference.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/test_progress.py` & `diffoscope-99/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/conftest.py` & `diffoscope-99/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/test_tools.py` & `diffoscope-99/tests/test_tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 import os
 import pytest
 
 
 def test_sbin_added_to_path():
     from diffoscope.tools import tool_required
 
-    @tool_required(os.listdir('/sbin')[0])
+    _, _, filenames = list(os.walk('/sbin'))[0]
+
+    @tool_required(filenames[0])
     def fn():
         pass
 
     fn()
 
 
 def test_required_tool_not_found():
```

### Comparing `diffoscope-98/tests/test_source.py` & `diffoscope-99/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/test_excludes.py` & `diffoscope-99/tests/test_excludes.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.rlib` & `diffoscope-99/tests/data/test1.rlib`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/rpm_fallback_expected_diff` & `diffoscope-99/tests/data/rpm_fallback_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.o` & `diffoscope-99/tests/data/test1.o`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/text_unicode_binary_fallback` & `diffoscope-99/tests/data/text_unicode_binary_fallback`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/Samyak-Malayalam1.ttf` & `diffoscope-99/tests/data/Samyak-Malayalam1.ttf`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/text_ascii2` & `diffoscope-99/tests/data/text_ascii2`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/rds_expected_diff` & `diffoscope-99/tests/data/rds_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/text_unicode1` & `diffoscope-99/tests/data/text_unicode1`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.rpm` & `diffoscope-99/tests/data/test1.rpm`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test_weird_non_unicode_chars2.pdf` & `diffoscope-99/tests/data/test_weird_non_unicode_chars2.pdf`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/iso9660_rockridge_expected_diff` & `diffoscope-99/tests/data/iso9660_rockridge_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test3.gif` & `diffoscope-99/tests/data/test3.gif`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/rpm_header_expected_diff` & `diffoscope-99/tests/data/rpm_header_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.o` & `diffoscope-99/tests/data/test2.o`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/mo_expected_diff` & `diffoscope-99/tests/data/mo_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/no-perms.tar` & `diffoscope-99/tests/data/no-perms.tar`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.pdf` & `diffoscope-99/tests/data/test2.pdf`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/berkeley_db_expected_diff` & `diffoscope-99/tests/data/berkeley_db_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.tar` & `diffoscope-99/tests/data/test2.tar`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/bug881937_1.deb` & `diffoscope-99/tests/data/bug881937_1.deb`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.xsb` & `diffoscope-99/tests/data/test2.xsb`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.a` & `diffoscope-99/tests/data/test1.a`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/epub_expected_diffs` & `diffoscope-99/tests/data/epub_expected_diffs`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/ttf_expected_diff` & `diffoscope-99/tests/data/ttf_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/ext4_expected_diffs` & `diffoscope-99/tests/data/ext4_expected_diffs`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/output.md` & `diffoscope-99/tests/data/output.md`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test_openssh_pub_key2.pub` & `diffoscope-99/tests/data/test_openssh_pub_key2.pub`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/mozzip_zipinfo_expected_diff` & `diffoscope-99/tests/data/mozzip_zipinfo_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/archive2.tar` & `diffoscope-99/tests/data/archive2.tar`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1_meta.jpg` & `diffoscope-99/tests/data/test1_meta.jpg`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/apk_manifest_expected_diff` & `diffoscope-99/tests/data/apk_manifest_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.gif` & `diffoscope-99/tests/data/test2.gif`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/pcap_expected_diff` & `diffoscope-99/tests/data/pcap_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/gif_expected_diff` & `diffoscope-99/tests/data/gif_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.odt` & `diffoscope-99/tests/data/test1.odt`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1-le64.cache-4` & `diffoscope-99/tests/data/test1-le64.cache-4`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.ogg` & `diffoscope-99/tests/data/test2.ogg`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.hi` & `diffoscope-99/tests/data/test2.hi`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/output.txt` & `diffoscope-99/tests/data/output.txt`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/haskell_expected_diff` & `diffoscope-99/tests/data/haskell_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/Samyak-Malayalam2.ttf` & `diffoscope-99/tests/data/Samyak-Malayalam2.ttf`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test4.changes` & `diffoscope-99/tests/data/test4.changes`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/device_expected_diff_freebsd` & `diffoscope-99/tests/data/device_expected_diff_freebsd`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/devicetree2.dtb` & `diffoscope-99/tests/data/devicetree2.dtb`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/binwalk_expected_diff` & `diffoscope-99/tests/data/binwalk_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/containers/b.tar.xz` & `diffoscope-99/tests/data/containers/b.tar.xz`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/containers/different_files_expected_diff` & `diffoscope-99/tests/data/containers/different_files_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/containers/b.tar.bz2` & `diffoscope-99/tests/data/containers/b.tar.bz2`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/containers/b.tar.gz` & `diffoscope-99/tests/data/containers/b.tar.gz`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/device_expected_diff_reverse_freebsd` & `diffoscope-99/tests/data/device_expected_diff_reverse_freebsd`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/ogg_expected_diff` & `diffoscope-99/tests/data/ogg_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/ppu_expected_diff` & `diffoscope-99/tests/data/ppu_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test_openssh_pub_key1.pub` & `diffoscope-99/tests/data/test_openssh_pub_key1.pub`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.odt` & `diffoscope-99/tests/data/test2.odt`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/archive12.diff.txt` & `diffoscope-99/tests/data/archive12.diff.txt`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2-le64.cache-4` & `diffoscope-99/tests/data/test2-le64.cache-4`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.binwalk` & `diffoscope-99/tests/data/test1.binwalk`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.tar` & `diffoscope-99/tests/data/test1.tar`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/bug881937_control_expected_diff` & `diffoscope-99/tests/data/bug881937_control_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/fuzzy1.tar` & `diffoscope-99/tests/data/fuzzy1.tar`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.sqlite3` & `diffoscope-99/tests/data/test1.sqlite3`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/device_expected_diff_reverse` & `diffoscope-99/tests/data/device_expected_diff_reverse`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.gnumeric` & `diffoscope-99/tests/data/test2.gnumeric`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test4.gif` & `diffoscope-99/tests/data/test4.gif`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/output.rst` & `diffoscope-99/tests/data/output.rst`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.cpio` & `diffoscope-99/tests/data/test1.cpio`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/bug881937_2.deb` & `diffoscope-99/tests/data/bug881937_2.deb`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.epub` & `diffoscope-99/tests/data/test1.epub`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/macho_expected_diff_disassembly` & `diffoscope-99/tests/data/macho_expected_diff_disassembly`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test_weird_non_unicode_chars1.pdf` & `diffoscope-99/tests/data/test_weird_non_unicode_chars1.pdf`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/quine_a.deb` & `diffoscope-99/tests/data/quine_a.deb`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/fuzzy3.tar` & `diffoscope-99/tests/data/fuzzy3.tar`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/xsb_expected_diff` & `diffoscope-99/tests/data/xsb_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.jpg` & `diffoscope-99/tests/data/test1.jpg`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.changes` & `diffoscope-99/tests/data/test2.changes`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.docx` & `diffoscope-99/tests/data/test1.docx`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/devicetree1.dtb` & `diffoscope-99/tests/data/devicetree1.dtb`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/deb_metadata_expected_diff` & `diffoscope-99/tests/data/deb_metadata_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.ppu` & `diffoscope-99/tests/data/test1.ppu`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/ps_internal_expected_diff` & `diffoscope-99/tests/data/ps_internal_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.ext4` & `diffoscope-99/tests/data/test1.ext4`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/cpio_listing_expected_diff` & `diffoscope-99/tests/data/cpio_listing_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/fuzzy2.tar` & `diffoscope-99/tests/data/fuzzy2.tar`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.hi` & `diffoscope-99/tests/data/test1.hi`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.iso` & `diffoscope-99/tests/data/test1.iso`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.debsrc.tar.gz` & `diffoscope-99/tests/data/test1.debsrc.tar.gz`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.icc` & `diffoscope-99/tests/data/test1.icc`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.exe` & `diffoscope-99/tests/data/test1.exe`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/base-files_157-r45918_ar71xx.ipk` & `diffoscope-99/tests/data/base-files_157-r45918_ar71xx.ipk`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/icc_expected_diff` & `diffoscope-99/tests/data/icc_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/dot_buildinfo_fallback_expected_diff` & `diffoscope-99/tests/data/dot_buildinfo_fallback_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.xsb` & `diffoscope-99/tests/data/test1.xsb`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/rlib_llvm_dis_expected_diff_5` & `diffoscope-99/tests/data/rlib_llvm_dis_expected_diff_5`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/fuzzy-tar-in-tar1.tar` & `diffoscope-99/tests/data/fuzzy-tar-in-tar1.tar`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.xz` & `diffoscope-99/tests/data/test2.xz`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.dex` & `diffoscope-99/tests/data/test2.dex`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/quine_b.deb` & `diffoscope-99/tests/data/quine_b.deb`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/ico_image_expected_diff` & `diffoscope-99/tests/data/ico_image_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/iso9660_rockridge_expected_diff_cdrtools` & `diffoscope-99/tests/data/iso9660_rockridge_expected_diff_cdrtools`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.gif` & `diffoscope-99/tests/data/test1.gif`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.jpg` & `diffoscope-99/tests/data/test2.jpg`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/text_iso8859_expected_diff` & `diffoscope-99/tests/data/text_iso8859_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/dot_changes_fallback_expected_diff` & `diffoscope-99/tests/data/dot_changes_fallback_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.exe` & `diffoscope-99/tests/data/test2.exe`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.zip` & `diffoscope-99/tests/data/test2.zip`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test3.zip` & `diffoscope-99/tests/data/test3.zip`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.ext4` & `diffoscope-99/tests/data/test2.ext4`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.epub` & `diffoscope-99/tests/data/test2.epub`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.macho` & `diffoscope-99/tests/data/test2.macho`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.a` & `diffoscope-99/tests/data/test2.a`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/debian-bug-876316-control.tar.gz` & `diffoscope-99/tests/data/debian-bug-876316-control.tar.gz`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/android1.img` & `diffoscope-99/tests/data/android1.img`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/device_expected_diff` & `diffoscope-99/tests/data/device_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/pgp_expected_diff` & `diffoscope-99/tests/data/pgp_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.pgp` & `diffoscope-99/tests/data/test1.pgp`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.apk` & `diffoscope-99/tests/data/test2.apk`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.zip` & `diffoscope-99/tests/data/test1.zip`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.icc` & `diffoscope-99/tests/data/test2.icc`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.dex` & `diffoscope-99/tests/data/test1.dex`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.deb` & `diffoscope-99/tests/data/test1.deb`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.sqlite3` & `diffoscope-99/tests/data/test2.sqlite3`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/dex_expected_diffs` & `diffoscope-99/tests/data/dex_expected_diffs`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/rlib_elf_expected_diff` & `diffoscope-99/tests/data/rlib_elf_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.ppu` & `diffoscope-99/tests/data/test2.ppu`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.buildinfo` & `diffoscope-99/tests/data/test2.buildinfo`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/gnu_debuglink_expected_diff` & `diffoscope-99/tests/data/gnu_debuglink_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/output.json` & `diffoscope-99/tests/data/output.json`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.ps` & `diffoscope-99/tests/data/test1.ps`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.deb` & `diffoscope-99/tests/data/test2.deb`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/android2.img` & `diffoscope-99/tests/data/android2.img`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.cpio` & `diffoscope-99/tests/data/test2.cpio`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.pcap` & `diffoscope-99/tests/data/test1.pcap`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.iso` & `diffoscope-99/tests/data/test2.iso`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/tar_listing_expected_diff` & `diffoscope-99/tests/data/tar_listing_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.pcap` & `diffoscope-99/tests/data/test2.pcap`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.rlib` & `diffoscope-99/tests/data/test2.rlib`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.ps` & `diffoscope-99/tests/data/test2.ps`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/text_unicode_expected_diff` & `diffoscope-99/tests/data/text_unicode_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/devicetree_expected_diff` & `diffoscope-99/tests/data/devicetree_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.docx` & `diffoscope-99/tests/data/test2.docx`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/fuzzy-tar-in-tar2.tar` & `diffoscope-99/tests/data/fuzzy-tar-in-tar2.tar`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test3.changes` & `diffoscope-99/tests/data/test3.changes`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/base-files_157-r45695_ar71xx.ipk` & `diffoscope-99/tests/data/base-files_157-r45695_ar71xx.ipk`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/debian-bug-875281.collapsed-diff.json` & `diffoscope-99/tests/data/debian-bug-875281.collapsed-diff.json`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/dbgsym/test-dbgsym_1.tar.gz` & `diffoscope-99/tests/data/dbgsym/test-dbgsym_1.tar.gz`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/dbgsym/add/test-dbgsym_1_amd64.deb` & `diffoscope-99/tests/data/dbgsym/add/test-dbgsym_1_amd64.deb`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/dbgsym/add/test-dbgsym-dbgsym_1_amd64.deb` & `diffoscope-99/tests/data/dbgsym/add/test-dbgsym-dbgsym_1_amd64.deb`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/dbgsym/mult/test-dbgsym_1_amd64.deb` & `diffoscope-99/tests/data/dbgsym/mult/test-dbgsym_1_amd64.deb`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/dbgsym/mult/test-dbgsym-dbgsym_1_amd64.deb` & `diffoscope-99/tests/data/dbgsym/mult/test-dbgsym-dbgsym_1_amd64.deb`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/mo_charsets_expected_diff` & `diffoscope-99/tests/data/mo_charsets_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/jpeg_image_meta_expected_diff` & `diffoscope-99/tests/data/jpeg_image_meta_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2_meta.jpg` & `diffoscope-99/tests/data/test2_meta.jpg`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.rpm` & `diffoscope-99/tests/data/test2.rpm`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/jpeg_image_expected_diff` & `diffoscope-99/tests/data/jpeg_image_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.squashfs` & `diffoscope-99/tests/data/test2.squashfs`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.macho` & `diffoscope-99/tests/data/test1.macho`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.apk` & `diffoscope-99/tests/data/test1.apk`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.ico` & `diffoscope-99/tests/data/test2.ico`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.pgp` & `diffoscope-99/tests/data/test2.pgp`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/fontconfig_expected_diff` & `diffoscope-99/tests/data/fontconfig_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/text_iso8859` & `diffoscope-99/tests/data/text_iso8859`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.binwalk` & `diffoscope-99/tests/data/test2.binwalk`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.pdf` & `diffoscope-99/tests/data/test1.pdf`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.db` & `diffoscope-99/tests/data/test1.db`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/android_expected_diff` & `diffoscope-99/tests/data/android_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/text_unicode2` & `diffoscope-99/tests/data/text_unicode2`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/text_ascii_expected_diff` & `diffoscope-99/tests/data/text_ascii_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.ogg` & `diffoscope-99/tests/data/test1.ogg`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/archive1.tar` & `diffoscope-99/tests/data/archive1.tar`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/output.colored.txt` & `diffoscope-99/tests/data/output.colored.txt`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.debsrc.tar.gz` & `diffoscope-99/tests/data/test2.debsrc.tar.gz`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.db` & `diffoscope-99/tests/data/test2.db`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/dot_dsc_fallback_expected_diff` & `diffoscope-99/tests/data/dot_dsc_fallback_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.gnumeric` & `diffoscope-99/tests/data/test1.gnumeric`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/rlib_llvm_dis_expected_diff` & `diffoscope-99/tests/data/rlib_llvm_dis_expected_diff`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test2.mozzip` & `diffoscope-99/tests/data/test2.mozzip`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test3.apk` & `diffoscope-99/tests/data/test3.apk`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.changes` & `diffoscope-99/tests/data/test1.changes`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.squashfs` & `diffoscope-99/tests/data/test1.squashfs`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/data/test1.buildinfo` & `diffoscope-99/tests/data/test1.buildinfo`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/test_readers.py` & `diffoscope-99/tests/test_readers.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/test_presenters.py` & `diffoscope-99/tests/test_presenters.py`

 * *Files identical despite different names*

### Comparing `diffoscope-98/tests/test_main.py` & `diffoscope-99/tests/test_main.py`

 * *Files identical despite different names*

