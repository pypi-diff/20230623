# Comparing `tmp/pretext-1.6.1.dev20230622.tar.gz` & `tmp/pretext-1.6.1.dev20230623.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.6.1.dev20230622.tar", max compression
+gzip compressed data, was "pretext-1.6.1.dev20230623.tar", max compression
```

## Comparing `pretext-1.6.1.dev20230622.tar` & `pretext-1.6.1.dev20230623.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-06-22 06:19:37.867540 pretext-1.6.1.dev20230622/LICENSE
--rw-r--r--   0        0        0     9757 2023-06-22 06:19:37.867540 pretext-1.6.1.dev20230622/README.md
--rw-r--r--   0        0        0     1909 2023-06-22 06:20:24.788210 pretext-1.6.1.dev20230622/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-06-22 06:19:37.867540 pretext-1.6.1.dev20230622/pretext/__main__.py
--rw-r--r--   0        0        0     8531 2023-06-22 06:19:37.867540 pretext-1.6.1.dev20230622/pretext/build.py
--rw-r--r--   0        0        0    25561 2023-06-22 06:19:37.867540 pretext-1.6.1.dev20230622/pretext/cli.py
--rw-r--r--   0        0        0     5856 2023-06-22 06:19:37.867540 pretext-1.6.1.dev20230622/pretext/codechat.py
--rw-r--r--   0        0        0     5943 2023-06-22 06:19:37.867540 pretext-1.6.1.dev20230622/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-06-22 06:19:37.867540 pretext-1.6.1.dev20230622/pretext/core/__init__.py
--rw-r--r--   0        0        0   172432 2023-06-22 06:20:30.368294 pretext-1.6.1.dev20230622/pretext/core/pretext.py
--rw-r--r--   0        0        0     1484 2023-06-22 06:19:37.867540 pretext-1.6.1.dev20230622/pretext/core/resources.py
--rw-r--r--   0        0        0  1035425 2023-06-22 06:20:30.368294 pretext-1.6.1.dev20230622/pretext/core/resources.zip
--rw-r--r--   0        0        0    16766 2023-06-22 06:19:37.867540 pretext-1.6.1.dev20230622/pretext/generate.py
--rw-r--r--   0        0        0    31778 2023-06-22 06:19:37.867540 pretext-1.6.1.dev20230622/pretext/project.py
--rw-r--r--   0        0        0      555 2023-06-22 06:19:37.867540 pretext-1.6.1.dev20230622/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-06-22 06:20:30.468296 pretext-1.6.1.dev20230622/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-06-22 06:20:30.468296 pretext-1.6.1.dev20230622/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160110 2023-06-22 06:20:30.460296 pretext-1.6.1.dev20230622/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7616 2023-06-22 06:20:30.428295 pretext-1.6.1.dev20230622/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173309 2023-06-22 06:20:30.448295 pretext-1.6.1.dev20230622/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2192 2023-06-22 06:20:30.468296 pretext-1.6.1.dev20230622/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4657 2023-06-22 06:20:30.432295 pretext-1.6.1.dev20230622/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-06-22 06:20:30.468296 pretext-1.6.1.dev20230622/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-06-22 06:20:30.468296 pretext-1.6.1.dev20230622/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8392 2023-06-22 06:20:30.464295 pretext-1.6.1.dev20230622/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    19529 2023-06-22 06:19:37.867540 pretext-1.6.1.dev20230622/pretext/utils.py
--rw-r--r--   0        0        0     3093 2023-06-22 06:20:24.788210 pretext-1.6.1.dev20230622/pyproject.toml
--rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230622/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-23 06:22:10.889545 pretext-1.6.1.dev20230623/LICENSE
+-rw-r--r--   0        0        0     9757 2023-06-23 06:22:10.889545 pretext-1.6.1.dev20230623/README.md
+-rw-r--r--   0        0        0     1909 2023-06-23 06:22:41.094138 pretext-1.6.1.dev20230623/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-23 06:22:10.893545 pretext-1.6.1.dev20230623/pretext/__main__.py
+-rw-r--r--   0        0        0     8531 2023-06-23 06:22:10.893545 pretext-1.6.1.dev20230623/pretext/build.py
+-rw-r--r--   0        0        0    25561 2023-06-23 06:22:10.893545 pretext-1.6.1.dev20230623/pretext/cli.py
+-rw-r--r--   0        0        0     5856 2023-06-23 06:22:10.893545 pretext-1.6.1.dev20230623/pretext/codechat.py
+-rw-r--r--   0        0        0     5943 2023-06-23 06:22:10.893545 pretext-1.6.1.dev20230623/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-06-23 06:22:10.893545 pretext-1.6.1.dev20230623/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172432 2023-06-23 06:22:46.406243 pretext-1.6.1.dev20230623/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1484 2023-06-23 06:22:10.893545 pretext-1.6.1.dev20230623/pretext/core/resources.py
+-rw-r--r--   0        0        0  1035425 2023-06-23 06:22:46.406243 pretext-1.6.1.dev20230623/pretext/core/resources.zip
+-rw-r--r--   0        0        0    16741 2023-06-23 06:22:10.893545 pretext-1.6.1.dev20230623/pretext/generate.py
+-rw-r--r--   0        0        0    31778 2023-06-23 06:22:10.893545 pretext-1.6.1.dev20230623/pretext/project.py
+-rw-r--r--   0        0        0      739 2023-06-23 06:22:10.893545 pretext-1.6.1.dev20230623/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-06-23 06:22:46.478245 pretext-1.6.1.dev20230623/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-23 06:22:46.478245 pretext-1.6.1.dev20230623/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160110 2023-06-23 06:22:46.454244 pretext-1.6.1.dev20230623/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7616 2023-06-23 06:22:46.458244 pretext-1.6.1.dev20230623/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173309 2023-06-23 06:22:46.478245 pretext-1.6.1.dev20230623/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2192 2023-06-23 06:22:46.478245 pretext-1.6.1.dev20230623/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4657 2023-06-23 06:22:46.462245 pretext-1.6.1.dev20230623/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-06-23 06:22:46.478245 pretext-1.6.1.dev20230623/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-06-23 06:22:46.478245 pretext-1.6.1.dev20230623/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8392 2023-06-23 06:22:46.462245 pretext-1.6.1.dev20230623/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    19529 2023-06-23 06:22:10.893545 pretext-1.6.1.dev20230623/pretext/utils.py
+-rw-r--r--   0        0        0     3333 2023-06-23 06:22:41.094138 pretext-1.6.1.dev20230623/pyproject.toml
+-rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230623/PKG-INFO
```

### Comparing `pretext-1.6.1.dev20230622/LICENSE` & `pretext-1.6.1.dev20230623/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230622/README.md` & `pretext-1.6.1.dev20230623/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230622/pretext/__init__.py` & `pretext-1.6.1.dev20230623/pretext/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230622/pretext/build.py` & `pretext-1.6.1.dev20230623/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230622/pretext/cli.py` & `pretext-1.6.1.dev20230623/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230622/pretext/codechat.py` & `pretext-1.6.1.dev20230623/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230622/pretext/config/xml_overlay.py` & `pretext-1.6.1.dev20230623/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230622/pretext/core/pretext.py` & `pretext-1.6.1.dev20230623/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230622/pretext/core/resources.py` & `pretext-1.6.1.dev20230623/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230622/pretext/core/resources.zip` & `pretext-1.6.1.dev20230623/pretext/core/resources.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,143 +1,143 @@
 Zip file size: 1035425 bytes, number of entries: 141
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 xsl/
--rw-r--r--  2.0 unx     2608 b- defN 23-Jun-22 06:20 css/colors_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-22 06:20 css/colors_green_plum.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jun-22 06:20 css/setcolors.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-22 06:20 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jun-22 06:20 css/mathbook-3.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-22 06:20 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-22 06:20 css/colors_orange_navy.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jun-22 06:20 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Jun-22 06:20 css/epub.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-22 06:20 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-22 06:20 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jun-22 06:20 css/README.md
--rw-r--r--  2.0 unx     1338 b- defN 23-Jun-22 06:20 css/colors_red_blue.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jun-22 06:20 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     1276 b- defN 23-Jun-22 06:20 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx      691 b- defN 23-Jun-22 06:20 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jun-22 06:20 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-22 06:20 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jun-22 06:20 css/pretext_add_on.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jun-22 06:20 css/update_css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jun-22 06:20 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-22 06:20 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     7761 b- defN 23-Jun-22 06:20 css/style_default.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jun-22 06:20 css/mathbook-content.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jun-22 06:20 css/kindle.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jun-22 06:20 css/style_soundwriting.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jun-22 06:20 css/pretext.css
--rw-r--r--  2.0 unx     4308 b- defN 23-Jun-22 06:20 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-22 06:20 css/colors_martiansands.css
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 xsl/utilities/
--rw-r--r--  2.0 unx     2248 b- defN 23-Jun-22 06:20 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx   109017 b- defN 23-Jun-22 06:20 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jun-22 06:20 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Jun-22 06:20 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx   112450 b- defN 23-Jun-22 06:20 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jun-22 06:20 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jun-22 06:20 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx   231248 b- defN 23-Jun-22 06:20 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   612399 b- defN 23-Jun-22 06:20 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jun-22 06:20 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jun-22 06:20 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-Jun-22 06:20 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jun-22 06:20 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jun-22 06:20 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jun-22 06:20 xsl/README.md
--rw-r--r--  2.0 unx    12084 b- defN 23-Jun-22 06:20 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-Jun-22 06:20 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jun-22 06:20 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jun-22 06:20 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-Jun-22 06:20 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Jun-22 06:20 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Jun-22 06:20 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jun-22 06:20 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jun-22 06:20 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jun-22 06:20 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jun-22 06:20 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jun-22 06:20 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jun-22 06:20 xsl/entities.ent
--rw-r--r--  2.0 unx   544229 b- defN 23-Jun-22 06:20 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Jun-22 06:20 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jun-22 06:20 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    89128 b- defN 23-Jun-22 06:20 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jun-22 06:20 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jun-22 06:20 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jun-22 06:20 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx   546938 b- defN 23-Jun-22 06:20 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-Jun-22 06:20 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-Jun-22 06:20 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jun-22 06:20 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-Jun-22 06:20 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx     4299 b- defN 23-Jun-22 06:20 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx    30257 b- defN 23-Jun-22 06:20 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx      513 b- defN 23-Jun-22 06:20 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     1810 b- defN 23-Jun-22 06:20 xsl/utilities/README.md
--rw-r--r--  2.0 unx      787 b- defN 23-Jun-22 06:20 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     7526 b- defN 23-Jun-22 06:20 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jun-22 06:20 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-Jun-22 06:20 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jun-22 06:20 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jun-22 06:20 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx    17065 b- defN 23-Jun-22 06:20 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    15566 b- defN 23-Jun-22 06:20 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-Jun-22 06:20 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    16518 b- defN 23-Jun-22 06:20 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    15938 b- defN 23-Jun-22 06:20 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-Jun-22 06:20 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-Jun-22 06:20 xsl/localizations/README.md
--rw-r--r--  2.0 unx    16296 b- defN 23-Jun-22 06:20 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-Jun-22 06:20 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx     2227 b- defN 23-Jun-22 06:20 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-Jun-22 06:20 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    16236 b- defN 23-Jun-22 06:20 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-Jun-22 06:20 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-Jun-22 06:20 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-Jun-22 06:20 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17285 b- defN 23-Jun-22 06:20 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-Jun-22 06:20 xsl/localizations/en-US.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 xsl/support/play-button/
--rw-r--r--  2.0 unx     5241 b- defN 23-Jun-22 06:20 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-Jun-22 06:20 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-Jun-22 06:20 xsl/support/README.md
--rw-r--r--  2.0 unx     5065 b- defN 23-Jun-22 06:20 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     5800 b- defN 23-Jun-22 06:20 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx    10306 b- defN 23-Jun-22 06:20 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-Jun-22 06:20 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     2657 b- defN 23-Jun-22 06:20 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-Jun-22 06:20 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx      722 b- defN 23-Jun-22 06:20 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-22 06:20 pretext/__init__.py
--rw-r--r--  2.0 unx     1955 b- defN 23-Jun-22 06:20 pretext/module-test.py
--rw-r--r--  2.0 unx     2566 b- defN 23-Jun-22 06:20 pretext/pretext.cfg
--rw-r--r--  2.0 unx     1367 b- defN 23-Jun-22 06:20 pretext/README.md
--rw-r--r--  2.0 unx    30908 b- defN 23-Jun-22 06:20 pretext/pretext
--rw-r--r--  2.0 unx   172432 b- defN 23-Jun-22 06:20 pretext/pretext.py
--rw-r--r--  2.0 unx    35449 b- defN 23-Jun-22 06:20 pretext/braille_format.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-Jun-22 06:20 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-Jun-22 06:20 script/mbx
--rw-r--r--  2.0 unx      481 b- defN 23-Jun-22 06:20 script/mjsre/README.md
--rw-r--r--  2.0 unx     9251 b- defN 23-Jun-22 06:20 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-22 06:20 script/mjsre/package.json
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 06:20 script/mjsre/update-sre
--rw-r--r--  2.0 unx   125135 b- defN 23-Jun-22 06:20 schema/pretext.xsd
--rw-r--r--  2.0 unx   101829 b- defN 23-Jun-22 06:20 schema/pretext.rng
--rw-r--r--  2.0 unx   134043 b- defN 23-Jun-22 06:20 schema/pretext.xml
--rw-r--r--  2.0 unx    18421 b- defN 23-Jun-22 06:20 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    58086 b- defN 23-Jun-22 06:20 schema/pretext.rnc
--rw-r--r--  2.0 unx     1180 b- defN 23-Jun-22 06:20 schema/README.md
--rw-r--r--  2.0 unx    17587 b- defN 23-Jun-22 06:20 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx      326 b- defN 23-Jun-22 06:20 schema/xml.xsd
--rw-r--r--  2.0 unx     3135 b- defN 23-Jun-22 06:20 schema/build.sh
--rw-r--r--  2.0 unx    25870 b- defN 23-Jun-22 06:20 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    34210 b- defN 23-Jun-22 06:20 schema/pretext-dev.rng
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-Jun-23 06:22 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-Jun-23 06:22 script/mbx
+-rw-r--r--  2.0 unx      481 b- defN 23-Jun-23 06:22 script/mjsre/README.md
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-23 06:22 script/mjsre/package.json
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 06:22 script/mjsre/update-sre
+-rw-r--r--  2.0 unx     9251 b- defN 23-Jun-23 06:22 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 06:22 pretext/__init__.py
+-rw-r--r--  2.0 unx    30908 b- defN 23-Jun-23 06:22 pretext/pretext
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jun-23 06:22 pretext/README.md
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jun-23 06:22 pretext/pretext.cfg
+-rw-r--r--  2.0 unx   172432 b- defN 23-Jun-23 06:22 pretext/pretext.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jun-23 06:22 pretext/module-test.py
+-rw-r--r--  2.0 unx    35449 b- defN 23-Jun-23 06:22 pretext/braille_format.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 xsl/utilities/
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jun-23 06:22 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx   612399 b- defN 23-Jun-23 06:22 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 23-Jun-23 06:22 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx   231248 b- defN 23-Jun-23 06:22 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-Jun-23 06:22 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jun-23 06:22 xsl/README.md
+-rw-r--r--  2.0 unx    39918 b- defN 23-Jun-23 06:22 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jun-23 06:22 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx   546938 b- defN 23-Jun-23 06:22 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Jun-23 06:22 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Jun-23 06:22 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx   109017 b- defN 23-Jun-23 06:22 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Jun-23 06:22 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-Jun-23 06:22 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jun-23 06:22 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Jun-23 06:22 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-Jun-23 06:22 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   544229 b- defN 23-Jun-23 06:22 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Jun-23 06:22 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Jun-23 06:22 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jun-23 06:22 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx   112450 b- defN 23-Jun-23 06:22 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jun-23 06:22 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-Jun-23 06:22 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jun-23 06:22 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jun-23 06:22 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Jun-23 06:22 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Jun-23 06:22 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-Jun-23 06:22 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jun-23 06:22 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jun-23 06:22 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Jun-23 06:22 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Jun-23 06:22 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    89128 b- defN 23-Jun-23 06:22 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Jun-23 06:22 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-Jun-23 06:22 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Jun-23 06:22 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Jun-23 06:22 xsl/entities.ent
+-rw-r--r--  2.0 unx     6066 b- defN 23-Jun-23 06:22 xsl/pretext-json-manifest.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 xsl/support/play-button/
+-rw-r--r--  2.0 unx      504 b- defN 23-Jun-23 06:22 xsl/support/README.md
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jun-23 06:22 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx    10306 b- defN 23-Jun-23 06:22 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jun-23 06:22 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Jun-23 06:22 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-Jun-23 06:22 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5879 b- defN 23-Jun-23 06:22 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jun-23 06:22 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx      722 b- defN 23-Jun-23 06:22 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     6621 b- defN 23-Jun-23 06:22 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    14482 b- defN 23-Jun-23 06:22 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Jun-23 06:22 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Jun-23 06:22 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jun-23 06:22 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Jun-23 06:22 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx    17040 b- defN 23-Jun-23 06:22 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx     2227 b- defN 23-Jun-23 06:22 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    16518 b- defN 23-Jun-23 06:22 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-Jun-23 06:22 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    17215 b- defN 23-Jun-23 06:22 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-Jun-23 06:22 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-Jun-23 06:22 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-Jun-23 06:22 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-Jun-23 06:22 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    17285 b- defN 23-Jun-23 06:22 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-Jun-23 06:22 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    15566 b- defN 23-Jun-23 06:22 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    15938 b- defN 23-Jun-23 06:22 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16236 b- defN 23-Jun-23 06:22 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-Jun-23 06:22 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-Jun-23 06:22 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-Jun-23 06:22 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx      787 b- defN 23-Jun-23 06:22 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jun-23 06:22 xsl/utilities/README.md
+-rw-r--r--  2.0 unx      513 b- defN 23-Jun-23 06:22 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4926 b- defN 23-Jun-23 06:22 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jun-23 06:22 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jun-23 06:22 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx    34210 b- defN 23-Jun-23 06:22 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx    17587 b- defN 23-Jun-23 06:22 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jun-23 06:22 schema/README.md
+-rw-r--r--  2.0 unx    18421 b- defN 23-Jun-23 06:22 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx   101829 b- defN 23-Jun-23 06:22 schema/pretext.rng
+-rw-r--r--  2.0 unx   134043 b- defN 23-Jun-23 06:22 schema/pretext.xml
+-rw-r--r--  2.0 unx    58086 b- defN 23-Jun-23 06:22 schema/pretext.rnc
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jun-23 06:22 schema/build.sh
+-rw-r--r--  2.0 unx      326 b- defN 23-Jun-23 06:22 schema/xml.xsd
+-rw-r--r--  2.0 unx    25870 b- defN 23-Jun-23 06:22 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx   125135 b- defN 23-Jun-23 06:22 schema/pretext.xsd
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-23 06:22 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-23 06:22 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jun-23 06:22 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Jun-23 06:22 css/update_css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jun-23 06:22 css/README.md
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-23 06:22 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Jun-23 06:22 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Jun-23 06:22 css/mathbook-content.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-23 06:22 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-Jun-23 06:22 css/colors_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-23 06:22 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jun-23 06:22 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Jun-23 06:22 css/colors_red_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-23 06:22 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-23 06:22 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jun-23 06:22 css/epub.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-23 06:22 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Jun-23 06:22 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-23 06:22 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-23 06:22 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Jun-23 06:22 css/kindle.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-Jun-23 06:22 css/style_default.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Jun-23 06:22 css/pretext_add_on.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Jun-23 06:22 css/setcolors.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Jun-23 06:22 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-Jun-23 06:22 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jun-23 06:22 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Jun-23 06:22 css/mathbook-3.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Jun-23 06:22 css/mathbook-add-on.css
 141 files, 4814466 bytes uncompressed, 1017983 bytes compressed:  78.9%
