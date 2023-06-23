# Comparing `tmp/np4k-0.0.94.tar.gz` & `tmp/np4k-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np4k-0.0.94.tar", last modified: Thu May 18 04:22:29 2023, max compression
+gzip compressed data, was "np4k-0.0.95.tar", last modified: Fri Jun 23 19:43:15 2023, max compression
```

## Comparing `np4k-0.0.94.tar` & `np4k-0.0.95.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 hamsa      (501) staff       (20)        0 2023-05-18 04:22:29.720635 np4k-0.0.94/
--rw-r--r--   0 hamsa      (501) staff       (20)     1062 2023-04-03 18:29:27.000000 np4k-0.0.94/LICENSE
--rw-r--r--   0 hamsa      (501) staff       (20)      129 2023-04-03 18:29:27.000000 np4k-0.0.94/MANIFEST.in
--rw-r--r--   0 hamsa      (501) staff       (20)      259 2023-05-18 04:22:29.720463 np4k-0.0.94/PKG-INFO
--rw-r--r--   0 hamsa      (501) staff       (20)        6 2023-04-03 18:29:27.000000 np4k-0.0.94/README.md
-drwxr-xr-x   0 hamsa      (501) staff       (20)        0 2023-05-18 04:22:29.713438 np4k-0.0.94/np4k/
--rw-r--r--   0 hamsa      (501) staff       (20)      792 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/__init__.py
--rw-r--r--   0 hamsa      (501) staff       (20)     2693 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/api.py
--rw-r--r--   0 hamsa      (501) staff       (20)    21558 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/article.py
--rw-r--r--   0 hamsa      (501) staff       (20)    10447 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/cleaners.py
--rw-r--r--   0 hamsa      (501) staff       (20)     4369 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/configuration.py
--rw-r--r--   0 hamsa      (501) staff       (20)      482 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/exceptions.py
--rw-r--r--   0 hamsa      (501) staff       (20)    42433 2023-05-18 04:15:59.000000 np4k-0.0.94/np4k/extractors.py
--rw-r--r--   0 hamsa      (501) staff       (20)     7556 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/images.py
--rw-r--r--   0 hamsa      (501) staff       (20)      636 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/lib.py
--rw-r--r--   0 hamsa      (501) staff       (20)     4030 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/mthreading.py
--rw-r--r--   0 hamsa      (501) staff       (20)     4437 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/network.py
--rw-r--r--   0 hamsa      (501) staff       (20)     5892 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/nlp.py
--rw-r--r--   0 hamsa      (501) staff       (20)     7225 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/outputformatters.py
--rw-r--r--   0 hamsa      (501) staff       (20)     7798 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/parsers.py
-drwxr-xr-x   0 hamsa      (501) staff       (20)        0 2023-05-18 04:22:29.710644 np4k-0.0.94/np4k/resources/
-drwxr-xr-x   0 hamsa      (501) staff       (20)        0 2023-05-18 04:22:29.714628 np4k-0.0.94/np4k/resources/misc/
--rw-r--r--   0 hamsa      (501) staff       (20)   349280 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/misc/google_sources.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     4264 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/misc/popular_sources.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     2389 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/misc/stopwords-nlp-en.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     4241 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/misc/useragents.txt
-drwxr-xr-x   0 hamsa      (501) staff       (20)        0 2023-05-18 04:22:29.719802 np4k-0.0.94/np4k/resources/text/
--rw-r--r--   0 hamsa      (501) staff       (20)     1450 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-ar.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      936 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-be.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     2409 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-bg.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      484 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-da.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     5967 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-de.txt
--rw-r--r--   0 hamsa      (501) staff       (20)    13903 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-el.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     3585 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-en.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     2185 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-es.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      189 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-et.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     7710 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-fa.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      464 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-fi.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     2002 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-fr.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     1836 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-he.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     2790 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-hi.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      870 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-hr.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     2337 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-hu.txt
--rw-r--r--   0 hamsa      (501) staff       (20)    10499 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-id.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     1696 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-it.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     1006 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-ja.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      459 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-ko.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      763 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-lt.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     1504 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-mk.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      587 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-nb.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      177 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-nl.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      513 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-no.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     2015 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-pl.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     3610 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-pt.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     1915 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-ro.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     4958 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-ru.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     2435 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-sl.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      776 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-sr.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     3956 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-sv.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      407 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-sw.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     1420 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-th.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     1368 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-tr.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     4029 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-uk.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      724 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-vi.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      623 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/resources/text/stopwords-zh.txt
--rw-r--r--   0 hamsa      (501) staff       (20)     1611 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/settings.py
--rw-r--r--   0 hamsa      (501) staff       (20)    15527 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/source.py
--rw-r--r--   0 hamsa      (501) staff       (20)     6027 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/text.py
--rw-r--r--   0 hamsa      (501) staff       (20)    10425 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/urls.py
--rw-r--r--   0 hamsa      (501) staff       (20)    15319 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/utils.py
--rw-r--r--   0 hamsa      (501) staff       (20)      277 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/version.py
-drwxr-xr-x   0 hamsa      (501) staff       (20)        0 2023-05-18 04:22:29.720274 np4k-0.0.94/np4k/videos/
--rw-r--r--   0 hamsa      (501) staff       (20)        0 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/videos/__init__.py
--rw-r--r--   0 hamsa      (501) staff       (20)     3793 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/videos/extractors.py
--rw-r--r--   0 hamsa      (501) staff       (20)      421 2023-04-03 18:29:27.000000 np4k-0.0.94/np4k/videos/videos.py
-drwxr-xr-x   0 hamsa      (501) staff       (20)        0 2023-05-18 04:22:29.713957 np4k-0.0.94/np4k.egg-info/
--rw-r--r--   0 hamsa      (501) staff       (20)      259 2023-05-18 04:22:29.000000 np4k-0.0.94/np4k.egg-info/PKG-INFO
--rw-r--r--   0 hamsa      (501) staff       (20)     2150 2023-05-18 04:22:29.000000 np4k-0.0.94/np4k.egg-info/SOURCES.txt
--rw-r--r--   0 hamsa      (501) staff       (20)        1 2023-05-18 04:22:29.000000 np4k-0.0.94/np4k.egg-info/dependency_links.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      384 2023-05-18 04:22:29.000000 np4k-0.0.94/np4k.egg-info/requires.txt
--rw-r--r--   0 hamsa      (501) staff       (20)        5 2023-05-18 04:22:29.000000 np4k-0.0.94/np4k.egg-info/top_level.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      711 2023-05-18 04:22:18.000000 np4k-0.0.94/pyproject.toml
--rw-r--r--   0 hamsa      (501) staff       (20)       38 2023-05-18 04:22:29.720682 np4k-0.0.94/setup.cfg
--rwxr-xr-x   0 hamsa      (501) staff       (20)     1120 2023-05-18 04:22:29.000000 np4k-0.0.94/setup.py
+drwxr-xr-x   0 stuartbaker   (501) staff       (20)        0 2023-06-23 19:43:15.933169 np4k-0.0.95/
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     1062 2023-02-17 23:03:34.000000 np4k-0.0.95/LICENSE
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      129 2023-02-17 23:03:34.000000 np4k-0.0.95/MANIFEST.in
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      259 2023-06-23 19:43:15.933019 np4k-0.0.95/PKG-INFO
+-rw-r--r--   0 stuartbaker   (501) staff       (20)        6 2023-02-17 23:03:34.000000 np4k-0.0.95/README.md
+drwxr-xr-x   0 stuartbaker   (501) staff       (20)        0 2023-06-23 19:43:15.921676 np4k-0.0.95/np4k/
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      792 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/__init__.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     2693 2023-03-22 04:23:32.000000 np4k-0.0.95/np4k/api.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)    21558 2023-03-22 04:54:05.000000 np4k-0.0.95/np4k/article.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)    10447 2023-03-14 23:22:11.000000 np4k-0.0.95/np4k/cleaners.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     4369 2023-03-14 23:18:39.000000 np4k-0.0.95/np4k/configuration.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      645 2023-06-23 19:38:09.000000 np4k-0.0.95/np4k/exceptions.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)    42288 2023-03-20 22:29:37.000000 np4k-0.0.95/np4k/extractors.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     7556 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/images.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      636 2023-03-21 19:09:45.000000 np4k-0.0.95/np4k/lib.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     4030 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/mthreading.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     4437 2023-03-14 23:18:39.000000 np4k-0.0.95/np4k/network.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     5892 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/nlp.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     7225 2023-03-22 04:56:19.000000 np4k-0.0.95/np4k/outputformatters.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     7798 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/parsers.py
+drwxr-xr-x   0 stuartbaker   (501) staff       (20)        0 2023-06-23 19:43:15.915367 np4k-0.0.95/np4k/resources/
+drwxr-xr-x   0 stuartbaker   (501) staff       (20)        0 2023-06-23 19:43:15.924188 np4k-0.0.95/np4k/resources/misc/
+-rw-r--r--   0 stuartbaker   (501) staff       (20)   349280 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/misc/google_sources.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     4264 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/misc/popular_sources.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     2389 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/misc/stopwords-nlp-en.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     4241 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/misc/useragents.txt
+drwxr-xr-x   0 stuartbaker   (501) staff       (20)        0 2023-06-23 19:43:15.932038 np4k-0.0.95/np4k/resources/text/
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     1450 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-ar.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      936 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-be.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     2409 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-bg.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      484 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-da.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     5967 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-de.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)    13903 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-el.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     3585 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-en.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     2185 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-es.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      189 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-et.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     7710 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-fa.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      464 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-fi.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     2002 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-fr.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     1836 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-he.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     2790 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-hi.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      870 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-hr.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     2337 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-hu.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)    10499 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-id.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     1696 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-it.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     1006 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-ja.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      459 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-ko.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      763 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-lt.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     1504 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-mk.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      587 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-nb.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      177 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-nl.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      513 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-no.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     2015 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-pl.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     3610 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-pt.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     1915 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-ro.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     4958 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-ru.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     2435 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-sl.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      776 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-sr.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     3956 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-sv.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      407 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-sw.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     1420 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-th.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     1368 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-tr.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     4029 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-uk.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      724 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-vi.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      623 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/resources/text/stopwords-zh.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     1611 2023-03-14 23:18:39.000000 np4k-0.0.95/np4k/settings.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)    15618 2023-06-23 19:38:09.000000 np4k-0.0.95/np4k/source.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     6027 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/text.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)    10425 2023-03-21 21:44:54.000000 np4k-0.0.95/np4k/urls.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)    15319 2023-03-15 00:28:01.000000 np4k-0.0.95/np4k/utils.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      277 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/version.py
+drwxr-xr-x   0 stuartbaker   (501) staff       (20)        0 2023-06-23 19:43:15.932680 np4k-0.0.95/np4k/videos/
+-rw-r--r--   0 stuartbaker   (501) staff       (20)        0 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/videos/__init__.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     3793 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/videos/extractors.py
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      421 2023-02-17 23:03:34.000000 np4k-0.0.95/np4k/videos/videos.py
+drwxr-xr-x   0 stuartbaker   (501) staff       (20)        0 2023-06-23 19:43:15.922302 np4k-0.0.95/np4k.egg-info/
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      259 2023-06-23 19:43:15.000000 np4k-0.0.95/np4k.egg-info/PKG-INFO
+-rw-r--r--   0 stuartbaker   (501) staff       (20)     2150 2023-06-23 19:43:15.000000 np4k-0.0.95/np4k.egg-info/SOURCES.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)        1 2023-06-23 19:43:15.000000 np4k-0.0.95/np4k.egg-info/dependency_links.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      362 2023-06-23 19:43:15.000000 np4k-0.0.95/np4k.egg-info/requires.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)        5 2023-06-23 19:43:15.000000 np4k-0.0.95/np4k.egg-info/top_level.txt
+-rw-r--r--   0 stuartbaker   (501) staff       (20)      693 2023-06-23 19:43:13.000000 np4k-0.0.95/pyproject.toml
+-rw-r--r--   0 stuartbaker   (501) staff       (20)       38 2023-06-23 19:43:15.933235 np4k-0.0.95/setup.cfg
+-rwxr-xr-x   0 stuartbaker   (501) staff       (20)     1094 2023-06-23 19:43:15.000000 np4k-0.0.95/setup.py
```

### Comparing `np4k-0.0.94/LICENSE` & `np4k-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/__init__.py` & `np4k-0.0.95/np4k/__init__.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/api.py` & `np4k-0.0.95/np4k/api.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/article.py` & `np4k-0.0.95/np4k/article.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/cleaners.py` & `np4k-0.0.95/np4k/cleaners.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/configuration.py` & `np4k-0.0.95/np4k/configuration.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/extractors.py` & `np4k-0.0.95/np4k/extractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -490,18 +490,15 @@
         """Returns site name of article, open graph protocol
         """
         return self.get_meta_content(doc, 'meta[property="og:site_name"]')
 
     def get_meta_description(self, doc):
         """If the article has meta description set in the source, use that
         """
