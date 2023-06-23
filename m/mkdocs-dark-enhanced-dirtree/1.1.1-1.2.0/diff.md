# Comparing `tmp/mkdocs-dark_enhanced_dirtree-1.1.1.tar.gz` & `tmp/mkdocs-dark_enhanced_dirtree-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-dark_enhanced_dirtree-1.1.1.tar", last modified: Sun Mar 19 21:49:35 2023, max compression
+gzip compressed data, was "mkdocs-dark_enhanced_dirtree-1.2.0.tar", last modified: Thu Jun 22 15:38:05 2023, max compression
```

## Comparing `mkdocs-dark_enhanced_dirtree-1.1.1.tar` & `mkdocs-dark_enhanced_dirtree-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,676 @@
-drwxr-xr-x   0 j         (1000) sam       (1000)        0 2023-03-19 21:49:35.586593 mkdocs-dark_enhanced_dirtree-1.1.1/
--rw-r--r--   0 j         (1000) sam       (1000)     1072 2023-03-06 17:34:55.000000 mkdocs-dark_enhanced_dirtree-1.1.1/LICENSE
--rw-r--r--   0 j         (1000) sam       (1000)      205 2023-03-06 17:34:55.000000 mkdocs-dark_enhanced_dirtree-1.1.1/MANIFEST.in
--rw-r--r--   0 j         (1000) sam       (1000)      276 2023-03-19 21:49:35.586593 mkdocs-dark_enhanced_dirtree-1.1.1/PKG-INFO
--rw-r--r--   0 j         (1000) sam       (1000)      382 2023-03-09 23:08:20.000000 mkdocs-dark_enhanced_dirtree-1.1.1/README.md
-drwxr-xr-x   0 j         (1000) sam       (1000)        0 2023-03-19 21:49:35.586593 mkdocs-dark_enhanced_dirtree-1.1.1/dark_enhanced_dirtree/
--rw-r--r--   0 j         (1000) sam       (1000)        0 2023-03-06 17:34:55.000000 mkdocs-dark_enhanced_dirtree-1.1.1/dark_enhanced_dirtree/__init__.py
-drwxr-xr-x   0 j         (1000) sam       (1000)        0 2023-03-19 21:49:35.586593 mkdocs-dark_enhanced_dirtree-1.1.1/mkdocs_dark_enhanced_dirtree.egg-info/
--rw-r--r--   0 j         (1000) sam       (1000)      276 2023-03-19 21:49:35.000000 mkdocs-dark_enhanced_dirtree-1.1.1/mkdocs_dark_enhanced_dirtree.egg-info/PKG-INFO
--rw-r--r--   0 j         (1000) sam       (1000)      386 2023-03-19 21:49:35.000000 mkdocs-dark_enhanced_dirtree-1.1.1/mkdocs_dark_enhanced_dirtree.egg-info/SOURCES.txt
--rw-r--r--   0 j         (1000) sam       (1000)        1 2023-03-19 21:49:35.000000 mkdocs-dark_enhanced_dirtree-1.1.1/mkdocs_dark_enhanced_dirtree.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) sam       (1000)       62 2023-03-19 21:49:35.000000 mkdocs-dark_enhanced_dirtree-1.1.1/mkdocs_dark_enhanced_dirtree.egg-info/entry_points.txt
--rw-r--r--   0 j         (1000) sam       (1000)        1 2023-03-09 23:07:29.000000 mkdocs-dark_enhanced_dirtree-1.1.1/mkdocs_dark_enhanced_dirtree.egg-info/not-zip-safe
--rw-r--r--   0 j         (1000) sam       (1000)       22 2023-03-19 21:49:35.000000 mkdocs-dark_enhanced_dirtree-1.1.1/mkdocs_dark_enhanced_dirtree.egg-info/top_level.txt
--rw-r--r--   0 j         (1000) sam       (1000)       38 2023-03-19 21:49:35.586593 mkdocs-dark_enhanced_dirtree-1.1.1/setup.cfg
--rw-r--r--   0 j         (1000) sam       (1000)      606 2023-03-19 21:49:34.000000 mkdocs-dark_enhanced_dirtree-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 15:38:05.598578 mkdocs-dark_enhanced_dirtree-1.2.0/
+-rw-rw-rw-   0        0        0     1085 2023-06-22 13:50:02.000000 mkdocs-dark_enhanced_dirtree-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      210 2023-06-22 15:37:36.000000 mkdocs-dark_enhanced_dirtree-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      285 2023-06-22 15:38:05.586367 mkdocs-dark_enhanced_dirtree-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2023-06-22 13:49:32.000000 mkdocs-dark_enhanced_dirtree-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 15:37:56.263955 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 15:37:56.275937 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/css/
+-rw-rw-rw-   0        0        0      365 2023-03-10 08:29:32.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/css/search.css
+-rw-rw-rw-   0        0        0     7117 2023-03-22 08:17:18.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/css/theme.css
+drwxrwxrwx   0        0        0        0 2023-06-22 15:37:56.299893 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/
+drwxrwxrwx   0        0        0        0 2023-06-22 15:37:56.345215 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/
+-rw-rw-rw-   0        0        0    78137 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/core.js
+-rw-rw-rw-   0        0        0    20561 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/core.min.js
+-rw-rw-rw-   0        0        0    78137 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/highlight.js
+drwxrwxrwx   0        0        0        0 2023-06-22 15:37:59.681734 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/
+-rw-rw-rw-   0        0        0   159637 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/1c.min.js
+-rw-rw-rw-   0        0        0      749 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/abnf.min.js
+-rw-rw-rw-   0        0        0      868 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/accesslog.min.js
+-rw-rw-rw-   0        0        0     1571 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/actionscript.min.js
+-rw-rw-rw-   0        0        0     2239 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/ada.min.js
+-rw-rw-rw-   0        0        0     1802 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/angelscript.min.js
+-rw-rw-rw-   0        0        0     1033 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/apache.min.js
+-rw-rw-rw-   0        0        0     2607 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/applescript.min.js
+-rw-rw-rw-   0        0        0     4043 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/arcade.min.js
+-rw-rw-rw-   0        0        0    10341 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/arduino.min.js
+-rw-rw-rw-   0        0        0     3241 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/armasm.min.js
+-rw-rw-rw-   0        0        0     2530 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/asciidoc.min.js
+-rw-rw-rw-   0        0        0     2776 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/aspectj.min.js
+-rw-rw-rw-   0        0        0     1008 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/autohotkey.min.js
+-rw-rw-rw-   0        0        0     6691 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/autoit.min.js
+-rw-rw-rw-   0        0        0     2058 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/avrasm.min.js
+-rw-rw-rw-   0        0        0      746 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/awk.min.js
+-rw-rw-rw-   0        0        0     1755 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/axapta.min.js
+-rw-rw-rw-   0        0        0     3099 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/bash.min.js
+-rw-rw-rw-   0        0        0     1900 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/basic.min.js
+-rw-rw-rw-   0        0        0      362 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/bnf.min.js
+-rw-rw-rw-   0        0        0      536 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/brainfuck.min.js
+-rw-rw-rw-   0        0        0     3950 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/c.min.js
+-rw-rw-rw-   0        0        0     1257 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/cal.min.js
+-rw-rw-rw-   0        0        0      868 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/capnproto.min.js
+-rw-rw-rw-   0        0        0     1331 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/ceylon.min.js
+-rw-rw-rw-   0        0        0      683 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/clean.min.js
+-rw-rw-rw-   0        0        0      272 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/clojure-repl.min.js
+-rw-rw-rw-   0        0        0     4204 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/clojure.min.js
+-rw-rw-rw-   0        0        0     2537 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/cmake.min.js
+-rw-rw-rw-   0        0        0     3105 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/coffeescript.min.js
+-rw-rw-rw-   0        0        0     4370 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/coq.min.js
+-rw-rw-rw-   0        0        0     1420 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/cos.min.js
+-rw-rw-rw-   0        0        0     5758 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/cpp.min.js
+-rw-rw-rw-   0        0        0     1492 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/crmsh.min.js
+-rw-rw-rw-   0        0        0     3796 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/crystal.min.js
+-rw-rw-rw-   0        0        0     4045 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/csharp.min.js
+-rw-rw-rw-   0        0        0      606 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/csp.min.js
+-rw-rw-rw-   0        0        0     9979 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/css.min.js
+-rw-rw-rw-   0        0        0     2530 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/d.min.js
+-rw-rw-rw-   0        0        0     2208 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/dart.min.js
+-rw-rw-rw-   0        0        0     2285 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/delphi.min.js
+-rw-rw-rw-   0        0        0      618 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/diff.min.js
+-rw-rw-rw-   0        0        0     1869 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/django.min.js
+-rw-rw-rw-   0        0        0     1900 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/dns.min.js
+-rw-rw-rw-   0        0        0      516 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/dockerfile.min.js
+-rw-rw-rw-   0        0        0     1433 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/dos.min.js
+-rw-rw-rw-   0        0        0      673 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/dsconfig.min.js
+-rw-rw-rw-   0        0        0     1509 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/dts.min.js
+-rw-rw-rw-   0        0        0      532 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/dust.min.js
+-rw-rw-rw-   0        0        0      471 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/ebnf.min.js
+-rw-rw-rw-   0        0        0     2550 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/elixir.min.js
+-rw-rw-rw-   0        0        0     1276 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/elm.min.js
+-rw-rw-rw-   0        0        0      285 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/erb.min.js
+-rw-rw-rw-   0        0        0      895 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/erlang-repl.min.js
+-rw-rw-rw-   0        0        0     2084 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/erlang.min.js
+-rw-rw-rw-   0        0        0     5359 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/excel.min.js
+-rw-rw-rw-   0        0        0      474 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/fix.min.js
+-rw-rw-rw-   0        0        0      733 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/flix.min.js
+-rw-rw-rw-   0        0        0     5783 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/fortran.min.js
+-rw-rw-rw-   0        0        0     4209 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/fsharp.min.js
+-rw-rw-rw-   0        0        0     3058 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/gams.min.js
+-rw-rw-rw-   0        0        0    13096 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/gauss.min.js
+-rw-rw-rw-   0        0        0     1104 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/gcode.min.js
+-rw-rw-rw-   0        0        0      619 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/gherkin.min.js
+-rw-rw-rw-   0        0        0     8401 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/glsl.min.js
+-rw-rw-rw-   0        0        0    56436 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/gml.min.js
+-rw-rw-rw-   0        0        0     1216 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/go.min.js
+-rw-rw-rw-   0        0        0      718 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/golo.min.js
+-rw-rw-rw-   0        0        0     1934 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/gradle.min.js
+-rw-rw-rw-   0        0        0      833 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/graphql.min.js
+-rw-rw-rw-   0        0        0     1670 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/groovy.min.js
+-rw-rw-rw-   0        0        0     1182 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/haml.min.js
+-rw-rw-rw-   0        0        0     2338 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/handlebars.min.js
+-rw-rw-rw-   0        0        0     2070 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/haskell.min.js
+-rw-rw-rw-   0        0        0     1993 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/haxe.min.js
+-rw-rw-rw-   0        0        0     3460 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/hsp.min.js
+-rw-rw-rw-   0        0        0      918 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/http.min.js
+-rw-rw-rw-   0        0        0     3049 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/hy.min.js
+-rw-rw-rw-   0        0        0      753 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/inform7.min.js
+-rw-rw-rw-   0        0        0     1056 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/ini.min.js
+-rw-rw-rw-   0        0        0     4833 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/irpf90.min.js
+-rw-rw-rw-   0        0        0    83289 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/isbl.min.js
+-rw-rw-rw-   0        0        0     2817 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/java.min.js
+-rw-rw-rw-   0        0        0     6479 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/javascript.min.js
+-rw-rw-rw-   0        0        0      951 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/jboss-cli.min.js
+-rw-rw-rw-   0        0        0      499 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/json.min.js
+-rw-rw-rw-   0        0        0      299 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/julia-repl.min.js
+-rw-rw-rw-   0        0        0     4091 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/julia.min.js
+-rw-rw-rw-   0        0        0     3546 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/kotlin.min.js
+-rw-rw-rw-   0        0        0     3134 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/lasso.min.js
+-rw-rw-rw-   0        0        0     3513 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/latex.min.js
+-rw-rw-rw-   0        0        0      315 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/ldif.min.js
+-rw-rw-rw-   0        0        0      516 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/leaf.min.js
+-rw-rw-rw-   0        0        0    11009 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/less.min.js
+-rw-rw-rw-   0        0        0     1237 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/lisp.min.js
+-rw-rw-rw-   0        0        0     8329 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/livecodeserver.min.js
+-rw-rw-rw-   0        0        0     3501 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/livescript.min.js
+-rw-rw-rw-   0        0        0     2708 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/llvm.min.js
+-rw-rw-rw-   0        0        0    11985 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/lsl.min.js
+-rw-rw-rw-   0        0        0     1980 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/lua.min.js
+-rw-rw-rw-   0        0        0     1168 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/makefile.min.js
+-rw-rw-rw-   0        0        0     2140 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/markdown.min.js
+-rw-rw-rw-   0        0        0   112951 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/mathematica.min.js
+-rw-rw-rw-   0        0        0     2364 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/matlab.min.js
+-rw-rw-rw-   0        0        0    28790 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/maxima.min.js
+-rw-rw-rw-   0        0        0    16606 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/mel.min.js
+-rw-rw-rw-   0        0        0     2152 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/mercury.min.js
+-rw-rw-rw-   0        0        0     2545 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/mipsasm.min.js
+-rw-rw-rw-   0        0        0      795 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/mizar.min.js
+-rw-rw-rw-   0        0        0      386 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/mojolicious.min.js
+-rw-rw-rw-   0        0        0     1599 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/monkey.min.js
+-rw-rw-rw-   0        0        0     1813 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/moonscript.min.js
+-rw-rw-rw-   0        0        0     3656 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/n1ql.min.js
+-rw-rw-rw-   0        0        0      635 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/nestedtext.min.js
+-rw-rw-rw-   0        0        0     1635 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/nginx.min.js
+-rw-rw-rw-   0        0        0     1759 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/nim.min.js
+-rw-rw-rw-   0        0        0      831 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/nix.min.js
+-rw-rw-rw-   0        0        0      322 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/node-repl.min.js
+-rw-rw-rw-   0        0        0     6403 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/nsis.min.js
+-rw-rw-rw-   0        0        0     2960 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/objectivec.min.js
+-rw-rw-rw-   0        0        0     1337 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/ocaml.min.js
+-rw-rw-rw-   0        0        0     1379 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/openscad.min.js
+-rw-rw-rw-   0        0        0     1983 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/oxygene.min.js
+-rw-rw-rw-   0        0        0      648 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/parser3.min.js
+-rw-rw-rw-   0        0        0     3998 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/perl.min.js
+-rw-rw-rw-   0        0        0     1358 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/pf.min.js
+-rw-rw-rw-   0        0        0    19044 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/pgsql.min.js
+-rw-rw-rw-   0        0        0      523 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/php-template.min.js
+-rw-rw-rw-   0        0        0     6274 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/php.min.js
+-rw-rw-rw-   0        0        0      205 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/plaintext.min.js
+-rw-rw-rw-   0        0        0     1036 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/pony.min.js
+-rw-rw-rw-   0        0        0     4476 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/powershell.min.js
+-rw-rw-rw-   0        0        0     4419 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/processing.min.js
+-rw-rw-rw-   0        0        0      581 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/profile.min.js
+-rw-rw-rw-   0        0        0      765 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/prolog.min.js
+-rw-rw-rw-   0        0        0      665 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/properties.min.js
+-rw-rw-rw-   0        0        0      767 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/protobuf.min.js
+-rw-rw-rw-   0        0        0     4202 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/puppet.min.js
+-rw-rw-rw-   0        0        0     1680 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/purebasic.min.js
+-rw-rw-rw-   0        0        0      323 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/python-repl.min.js
+-rw-rw-rw-   0        0        0     3565 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/python.min.js
+-rw-rw-rw-   0        0        0     1229 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/q.min.js
+-rw-rw-rw-   0        0        0     2805 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/qml.min.js
+-rw-rw-rw-   0        0        0     3052 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/r.min.js
+-rw-rw-rw-   0        0        0     3430 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/reasonml.min.js
+-rw-rw-rw-   0        0        0     1378 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/rib.min.js
+-rw-rw-rw-   0        0        0      813 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/roboconf.min.js
+-rw-rw-rw-   0        0        0     2570 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/routeros.min.js
+-rw-rw-rw-   0        0        0     1377 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/rsl.min.js
+-rw-rw-rw-   0        0        0     4085 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/ruby.min.js
+-rw-rw-rw-   0        0        0     3927 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/ruleslanguage.min.js
+-rw-rw-rw-   0        0        0     2932 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/rust.min.js
+-rw-rw-rw-   0        0        0     4842 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/sas.min.js
+-rw-rw-rw-   0        0        0     1939 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/scala.min.js
+-rw-rw-rw-   0        0        0     3416 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/scheme.min.js
+-rw-rw-rw-   0        0        0     1299 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/scilab.min.js
+-rw-rw-rw-   0        0        0    11093 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/scss.min.js
+-rw-rw-rw-   0        0        0      327 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/shell.min.js
+-rw-rw-rw-   0        0        0     1101 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/smali.min.js
+-rw-rw-rw-   0        0        0      725 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/smalltalk.min.js
+-rw-rw-rw-   0        0        0     1234 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/sml.min.js
+-rw-rw-rw-   0        0        0    41297 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/sqf.min.js
+-rw-rw-rw-   0        0        0     6547 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/sql.min.js
+-rw-rw-rw-   0        0        0     5887 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/stan.min.js
+-rw-rw-rw-   0        0        0    16805 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/stata.min.js
+-rw-rw-rw-   0        0        0      710 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/step21.min.js
+-rw-rw-rw-   0        0        0    10306 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/stylus.min.js
+-rw-rw-rw-   0        0        0      600 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/subunit.min.js
+-rw-rw-rw-   0        0        0     7557 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/swift.min.js
+-rw-rw-rw-   0        0        0      522 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/taggerscript.min.js
+-rw-rw-rw-   0        0        0      478 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/tap.min.js
+-rw-rw-rw-   0        0        0     2020 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/tcl.min.js
+-rw-rw-rw-   0        0        0      778 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/thrift.min.js
+-rw-rw-rw-   0        0        0     1721 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/tp.min.js
+-rw-rw-rw-   0        0        0     2535 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/twig.min.js
+-rw-rw-rw-   0        0        0     7593 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/typescript.min.js
+-rw-rw-rw-   0        0        0      993 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/vala.min.js
+-rw-rw-rw-   0        0        0     2746 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/vbnet.min.js
+-rw-rw-rw-   0        0        0      247 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/vbscript-html.min.js
+-rw-rw-rw-   0        0        0     1949 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/vbscript.min.js
+-rw-rw-rw-   0        0        0     6117 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/verilog.min.js
+-rw-rw-rw-   0        0        0     2060 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/vhdl.min.js
+-rw-rw-rw-   0        0        0     8696 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/vim.min.js
+-rw-rw-rw-   0        0        0     1775 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/wasm.min.js
+-rw-rw-rw-   0        0        0     2367 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/wren.min.js
+-rw-rw-rw-   0        0        0    19134 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/x86asm.min.js
+-rw-rw-rw-   0        0        0     1981 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/xl.min.js
+-rw-rw-rw-   0        0        0     2048 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/xml.min.js
+-rw-rw-rw-   0        0        0     5718 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/xquery.min.js
+-rw-rw-rw-   0        0        0     1829 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/yaml.min.js
+-rw-rw-rw-   0        0        0     1689 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/es/languages/zephir.min.js
+-rw-rw-rw-   0        0        0    87297 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/highlight.js
+-rw-rw-rw-   0        0        0   150471 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/highlight.min.js
+drwxrwxrwx   0        0        0        0 2023-06-22 15:38:02.659323 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/
+-rw-rw-rw-   0        0        0   159640 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/1c.min.js
+-rw-rw-rw-   0        0        0      752 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/abnf.min.js
+-rw-rw-rw-   0        0        0      878 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/accesslog.min.js
+-rw-rw-rw-   0        0        0     1584 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/actionscript.min.js
+-rw-rw-rw-   0        0        0     2243 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/ada.min.js
+-rw-rw-rw-   0        0        0     1814 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/angelscript.min.js
+-rw-rw-rw-   0        0        0     1040 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/apache.min.js
+-rw-rw-rw-   0        0        0     2621 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/applescript.min.js
+-rw-rw-rw-   0        0        0     4048 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/arcade.min.js
+-rw-rw-rw-   0        0        0    10349 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/arduino.min.js
+-rw-rw-rw-   0        0        0     3248 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/armasm.min.js
+-rw-rw-rw-   0        0        0     2539 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/asciidoc.min.js
+-rw-rw-rw-   0        0        0     2786 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/aspectj.min.js
+-rw-rw-rw-   0        0        0     1021 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/autohotkey.min.js
+-rw-rw-rw-   0        0        0     6698 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/autoit.min.js
+-rw-rw-rw-   0        0        0     2065 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/avrasm.min.js
+-rw-rw-rw-   0        0        0      750 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/awk.min.js
+-rw-rw-rw-   0        0        0     1764 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/axapta.min.js
+-rw-rw-rw-   0        0        0     3104 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/bash.min.js
+-rw-rw-rw-   0        0        0     1908 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/basic.min.js
+-rw-rw-rw-   0        0        0      366 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/bnf.min.js
+-rw-rw-rw-   0        0        0      546 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/brainfuck.min.js
+-rw-rw-rw-   0        0        0     3952 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/c.min.js
+-rw-rw-rw-   0        0        0     1261 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/cal.min.js
+-rw-rw-rw-   0        0        0      878 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/capnproto.min.js
+-rw-rw-rw-   0        0        0     1338 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/ceylon.min.js
+-rw-rw-rw-   0        0        0      689 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/clean.min.js
+-rw-rw-rw-   0        0        0      285 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/clojure-repl.min.js
+-rw-rw-rw-   0        0        0     4212 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/clojure.min.js
+-rw-rw-rw-   0        0        0     2543 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/cmake.min.js
+-rw-rw-rw-   0        0        0     3120 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/coffeescript.min.js
+-rw-rw-rw-   0        0        0     4374 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/coq.min.js
+-rw-rw-rw-   0        0        0     1424 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/cos.min.js
+-rw-rw-rw-   0        0        0     5764 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/cpp.min.js
+-rw-rw-rw-   0        0        0     1498 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/crmsh.min.js
+-rw-rw-rw-   0        0        0     3804 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/crystal.min.js
+-rw-rw-rw-   0        0        0     4052 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/csharp.min.js
+-rw-rw-rw-   0        0        0      612 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/csp.min.js
+-rw-rw-rw-   0        0        0     9983 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/css.min.js
+-rw-rw-rw-   0        0        0     2532 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/d.min.js
+-rw-rw-rw-   0        0        0     2213 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/dart.min.js
+-rw-rw-rw-   0        0        0     2292 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/delphi.min.js
+-rw-rw-rw-   0        0        0      623 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/diff.min.js
+-rw-rw-rw-   0        0        0     1876 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/django.min.js
+-rw-rw-rw-   0        0        0     1904 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/dns.min.js
+-rw-rw-rw-   0        0        0      527 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/dockerfile.min.js
+-rw-rw-rw-   0        0        0     1435 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/dos.min.js
+-rw-rw-rw-   0        0        0      682 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/dsconfig.min.js
+-rw-rw-rw-   0        0        0     1513 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/dts.min.js
+-rw-rw-rw-   0        0        0      537 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/dust.min.js
+-rw-rw-rw-   0        0        0      476 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/ebnf.min.js
+-rw-rw-rw-   0        0        0     2557 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/elixir.min.js
+-rw-rw-rw-   0        0        0     1280 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/elm.min.js
+-rw-rw-rw-   0        0        0      289 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/erb.min.js
+-rw-rw-rw-   0        0        0      907 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/erlang-repl.min.js
+-rw-rw-rw-   0        0        0     2091 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/erlang.min.js
+-rw-rw-rw-   0        0        0     5365 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/excel.min.js
+-rw-rw-rw-   0        0        0      478 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/fix.min.js
+-rw-rw-rw-   0        0        0      738 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/flix.min.js
+-rw-rw-rw-   0        0        0     5791 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/fortran.min.js
+-rw-rw-rw-   0        0        0     4216 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/fsharp.min.js
+-rw-rw-rw-   0        0        0     3063 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/gams.min.js
+-rw-rw-rw-   0        0        0    13102 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/gauss.min.js
+-rw-rw-rw-   0        0        0     1108 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/gcode.min.js
+-rw-rw-rw-   0        0        0      625 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/gherkin.min.js
+-rw-rw-rw-   0        0        0     8406 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/glsl.min.js
+-rw-rw-rw-   0        0        0    56440 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/gml.min.js
+-rw-rw-rw-   0        0        0     1219 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/go.min.js
+-rw-rw-rw-   0        0        0      723 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/golo.min.js
+-rw-rw-rw-   0        0        0     1939 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/gradle.min.js
+-rw-rw-rw-   0        0        0      841 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/graphql.min.js
+-rw-rw-rw-   0        0        0     1677 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/groovy.min.js
+-rw-rw-rw-   0        0        0     1187 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/haml.min.js
+-rw-rw-rw-   0        0        0     2349 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/handlebars.min.js
+-rw-rw-rw-   0        0        0     2078 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/haskell.min.js
+-rw-rw-rw-   0        0        0     1996 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/haxe.min.js
+-rw-rw-rw-   0        0        0     3464 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/hsp.min.js
+-rw-rw-rw-   0        0        0      923 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/http.min.js
+-rw-rw-rw-   0        0        0     3054 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/hy.min.js
+-rw-rw-rw-   0        0        0      763 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/inform7.min.js
+-rw-rw-rw-   0        0        0     1058 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/ini.min.js
+-rw-rw-rw-   0        0        0     4840 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/irpf90.min.js
+-rw-rw-rw-   0        0        0    83294 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/isbl.min.js
+-rw-rw-rw-   0        0        0     2822 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/java.min.js
+-rw-rw-rw-   0        0        0     6490 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/javascript.min.js
+-rw-rw-rw-   0        0        0      961 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/jboss-cli.min.js
+-rw-rw-rw-   0        0        0      502 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/json.min.js
+-rw-rw-rw-   0        0        0      312 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/julia-repl.min.js
+-rw-rw-rw-   0        0        0     4097 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/julia.min.js
+-rw-rw-rw-   0        0        0     3553 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/kotlin.min.js
+-rw-rw-rw-   0        0        0     3140 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/lasso.min.js
+-rw-rw-rw-   0        0        0     3517 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/latex.min.js
+-rw-rw-rw-   0        0        0      320 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/ldif.min.js
+-rw-rw-rw-   0        0        0      521 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/leaf.min.js
+-rw-rw-rw-   0        0        0    11014 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/less.min.js
+-rw-rw-rw-   0        0        0     1244 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/lisp.min.js
+-rw-rw-rw-   0        0        0     8344 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/livecodeserver.min.js
+-rw-rw-rw-   0        0        0     3512 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/livescript.min.js
+-rw-rw-rw-   0        0        0     2713 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/llvm.min.js
+-rw-rw-rw-   0        0        0    11989 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/lsl.min.js
+-rw-rw-rw-   0        0        0     1986 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/lua.min.js
+-rw-rw-rw-   0        0        0     1177 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/makefile.min.js
+-rw-rw-rw-   0        0        0     2149 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/markdown.min.js
+-rw-rw-rw-   0        0        0   112963 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/mathematica.min.js
+-rw-rw-rw-   0        0        0     2371 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/matlab.min.js
+-rw-rw-rw-   0        0        0    28797 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/maxima.min.js
+-rw-rw-rw-   0        0        0    16610 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/mel.min.js
+-rw-rw-rw-   0        0        0     2160 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/mercury.min.js
+-rw-rw-rw-   0        0        0     2553 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/mipsasm.min.js
+-rw-rw-rw-   0        0        0      801 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/mizar.min.js
+-rw-rw-rw-   0        0        0      398 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/mojolicious.min.js
+-rw-rw-rw-   0        0        0     1606 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/monkey.min.js
+-rw-rw-rw-   0        0        0     1824 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/moonscript.min.js
+-rw-rw-rw-   0        0        0     3661 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/n1ql.min.js
+-rw-rw-rw-   0        0        0      646 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/nestedtext.min.js
+-rw-rw-rw-   0        0        0     1641 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/nginx.min.js
+-rw-rw-rw-   0        0        0     1763 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/nim.min.js
+-rw-rw-rw-   0        0        0      837 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/nix.min.js
+-rw-rw-rw-   0        0        0      332 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/node-repl.min.js
+-rw-rw-rw-   0        0        0     6408 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/nsis.min.js
+-rw-rw-rw-   0        0        0     2971 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/objectivec.min.js
+-rw-rw-rw-   0        0        0     1343 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/ocaml.min.js
+-rw-rw-rw-   0        0        0     1388 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/openscad.min.js
+-rw-rw-rw-   0        0        0     1991 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/oxygene.min.js
+-rw-rw-rw-   0        0        0      656 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/parser3.min.js
+-rw-rw-rw-   0        0        0     4003 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/perl.min.js
+-rw-rw-rw-   0        0        0     1363 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/pf.min.js
+-rw-rw-rw-   0        0        0    19050 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/pgsql.min.js
+-rw-rw-rw-   0        0        0      536 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/php-template.min.js
+-rw-rw-rw-   0        0        0     6278 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/php.min.js
+-rw-rw-rw-   0        0        0      217 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/plaintext.min.js
+-rw-rw-rw-   0        0        0     1041 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/pony.min.js
+-rw-rw-rw-   0        0        0     4485 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/powershell.min.js
+-rw-rw-rw-   0        0        0     4430 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/processing.min.js
+-rw-rw-rw-   0        0        0      589 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/profile.min.js
+-rw-rw-rw-   0        0        0      772 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/prolog.min.js
+-rw-rw-rw-   0        0        0      676 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/properties.min.js
+-rw-rw-rw-   0        0        0      776 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/protobuf.min.js
+-rw-rw-rw-   0        0        0     4209 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/puppet.min.js
+-rw-rw-rw-   0        0        0     1690 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/purebasic.min.js
+-rw-rw-rw-   0        0        0      335 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/python-repl.min.js
+-rw-rw-rw-   0        0        0     3572 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/python.min.js
+-rw-rw-rw-   0        0        0     1231 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/q.min.js
+-rw-rw-rw-   0        0        0     2809 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/qml.min.js
+-rw-rw-rw-   0        0        0     3054 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/r.min.js
+-rw-rw-rw-   0        0        0     3439 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/reasonml.min.js
+-rw-rw-rw-   0        0        0     1382 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/rib.min.js
+-rw-rw-rw-   0        0        0      820 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/roboconf.min.js
+-rw-rw-rw-   0        0        0     2579 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/routeros.min.js
+-rw-rw-rw-   0        0        0     1381 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/rsl.min.js
+-rw-rw-rw-   0        0        0     4090 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/ruby.min.js
+-rw-rw-rw-   0        0        0     3941 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/ruleslanguage.min.js
+-rw-rw-rw-   0        0        0     2937 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/rust.min.js
+-rw-rw-rw-   0        0        0     4848 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/sas.min.js
+-rw-rw-rw-   0        0        0     1945 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/scala.min.js
+-rw-rw-rw-   0        0        0     3425 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/scheme.min.js
+-rw-rw-rw-   0        0        0     1306 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/scilab.min.js
+-rw-rw-rw-   0        0        0    11098 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/scss.min.js
+-rw-rw-rw-   0        0        0      333 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/shell.min.js
+-rw-rw-rw-   0        0        0     1107 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/smali.min.js
+-rw-rw-rw-   0        0        0      735 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/smalltalk.min.js
+-rw-rw-rw-   0        0        0     1238 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/sml.min.js
+-rw-rw-rw-   0        0        0    41301 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/sqf.min.js
+-rw-rw-rw-   0        0        0     6551 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/sql.min.js
+-rw-rw-rw-   0        0        0     5892 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/stan.min.js
+-rw-rw-rw-   0        0        0    16811 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/stata.min.js
+-rw-rw-rw-   0        0        0      717 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/step21.min.js
+-rw-rw-rw-   0        0        0    10313 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/stylus.min.js
+-rw-rw-rw-   0        0        0      606 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/subunit.min.js
+-rw-rw-rw-   0        0        0     7563 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/swift.min.js
+-rw-rw-rw-   0        0        0      537 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/taggerscript.min.js
+-rw-rw-rw-   0        0        0      482 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/tap.min.js
+-rw-rw-rw-   0        0        0     2024 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/tcl.min.js
+-rw-rw-rw-   0        0        0      785 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/thrift.min.js
+-rw-rw-rw-   0        0        0     1724 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/tp.min.js
+-rw-rw-rw-   0        0        0     2540 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/twig.min.js
+-rw-rw-rw-   0        0        0     7606 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/typescript.min.js
+-rw-rw-rw-   0        0        0      998 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/vala.min.js
+-rw-rw-rw-   0        0        0     2752 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/vbnet.min.js
+-rw-rw-rw-   0        0        0      261 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/vbscript-html.min.js
+-rw-rw-rw-   0        0        0     1958 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/vbscript.min.js
+-rw-rw-rw-   0        0        0     6125 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/verilog.min.js
+-rw-rw-rw-   0        0        0     2065 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/vhdl.min.js
+-rw-rw-rw-   0        0        0     8700 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/vim.min.js
+-rw-rw-rw-   0        0        0     1778 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/wasm.min.js
+-rw-rw-rw-   0        0        0     2372 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/wren.min.js
+-rw-rw-rw-   0        0        0    19143 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/x86asm.min.js
+-rw-rw-rw-   0        0        0     1984 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/xl.min.js
+-rw-rw-rw-   0        0        0     2052 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/xml.min.js
+-rw-rw-rw-   0        0        0     5723 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/xquery.min.js
+-rw-rw-rw-   0        0        0     1834 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/yaml.min.js
+-rw-rw-rw-   0        0        0     1696 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/languages/zephir.min.js
+drwxrwxrwx   0        0        0        0 2023-06-22 15:38:03.360330 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/
+-rw-rw-rw-   0        0        0     1164 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/a11y-dark.min.css
+-rw-rw-rw-   0        0        0     1152 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/a11y-light.min.css
+-rw-rw-rw-   0        0        0     1376 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/agate.min.css
+-rw-rw-rw-   0        0        0      969 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/an-old-hope.min.css
+-rw-rw-rw-   0        0        0      611 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/androidstudio.min.css
+-rw-rw-rw-   0        0        0      844 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/arduino-light.min.css
+-rw-rw-rw-   0        0        0      673 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/arta.min.css
+-rw-rw-rw-   0        0        0      454 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/ascetic.min.css
+-rw-rw-rw-   0        0        0     1193 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/atom-one-dark-reasonable.min.css
+-rw-rw-rw-   0        0        0      856 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/atom-one-dark.min.css
+-rw-rw-rw-   0        0        0      856 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/atom-one-light.min.css
+drwxrwxrwx   0        0        0        0 2023-06-22 15:38:05.406392 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/
+-rw-rw-rw-   0        0        0     1404 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/3024.min.css
+-rw-rw-rw-   0        0        0     1409 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/apathy.min.css
+-rw-rw-rw-   0        0        0     1374 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/apprentice.min.css
+-rw-rw-rw-   0        0        0     1408 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/ashes.min.css
+-rw-rw-rw-   0        0        0     1420 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-cave-light.min.css
+-rw-rw-rw-   0        0        0     1414 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-cave.min.css
+-rw-rw-rw-   0        0        0     1420 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-dune-light.min.css
+-rw-rw-rw-   0        0        0     1414 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-dune.min.css
+-rw-rw-rw-   0        0        0     1423 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-estuary-light.min.css
+-rw-rw-rw-   0        0        0     1417 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-estuary.min.css
+-rw-rw-rw-   0        0        0     1422 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-forest-light.min.css
+-rw-rw-rw-   0        0        0     1416 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-forest.min.css
+-rw-rw-rw-   0        0        0     1418 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-heath-light.min.css
+-rw-rw-rw-   0        0        0     1412 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-heath.min.css
+-rw-rw-rw-   0        0        0     1424 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-lakeside-light.min.css
+-rw-rw-rw-   0        0        0     1418 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-lakeside.min.css
+-rw-rw-rw-   0        0        0     1423 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-plateau-light.min.css
+-rw-rw-rw-   0        0        0     1417 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-plateau.min.css
+-rw-rw-rw-   0        0        0     1423 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-savanna-light.min.css
+-rw-rw-rw-   0        0        0     1417 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-savanna.min.css
+-rw-rw-rw-   0        0        0     1423 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-seaside-light.min.css
+-rw-rw-rw-   0        0        0     1417 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-seaside.min.css
+-rw-rw-rw-   0        0        0     1427 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-sulphurpool-light.min.css
+-rw-rw-rw-   0        0        0     1421 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atelier-sulphurpool.min.css
+-rw-rw-rw-   0        0        0     1397 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/atlas.min.css
+-rw-rw-rw-   0        0        0     1374 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/bespin.min.css
+-rw-rw-rw-   0        0        0     1391 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/black-metal-bathory.min.css
+-rw-rw-rw-   0        0        0     1381 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/black-metal-burzum.min.css
+-rw-rw-rw-   0        0        0     1396 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/black-metal-dark-funeral.min.css
+-rw-rw-rw-   0        0        0     1393 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/black-metal-gorgoroth.min.css
+-rw-rw-rw-   0        0        0     1383 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/black-metal-immortal.min.css
+-rw-rw-rw-   0        0        0     1389 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/black-metal-khold.min.css
+-rw-rw-rw-   0        0        0     1390 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/black-metal-marduk.min.css
+-rw-rw-rw-   0        0        0     1390 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/black-metal-mayhem.min.css
+-rw-rw-rw-   0        0        0     1379 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/black-metal-nile.min.css
+-rw-rw-rw-   0        0        0     1389 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/black-metal-venom.min.css
+-rw-rw-rw-   0        0        0     1378 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/black-metal.min.css
+-rw-rw-rw-   0        0        0     1410 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/brewer.min.css
+-rw-rw-rw-   0        0        0     1402 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/bright.min.css
+-rw-rw-rw-   0        0        0     1413 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/brogrammer.min.css
+-rw-rw-rw-   0        0        0     1418 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/brush-trees-dark.min.css
+-rw-rw-rw-   0        0        0     1413 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/brush-trees.min.css
+-rw-rw-rw-   0        0        0     1404 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/chalk.min.css
+-rw-rw-rw-   0        0        0     1457 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/circus.min.css
+-rw-rw-rw-   0        0        0     1406 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/classic-dark.min.css
+-rw-rw-rw-   0        0        0     1407 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/classic-light.min.css
+-rw-rw-rw-   0        0        0     1379 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/codeschool.min.css
+-rw-rw-rw-   0        0        0     1367 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/colors.min.css
+-rw-rw-rw-   0        0        0     1406 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/cupcake.min.css
+-rw-rw-rw-   0        0        0     1353 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/cupertino.min.css
+-rw-rw-rw-   0        0        0     1414 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/danqing.min.css
+-rw-rw-rw-   0        0        0     1373 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/darcula.min.css
+-rw-rw-rw-   0        0        0     1418 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/dark-violet.min.css
+-rw-rw-rw-   0        0        0     1412 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/darkmoss.min.css
+-rw-rw-rw-   0        0        0     1412 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/darktooth.min.css
+-rw-rw-rw-   0        0        0     1404 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/decaf.min.css
+-rw-rw-rw-   0        0        0     1411 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/default-dark.min.css
+-rw-rw-rw-   0        0        0     1412 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/default-light.min.css
+-rw-rw-rw-   0        0        0     1379 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/dirtysea.min.css
+-rw-rw-rw-   0        0        0     1462 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/dracula.min.css
+-rw-rw-rw-   0        0        0     1393 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/edge-dark.min.css
+-rw-rw-rw-   0        0        0     1394 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/edge-light.min.css
+-rw-rw-rw-   0        0        0     1386 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/eighties.min.css
+-rw-rw-rw-   0        0        0     1409 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/embers.min.css
+-rw-rw-rw-   0        0        0     1388 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/equilibrium-dark.min.css
+-rw-rw-rw-   0        0        0     1387 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/equilibrium-gray-dark.min.css
+-rw-rw-rw-   0        0        0     1391 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/equilibrium-gray-light.min.css
+-rw-rw-rw-   0        0        0     1389 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/equilibrium-light.min.css
+-rw-rw-rw-   0        0        0     1430 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/espresso.min.css
+-rw-rw-rw-   0        0        0     1402 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/eva-dim.min.css
+-rw-rw-rw-   0        0        0     1389 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/eva.min.css
+-rw-rw-rw-   0        0        0     1403 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/flat.min.css
+-rw-rw-rw-   0        0        0     1400 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/framer.min.css
+-rw-rw-rw-   0        0        0     1375 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/fruit-soda.min.css
+-rw-rw-rw-   0        0        0     1410 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/gigavolt.min.css
+-rw-rw-rw-   0        0        0     1345 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/github.min.css
+-rw-rw-rw-   0        0        0     1393 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/google-dark.min.css
+-rw-rw-rw-   0        0        0     1391 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/google-light.min.css
+-rw-rw-rw-   0        0        0     1417 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/grayscale-dark.min.css
+-rw-rw-rw-   0        0        0     1418 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/grayscale-light.min.css
+-rw-rw-rw-   0        0        0     1360 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/green-screen.min.css
+-rw-rw-rw-   0        0        0     1455 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/gruvbox-dark-hard.min.css
+-rw-rw-rw-   0        0        0     1457 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/gruvbox-dark-medium.min.css
+-rw-rw-rw-   0        0        0     1455 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/gruvbox-dark-pale.min.css
+-rw-rw-rw-   0        0        0     1455 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/gruvbox-dark-soft.min.css
+-rw-rw-rw-   0        0        0     1456 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/gruvbox-light-hard.min.css
+-rw-rw-rw-   0        0        0     1458 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/gruvbox-light-medium.min.css
+-rw-rw-rw-   0        0        0     1456 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/gruvbox-light-soft.min.css
+-rw-rw-rw-   0        0        0     1380 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/hardcore.min.css
+-rw-rw-rw-   0        0        0     1418 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/harmonic16-dark.min.css
+-rw-rw-rw-   0        0        0     1419 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/harmonic16-light.min.css
+-rw-rw-rw-   0        0        0     1404 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/heetch-dark.min.css
+-rw-rw-rw-   0        0        0     1405 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/heetch-light.min.css
+-rw-rw-rw-   0        0        0     1407 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/helios.min.css
+-rw-rw-rw-   0        0        0     1380 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/hopscotch.min.css
+-rw-rw-rw-   0        0        0     1419 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/horizon-dark.min.css
+-rw-rw-rw-   0        0        0     1420 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/horizon-light.min.css
+-rw-rw-rw-   0        0        0     1394 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/humanoid-dark.min.css
+-rw-rw-rw-   0        0        0     1395 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/humanoid-light.min.css
+-rw-rw-rw-   0        0        0     1392 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/ia-dark.min.css
+-rw-rw-rw-   0        0        0     1402 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/ia-light.min.css
+-rw-rw-rw-   0        0        0     1396 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/icy-dark.min.css
+-rw-rw-rw-   0        0        0     1408 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/ir-black.min.css
+-rw-rw-rw-   0        0        0     1340 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/isotope.min.css
+-rw-rw-rw-   0        0        0     1404 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/kimber.min.css
+-rw-rw-rw-   0        0        0     1382 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/london-tube.min.css
+-rw-rw-rw-   0        0        0     1395 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/macintosh.min.css
+-rw-rw-rw-   0        0        0     1414 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/marrakesh.min.css
+-rw-rw-rw-   0        0        0     1369 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/materia.min.css
+-rw-rw-rw-   0        0        0     1379 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/material-darker.min.css
+-rw-rw-rw-   0        0        0     1389 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/material-lighter.min.css
+-rw-rw-rw-   0        0        0     1391 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/material-palenight.min.css
+-rw-rw-rw-   0        0        0     1384 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/material-vivid.min.css
+-rw-rw-rw-   0        0        0     1372 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/material.min.css
+-rw-rw-rw-   0        0        0     1369 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/mellow-purple.min.css
+-rw-rw-rw-   0        0        0     1387 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/mexico-light.min.css
+-rw-rw-rw-   0        0        0     1404 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/mocha.min.css
+-rw-rw-rw-   0        0        0     1403 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/monokai.min.css
+-rw-rw-rw-   0        0        0     1412 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/nebula.min.css
+-rw-rw-rw-   0        0        0     1379 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/nord.min.css
+-rw-rw-rw-   0        0        0     1436 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/nova.min.css
+-rw-rw-rw-   0        0        0     1404 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/ocean.min.css
+-rw-rw-rw-   0        0        0     1424 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/oceanicnext.min.css
+-rw-rw-rw-   0        0        0     1416 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/one-light.min.css
+-rw-rw-rw-   0        0        0     1409 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/onedark.min.css
+-rw-rw-rw-   0        0        0     1422 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/outrun-dark.min.css
+-rw-rw-rw-   0        0        0     1482 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/papercolor-dark.min.css
+-rw-rw-rw-   0        0        0     1466 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/papercolor-light.min.css
+-rw-rw-rw-   0        0        0     1378 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/paraiso.min.css
+-rw-rw-rw-   0        0        0     1412 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/pasque.min.css
+-rw-rw-rw-   0        0        0     1408 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/phd.min.css
+-rw-rw-rw-   0        0        0     1403 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/pico.min.css
+-rw-rw-rw-   0        0        0     1396 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/pop.min.css
+-rw-rw-rw-   0        0        0     1415 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/porple.min.css
+-rw-rw-rw-   0        0        0     1369 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/qualia.min.css
+-rw-rw-rw-   0        0        0     1404 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/railscasts.min.css
+-rw-rw-rw-   0        0        0     1461 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/rebecca.min.css
+-rw-rw-rw-   0        0        0     1408 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/ros-pine-dawn.min.css
+-rw-rw-rw-   0        0        0     1408 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/ros-pine-moon.min.css
+-rw-rw-rw-   0        0        0     1403 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/ros-pine.min.css
+-rw-rw-rw-   0        0        0     1386 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/sagelight.min.css
+-rw-rw-rw-   0        0        0     1382 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/sandcastle.min.css
+-rw-rw-rw-   0        0        0     1367 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/seti-ui.min.css
+-rw-rw-rw-   0        0        0     1403 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/shapeshifter.min.css
+-rw-rw-rw-   0        0        0     1415 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/silk-dark.min.css
+-rw-rw-rw-   0        0        0     1416 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/silk-light.min.css
+-rw-rw-rw-   0        0        0     1482 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/snazzy.min.css
+-rw-rw-rw-   0        0        0     1419 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/solar-flare-light.min.css
+-rw-rw-rw-   0        0        0     1413 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/solar-flare.min.css
+-rw-rw-rw-   0        0        0     1417 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/solarized-dark.min.css
+-rw-rw-rw-   0        0        0     1418 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/solarized-light.min.css
+-rw-rw-rw-   0        0        0     1431 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/spacemacs.min.css
+-rw-rw-rw-   0        0        0     1398 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/summercamp.min.css
+-rw-rw-rw-   0        0        0     1415 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/summerfruit-dark.min.css
+-rw-rw-rw-   0        0        0     1410 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/summerfruit-light.min.css
+-rw-rw-rw-   0        0        0     1435 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/synth-midnight-terminal-dark.min.css
+-rw-rw-rw-   0        0        0     1436 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/synth-midnight-terminal-light.min.css
+-rw-rw-rw-   0        0        0     1407 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/tango.min.css
+-rw-rw-rw-   0        0        0     1415 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/tender.min.css
+-rw-rw-rw-   0        0        0     1380 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/tomorrow-night.min.css
+-rw-rw-rw-   0        0        0     1404 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/tomorrow.min.css
+-rw-rw-rw-   0        0        0     1407 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/twilight.min.css
+-rw-rw-rw-   0        0        0     1399 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/unikitty-dark.min.css
+-rw-rw-rw-   0        0        0     1397 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/unikitty-light.min.css
+-rw-rw-rw-   0        0        0     1356 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/vulcan.min.css
+-rw-rw-rw-   0        0        0     1417 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/windows-10-light.min.css
+-rw-rw-rw-   0        0        0     1405 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/windows-10.min.css
+-rw-rw-rw-   0        0        0     1420 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/windows-95-light.min.css
+-rw-rw-rw-   0        0        0     1411 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/windows-95.min.css
+-rw-rw-rw-   0        0        0     1415 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/windows-high-contrast-light.min.css
+-rw-rw-rw-   0        0        0     1415 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/windows-high-contrast.min.css
+-rw-rw-rw-   0        0        0     1386 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/windows-nt-light.min.css
+-rw-rw-rw-   0        0        0     1373 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/windows-nt.min.css
+-rw-rw-rw-   0        0        0     1404 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/woodland.min.css
+-rw-rw-rw-   0        0        0     1415 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/xcode-dusk.min.css
+-rw-rw-rw-   0        0        0     1367 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/base16/zenburn.min.css
+-rw-rw-rw-   0        0        0      656 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/brown-paper.min.css
+-rw-rw-rw-   0        0        0    18198 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/brown-papersq.png
+-rw-rw-rw-   0        0        0      600 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/codepen-embed.min.css
+-rw-rw-rw-   0        0        0      631 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/color-brewer.min.css
+-rw-rw-rw-   0        0        0      625 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/dark.min.css
+-rw-rw-rw-   0        0        0     1503 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/default.min.css
+-rw-rw-rw-   0        0        0     1086 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/devibeans.min.css
+-rw-rw-rw-   0        0        0      837 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/docco.min.css
+-rw-rw-rw-   0        0        0      669 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/far.min.css
+-rw-rw-rw-   0        0        0     1175 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/felipec.min.css
+-rw-rw-rw-   0        0        0      779 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/foundation.min.css
+-rw-rw-rw-   0        0        0     1259 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/github-dark-dimmed.min.css
+-rw-rw-rw-   0        0        0     1324 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/github-dark.min.css
+-rw-rw-rw-   0        0        0     1318 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/github.min.css
+-rw-rw-rw-   0        0        0      787 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/gml.min.css
+-rw-rw-rw-   0        0        0      835 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/googlecode.min.css
+-rw-rw-rw-   0        0        0     1089 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/gradient-dark.min.css
+-rw-rw-rw-   0        0        0     1112 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/gradient-light.min.css
+-rw-rw-rw-   0        0        0     1674 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/grayscale.min.css
+-rw-rw-rw-   0        0        0      897 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/hybrid.min.css
+-rw-rw-rw-   0        0        0      906 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/idea.min.css
+-rw-rw-rw-   0        0        0     1051 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/intellij-light.min.css
+-rw-rw-rw-   0        0        0      694 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/ir-black.min.css
+-rw-rw-rw-   0        0        0      971 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/isbl-editor-dark.min.css
+-rw-rw-rw-   0        0        0      952 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/isbl-editor-light.min.css
+-rw-rw-rw-   0        0        0      652 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/kimbie-dark.min.css
+-rw-rw-rw-   0        0        0      652 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/kimbie-light.min.css
+-rw-rw-rw-   0        0        0      831 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/lightfair.min.css
+-rw-rw-rw-   0        0        0      715 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/lioshi.min.css
+-rw-rw-rw-   0        0        0      642 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/magula.min.css
+-rw-rw-rw-   0        0        0      631 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/mono-blue.min.css
+-rw-rw-rw-   0        0        0      826 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/monokai-sublime.min.css
+-rw-rw-rw-   0        0        0      790 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/monokai.min.css
+-rw-rw-rw-   0        0        0     1421 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/night-owl.min.css
+-rw-rw-rw-   0        0        0     1420 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/nnfx-dark.min.css
+-rw-rw-rw-   0        0        0     1421 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/nnfx-light.min.css
+-rw-rw-rw-   0        0        0     2684 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/nord.min.css
+-rw-rw-rw-   0        0        0      882 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/obsidian.min.css
+-rw-rw-rw-   0        0        0     1095 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/panda-syntax-dark.min.css
+-rw-rw-rw-   0        0        0     1069 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/panda-syntax-light.min.css
+-rw-rw-rw-   0        0        0      637 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/paraiso-dark.min.css
+-rw-rw-rw-   0        0        0      637 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/paraiso-light.min.css
+-rw-rw-rw-   0        0        0      814 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/pojoaque.min.css
+-rw-rw-rw-   0        0        0      734 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/purebasic.min.css
+-rw-rw-rw-   0        0        0      815 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/qtcreator-dark.min.css
+-rw-rw-rw-   0        0        0      810 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/qtcreator-light.min.css
+-rw-rw-rw-   0        0        0      826 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/rainbow.min.css
+-rw-rw-rw-   0        0        0      862 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/routeros.min.css
+-rw-rw-rw-   0        0        0      664 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/school-book.min.css
+-rw-rw-rw-   0        0        0      854 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/shades-of-purple.min.css
+-rw-rw-rw-   0        0        0      795 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/srcery.min.css
+-rw-rw-rw-   0        0        0     1283 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/stackoverflow-dark.min.css
+-rw-rw-rw-   0        0        0     1297 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/stackoverflow-light.min.css
+-rw-rw-rw-   0        0        0      950 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/sunburst.min.css
+-rw-rw-rw-   0        0        0     1241 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/tokyo-night-dark.min.css
+-rw-rw-rw-   0        0        0     1242 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/tokyo-night-light.min.css
+-rw-rw-rw-   0        0        0      648 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/tomorrow-night-blue.min.css
+-rw-rw-rw-   0        0        0      648 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/tomorrow-night-bright.min.css
+-rw-rw-rw-   0        0        0      640 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/vs.min.css
+-rw-rw-rw-   0        0        0     1088 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/vs2015.min.css
+-rw-rw-rw-   0        0        0      945 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/xcode.min.css
+-rw-rw-rw-   0        0        0      765 2023-03-06 08:25:28.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/highlight/styles/xt256.min.css
+drwxrwxrwx   0        0        0        0 2023-06-22 15:38:05.454295 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/html/
+-rw-rw-rw-   0        0        0      101 2023-03-06 08:25:27.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/html/index.html
+-rw-rw-rw-   0        0        0      569 2023-03-10 14:35:32.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/html/nav-item2.html
+-rw-rw-rw-   0        0        0      284 2023-03-10 14:37:55.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/html/nav.html
+-rw-rw-rw-   0        0        0      233 2023-03-10 08:29:32.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/html/search-modal.html
+drwxrwxrwx   0        0        0        0 2023-06-22 15:38:05.509732 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/js/
+-rw-rw-rw-   0        0        0     9160 2023-03-20 08:39:36.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/js/clipboard.min.js
+-rw-rw-rw-   0        0        0     3409 2023-03-10 08:29:32.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/js/nav.js
+-rw-rw-rw-   0        0        0     1762 2023-03-20 09:20:30.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/js/theme.js
+-rw-rw-rw-   0        0        0     1186 2023-06-22 09:30:03.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/main.html
+-rw-rw-rw-   0        0        0      163 2023-06-22 15:30:24.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/mkdocs_theme.yml
+drwxrwxrwx   0        0        0        0 2023-06-22 15:38:05.520827 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/raw/
+-rw-rw-rw-   0        0        0     2486 2023-03-14 16:10:26.000000 mkdocs-dark_enhanced_dirtree-1.2.0/dark_enhanced_dirtree/raw/donotload.js
+drwxrwxrwx   0        0        0        0 2023-06-22 15:38:05.579867 mkdocs-dark_enhanced_dirtree-1.2.0/mkdocs_dark_enhanced_dirtree.egg-info/
+-rw-rw-rw-   0        0        0      285 2023-06-22 15:37:55.000000 mkdocs-dark_enhanced_dirtree-1.2.0/mkdocs_dark_enhanced_dirtree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    39098 2023-06-22 15:37:56.000000 mkdocs-dark_enhanced_dirtree-1.2.0/mkdocs_dark_enhanced_dirtree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 15:37:55.000000 mkdocs-dark_enhanced_dirtree-1.2.0/mkdocs_dark_enhanced_dirtree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-22 15:37:55.000000 mkdocs-dark_enhanced_dirtree-1.2.0/mkdocs_dark_enhanced_dirtree.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-22 13:35:15.000000 mkdocs-dark_enhanced_dirtree-1.2.0/mkdocs_dark_enhanced_dirtree.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       22 2023-06-22 15:37:55.000000 mkdocs-dark_enhanced_dirtree-1.2.0/mkdocs_dark_enhanced_dirtree.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 15:38:05.599439 mkdocs-dark_enhanced_dirtree-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      629 2023-06-22 09:29:19.000000 mkdocs-dark_enhanced_dirtree-1.2.0/setup.py
```

### Comparing `mkdocs-dark_enhanced_dirtree-1.1.1/setup.py` & `mkdocs-dark_enhanced_dirtree-1.2.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from setuptools import setup, find_packages
-
-# https://pypi.org/project/mkdocs-dark-minimal-dirtree
-
-VERSION = "1.1.1"
-
-setup(
-    name="mkdocs-dark_enhanced_dirtree",
-    version=VERSION,
-    url="https://github.com/Jakkins/dark_enhanced_dirtree",
-    license="MIT License",
-    description="MkDocs theme to praise the holy (dir) tree",
-    author="jakkins",
-    author_email="sjakkins@proton.me",
-    packages=find_packages(),
-    include_package_data=True,
-    entry_points={
-        "mkdocs.themes": [
-            "dark_enhanced_dirtree = dark_enhanced_dirtree",
-        ]
-    },
-    zip_safe=False,
-)
+from setuptools import setup, find_packages
+
+# https://pypi.org/project/mkdocs-dark-minimal-dirtree
+
+VERSION = "1.2.0"
+
+setup(
+    name="mkdocs-dark_enhanced_dirtree",
+    version=VERSION,
+    url="https://github.com/Jakkins/dark_enhanced_dirtree",
+    license="MIT License",
+    description="MkDocs theme to praise the holy (dir) tree",
+    author="jakkins",
+    author_email="sjakkins@proton.me",
+    packages=find_packages(),
+    include_package_data=True,
+    entry_points={
+        "mkdocs.themes": [
+            "dark_enhanced_dirtree = dark_enhanced_dirtree",
+        ]
+    },
+    zip_safe=False,
+)
```