```

#### zipnote {}

```diff
@@ -9,416 +9,416 @@
 
 Filename: script/
 Comment: 
 
 Filename: xsl/
 Comment: 
 
-Filename: css/colors_default.css
+Filename: script/mjsre/
 Comment: 
 
-Filename: css/colors_green_plum.css
+Filename: script/README.md
 Comment: 
 
-Filename: css/setcolors.css
+Filename: script/mbx
 Comment: 
 
-Filename: css/colors_ruby_emerald.css
+Filename: script/mjsre/README.md
 Comment: 
 
-Filename: css/mathbook-3.css
+Filename: script/mjsre/package.json
 Comment: 
 
-Filename: css/colors_blue_red.css
+Filename: script/mjsre/update-sre
 Comment: 
 
-Filename: css/colors_orange_navy.css
+Filename: script/mjsre/mj-sre-page.js
 Comment: 
 
-Filename: css/mathbook-add-on.css
+Filename: pretext/__init__.py
 Comment: 
 
-Filename: css/epub.css
+Filename: pretext/pretext
 Comment: 
 
-Filename: css/colors_green_blue.css
+Filename: pretext/README.md
 Comment: 
 
-Filename: css/colors_ruby_turquoise.css
+Filename: pretext/pretext.cfg
 Comment: 
 