-        description = self.get_meta_content(doc, "meta[name=description]")
-        if description != '':
-            return description
-        return self.get_meta_content(doc, 'meta[property="og:description"]')
+        return self.get_meta_content(doc, "meta[name=description]")
 
     def get_meta_keywords(self, doc):
         """If the article has meta keywords set in the source, use that
         """
         return self.get_meta_content(doc, "meta[name=keywords]")
 
     def get_meta_data(self, doc):
```

### Comparing `np4k-0.0.94/np4k/images.py` & `np4k-0.0.95/np4k/images.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/lib.py` & `np4k-0.0.95/np4k/lib.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/mthreading.py` & `np4k-0.0.95/np4k/mthreading.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/network.py` & `np4k-0.0.95/np4k/network.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/nlp.py` & `np4k-0.0.95/np4k/nlp.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/outputformatters.py` & `np4k-0.0.95/np4k/outputformatters.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/parsers.py` & `np4k-0.0.95/np4k/parsers.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/misc/google_sources.txt` & `np4k-0.0.95/np4k/resources/misc/google_sources.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/misc/popular_sources.txt` & `np4k-0.0.95/np4k/resources/misc/popular_sources.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/misc/stopwords-nlp-en.txt` & `np4k-0.0.95/np4k/resources/misc/stopwords-nlp-en.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/misc/useragents.txt` & `np4k-0.0.95/np4k/resources/misc/useragents.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-ar.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-ar.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-be.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-be.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-bg.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-bg.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-de.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-de.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-el.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-el.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-en.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-en.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-es.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-es.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-fa.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-fa.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-fr.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-fr.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-he.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-he.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-hi.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-hi.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-hr.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-hr.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-hu.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-hu.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-id.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-id.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-it.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-it.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-ja.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-ja.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-lt.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-lt.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-mk.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-mk.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-nb.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-nb.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-no.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-no.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-pl.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-pl.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-pt.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-pt.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-ro.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-ro.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-ru.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-ru.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-sl.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-sl.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-sr.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-sr.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-sv.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-sv.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-th.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-th.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-tr.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-tr.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-uk.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-uk.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-vi.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-vi.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/resources/text/stopwords-zh.txt` & `np4k-0.0.95/np4k/resources/text/stopwords-zh.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/settings.py` & `np4k-0.0.95/np4k/settings.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/source.py` & `np4k-0.0.95/np4k/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from tldextract import tldextract
 
 from . import network
 from . import urls
 from . import utils
 from .article import Article
 from .configuration import Configuration