-Filename: css/README.md
+Filename: pretext/pretext.py
 Comment: 
 
-Filename: css/colors_red_blue.css
+Filename: pretext/module-test.py
 Comment: 
 
-Filename: css/style_oscarlevin.css
+Filename: pretext/braille_format.py
 Comment: 
 
-Filename: css/colors_maroon_grey.css
+Filename: xsl/latex/
 Comment: 
 
-Filename: css/colors_pastel_blue_orange.css
+Filename: xsl/localizations/
 Comment: 
 
-Filename: css/colors_brown_gold.css
+Filename: xsl/support/
 Comment: 
 
-Filename: css/colors_ruby_amethyst.css
+Filename: xsl/utilities/
 Comment: 
 
-Filename: css/pretext_add_on.css
+Filename: xsl/extract-mom.xsl
 Comment: 
 
-Filename: css/update_css
+Filename: xsl/pretext-html.xsl
 Comment: 
 
-Filename: css/colors_blue_grey.css
+Filename: xsl/xml-to-json.xsl
 Comment: 
 
-Filename: css/colors_darkmartiansands.css
+Filename: xsl/publisher-variables.xsl
 Comment: 
 
-Filename: css/style_default.css
+Filename: xsl/pretext-units.xsl
 Comment: 
 
-Filename: css/mathbook-content.css
+Filename: xsl/README.md
 Comment: 
 