+from .exceptions import BadURLException
 from .extractors import ContentExtractor
 from .settings import ANCHOR_DIRECTORY
 
 log = logging.getLogger(__name__)
 
 
 class Category:
@@ -54,15 +55,17 @@
     """
 
     def __init__(self, url: str, config: Optional[Configuration] = None, **kwargs):
         """The config object for this source will be passed into all of this
         source's children articles unless specified otherwise or re-set.
         """
         if (url is None) or ('://' not in url) or (url[:4] != 'http'):
-            raise Exception('Input url is bad!')
+            if url is None:
+                url = 'None'
+            raise BadURLException(url=url)
 
         self.config = config or Configuration()
         self.config = utils.extend_config(self.config, kwargs)
 
         self.extractor = ContentExtractor(self.config)
 
         self.url = url
```

### Comparing `np4k-0.0.94/np4k/text.py` & `np4k-0.0.95/np4k/text.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/urls.py` & `np4k-0.0.95/np4k/urls.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/utils.py` & `np4k-0.0.95/np4k/utils.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k/videos/extractors.py` & `np4k-0.0.95/np4k/videos/extractors.py`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/np4k.egg-info/SOURCES.txt` & `np4k-0.0.95/np4k.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `np4k-0.0.94/setup.py` & `np4k-0.0.95/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,20 +18,19 @@
  'nltk>=3.8.1,<4.0.0',
  'pillow>=9.4.0,<10.0.0',
  'pythainlp>=3.1.1,<4.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.2,<3.0.0',
  'tinysegmenter>=0.4,<0.5',
- 'tldextract>=3.4.0,<4.0.0',
- 'wheel>=0.40.0,<0.41.0']
+ 'tldextract>=3.4.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'np4k',
-    'version': '0.0.94',
+    'version': '0.0.95',
     'description': '',
     'long_description': '\n\nnp4k',
     'author': 'Airvue',
     'author_email': 'dev@airvue.news',
     'maintainer': 'Airvue',
     'maintainer_email': 'dev@airvue.news',
     'url': 'https://github.com/airvuetech/newspaper4k/',
```