-Filename: css/kindle.css
+Filename: xsl/pretext-runestone-static.xsl
 Comment: 
 
-Filename: css/style_soundwriting.css
+Filename: xsl/pretext-smc.xsl
 Comment: 
 
-Filename: css/pretext.css
+Filename: xsl/pretext-common.xsl
 Comment: 
 
-Filename: css/colors_blue_green.css
+Filename: xsl/pretext-sage-doctest.xsl
 Comment: 
 
-Filename: css/colors_martiansands.css
+Filename: xsl/pretext-text-utilities.xsl
 Comment: 
 
-Filename: xsl/latex/
+Filename: xsl/pretext-runestone.xsl
 Comment: 
 
-Filename: xsl/localizations/
+Filename: xsl/pretext-text.xsl
 Comment: 
 
-Filename: xsl/support/
+Filename: xsl/pretext-solution-manual-latex.xsl
 Comment: 
 
-Filename: xsl/utilities/
+Filename: xsl/extract-datafile.xsl
 Comment: 
 
-Filename: xsl/extract-mom.xsl
+Filename: xsl/pretext-jupyter.xsl
 Comment: 
 
-Filename: xsl/pretext-runestone.xsl
+Filename: xsl/pretext-ww-problem-sets.xsl
 Comment: 
 
-Filename: xsl/pretext-view-source.xsl
+Filename: xsl/pretext-latex.xsl
 Comment: 
 
-Filename: xsl/pretext-json-manifest.xsl
+Filename: xsl/extract-latex-image.xsl
 Comment: 
 
-Filename: xsl/pretext-assembly.xsl
+Filename: xsl/pretext-view-source.xsl
 Comment: 
 
-Filename: xsl/pretext-beamer.xsl
+Filename: xsl/extract-youtube.xsl
 Comment: 
 
-Filename: xsl/pretext-jupyter.xsl
+Filename: xsl/pretext-assembly.xsl
 Comment: 
 
-Filename: xsl/publisher-variables.xsl
+Filename: xsl/extract-identity.xsl
 Comment: 
 
-Filename: xsl/pretext-html.xsl
+Filename: xsl/extract-asymptote.xsl
 Comment: 
 
-Filename: xsl/extract-identity.xsl
+Filename: xsl/pretext-merge.xsl
 Comment: 
 
-Filename: xsl/pretext-text-utilities.xsl
+Filename: xsl/extract-qrcode.xsl
 Comment: 
 
-Filename: xsl/pretext-epub.xsl
+Filename: xsl/extract-sageplot.xsl
 Comment: 
 
-Filename: xsl/pretext-smc.xsl
+Filename: xsl/pretext-numbers.xsl
 Comment: 
 
-Filename: xsl/pretext-text.xsl
+Filename: xsl/extract-interactive.xsl
 Comment: 
 
-Filename: xsl/README.md
+Filename: xsl/pretext-litprog.xsl
 Comment: 
 
-Filename: xsl/xml-to-json.xsl
+Filename: xsl/extract-trace.xsl
 Comment: 
 
-Filename: xsl/pretext-ww-problem-sets.xsl
+Filename: xsl/pretext-revealjs.xsl
 Comment: 
 
-Filename: xsl/extract-pg.xsl
+Filename: xsl/pretext-beamer.xsl
 Comment: 
 
-Filename: xsl/extract-qrcode.xsl
+Filename: xsl/pretext-braille-preprint.xsl
 Comment: 
 
-Filename: xsl/pretext-solution-manual-latex.xsl
+Filename: xsl/extract-pg.xsl
 Comment: 
 
-Filename: xsl/pretext-numbers.xsl
+Filename: xsl/pretext-epub.xsl
 Comment: 
 
-Filename: xsl/extract-sageplot.xsl
+Filename: xsl/pretext-basic-html.xsl
 Comment: 
 
-Filename: xsl/extract-youtube.xsl
+Filename: xsl/entities.ent
 Comment: 
 
-Filename: xsl/pretext-litprog.xsl
+Filename: xsl/pretext-json-manifest.xsl
 Comment: 
 
-Filename: xsl/pretext-basic-html.xsl
+Filename: xsl/support/play-button/
 Comment: 
 
-Filename: xsl/pretext-sage-doctest.xsl
+Filename: xsl/support/README.md
 Comment: 
 
-Filename: xsl/extract-latex-image.xsl
+Filename: xsl/support/extract-latex-image-labels.xsl
 Comment: 
 
-Filename: xsl/entities.ent
+Filename: xsl/support/extract-math.xsl
 Comment: 
 
-Filename: xsl/pretext-latex.xsl
+Filename: xsl/support/tactile-svg.xsl
 Comment: 
 
-Filename: xsl/pretext-runestone-static.xsl
+Filename: xsl/support/pretext-pg-macros.xsl
 Comment: 
 
-Filename: xsl/extract-interactive.xsl
+Filename: xsl/support/runestone-services.xml
 Comment: 
 
-Filename: xsl/pretext-braille-preprint.xsl
+Filename: xsl/support/package-math.xsl
 Comment: 
 
-Filename: xsl/extract-trace.xsl
+Filename: xsl/support/play-button/README.md
 Comment: 
 
-Filename: xsl/pretext-merge.xsl
+Filename: xsl/support/play-button/play-button.svg
 Comment: 
 
-Filename: xsl/pretext-revealjs.xsl
+Filename: xsl/support/play-button/play-button.png
 Comment: 
 
-Filename: xsl/pretext-common.xsl
+Filename: xsl/latex/pretext-latex-chaos.xsl
 Comment: 
 
-Filename: xsl/extract-asymptote.xsl
+Filename: xsl/latex/pretext-latex-CLP.xsl
 Comment: 
 
-Filename: xsl/pretext-units.xsl
+Filename: xsl/latex/pretext-latex-dyslexic-font.xsl
 Comment: 
 
-Filename: xsl/extract-datafile.xsl
+Filename: xsl/latex/pretext-latex-guide.xsl
 Comment: 
 
-Filename: xsl/utilities/pretext-enhanced-source.xsl
+Filename: xsl/latex/pretext-latex-AIM.xsl
 Comment: 
 
-Filename: xsl/utilities/author-report.xsl
+Filename: xsl/localizations/bg-BG.xml
 Comment: 
 
-Filename: xsl/utilities/fix-deprecations.xsl
+Filename: xsl/localizations/localizations.xml
 Comment: 
 
-Filename: xsl/utilities/deprecate-autoname.sed
+Filename: xsl/localizations/es-ES.xml
 Comment: 
 
-Filename: xsl/utilities/README.md
+Filename: xsl/localizations/README.md
 Comment: 
 
-Filename: xsl/utilities/deprecate-index.sed
+Filename: xsl/localizations/de-DE.xml
 Comment: 
 
-Filename: xsl/latex/pretext-latex-CLP.xsl
+Filename: xsl/localizations/af-ZA.xml
 Comment: 
 
-Filename: xsl/latex/pretext-latex-AIM.xsl
+Filename: xsl/localizations/fr-FR.xml
 Comment: 
 
-Filename: xsl/latex/pretext-latex-chaos.xsl
+Filename: xsl/localizations/fr-CA.xml
 Comment: 
 
-Filename: xsl/latex/pretext-latex-dyslexic-font.xsl
+Filename: xsl/localizations/pt-PT.xml
 Comment: 
 
-Filename: xsl/latex/pretext-latex-guide.xsl
+Filename: xsl/localizations/fi-FI.xml
 Comment: 
 
-Filename: xsl/localizations/pt-PT.xml
+Filename: xsl/localizations/nl-NL.xml
 Comment: 
 
 Filename: xsl/localizations/cs-CZ.xml
 Comment: 
 
-Filename: xsl/localizations/hu-HU.xml
+Filename: xsl/localizations/it-IT.xml
 Comment: 
 
-Filename: xsl/localizations/es-ES.xml
+Filename: xsl/localizations/ca-ES.xml
 Comment: 
 
-Filename: xsl/localizations/it-IT.xml
+Filename: xsl/localizations/pt-BR.xml
 Comment: 
 
-Filename: xsl/localizations/fr-FR.xml
+Filename: xsl/localizations/en-US.xml
 Comment: 
 
-Filename: xsl/localizations/README.md
+Filename: xsl/localizations/hu-HU.xml
 Comment: 
 
-Filename: xsl/localizations/pt-BR.xml
+Filename: xsl/utilities/deprecate-index.sed
 Comment: 
 
-Filename: xsl/localizations/af-ZA.xml
+Filename: xsl/utilities/README.md
 Comment: 
 
-Filename: xsl/localizations/localizations.xml
+Filename: xsl/utilities/deprecate-autoname.sed
 Comment: 
 
-Filename: xsl/localizations/nl-NL.xml
+Filename: xsl/utilities/pretext-enhanced-source.xsl
 Comment: 
 
-Filename: xsl/localizations/ca-ES.xml
+Filename: xsl/utilities/fix-deprecations.xsl
 Comment: 
 
-Filename: xsl/localizations/de-DE.xml
+Filename: xsl/utilities/author-report.xsl
 Comment: 
 
-Filename: xsl/localizations/bg-BG.xml
+Filename: schema/pretext-dev.rng
 Comment: 
 
-Filename: xsl/localizations/fr-CA.xml
+Filename: schema/pretext-dev.rnc
 Comment: 
 
-Filename: xsl/localizations/fi-FI.xml
+Filename: schema/README.md
 Comment: 
 
-Filename: xsl/localizations/en-US.xml
+Filename: schema/pretext-schematron.xsl
 Comment: 
 
-Filename: xsl/support/play-button/
+Filename: schema/pretext.rng
 Comment: 
 
-Filename: xsl/support/pretext-pg-macros.xsl
+Filename: schema/pretext.xml
 Comment: 
 
-Filename: xsl/support/package-math.xsl
+Filename: schema/pretext.rnc
 Comment: 
 
-Filename: xsl/support/README.md
+Filename: schema/build.sh
 Comment: 
 
-Filename: xsl/support/extract-latex-image-labels.xsl
+Filename: schema/xml.xsd
 Comment: 
 
-Filename: xsl/support/tactile-svg.xsl
+Filename: schema/pretext-validation-plus.xsl
 Comment: 
 
-Filename: xsl/support/extract-math.xsl
+Filename: schema/pretext.xsd
 Comment: 
 
-Filename: xsl/support/runestone-services.xml
+Filename: css/colors_martiansands.css
 Comment: 
 
-Filename: xsl/support/play-button/README.md
+Filename: css/colors_darkmartiansands.css
 Comment: 
 
-Filename: xsl/support/play-button/play-button.png
+Filename: css/colors_maroon_grey.css
 Comment: 
 
-Filename: xsl/support/play-button/play-button.svg
+Filename: css/update_css
 Comment: 
 
-Filename: pretext/__init__.py
+Filename: css/README.md
 Comment: 
 
-Filename: pretext/module-test.py
+Filename: css/colors_pastel_blue_orange.css
 Comment: 
 
-Filename: pretext/pretext.cfg
+Filename: css/style_oscarlevin.css
 Comment: 
 
-Filename: pretext/README.md
+Filename: css/mathbook-content.css
 Comment: 
 
-Filename: pretext/pretext
+Filename: css/colors_blue_red.css
 Comment: 
 
-Filename: pretext/pretext.py
+Filename: css/colors_default.css
 Comment: 
 
-Filename: pretext/braille_format.py
+Filename: css/colors_ruby_amethyst.css
 Comment: 
 
-Filename: script/mjsre/
+Filename: css/colors_blue_grey.css
 Comment: 
 
-Filename: script/README.md
+Filename: css/colors_red_blue.css
 Comment: 
 
-Filename: script/mbx
+Filename: css/colors_orange_navy.css
 Comment: 
 
-Filename: script/mjsre/README.md
+Filename: css/colors_green_blue.css
 Comment: 
 
-Filename: script/mjsre/mj-sre-page.js
+Filename: css/epub.css
 Comment: 
 
-Filename: script/mjsre/package.json
+Filename: css/colors_ruby_turquoise.css
 Comment: 
 
-Filename: script/mjsre/update-sre
+Filename: css/pretext.css
 Comment: 
 
-Filename: schema/pretext.xsd
+Filename: css/colors_ruby_emerald.css
 Comment: 
 
-Filename: schema/pretext.rng
+Filename: css/colors_green_plum.css
 Comment: 
 
-Filename: schema/pretext.xml
+Filename: css/kindle.css
 Comment: 
 
-Filename: schema/pretext-schematron.xsl
+Filename: css/style_default.css
 Comment: 
 
-Filename: schema/pretext.rnc
+Filename: css/pretext_add_on.css
 Comment: 
 
-Filename: schema/README.md
+Filename: css/setcolors.css
 Comment: 
 
-Filename: schema/pretext-dev.rnc
+Filename: css/style_soundwriting.css
 Comment: 
 
-Filename: schema/xml.xsd
+Filename: css/colors_blue_green.css
 Comment: 
 
-Filename: schema/build.sh
+Filename: css/colors_brown_gold.css
 Comment: 
 
-Filename: schema/pretext-validation-plus.xsl
+Filename: css/mathbook-3.css
 Comment: 
 
-Filename: schema/pretext-dev.rng
+Filename: css/mathbook-add-on.css
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230622/pretext/generate.py` & `pretext-1.6.1.dev20230623/pretext/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     params: Dict[str, str],
     target_format: str,
     xmlid_root: Optional[str],
     pdf_method: str,
     all_formats: bool = False,
 ) -> None:
     # Dictionary of formats for images based on target
-    formats = {
+    formats: Dict[str, List[str]] = {
         "pdf": [],
         "latex": [],
         "html": ["svg"],
         "epub": ["svg"],
         "kindle": ["png"],
     }
     # set overwrite formats to all when appropriate
@@ -39,15 +39,15 @@
     for _ in range(20):
         source_xml.xinclude()
     if (
         isinstance(
             li := source_xml.xpath("/pretext/*[not(docinfo)]//latex-image"), List
         )
         and len(li) > 0
-        and formats[target_format] is not None
+        and formats[target_format] != []
     ):
         image_output = (output / "latex-image").resolve()
         os.makedirs(image_output, exist_ok=True)
         log.info("Now generating latex-images\n\n")
         # Check for external requirements
         utils.check_asset_execs("latex-image", formats[target_format])
         # call pretext-core's latex image module:
@@ -155,15 +155,15 @@
         "latex": ["pdf"],
         "html": ["html"],
         "epub": ["svg"],
         "kindle": ["png"],
     }
     # set overwrite formats to all when appropriate
     if all_formats:
-        formats[target_format] = {key: ["all"] for key in formats[target_format]}
+        formats[target_format] = ["all"]
     # We assume passed paths are absolute.
     # parse source so we can check for asymptote.
     source_xml = ET.parse(ptxfile)
     for _ in range(20):
         source_xml.xinclude()
     if (
         isinstance(li := source_xml.xpath("/pretext/*[not(docinfo)]//asymptote"), List)
```

### Comparing `pretext-1.6.1.dev20230622/pretext/project.py` & `pretext-1.6.1.dev20230623/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230622/pretext/templates/resources/.gitignore` & `pretext-1.6.1.dev20230623/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230622/pretext/templates/resources/article.zip` & `pretext-1.6.1.dev20230623/pretext/templates/resources/article.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 160110 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:19 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:19 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-22 06:20 .gitignore
--rw-r--r--  2.0 unx       86 b- defN 23-Jun-22 06:19 README.md
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-22 06:20 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-22 06:20 project.ptx
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-22 06:19 assets/frog.jpg
--rw-r--r--  2.0 unx      449 b- defN 23-Jun-22 06:19 source/section-1.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jun-22 06:19 source/main.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-22 06:19 source/section-2.ptx
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-22 06:20 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-22 06:19 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 source/
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-23 06:22 project.ptx
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-23 06:22 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-23 06:22 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-23 06:22 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-23 06:22 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-23 06:22 assets/frog.jpg
+-rw-r--r--  2.0 unx      449 b- defN 23-Jun-23 06:22 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-23 06:22 source/section-2.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Jun-23 06:22 source/main.ptx
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-23 06:22 publication/publication.ptx
 14 files, 164841 bytes uncompressed, 158588 bytes compressed:  3.8%
```

#### zipnote {}

```diff
@@ -6,38 +6,38 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
-Filename: .gitignore
+Filename: project.ptx
 Comment: 
 
 Filename: README.md
 Comment: 
 
+Filename: .gitignore
+Comment: 
+
 Filename: codechat_config.yaml
 Comment: 
 
-Filename: project.ptx
+Filename: .devcontainer/devcontainer.json
 Comment: 
 
 Filename: assets/frog.jpg
 Comment: 
 
 Filename: source/section-1.ptx
 Comment: 
 
-Filename: source/main.ptx
-Comment: 
-
 Filename: source/section-2.ptx
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: source/main.ptx
 Comment: 
 
 Filename: publication/publication.ptx
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230622/pretext/templates/resources/book.zip` & `pretext-1.6.1.dev20230623/pretext/templates/resources/book.zip`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 7616 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:19 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-22 06:20 .gitignore
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-22 06:19 README.md
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-22 06:20 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-22 06:20 project.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-Jun-22 06:19 source/main.ptx
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-22 06:20 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     6114 b- defN 23-Jun-22 06:19 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 source/
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-23 06:22 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-23 06:22 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-23 06:22 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-23 06:22 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-23 06:22 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     1767 b- defN 23-Jun-23 06:22 source/main.ptx
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jun-23 06:22 publication/publication.ptx
 10 files, 15809 bytes uncompressed, 6522 bytes compressed:  58.7%
```

#### zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
-Filename: .gitignore
+Filename: project.ptx
 Comment: 
 
 Filename: README.md
 Comment: 
 
-Filename: codechat_config.yaml
+Filename: .gitignore
 Comment: 
 
-Filename: project.ptx
+Filename: codechat_config.yaml
 Comment: 
 
-Filename: source/main.ptx
+Filename: .devcontainer/devcontainer.json
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: source/main.ptx
 Comment: 
 
 Filename: publication/publication.ptx
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230622/pretext/templates/resources/demo.zip` & `pretext-1.6.1.dev20230623/pretext/templates/resources/demo.zip`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
 Zip file size: 173309 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:19 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:19 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-22 06:20 .gitignore
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-22 06:19 README.md
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-22 06:20 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-22 06:20 project.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:19 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-22 06:19 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jun-22 06:19 assets/jsxgraph/infinity.js
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:19 source/images/
--rw-r--r--  2.0 unx      375 b- defN 23-Jun-22 06:19 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jun-22 06:19 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jun-22 06:19 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jun-22 06:19 source/ch-empty.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-Jun-22 06:19 source/main.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-Jun-22 06:19 source/ex-first.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jun-22 06:19 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jun-22 06:19 source/docinfo.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jun-22 06:19 source/ch-features.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jun-22 06:19 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-Jun-22 06:19 source/ch-generate.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-Jun-22 06:19 source/sec-features.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jun-22 06:19 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jun-22 06:19 source/backmatter.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jun-22 06:19 source/frontmatter.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Jun-22 06:19 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-22 06:19 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      835 b- defN 23-Jun-22 06:19 source/images/cflag.asy
--rw-r--r--  2.0 unx      357 b- defN 23-Jun-22 06:19 source/images/tikz.tex
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-22 06:19 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-22 06:20 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     6092 b- defN 23-Jun-22 06:19 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 source/
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-23 06:22 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-23 06:22 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-23 06:22 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-23 06:22 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-23 06:22 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-23 06:22 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jun-23 06:22 assets/jsxgraph/infinity.js
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 source/images/
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jun-23 06:22 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jun-23 06:22 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-23 06:22 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Jun-23 06:22 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Jun-23 06:22 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Jun-23 06:22 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Jun-23 06:22 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-Jun-23 06:22 source/sec-features.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Jun-23 06:22 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jun-23 06:22 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-Jun-23 06:22 source/ch-features.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jun-23 06:22 source/docinfo.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Jun-23 06:22 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jun-23 06:22 source/main.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Jun-23 06:22 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Jun-23 06:22 source/backmatter.ptx
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-23 06:22 source/images/cflag.asy
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-23 06:22 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-23 06:22 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Jun-23 06:22 source/images/tikz.tex
+-rw-r--r--  2.0 unx     6092 b- defN 23-Jun-23 06:22 publication/publication.ptx
 34 files, 190104 bytes uncompressed, 169353 bytes compressed:  10.9%
```

#### zipnote {}

```diff
@@ -6,98 +6,98 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
-Filename: .gitignore
+Filename: project.ptx
 Comment: 
 
 Filename: README.md
 Comment: 
 
+Filename: .gitignore
+Comment: 
+
 Filename: codechat_config.yaml
 Comment: 
 
-Filename: project.ptx
+Filename: .devcontainer/devcontainer.json
 Comment: 
 
 Filename: assets/jsxgraph/
 Comment: 
 
 Filename: assets/frog.jpg
 Comment: 
 
 Filename: assets/jsxgraph/infinity.js
 Comment: 
 
 Filename: source/images/
 Comment: 
 
-Filename: source/fig-sage2d.ptx
-Comment: 
-
-Filename: source/fig-sage3d.ptx
+Filename: source/ex-first.ptx
 Comment: 
 
-Filename: source/sec-first-examples.ptx
+Filename: source/ch-first with spaces.ptx
 Comment: 
 
 Filename: source/ch-empty.ptx
 Comment: 
 
-Filename: source/main.ptx
+Filename: source/fig-sage3d.ptx
 Comment: 
 
-Filename: source/ex-first.ptx
+Filename: source/frontmatter.ptx
 Comment: 
 
-Filename: source/sec-first-intro.ptx
+Filename: source/sec-first-examples.ptx
 Comment: 
 
-Filename: source/docinfo.ptx
+Filename: source/fig-asymptote.ptx
 Comment: 
 
-Filename: source/ch-features.ptx
+Filename: source/sec-features.ptx
 Comment: 
 
-Filename: source/fig-asymptote.ptx
+Filename: source/fig-tikz.ptx
 Comment: 
 
 Filename: source/ch-generate.ptx
 Comment: 
 
-Filename: source/sec-features.ptx
+Filename: source/ch-features.ptx
 Comment: 
 
-Filename: source/fig-tikz.ptx
+Filename: source/docinfo.ptx
 Comment: 
 
-Filename: source/backmatter.ptx
+Filename: source/sec-first-intro.ptx
 Comment: 
 
-Filename: source/frontmatter.ptx
+Filename: source/main.ptx
 Comment: 
 
-Filename: source/ch-first with spaces.ptx
+Filename: source/fig-sage2d.ptx
 Comment: 
 
-Filename: source/images/sageplot3d.sage
+Filename: source/backmatter.ptx
 Comment: 
 
 Filename: source/images/cflag.asy
 Comment: 
 
-Filename: source/images/tikz.tex
+Filename: source/images/sageplot2d.sage
 Comment: 
 
-Filename: source/images/sageplot2d.sage
+Filename: source/images/sageplot3d.sage
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: source/images/tikz.tex
 Comment: 
 
 Filename: publication/publication.ptx
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230622/pretext/templates/resources/devcontainer.json` & `pretext-1.6.1.dev20230623/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230622/pretext/templates/resources/hello.zip` & `pretext-1.6.1.dev20230623/pretext/templates/resources/hello.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 4657 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:19 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-22 06:20 .gitignore
--rw-r--r--  2.0 unx       69 b- defN 23-Jun-22 06:19 README.md
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-22 06:20 codechat_config.yaml
--rw-r--r--  2.0 unx     1217 b- defN 23-Jun-22 06:19 project.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-Jun-22 06:19 source/main.ptx
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-22 06:20 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-22 06:19 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 source/
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jun-23 06:22 project.ptx
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-23 06:22 README.md
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-23 06:22 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-23 06:22 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-23 06:22 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-23 06:22 source/main.ptx
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-23 06:22 publication/publication.ptx
 10 files, 7820 bytes uncompressed, 3563 bytes compressed:  54.4%
```

#### zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
-Filename: .gitignore
+Filename: project.ptx
 Comment: 
 
 Filename: README.md
 Comment: 
 
-Filename: codechat_config.yaml
+Filename: .gitignore
 Comment: 
 
-Filename: project.ptx
+Filename: codechat_config.yaml
 Comment: 
 
-Filename: source/main.ptx
+Filename: .devcontainer/devcontainer.json
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: source/main.ptx
 Comment: 
 
 Filename: publication/publication.ptx
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230622/pretext/templates/resources/project.ptx` & `pretext-1.6.1.dev20230623/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230622/pretext/templates/resources/slideshow.zip` & `pretext-1.6.1.dev20230623/pretext/templates/resources/slideshow.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8392 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:20 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:19 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-22 06:19 xsl/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-22 06:20 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-22 06:20 codechat_config.yaml
--rw-r--r--  2.0 unx      784 b- defN 23-Jun-22 06:19 project.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-Jun-22 06:19 source/main.ptx
--rw-r--r--  2.0 unx      190 b- defN 23-Jun-22 06:19 xsl/slides.xsl
--rw-r--r--  2.0 unx     2192 b- defN 23-Jun-22 06:20 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     2097 b- defN 23-Jun-22 06:19 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 06:22 xsl/
+-rw-r--r--  2.0 unx      784 b- defN 23-Jun-23 06:22 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-23 06:22 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-23 06:22 codechat_config.yaml
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jun-23 06:22 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-23 06:22 xsl/slides.xsl
+-rw-r--r--  2.0 unx    11200 b- defN 23-Jun-23 06:22 source/main.ptx
+-rw-r--r--  2.0 unx     2097 b- defN 23-Jun-23 06:22 publication/publication.ptx
 11 files, 20407 bytes uncompressed, 7204 bytes compressed:  64.7%
```

#### zipnote {}

```diff
@@ -6,29 +6,29 @@
 
 Filename: source/
 Comment: 
 
 Filename: xsl/
 Comment: 
 
-Filename: .gitignore
+Filename: project.ptx
 Comment: 
 
-Filename: codechat_config.yaml
+Filename: .gitignore
 Comment: 
 
-Filename: project.ptx
+Filename: codechat_config.yaml
 Comment: 
 
-Filename: source/main.ptx
+Filename: .devcontainer/devcontainer.json
 Comment: 
 
 Filename: xsl/slides.xsl
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: source/main.ptx
 Comment: 
 
 Filename: publication/publication.ptx
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230622/pretext/utils.py` & `pretext-1.6.1.dev20230623/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230622/pyproject.toml` & `pretext-1.6.1.dev20230623/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "1.6.1.dev20230622"
+version = "1.6.1.dev20230623"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
@@ -75,28 +75,32 @@
 # mypy configuration
 # ==================
 # To run, execute ``mypy`` from the directory containing this file.
 #
 # This section `must <https://mypy.readthedocs.io/en/stable/config_file.html#config-file-format>`_ be present.
 [tool.mypy]
 # See `files <https://mypy.readthedocs.io/en/stable/config_file.html#confval-files>`_.
-files = "pretext"
-exclude = "^pretext/core/pretext.py"
+files = "pretext,scripts,tests"
+exclude = "^pretext/core/pretext\\.py$"
 check_untyped_defs = true
 disallow_untyped_defs = true
 
 # Ignores for libraries with no type hints
 # ----------------------------------------
 [[tool.mypy.overrides]]
 module = [
     "click_log",
     "single_version",
     "ghp_import",
     # We're installing ``lxml-stubs``, but it doesn't have stubs for this yet.
     "lxml.ElementInclude",
+    # TODO: Currently, the ``tomli`` package doesn't support Python 3.11, so
+    # it's not installed there. For now, ignore this module. Remove the ignore
+    # when ``tomli`` provide support for Python 3.11.
+    "tomli",
 ]
 ignore_missing_imports = true
 
 
 # Coverage configuration
 # ======================
 [tool.coverage.run]
```

### Comparing `pretext-1.6.1.dev20230622/PKG-INFO` & `pretext-1.6.1.dev20230623/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.6.1.dev20230622
+Version: 1.6.1.dev20230623
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

