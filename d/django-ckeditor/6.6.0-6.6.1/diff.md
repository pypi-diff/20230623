# Comparing `tmp/django-ckeditor-6.6.0.tar.gz` & `tmp/django-ckeditor-6.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ckeditor-6.6.0.tar", last modified: Fri Jun 23 08:10:44 2023, max compression
+gzip compressed data, was "django-ckeditor-6.6.1.tar", last modified: Fri Jun 23 08:17:07 2023, max compression
```

## Comparing `django-ckeditor-6.6.0.tar` & `django-ckeditor-6.6.1.tar`

### file list

```diff
@@ -1,1518 +1,1518 @@
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      683 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/AUTHORS.rst
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    11154 2023-06-23 08:09:49.000000 django-ckeditor-6.6.0/CHANGELOG.rst
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1484 2022-04-11 07:31:10.000000 django-ckeditor-6.6.0/LICENSE
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      354 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/MANIFEST.in
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    32080 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    19300 2022-04-11 07:31:10.000000 django-ckeditor-6.6.0/README.rst
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.699738 django-ckeditor-6.6.0/ckeditor/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       62 2023-06-23 08:09:58.000000 django-ckeditor-6.6.0/ckeditor/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      672 2023-04-14 07:34:40.000000 django-ckeditor-6.6.0/ckeditor/configs.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1259 2022-04-14 19:26:20.000000 django-ckeditor-6.6.0/ckeditor/fields.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.679738 django-ckeditor-6.6.0/ckeditor/static/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.699738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.699738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/
--rw-r--r--   0 matthias  (1000) matthias  (1000)   312603 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/CHANGES.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)    77827 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/LICENSE.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1383 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/README.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)      578 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/SECURITY.md
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.699738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/adapters/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3180 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/adapters/jquery.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)      246 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/bender-runner.config.json
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3585 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/build-config.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)   758081 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/ckeditor.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)      336 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/config.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3092 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/contents.css
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.709738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    17658 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/af.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    22093 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ar.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19554 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/az.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    26713 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/bg.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    23072 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/bn.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    17707 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/bs.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19415 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ca.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19445 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/cs.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    18112 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/cy.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    18472 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/da.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19320 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/de-ch.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19298 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/de.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    28609 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/el.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    17611 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/en-au.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    17608 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/en-ca.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    17633 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/en-gb.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    17623 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/en.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    18846 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/eo.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19675 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/es-mx.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19605 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/es.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    18275 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/et.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19320 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/eu.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    24193 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/fa.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    18689 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/fi.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    18616 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/fo.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19190 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/fr-ca.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    20170 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/fr.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19673 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/gl.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    28699 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/gu.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    21675 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/he.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    23513 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/hi.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    18231 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/hr.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19815 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/hu.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    18031 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/id.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    18191 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/is.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19537 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/it.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    21405 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ja.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    31095 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ka.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    32492 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/km.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19134 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ko.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    26297 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ku.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19344 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/lt.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19577 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/lv.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19360 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/mk.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    22367 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/mn.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    17912 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ms.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    18026 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/nb.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    18653 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/nl.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    18047 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/no.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19826 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/oc.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19639 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/pl.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19669 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/pt-br.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19542 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/pt.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    20386 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ro.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    27538 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ru.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    24449 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/si.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19729 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/sk.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    18411 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/sl.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    20147 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/sq.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    18615 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/sr-latn.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    25807 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/sr.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    18178 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/sv.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    27007 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/th.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19330 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/tr.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    22884 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/tt.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    25797 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ug.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    27576 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/uk.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    21086 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/vi.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    17296 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/zh-cn.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    17174 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/zh.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.709738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.679738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.709738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2953 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/a11yhelp.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.709738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      887 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/_translationstatus.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4156 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/af.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4351 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ar.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4332 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/az.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4565 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/bg.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4788 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ca.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4938 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/cs.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4389 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/cy.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4247 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/da.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4712 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/de-ch.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4656 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/de.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     7631 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/el.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4203 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/en-au.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4203 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/en-gb.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4200 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/en.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4797 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/eo.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4893 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/es-mx.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4799 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/es.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4418 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/et.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4505 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/eu.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6152 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fa.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4760 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fi.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4202 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fo.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4922 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fr-ca.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5309 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fr.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4814 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/gl.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4410 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/gu.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4955 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/he.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4214 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/hi.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4281 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/hr.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4766 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/hu.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4039 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/id.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5237 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/it.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5200 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ja.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5218 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/km.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5599 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ko.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6033 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ku.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4209 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/lt.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4832 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/lv.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4591 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/mk.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4207 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/mn.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4457 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/nb.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4532 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/nl.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4443 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/no.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5098 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/oc.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5160 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/pl.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4927 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/pt-br.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4568 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/pt.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4559 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ro.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6646 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ru.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6145 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/si.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4769 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sk.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4548 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sl.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4933 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sq.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4896 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sr-latn.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     7514 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sr.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4369 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sv.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4578 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/th.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4579 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/tr.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4518 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/tt.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6936 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ug.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6926 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/uk.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5400 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/vi.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4148 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/zh-cn.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4357 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/zh.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.679738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/about/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.709738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1827 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/about.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.709738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/hidpi/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    12236 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/hidpi/logo_ckeditor.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5650 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/logo_ckeditor.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.719738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/adobeair/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2486 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/adobeair/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.719738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/ajax/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1277 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/ajax/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.719738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.719738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      165 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      191 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      164 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      190 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      238 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      169 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      189 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      173 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      184 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      162 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/zh.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2334 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.719738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autogrow/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1912 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autogrow/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.719738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autolink/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      584 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autolink/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.719738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/bbcode/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     9190 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/bbcode/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.679738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/clipboard/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.719738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/clipboard/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3809 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/clipboard/dialogs/paste.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.719738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.719738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1179 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/codesnippet.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.719738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/icons/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      597 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/icons/codesnippet.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.719738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1887 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/codesnippet.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.719738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      454 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ar.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      457 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/bg.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      397 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      376 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      360 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/da.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      380 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      526 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/el.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      372 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/en-gb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      369 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      358 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/eo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      419 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/es.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      373 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/et.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      398 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/fa.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      362 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/fi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      369 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/fr-ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      395 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/fr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      416 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/gl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      389 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/he.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      370 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/hr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      379 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/hu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      413 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      431 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ja.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      388 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/km.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      396 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ko.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      419 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      386 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/lt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      373 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/lv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      360 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      352 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/nl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      368 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/no.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      363 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      415 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      384 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/pt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      383 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ro.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      423 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ru.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      374 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/sk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      366 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/sl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      370 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/sq.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      355 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/sv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      431 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/th.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      373 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      419 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/tt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      388 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ug.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      392 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/uk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      382 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/vi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      365 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/zh-cn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      380 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/zh.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.679738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.719738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    30194 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/CHANGES.md
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1498 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/LICENSE
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     7705 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.ru.md
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    30179 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/highlight.pack.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.729738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2514 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/arta.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      853 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ascetic.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1811 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.dark.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1825 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.light.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1836 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.dark.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1845 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.light.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1826 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.dark.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1835 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.light.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1857 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.dark.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1866 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.light.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1847 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.dark.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1856 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.light.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1896 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_paper.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    18198 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_papersq.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1864 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/dark.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2804 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/default.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1908 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/docco.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2016 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/far.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1715 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/foundation.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1809 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/github.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2309 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/googlecode.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1856 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/idea.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1567 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ir_black.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2046 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/magula.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      961 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/mono-blue.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2141 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2485 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai_sublime.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2470 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/obsidian.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1586 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.dark.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1587 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.light.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1747 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1186 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.jpg
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2736 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/railscasts.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1707 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/rainbow.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2096 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      486 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1709 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_dark.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1709 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_light.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2398 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/sunburst.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1696 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-blue.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1625 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-bright.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1629 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-eighties.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1693 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1519 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1650 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/vs.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2452 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/xcode.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1971 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/zenburn.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3824 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.729738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippetgeshi/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3104 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippetgeshi/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.679738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/colordialog/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.729738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/colordialog/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      790 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/colordialog/dialogs/colordialog.css
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5327 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/colordialog/dialogs/colordialog.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.679738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.729738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/cursors/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4012 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/cursors/cursor-disabled.svg
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2759 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/cursors/cursor.svg
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.729738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/styles/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1511 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/styles/copyformatting.css
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.729738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.729738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      909 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/_translationstatus.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      370 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ar.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      415 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/bg.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      365 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      324 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      331 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/cy.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      333 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/da.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      323 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      442 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/el.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      326 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/en-gb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      321 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      348 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/eo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      364 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/es.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      319 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/et.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      350 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/eu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      355 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/fa.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      334 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/fi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      352 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/fr-ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      362 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/fr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      348 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/gl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      442 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/gu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      351 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/he.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      337 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/hr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      320 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/hu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      317 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/id.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      331 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      349 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ja.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      458 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/km.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      338 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ko.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      385 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      344 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/lt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      337 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/lv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      326 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      318 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/nl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      326 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/no.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      336 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      348 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      351 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/pt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      345 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ro.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      389 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ru.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      452 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/si.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      326 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/sk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      324 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/sl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      350 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/sq.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      318 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/sv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      323 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      429 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/tt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      389 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ug.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      437 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/uk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      324 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/vi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      326 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/zh-cn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      317 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/zh.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2451 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.729738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/dialog/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      166 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/dialog/dialogDefinition.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.729738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/dialog/styles/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      249 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/dialog/styles/dialog.css
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.679738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/div/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.729738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/div/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4676 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/div/dialogs/div.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.729738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/divarea/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      556 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/divarea/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.729738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.729738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/dialogs/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    10823 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/dialogs/docprops.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.729738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      840 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/docprops-rtl.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      844 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/docprops.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.729738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/hidpi/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1909 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/hidpi/docprops-rtl.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1941 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/hidpi/docprops.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1107 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/af.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1384 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ar.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1304 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/bg.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1752 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/bn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1120 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/bs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1211 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1125 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1152 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/cy.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1109 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/da.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1170 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1752 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/el.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1123 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en-au.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1123 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en-ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1125 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en-gb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1120 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1076 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/eo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1171 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/es.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1133 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/et.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1195 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/eu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1405 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fa.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1092 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1149 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1096 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fr-ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1109 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1236 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/gl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2115 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/gu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1293 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/he.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2035 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/hi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1120 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/hr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1129 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/hu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1123 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/id.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1101 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/is.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1132 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1235 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ja.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2013 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ka.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2027 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/km.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1157 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ko.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1564 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1223 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/lt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1153 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/lv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1120 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/mk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1532 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/mn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1123 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ms.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1060 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1129 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/nl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1059 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/no.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1184 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1217 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1199 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/pt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1281 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ro.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1703 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ru.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1583 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/si.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1171 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1079 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1252 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sq.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1151 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sr-latn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1469 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1073 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1969 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/th.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1143 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1282 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/tt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1586 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ug.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1630 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/uk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1275 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/vi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1030 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/zh-cn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1070 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/zh.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      910 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embed/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embed/icons/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      389 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embed/icons/embed.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embed/icons/hidpi/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      728 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embed/icons/hidpi/embed.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1058 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embed/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/dialogs/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1095 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/dialogs/embedbase.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      463 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      475 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/da.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      515 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      470 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      475 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/eo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      553 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/fr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      533 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/gl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      565 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      606 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/ko.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      791 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      482 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      513 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/nl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      594 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      529 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      722 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/ru.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      483 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/sv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      516 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      418 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/zh-cn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      453 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/zh.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3405 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/icons/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      389 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/icons/embedsemantic.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/icons/hidpi/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      728 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/icons/hidpi/embedsemantic.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1460 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3004 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/CHANGELOG.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)      973 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/LICENSE.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6314 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/README.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)        3 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/plugindefinition.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/_helpers/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      673 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/_helpers/tools.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3033 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/authentication.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4826 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/exportpdf.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      694 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/configfilename.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1267 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/configfilename.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)      432 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/emptyeditor.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      906 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/emptyeditor.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5396 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integration.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1135 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integration.md
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integrations/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      814 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integrations/easyimage.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      882 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integrations/easyimage.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)      396 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/notifications.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1161 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/notifications.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1047 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/notificationsasync.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      799 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/notificationsasync.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1273 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/paperformat.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      637 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/paperformat.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)      411 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/readonly.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      611 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/readonly.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1200 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/stylesheets.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      651 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/stylesheets.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)      568 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokenfetching.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      666 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokenfetching.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1064 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorscorrect.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      515 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorscorrect.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1088 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorswrong.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      524 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorswrong.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)      475 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokenwithouturl.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      862 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokenwithouturl.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)      488 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/wrongendpoint.html
--rw-r--r--   0 matthias  (1000) matthias  (1000)      824 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/wrongendpoint.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1974 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/notification.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4749 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/resourcespaths.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1096 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/statistics.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     9882 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/stylesheets.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.739738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      650 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      624 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/da.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      742 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      599 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      624 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/eo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      771 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/fr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      703 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/gl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      769 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      721 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/ko.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      896 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      603 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      611 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/nl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      648 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      675 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      738 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/ru.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      590 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/sv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      606 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      608 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/zh-cn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      614 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/zh.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4383 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/find/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/find/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    11424 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/find/dialogs/find.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/flash/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/flash/dialogs/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    10230 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/flash/dialogs/flash.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/flash/images/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      256 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/flash/images/placeholder.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1863 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/button.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2577 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/checkbox.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2127 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/form.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1706 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/hiddenfield.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2387 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/radio.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     8526 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/select.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2334 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/textarea.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3437 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/textfield.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/images/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      178 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/images/hiddenfield.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)    12237 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/icons.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)    38309 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/icons_hidpi.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/iframe/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/iframe/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3479 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/iframe/dialogs/iframe.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/iframe/images/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      265 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/iframe/images/placeholder.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/iframedialog/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1953 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/iframedialog/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    21529 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image/dialogs/image.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image/images/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1610 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image/images/noimage.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/dialogs/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     5101 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/dialogs/image2.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/icons/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/icons/hidpi/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1745 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/icons/hidpi/image.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      756 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/icons/image.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      449 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/af.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      539 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ar.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      752 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/bg.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      648 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/bn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      416 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/bs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      476 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      469 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      441 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/cy.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      460 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/da.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      470 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      749 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/el.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      417 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/en-au.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      417 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/en-ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      417 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/en-gb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      414 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      471 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/eo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      470 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/es.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      421 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/et.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      447 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/eu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      590 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/fa.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      468 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/fi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      435 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/fo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      493 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/fr-ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      504 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/fr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      450 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/gl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      607 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/gu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      514 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/he.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      619 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/hi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      416 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/hr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      459 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/hu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      408 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/id.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      415 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/is.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      473 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      511 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ja.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      736 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ka.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      892 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/km.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      486 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ko.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      584 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      440 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/lt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      499 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/lv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      414 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/mk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      578 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/mn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      416 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ms.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      454 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      510 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/nl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      451 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/no.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      458 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      488 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      473 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/pt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      470 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ro.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      712 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ru.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      635 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/si.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      464 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/sk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      451 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/sl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      478 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/sq.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      427 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/sr-latn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      522 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/sr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      454 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/sv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      839 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/th.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      473 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      579 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/tt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      535 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ug.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      726 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/uk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      500 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/vi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      412 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/zh-cn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      405 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/zh.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    13531 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/icons/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.749738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/icons/hidpi/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1678 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/icons/hidpi/language.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      668 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/icons/language.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      246 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/ar.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      256 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/bg.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      243 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      241 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      234 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/cy.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      234 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/da.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      246 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/el.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      242 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/en-gb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      239 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      241 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/eo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      241 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/es.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      246 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/fa.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      235 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/fi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      242 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/fo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      249 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/fr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      248 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/gl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      238 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/he.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      237 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/hr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      252 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/hu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      240 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      242 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/ja.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/km.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      248 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/ko.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      264 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      235 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      242 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/nl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      235 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/no.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      236 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      247 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      240 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/pt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      264 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/ru.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      244 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/sk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      239 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/sl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      247 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/sq.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      238 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/sv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      233 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      254 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/tt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/uk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      260 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/vi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      239 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/zh-cn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      236 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/zh.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2093 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/lineutils/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     9203 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/lineutils/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/link/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/link/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2207 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/link/dialogs/anchor.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)    13234 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/link/dialogs/link.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/link/images/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      752 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/link/images/anchor.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/link/images/hidpi/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1109 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/link/images/hidpi/anchor.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/liststyle/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/liststyle/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2883 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/liststyle/dialogs/liststyle.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/magicline/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/magicline/images/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/magicline/images/hidpi/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      176 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/magicline/images/hidpi/icon-rtl.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      199 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/magicline/images/hidpi/icon.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      138 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/magicline/images/icon-rtl.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      133 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/magicline/images/icon.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/dialogs/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1385 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/dialogs/mathjax.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/icons/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/icons/hidpi/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1437 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/icons/hidpi/mathjax.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      703 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/icons/mathjax.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/images/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      784 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/images/loader.gif
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      239 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/af.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      296 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/ar.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      359 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/bg.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      264 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      248 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/cy.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      247 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/da.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      259 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      350 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/el.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      245 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/en-gb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      243 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      258 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/eo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      252 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/es.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      317 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/fa.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/fi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      279 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/fr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      269 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/gl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      277 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/he.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      261 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/hr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      247 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/hu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      258 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      274 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/ja.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      411 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/km.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      301 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/ko.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      304 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      254 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/lt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      242 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      241 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/nl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      242 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/no.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      274 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      265 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      265 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/pt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      253 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/ro.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      316 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/ru.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      254 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/sk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      260 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/sl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      268 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/sq.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      241 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/sv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      269 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      373 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/tt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      339 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/uk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      256 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/vi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      347 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/zh-cn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      244 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/zh.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     5866 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/menubutton/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1171 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/menubutton/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.759738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/da.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       90 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       75 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/eo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       87 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/fr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/gl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       77 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       78 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/ko.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      103 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       77 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       78 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/nl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       95 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       86 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       98 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/ru.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/sv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       82 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/zh-cn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       79 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/zh.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     6761 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notificationaggregator/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2718 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notificationaggregator/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pagebreak/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pagebreak/images/
--rw-r--r--   0 matthias  (1000) matthias  (1000)       99 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pagebreak/images/pagebreak.gif
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastefromgdocs/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastefromgdocs/filter/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2209 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastefromgdocs/filter/default.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastefromlibreoffice/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastefromlibreoffice/filter/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3510 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastefromlibreoffice/filter/default.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastefromword/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastefromword/filter/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    19568 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastefromword/filter/default.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastetools/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastetools/filter/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    10380 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastetools/filter/common.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3932 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastetools/filter/image.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/dialogs/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      599 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/dialogs/placeholder.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/icons/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/icons/hidpi/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1775 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/icons/hidpi/placeholder.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      714 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/icons/placeholder.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      400 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/af.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      496 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ar.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      438 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/bg.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      453 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      443 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      404 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/cy.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      414 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/da.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      396 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      693 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/el.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      409 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/en-gb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      402 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      430 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/eo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      482 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/es.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      406 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/et.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      403 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/eu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      541 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/fa.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      401 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/fi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      432 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/fr-ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      440 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/fr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      475 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/gl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      453 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/he.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      448 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/hr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      414 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/hu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      413 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/id.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      410 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      461 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ja.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      525 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/km.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      432 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ko.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      492 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      408 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/lv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      408 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      416 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/nl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      408 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/no.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      432 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      456 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      409 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/pt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      527 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ru.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      491 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/si.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      421 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/sk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      399 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/sl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      428 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/sq.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      430 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/sv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      474 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/th.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      394 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      473 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/tt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      433 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ug.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      523 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/uk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      418 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/vi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      377 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/zh-cn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      389 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/zh.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1479 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/preview/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/preview/images/
--rw-r--r--   0 matthias  (1000) matthias  (1000)       99 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/preview/images/pagebreak.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      259 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/preview/preview.html
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/preview/styles/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      242 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/preview/styles/screen.css
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/scayt/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      225 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/scayt/CHANGELOG.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1476 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/scayt/LICENSE.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4565 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/scayt/README.md
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/scayt/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      419 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/scayt/dialogs/dialog.css
--rw-r--r--   0 matthias  (1000) matthias  (1000)    16136 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/scayt/dialogs/options.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1302 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/scayt/dialogs/toolbar.css
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/scayt/skins/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/scayt/skins/moono-lisa/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      381 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/scayt/skins/moono-lisa/scayt.css
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sharedspace/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1522 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sharedspace/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      152 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_address.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      154 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_blockquote.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      127 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_div.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      120 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_h1.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      127 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_h2.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      123 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_h3.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      123 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_h4.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      126 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_h5.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      123 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_h6.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      115 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_p.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      128 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_pre.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.769738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3461 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/dialogs/smiley.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.779738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1245 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angel_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1172 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angel_smile.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1219 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angry_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1220 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angry_smile.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      732 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/broken_heart.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1139 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/broken_heart.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1202 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/confused_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1101 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/confused_smile.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      795 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/cry_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1214 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/cry_smile.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1239 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/devil_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1220 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/devil_smile.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      786 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/embaressed_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      786 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/embarrassed_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1145 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/embarrassed_smile.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      506 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/envelope.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      760 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/envelope.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      692 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/heart.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      999 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/heart.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      683 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/kiss.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1003 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/kiss.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      660 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/lightbulb.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      919 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/lightbulb.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      820 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/omg_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1122 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/omg_smile.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1209 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/regular_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1084 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/regular_smile.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      782 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/sad_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1115 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/sad_smile.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1231 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/shades_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1204 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/shades_smile.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1201 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/teeth_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1183 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/teeth_smile.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      715 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_down.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      985 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_down.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      714 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_up.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      959 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_up.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1210 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/tongue_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1132 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/tongue_smile.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1210 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/tounge_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      775 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/whatchutalkingabout_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1039 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/whatchutalkingabout_smile.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1202 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/wink_smile.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1114 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/wink_smile.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.779738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.779738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/dialogs/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      924 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/dialogs/sourcedialog.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.779738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.779738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/hidpi/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1968 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/hidpi/sourcedialog-rtl.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1999 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/hidpi/sourcedialog.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      762 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/sourcedialog-rtl.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      764 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/sourcedialog.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.779738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       79 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/af.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       95 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ar.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      103 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/bg.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      101 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/bn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       89 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/bs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       89 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       79 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/cy.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/da.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       89 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       99 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/el.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       86 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/en-au.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       86 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/en-ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       86 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/en-gb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/eo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       93 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/es.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       91 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/et.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       99 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/eu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       87 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/fa.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/fi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/fo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       86 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/fr-ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/fr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/gl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      203 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/gu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       87 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/he.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      101 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/hi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       79 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/hr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       93 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/hu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/id.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/is.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       87 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       89 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ja.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      107 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ka.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      125 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/km.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ko.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       99 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       89 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/lt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       89 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/lv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/mn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ms.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       87 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/nl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/no.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      109 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      100 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/pt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ro.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      103 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ru.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      125 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/si.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/sk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       95 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/sl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/sq.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       84 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/sr-latn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/sr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/sv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      117 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/th.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       99 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/tt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       91 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ug.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       99 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/uk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       87 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/vi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       86 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/zh-cn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       89 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/zh.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      746 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.779738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.789738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      738 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/_translationstatus.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4547 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/af.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4796 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ar.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3407 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/az.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4820 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/bg.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5028 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ca.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4985 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/cs.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4909 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/cy.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3380 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/da.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4807 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/de-ch.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4798 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/de.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     7746 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/el.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4564 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en-au.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4564 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en-ca.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4564 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en-gb.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4561 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4082 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/eo.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4790 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/es-mx.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4961 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/es.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3831 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/et.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4563 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/eu.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5786 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fa.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4599 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fi.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3234 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fr-ca.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3870 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fr.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5018 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/gl.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5000 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/he.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4405 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/hr.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4149 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/hu.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4568 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/id.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5034 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/it.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3998 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ja.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4765 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/km.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4934 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ko.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     7578 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ku.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4606 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/lt.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5036 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/lv.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3446 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/nb.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4740 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/nl.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3446 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/no.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3844 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/oc.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4343 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/pl.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3844 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/pt-br.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4809 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/pt.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4692 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ro.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     7561 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ru.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4902 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/si.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4778 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sk.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4363 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sl.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5005 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sq.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4728 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sr-latn.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     7530 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sr.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3498 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sv.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4690 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/th.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4493 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/tr.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6743 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/tt.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5017 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ug.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6384 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/uk.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6099 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/vi.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4395 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/zh-cn.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4175 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/zh.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5005 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/specialchar.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.789738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/stylesheetparser/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1316 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/stylesheetparser/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/table/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.789738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/table/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     9043 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/table/dialogs/table.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.789738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/tableresize/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4460 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/tableresize/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/tableselection/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.789738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/tableselection/styles/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1145 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/tableselection/styles/tableselection.css
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.689738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/tabletools/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.789738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/tabletools/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     7354 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/tabletools/dialogs/tableCell.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.789738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.789738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/dialogs/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1588 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/dialogs/templates.css
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3403 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/dialogs/templates.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)      166 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/templatedefinition.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.789738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1961 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/default.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.789738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/images/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      539 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/images/template1.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      497 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/images/template2.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)      557 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/images/template3.gif
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.789738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.789738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/dialogs/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2657 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/dialogs/uicolor.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.789738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/icons/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.789738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/icons/hidpi/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2287 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/icons/hidpi/uicolor.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      965 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/icons/uicolor.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.799738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      909 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/_translationstatus.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      322 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/af.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      375 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/ar.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      399 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/bg.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      337 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      350 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      341 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/cy.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      346 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/da.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      343 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      463 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/el.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      330 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/en-gb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      325 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      341 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/eo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      370 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/es.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      347 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/et.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      366 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/eu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      433 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/fa.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      355 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/fi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      348 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/fr-ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      364 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/fr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      369 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/gl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      403 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/he.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      340 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/hr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      353 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/hu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      333 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/id.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      338 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      362 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/ja.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      555 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/km.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      338 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/ko.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      462 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      344 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/lv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      403 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/mk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      365 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      335 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/nl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      365 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/no.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      360 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      343 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      355 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/pt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      454 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/ru.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      492 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/si.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      343 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/sk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      344 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/sl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      354 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/sq.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      359 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/sv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      351 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      425 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/tt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      456 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/ug.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      399 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/uk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      385 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/vi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      339 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/zh-cn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      348 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/zh.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      834 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.799738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.799738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1120 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/hue_bg.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      195 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/hue_thumb.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    12174 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/picker_mask.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      192 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/picker_thumb.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2541 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/yui.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)   109872 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/yui.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.799738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadimage/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1509 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadimage/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.799738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.799738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      454 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      422 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/da.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      475 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      432 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      444 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/eo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      515 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/fr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      468 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/gl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      459 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/hu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      481 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      523 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/ko.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      577 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      448 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      456 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/nl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      456 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      449 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      537 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/ru.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      445 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/sv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      506 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      448 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/zh-cn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      443 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/zh.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3105 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.799738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.799738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/images/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      220 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/images/handle.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.799738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      223 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/af.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      233 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/ar.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      254 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/bg.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      227 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      235 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      220 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/cy.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      225 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/da.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      234 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      294 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/el.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      223 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/en-gb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      220 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      222 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/eo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      229 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/es.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      244 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/fa.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      233 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/fi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      231 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/fr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      225 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/gl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      226 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/he.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      226 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/hr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      231 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/hu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      233 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      222 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/ja.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      282 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/km.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      244 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/ko.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      252 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      234 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/lv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      224 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      229 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/nl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      224 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/no.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      237 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      227 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      225 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/pt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      236 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/ru.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      234 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/sk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      234 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/sl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      233 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/sq.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      229 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/sv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      241 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      260 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/tt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/uk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      239 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/vi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      225 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/zh-cn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      213 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/zh.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    29663 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.799738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1474 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/LICENSE.md
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4528 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/README.md
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.799738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1690 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/ciframe.html
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1962 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/tmpFrameset.html
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1232 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/wsc.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    47292 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/wsc.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3404 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/wsc_ie.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.799738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/icons/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.799738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/icons/hidpi/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2816 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/icons/hidpi/spellchecker.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      836 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/icons/spellchecker.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.809738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      728 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/af.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1113 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ar.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      962 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/bg.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1335 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/bn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      725 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/bs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      829 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      834 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/cs.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      788 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/cy.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      708 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/da.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      892 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/de.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1304 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/el.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      728 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en-au.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      728 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en-ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      728 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en-gb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      725 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      827 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/eo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      840 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/es.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      823 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/et.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      841 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/eu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1105 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fa.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      786 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      786 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fo.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      864 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fr-ca.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      946 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      862 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/gl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1527 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/gu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      911 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/he.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1372 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/hi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      757 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/hr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      870 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/hu.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      699 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/is.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      841 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/it.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      988 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ja.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1564 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ka.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1569 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/km.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      850 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ko.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1218 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ku.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      817 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/lt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      899 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/lv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      725 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/mk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1036 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/mn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      788 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ms.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      747 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/nb.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      844 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/nl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      747 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/no.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      798 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/pl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      938 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/pt-br.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      876 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/pt.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      914 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ro.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1320 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ru.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      878 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      792 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sl.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      817 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sr-latn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1136 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      783 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sv.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1307 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/th.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      831 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/tr.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1206 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ug.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1259 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/uk.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1031 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/vi.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      731 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/zh-cn.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      712 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/zh.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2188 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.699738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/skins/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.809738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/skins/moono-lisa/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1306 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/skins/moono-lisa/wsc.css
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.809738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/xml/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/xml/plugin.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.699738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.809738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    13430 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    14341 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_ie.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    14898 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_ie7.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    14513 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_ie8.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    14370 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_iequirks.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    43055 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/editor.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    43136 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_gecko.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    44054 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_ie.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    46078 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_ie7.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    44229 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_ie8.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    44703 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_iequirks.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    20634 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/icons.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    67753 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/icons_hidpi.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.809738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      191 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/arrow.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      468 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/close.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.809738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1271 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/close.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1329 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/lock-open.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1299 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/lock.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1842 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/refresh.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      349 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/lock-open.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      475 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/lock.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      422 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/refresh.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2984 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/spinner.gif
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2364 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/readme.md
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.809738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    13634 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog.css
--rw-r--r--   0 matthias  (1000) matthias  (1000)    14657 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog_ie.css
--rw-r--r--   0 matthias  (1000) matthias  (1000)    15206 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog_ie8.css
--rw-r--r--   0 matthias  (1000) matthias  (1000)    14686 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog_iequirks.css
--rw-r--r--   0 matthias  (1000) matthias  (1000)    48309 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor.css
--rw-r--r--   0 matthias  (1000) matthias  (1000)    48390 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_gecko.css
--rw-r--r--   0 matthias  (1000) matthias  (1000)    49308 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_ie.css
--rw-r--r--   0 matthias  (1000) matthias  (1000)    50114 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_ie8.css
--rw-r--r--   0 matthias  (1000) matthias  (1000)    49957 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_iequirks.css
--rw-r--r--   0 matthias  (1000) matthias  (1000)    12237 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/icons.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)    38309 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/icons_hidpi.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.809738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      191 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/arrow.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      615 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/close.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.809738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1238 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/close.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1071 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/lock-open.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1062 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/lock.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1623 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/refresh.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      511 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/lock-open.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      506 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/lock.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)      757 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/refresh.png
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2984 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/spinner.gif
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2284 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/readme.md
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5577 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/styles.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.809738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/vendor/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6297 2023-03-22 10:03:03.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/vendor/promise.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1526 2022-12-08 11:14:37.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor-init.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      584 2023-06-23 08:08:18.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor.css
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.809738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/file-icons/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2066 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/file-icons/doc.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1270 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/file-icons/file.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1929 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/file-icons/pdf.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1766 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/file-icons/ppt.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1970 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/file-icons/swf.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1898 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/file-icons/txt.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1659 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/file-icons/xls.png
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.699738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1043 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/basic.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      865 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/black.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3542 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/caption.png
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3363 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/galleriffic-1.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3166 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/galleriffic-2.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3167 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/galleriffic-3.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3373 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/galleriffic-4.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3451 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/galleriffic-5.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1836 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/jush.css
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    10453 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/loader.gif
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    10294 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/loaderWhite.gif
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       79 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/nextPageArrow.gif
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       79 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/nextPageArrowWhite.gif
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       78 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/prevPageArrow.gif
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       78 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/prevPageArrowWhite.gif
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      849 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/white.css
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/js/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)   120619 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/js/jquery-1.3.2.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    33266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/js/jquery.galleriffic.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     6465 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/js/jquery.history.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      937 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/js/jquery.opacityrollover.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)   111151 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/js/jush.js
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.699738 django-ckeditor-6.6.0/ckeditor/templates/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/ckeditor/templates/ckeditor/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      461 2022-05-19 09:30:59.000000 django-ckeditor-6.6.0/ckeditor/templates/ckeditor/widget.html
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4214 2023-06-23 08:08:18.000000 django-ckeditor-6.6.0/ckeditor/widgets.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/ckeditor_demo/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor_demo/__init__.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/ckeditor_demo/demo_application/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      148 2022-04-11 07:31:10.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/admin.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      177 2022-04-11 07:31:10.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/apps.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1938 2022-05-19 09:30:59.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/forms.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/ckeditor_demo/demo_application/migrations/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1222 2023-06-23 08:08:18.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/migrations/0001_initial.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/migrations/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      282 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/models.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      431 2022-02-23 10:18:39.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/test_custom_backend.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3304 2022-04-11 07:31:10.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/test_deprecation.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3959 2022-04-11 07:31:10.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/test_dummy.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3390 2022-05-19 09:30:59.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/test_fields.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     7931 2022-04-11 07:31:10.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/test_pillow.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     5299 2022-05-19 09:30:59.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/test_widget_context.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     5181 2022-08-10 12:04:12.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/tests_functional.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2120 2022-04-11 07:31:10.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/utils.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      611 2022-04-11 07:31:10.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/views.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      157 2022-04-11 07:31:10.000000 django-ckeditor-6.6.0/ckeditor_demo/demo_application/widgets.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4850 2022-04-11 07:31:10.000000 django-ckeditor-6.6.0/ckeditor_demo/settings.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      688 2023-06-23 08:08:18.000000 django-ckeditor-6.6.0/ckeditor_demo/urls.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      405 2022-04-11 07:31:10.000000 django-ckeditor-6.6.0/ckeditor_demo/wsgi.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/ckeditor_uploader/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      733 2022-04-21 08:48:39.000000 django-ckeditor-6.6.0/ckeditor_uploader/__init__.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/ckeditor_uploader/backends/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1329 2022-04-21 08:48:39.000000 django-ckeditor-6.6.0/ckeditor_uploader/backends/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      465 2022-04-21 08:48:39.000000 django-ckeditor-6.6.0/ckeditor_uploader/backends/dummy_backend.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2525 2022-04-21 08:48:39.000000 django-ckeditor-6.6.0/ckeditor_uploader/backends/pillow_backend.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      409 2022-04-21 08:48:39.000000 django-ckeditor-6.6.0/ckeditor_uploader/fields.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      177 2022-04-21 08:48:39.000000 django-ckeditor-6.6.0/ckeditor_uploader/forms.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/ckeditor_uploader/management/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-04-21 08:48:39.000000 django-ckeditor-6.6.0/ckeditor_uploader/management/__init__.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/ckeditor_uploader/management/commands/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-04-21 08:48:39.000000 django-ckeditor-6.6.0/ckeditor_uploader/management/commands/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1363 2022-05-31 09:45:18.000000 django-ckeditor-6.6.0/ckeditor_uploader/management/commands/generateckeditorthumbnails.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.699738 django-ckeditor-6.6.0/ckeditor_uploader/static/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.699738 django-ckeditor-6.6.0/ckeditor_uploader/static/ckeditor/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/ckeditor_uploader/static/ckeditor/ckeditor_uploader/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1429 2022-04-21 08:48:39.000000 django-ckeditor-6.6.0/ckeditor_uploader/static/ckeditor/ckeditor_uploader/admin_base.css
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.699738 django-ckeditor-6.6.0/ckeditor_uploader/templates/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/ckeditor_uploader/templates/ckeditor/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     9963 2022-04-21 08:48:39.000000 django-ckeditor-6.6.0/ckeditor_uploader/templates/ckeditor/browse.html
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      417 2022-04-21 08:48:39.000000 django-ckeditor-6.6.0/ckeditor_uploader/urls.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2542 2022-04-21 08:48:39.000000 django-ckeditor-6.6.0/ckeditor_uploader/utils.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     7951 2022-04-21 08:48:39.000000 django-ckeditor-6.6.0/ckeditor_uploader/views.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      458 2022-04-21 08:48:39.000000 django-ckeditor-6.6.0/ckeditor_uploader/widgets.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/django_ckeditor.egg-info/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    32080 2023-06-23 08:10:44.000000 django-ckeditor-6.6.0/django_ckeditor.egg-info/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)    83940 2023-06-23 08:10:44.000000 django-ckeditor-6.6.0/django_ckeditor.egg-info/SOURCES.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2023-06-23 08:10:44.000000 django-ckeditor-6.6.0/django_ckeditor.egg-info/dependency_links.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-05-19 09:31:28.000000 django-ckeditor-6.6.0/django_ckeditor.egg-info/not-zip-safe
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       33 2023-06-23 08:10:44.000000 django-ckeditor-6.6.0/django_ckeditor.egg-info/requires.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       41 2023-06-23 08:10:44.000000 django-ckeditor-6.6.0/django_ckeditor.egg-info/top_level.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      312 2023-06-23 08:10:44.819738 django-ckeditor-6.6.0/setup.cfg
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1997 2022-12-08 11:14:37.000000 django-ckeditor-6.6.0/setup.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.949699 django-ckeditor-6.6.1/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      683 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/AUTHORS.rst
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    11154 2023-06-23 08:09:49.000000 django-ckeditor-6.6.1/CHANGELOG.rst
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1484 2022-04-11 07:31:10.000000 django-ckeditor-6.6.1/LICENSE
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      354 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/MANIFEST.in
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    32080 2023-06-23 08:17:07.949699 django-ckeditor-6.6.1/PKG-INFO
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    19300 2022-04-11 07:31:10.000000 django-ckeditor-6.6.1/README.rst
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       62 2023-06-23 08:16:43.000000 django-ckeditor-6.6.1/ckeditor/__init__.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      672 2023-04-14 07:34:40.000000 django-ckeditor-6.6.1/ckeditor/configs.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1259 2022-04-14 19:26:20.000000 django-ckeditor-6.6.1/ckeditor/fields.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.799699 django-ckeditor-6.6.1/ckeditor/static/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.829699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)   312603 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/CHANGES.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    77827 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/LICENSE.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1383 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/README.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      578 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/SECURITY.md
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.829699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/adapters/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3180 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/adapters/jquery.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      246 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/bender-runner.config.json
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3585 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/build-config.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)   758081 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/ckeditor.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      336 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/config.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3092 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/contents.css
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.829699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    17658 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/af.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    22093 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ar.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19554 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/az.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    26713 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/bg.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    23072 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/bn.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    17707 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/bs.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19415 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ca.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19445 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/cs.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18112 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/cy.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18472 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/da.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19320 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/de-ch.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19298 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/de.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    28609 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/el.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    17611 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/en-au.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    17608 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/en-ca.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    17633 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/en-gb.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    17623 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/en.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18846 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/eo.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19675 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/es-mx.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19605 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/es.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18275 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/et.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19320 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/eu.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    24193 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/fa.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18689 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/fi.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18616 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/fo.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19190 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/fr-ca.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    20170 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/fr.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19673 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/gl.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    28699 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/gu.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    21675 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/he.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    23513 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/hi.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18231 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/hr.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19815 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/hu.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18031 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/id.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18191 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/is.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19537 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/it.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    21405 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ja.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    31095 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ka.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    32492 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/km.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19134 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ko.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    26297 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ku.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19344 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/lt.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19577 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/lv.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19360 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/mk.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    22367 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/mn.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    17912 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ms.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18026 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/nb.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18653 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/nl.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18047 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/no.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19826 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/oc.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19639 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/pl.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19669 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/pt-br.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19542 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/pt.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    20386 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ro.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    27538 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ru.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    24449 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/si.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19729 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/sk.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18411 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/sl.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    20147 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/sq.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18615 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/sr-latn.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    25807 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/sr.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18178 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/sv.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    27007 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/th.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19330 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/tr.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    22884 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/tt.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    25797 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ug.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    27576 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/uk.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    21086 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/vi.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    17296 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/zh-cn.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    17174 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/zh.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.829699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.799699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.829699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2953 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/a11yhelp.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.839699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      887 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/_translationstatus.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4156 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/af.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4351 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ar.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4332 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/az.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4565 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/bg.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4788 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ca.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4938 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/cs.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4389 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/cy.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4247 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/da.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4712 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/de-ch.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4656 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/de.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     7631 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/el.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4203 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/en-au.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4203 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/en-gb.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4200 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/en.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4797 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/eo.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4893 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/es-mx.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4799 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/es.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4418 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/et.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4505 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/eu.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6152 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fa.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4760 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fi.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4202 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fo.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4922 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fr-ca.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5309 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fr.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4814 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/gl.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4410 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/gu.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4955 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/he.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4214 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/hi.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4281 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/hr.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4766 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/hu.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4039 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/id.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5237 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/it.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5200 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ja.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5218 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/km.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5599 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ko.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6033 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ku.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4209 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/lt.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4832 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/lv.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4591 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/mk.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4207 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/mn.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4457 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/nb.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4532 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/nl.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4443 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/no.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5098 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/oc.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5160 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/pl.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4927 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/pt-br.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4568 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/pt.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4559 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ro.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6646 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ru.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6145 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/si.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4769 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sk.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4548 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sl.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4933 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sq.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4896 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sr-latn.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     7514 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sr.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4369 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sv.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4578 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/th.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4579 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/tr.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4518 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/tt.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6936 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ug.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6926 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/uk.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5400 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/vi.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4148 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/zh-cn.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4357 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/zh.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.799699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/about/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.839699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1827 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/about.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.839699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/hidpi/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    12236 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/hidpi/logo_ckeditor.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5650 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/logo_ckeditor.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.839699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/adobeair/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2486 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/adobeair/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.839699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/ajax/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1277 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/ajax/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.839699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.839699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      165 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      191 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      164 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      190 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      238 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      169 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      189 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      173 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      184 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      162 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/lang/zh.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2334 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.839699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autogrow/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1912 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autogrow/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.839699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autolink/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      584 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autolink/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.839699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/bbcode/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     9190 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/bbcode/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/clipboard/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.839699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/clipboard/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3809 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/clipboard/dialogs/paste.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.839699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.839699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1179 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/codesnippet.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.839699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/icons/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      597 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/icons/codesnippet.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.839699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1887 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/codesnippet.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.849699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      454 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ar.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      457 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/bg.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      397 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      376 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      360 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/da.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      380 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      526 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/el.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      372 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/en-gb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      369 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      358 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/eo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      419 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/es.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      373 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/et.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      398 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/fa.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      362 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/fi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      369 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/fr-ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      395 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/fr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      416 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/gl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      389 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/he.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      370 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/hr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      379 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/hu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      413 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      431 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ja.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      388 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/km.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      396 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ko.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      419 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      386 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/lt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      373 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/lv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      360 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      352 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/nl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      368 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/no.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      363 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      415 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      384 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/pt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      383 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ro.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      423 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ru.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      374 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/sk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      366 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/sl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      370 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/sq.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      355 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/sv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      431 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/th.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      373 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      419 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/tt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      388 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/ug.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      392 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/uk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      382 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/vi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      365 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/zh-cn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      380 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/zh.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.849699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    30194 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/CHANGES.md
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1498 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/LICENSE
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     7705 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.ru.md
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    30179 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/highlight.pack.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.849699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2514 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/arta.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      853 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ascetic.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1811 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.dark.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1825 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.light.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1836 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.dark.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1845 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.light.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1826 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.dark.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1835 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.light.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1857 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.dark.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1866 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.light.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1847 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.dark.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1856 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.light.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1896 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_paper.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    18198 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_papersq.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1864 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/dark.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2804 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/default.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1908 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/docco.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2016 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/far.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1715 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/foundation.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1809 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/github.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2309 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/googlecode.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1856 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/idea.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1567 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ir_black.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2046 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/magula.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      961 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/mono-blue.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2141 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2485 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai_sublime.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2470 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/obsidian.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1586 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.dark.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1587 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.light.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1747 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1186 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.jpg
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2736 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/railscasts.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1707 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/rainbow.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2096 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      486 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1709 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_dark.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1709 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_light.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2398 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/sunburst.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1696 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-blue.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1625 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-bright.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1629 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-eighties.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1693 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1519 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1650 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/vs.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2452 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/xcode.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1971 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/zenburn.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3824 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.849699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippetgeshi/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3104 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippetgeshi/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/colordialog/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.849699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/colordialog/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      790 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/colordialog/dialogs/colordialog.css
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5327 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/colordialog/dialogs/colordialog.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.849699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/cursors/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4012 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/cursors/cursor-disabled.svg
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2759 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/cursors/cursor.svg
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.849699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/styles/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1511 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/styles/copyformatting.css
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.849699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.859699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      909 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/_translationstatus.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      370 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ar.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      415 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/bg.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      365 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      324 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      331 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/cy.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      333 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/da.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      323 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      442 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/el.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      326 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/en-gb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      321 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      348 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/eo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      364 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/es.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      319 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/et.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      350 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/eu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      355 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/fa.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      334 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/fi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      352 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/fr-ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      362 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/fr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      348 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/gl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      442 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/gu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      351 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/he.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      337 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/hr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      320 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/hu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      317 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/id.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      331 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      349 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ja.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      458 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/km.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      338 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ko.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      385 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      344 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/lt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      337 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/lv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      326 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      318 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/nl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      326 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/no.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      336 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      348 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      351 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/pt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      345 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ro.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      389 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ru.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      452 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/si.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      326 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/sk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      324 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/sl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      350 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/sq.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      318 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/sv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      323 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      429 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/tt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      389 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/ug.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      437 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/uk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      324 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/vi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      326 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/zh-cn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      317 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/zh.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2451 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.859699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/dialog/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      166 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/dialog/dialogDefinition.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.859699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/dialog/styles/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      249 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/dialog/styles/dialog.css
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/div/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.859699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/div/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4676 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/div/dialogs/div.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.859699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/divarea/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      556 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/divarea/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.859699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.859699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/dialogs/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    10823 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/dialogs/docprops.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.859699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      840 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/docprops-rtl.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      844 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/docprops.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.859699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/hidpi/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1909 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/hidpi/docprops-rtl.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1941 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/hidpi/docprops.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.859699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1107 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/af.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1384 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ar.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1304 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/bg.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1752 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/bn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1120 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/bs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1211 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1125 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1152 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/cy.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1109 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/da.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1170 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1752 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/el.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1123 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en-au.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1123 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en-ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1125 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en-gb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1120 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1076 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/eo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1171 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/es.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1133 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/et.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1195 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/eu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1405 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fa.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1092 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1149 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1096 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fr-ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1109 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1236 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/gl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2115 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/gu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1293 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/he.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2035 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/hi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1120 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/hr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1129 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/hu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1123 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/id.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1101 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/is.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1132 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1235 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ja.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2013 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ka.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2027 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/km.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1157 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ko.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1564 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1223 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/lt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1153 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/lv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1120 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/mk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1532 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/mn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1123 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ms.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1060 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1129 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/nl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1059 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/no.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1184 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1217 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1199 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/pt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1281 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ro.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1703 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ru.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1583 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/si.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1171 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1079 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1252 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sq.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1151 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sr-latn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1469 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1073 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1969 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/th.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1143 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1282 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/tt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1586 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ug.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1630 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/uk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1275 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/vi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1030 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/zh-cn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1070 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/zh.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      910 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.859699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embed/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.859699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embed/icons/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      389 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embed/icons/embed.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.859699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embed/icons/hidpi/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      728 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embed/icons/hidpi/embed.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1058 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embed/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.859699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.859699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/dialogs/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1095 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/dialogs/embedbase.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      463 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      475 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/da.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      515 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      470 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      475 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/eo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      553 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/fr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      533 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/gl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      565 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      606 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/ko.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      791 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      482 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      513 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/nl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      594 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      529 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      722 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/ru.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      483 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/sv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      516 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      418 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/zh-cn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      453 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/zh.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3405 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/icons/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      389 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/icons/embedsemantic.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/icons/hidpi/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      728 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/icons/hidpi/embedsemantic.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1460 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3004 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/CHANGELOG.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      973 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/LICENSE.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6314 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/README.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        3 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/plugindefinition.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/_helpers/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      673 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/_helpers/tools.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3033 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/authentication.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4826 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/exportpdf.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      694 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/configfilename.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1267 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/configfilename.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      432 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/emptyeditor.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      906 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/emptyeditor.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5396 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integration.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1135 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integration.md
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integrations/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      814 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integrations/easyimage.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      882 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integrations/easyimage.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      396 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/notifications.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1161 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/notifications.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1047 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/notificationsasync.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      799 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/notificationsasync.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1273 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/paperformat.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      637 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/paperformat.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      411 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/readonly.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      611 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/readonly.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1200 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/stylesheets.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      651 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/stylesheets.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      568 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokenfetching.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      666 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokenfetching.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1064 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorscorrect.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      515 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorscorrect.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1088 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorswrong.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      524 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorswrong.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      475 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokenwithouturl.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      862 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokenwithouturl.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      488 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/wrongendpoint.html
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      824 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/wrongendpoint.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1974 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/notification.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4749 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/resourcespaths.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1096 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/statistics.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     9882 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/stylesheets.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      650 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      624 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/da.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      742 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      599 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      624 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/eo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      771 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/fr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      703 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/gl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      769 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      721 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/ko.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      896 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      603 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      611 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/nl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      648 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      675 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      738 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/ru.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      590 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/sv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      606 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      608 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/zh-cn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      614 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/zh.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     4383 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/find/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/find/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    11424 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/find/dialogs/find.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/flash/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/flash/dialogs/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    10230 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/flash/dialogs/flash.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/flash/images/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      256 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/flash/images/placeholder.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1863 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/button.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2577 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/checkbox.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2127 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/form.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1706 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/hiddenfield.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2387 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/radio.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     8526 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/select.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2334 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/textarea.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3437 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/textfield.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/images/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      178 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/images/hiddenfield.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    12237 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/icons.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    38309 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/icons_hidpi.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/iframe/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/iframe/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3479 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/iframe/dialogs/iframe.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/iframe/images/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      265 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/iframe/images/placeholder.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/iframedialog/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1953 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/iframedialog/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    21529 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image/dialogs/image.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image/images/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1610 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image/images/noimage.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/dialogs/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     5101 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/dialogs/image2.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/icons/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.869699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/icons/hidpi/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1745 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/icons/hidpi/image.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      756 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/icons/image.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      449 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/af.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      539 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ar.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      752 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/bg.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      648 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/bn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      416 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/bs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      476 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      469 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      441 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/cy.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      460 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/da.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      470 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      749 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/el.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      417 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/en-au.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      417 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/en-ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      417 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/en-gb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      414 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      471 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/eo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      470 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/es.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      421 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/et.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      447 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/eu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      590 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/fa.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      468 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/fi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      435 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/fo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      493 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/fr-ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      504 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/fr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      450 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/gl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      607 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/gu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      514 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/he.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      619 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/hi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      416 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/hr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      459 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/hu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      408 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/id.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      415 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/is.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      473 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      511 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ja.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      736 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ka.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      892 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/km.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      486 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ko.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      584 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      440 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/lt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      499 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/lv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      414 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/mk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      578 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/mn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      416 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ms.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      454 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      510 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/nl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      451 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/no.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      458 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      488 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      473 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/pt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      470 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ro.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      712 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ru.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      635 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/si.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      464 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/sk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      451 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/sl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      478 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/sq.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      427 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/sr-latn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      522 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/sr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      454 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/sv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      839 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/th.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      473 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      579 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/tt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      535 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ug.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      726 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/uk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      500 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/vi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      412 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/zh-cn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      405 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/zh.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    13531 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/icons/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/icons/hidpi/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1678 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/icons/hidpi/language.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      668 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/icons/language.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      246 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/ar.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      256 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/bg.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      243 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      241 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      234 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/cy.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      234 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/da.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      246 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/el.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      242 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/en-gb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      239 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      241 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/eo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      241 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/es.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      246 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/fa.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      235 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/fi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      242 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/fo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      249 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/fr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      248 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/gl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      238 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/he.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      237 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/hr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      252 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/hu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      240 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      242 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/ja.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/km.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      248 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/ko.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      264 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      235 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      242 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/nl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      235 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/no.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      236 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      247 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      240 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/pt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      264 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/ru.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      244 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/sk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      239 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/sl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      247 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/sq.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      238 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/sv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      233 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      254 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/tt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/uk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      260 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/vi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      239 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/zh-cn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      236 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/lang/zh.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2093 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/lineutils/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     9203 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/lineutils/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/link/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/link/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2207 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/link/dialogs/anchor.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    13234 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/link/dialogs/link.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/link/images/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      752 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/link/images/anchor.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/link/images/hidpi/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1109 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/link/images/hidpi/anchor.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/liststyle/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/liststyle/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2883 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/liststyle/dialogs/liststyle.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/magicline/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/magicline/images/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/magicline/images/hidpi/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      176 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/magicline/images/hidpi/icon-rtl.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      199 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/magicline/images/hidpi/icon.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      138 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/magicline/images/icon-rtl.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      133 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/magicline/images/icon.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/dialogs/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1385 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/dialogs/mathjax.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/icons/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.879699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/icons/hidpi/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1437 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/icons/hidpi/mathjax.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      703 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/icons/mathjax.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.889699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/images/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      784 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/images/loader.gif
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.889699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      239 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/af.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      296 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/ar.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      359 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/bg.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      264 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      248 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/cy.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      247 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/da.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      259 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      350 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/el.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      245 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/en-gb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      243 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      258 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/eo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      252 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/es.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      317 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/fa.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/fi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      279 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/fr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      269 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/gl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      277 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/he.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      261 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/hr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      247 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/hu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      258 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      274 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/ja.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      411 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/km.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      301 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/ko.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      304 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      254 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/lt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      242 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      241 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/nl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      242 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/no.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      274 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      265 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      265 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/pt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      253 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/ro.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      316 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/ru.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      254 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/sk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      260 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/sl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      268 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/sq.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      241 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/sv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      269 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      373 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/tt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      339 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/uk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      256 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/vi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      347 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/zh-cn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      244 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/lang/zh.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     5866 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.889699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/menubutton/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1171 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/menubutton/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.889699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.889699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/da.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       90 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       75 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/eo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       87 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/fr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/gl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       77 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       78 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/ko.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      103 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       77 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       78 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/nl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       95 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       86 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       98 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/ru.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/sv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       82 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/zh-cn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       79 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/lang/zh.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     6761 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.889699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notificationaggregator/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2718 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notificationaggregator/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pagebreak/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.889699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pagebreak/images/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       99 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pagebreak/images/pagebreak.gif
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastefromgdocs/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.889699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastefromgdocs/filter/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2209 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastefromgdocs/filter/default.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.809699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastefromlibreoffice/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.889699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastefromlibreoffice/filter/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3510 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastefromlibreoffice/filter/default.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastefromword/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.889699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastefromword/filter/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19568 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastefromword/filter/default.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastetools/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.889699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastetools/filter/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    10380 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastetools/filter/common.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3932 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastetools/filter/image.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.889699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.889699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/dialogs/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      599 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/dialogs/placeholder.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.889699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/icons/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.889699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/icons/hidpi/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1775 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/icons/hidpi/placeholder.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      714 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/icons/placeholder.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.899699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      400 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/af.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      496 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ar.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      438 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/bg.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      453 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      443 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      404 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/cy.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      414 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/da.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      396 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      693 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/el.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      409 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/en-gb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      402 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      430 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/eo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      482 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/es.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      406 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/et.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      403 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/eu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      541 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/fa.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      401 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/fi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      432 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/fr-ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      440 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/fr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      475 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/gl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      453 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/he.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      448 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/hr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      414 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/hu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      413 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/id.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      410 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      461 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ja.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      525 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/km.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      432 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ko.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      492 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      408 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/lv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      408 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      416 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/nl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      408 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/no.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      432 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      456 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      409 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/pt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      527 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ru.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      491 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/si.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      421 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/sk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      399 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/sl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      428 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/sq.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      430 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/sv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      474 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/th.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      394 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      473 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/tt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      433 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ug.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      523 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/uk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      418 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/vi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      377 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/zh-cn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      389 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/zh.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1479 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.899699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/preview/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.899699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/preview/images/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       99 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/preview/images/pagebreak.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      259 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/preview/preview.html
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.899699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/preview/styles/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      242 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/preview/styles/screen.css
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.899699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/scayt/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      225 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/scayt/CHANGELOG.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1476 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/scayt/LICENSE.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4565 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/scayt/README.md
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.899699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/scayt/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      419 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/scayt/dialogs/dialog.css
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    16136 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/scayt/dialogs/options.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1302 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/scayt/dialogs/toolbar.css
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/scayt/skins/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.899699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/scayt/skins/moono-lisa/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      381 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/scayt/skins/moono-lisa/scayt.css
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.899699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sharedspace/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1522 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sharedspace/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.899699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      152 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_address.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      154 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_blockquote.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      127 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_div.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      120 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_h1.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      127 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_h2.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      123 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_h3.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      123 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_h4.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      126 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_h5.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      123 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_h6.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      115 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_p.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      128 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/showblocks/images/block_pre.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.899699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3461 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/dialogs/smiley.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.899699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1245 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angel_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1172 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angel_smile.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1219 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angry_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1220 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angry_smile.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      732 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/broken_heart.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1139 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/broken_heart.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1202 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/confused_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1101 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/confused_smile.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      795 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/cry_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1214 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/cry_smile.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1239 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/devil_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1220 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/devil_smile.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      786 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/embaressed_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      786 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/embarrassed_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1145 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/embarrassed_smile.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      506 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/envelope.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      760 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/envelope.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      692 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/heart.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      999 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/heart.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      683 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/kiss.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1003 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/kiss.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      660 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/lightbulb.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      919 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/lightbulb.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      820 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/omg_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1122 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/omg_smile.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1209 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/regular_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1084 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/regular_smile.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      782 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/sad_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1115 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/sad_smile.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1231 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/shades_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1204 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/shades_smile.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1201 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/teeth_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1183 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/teeth_smile.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      715 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_down.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      985 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_down.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      714 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_up.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      959 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_up.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1210 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/tongue_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1132 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/tongue_smile.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1210 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/tounge_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      775 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/whatchutalkingabout_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1039 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/whatchutalkingabout_smile.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1202 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/wink_smile.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1114 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/wink_smile.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.899699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.899699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/dialogs/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      924 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/dialogs/sourcedialog.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.899699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.899699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/hidpi/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1968 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/hidpi/sourcedialog-rtl.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1999 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/hidpi/sourcedialog.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      762 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/sourcedialog-rtl.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      764 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/sourcedialog.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.909699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       79 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/af.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       95 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ar.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      103 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/bg.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      101 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/bn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       89 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/bs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       89 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       79 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/cy.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/da.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       89 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       99 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/el.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       86 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/en-au.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       86 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/en-ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       86 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/en-gb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/eo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       93 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/es.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       91 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/et.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       99 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/eu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       87 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/fa.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/fi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/fo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       86 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/fr-ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/fr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/gl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      203 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/gu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       87 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/he.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      101 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/hi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       79 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/hr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       93 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/hu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/id.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/is.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       87 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       89 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ja.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      107 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ka.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      125 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/km.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ko.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       99 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       89 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/lt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       89 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/lv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/mn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ms.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       87 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/nl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/no.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      109 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      100 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/pt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ro.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      103 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ru.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      125 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/si.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/sk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       95 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/sl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/sq.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       84 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/sr-latn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       81 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/sr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/sv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      117 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/th.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       83 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       99 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/tt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       91 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/ug.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       99 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/uk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       87 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/vi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       86 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/zh-cn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       89 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/lang/zh.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      746 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.909699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.909699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      738 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/_translationstatus.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4547 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/af.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4796 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ar.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3407 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/az.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4820 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/bg.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5028 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ca.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4985 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/cs.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4909 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/cy.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3380 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/da.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4807 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/de-ch.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4798 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/de.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     7746 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/el.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4564 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en-au.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4564 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en-ca.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4564 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en-gb.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4561 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4082 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/eo.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4790 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/es-mx.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4961 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/es.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3831 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/et.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4563 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/eu.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5786 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fa.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4599 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fi.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3234 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fr-ca.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3870 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fr.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5018 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/gl.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5000 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/he.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4405 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/hr.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4149 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/hu.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4568 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/id.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5034 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/it.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3998 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ja.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4765 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/km.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4934 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ko.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     7578 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ku.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4606 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/lt.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5036 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/lv.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3446 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/nb.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4740 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/nl.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3446 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/no.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3844 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/oc.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4343 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/pl.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3844 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/pt-br.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4809 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/pt.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4692 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ro.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     7561 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ru.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4902 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/si.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4778 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sk.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4363 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sl.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5005 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sq.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4728 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sr-latn.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     7530 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sr.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3498 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sv.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4690 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/th.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4493 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/tr.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6743 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/tt.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5017 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ug.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6384 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/uk.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6099 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/vi.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4395 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/zh-cn.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4175 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/zh.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5005 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/specialchar.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/stylesheetparser/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1316 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/stylesheetparser/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/table/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/table/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     9043 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/table/dialogs/table.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/tableresize/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     4460 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/tableresize/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/tableselection/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/tableselection/styles/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1145 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/tableselection/styles/tableselection.css
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/tabletools/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/tabletools/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     7354 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/tabletools/dialogs/tableCell.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/dialogs/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1588 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/dialogs/templates.css
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3403 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/dialogs/templates.js
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      166 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/templatedefinition.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1961 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/default.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/images/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      539 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/images/template1.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      497 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/images/template2.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      557 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/images/template3.gif
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/dialogs/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2657 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/dialogs/uicolor.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/icons/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/icons/hidpi/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2287 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/icons/hidpi/uicolor.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      965 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/icons/uicolor.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      909 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/_translationstatus.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      322 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/af.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      375 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/ar.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      399 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/bg.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      337 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      350 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      341 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/cy.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      346 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/da.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      343 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      463 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/el.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      330 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/en-gb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      325 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      341 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/eo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      370 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/es.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      347 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/et.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      366 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/eu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      433 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/fa.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      355 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/fi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      348 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/fr-ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      364 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/fr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      369 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/gl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      403 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/he.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      340 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/hr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      353 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/hu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      333 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/id.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      338 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      362 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/ja.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      555 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/km.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      338 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/ko.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      462 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      344 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/lv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      403 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/mk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      365 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      335 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/nl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      365 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/no.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      360 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      343 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      355 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/pt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      454 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/ru.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      492 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/si.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      343 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/sk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      344 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/sl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      354 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/sq.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      359 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/sv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      351 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      425 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/tt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      456 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/ug.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      399 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/uk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      385 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/vi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      339 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/zh-cn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      348 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/zh.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      834 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1120 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/hue_bg.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      195 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/hue_thumb.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    12174 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/picker_mask.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      192 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/picker_thumb.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2541 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/yui.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)   109872 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/yui.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadimage/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1509 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadimage/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      454 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      422 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/da.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      475 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      432 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      444 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/eo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      515 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/fr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      468 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/gl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      459 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/hu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      481 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      523 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/ko.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      577 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      448 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      456 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/nl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      456 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      449 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      537 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/ru.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      445 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/sv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      506 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      448 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/zh-cn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      443 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/zh.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3105 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.919699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/images/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      220 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/images/handle.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.929699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      223 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/af.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      233 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/ar.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      254 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/bg.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      227 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      235 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      220 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/cy.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      225 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/da.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      234 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      294 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/el.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      223 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/en-gb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      220 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      222 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/eo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      229 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/es.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      244 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/fa.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      233 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/fi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      231 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/fr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      225 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/gl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      226 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/he.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      226 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/hr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      231 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/hu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      233 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      222 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/ja.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      282 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/km.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      244 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/ko.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      252 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      234 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/lv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      224 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      229 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/nl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      224 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/no.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      237 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      227 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      225 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/pt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      236 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/ru.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      234 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/sk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      234 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/sl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      233 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/sq.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      229 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/sv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      241 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      260 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/tt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/uk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      239 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/vi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      225 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/zh-cn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      213 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/lang/zh.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    29663 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.929699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1474 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/LICENSE.md
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     4528 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/README.md
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.929699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1690 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/ciframe.html
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1962 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/tmpFrameset.html
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1232 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/wsc.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    47292 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/wsc.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3404 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/wsc_ie.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.929699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/icons/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.929699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/icons/hidpi/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2816 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/icons/hidpi/spellchecker.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      836 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/icons/spellchecker.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.929699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      728 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/af.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1113 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ar.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      962 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/bg.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1335 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/bn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      725 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/bs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      829 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      834 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/cs.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      788 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/cy.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      708 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/da.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      892 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/de.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1304 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/el.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      728 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en-au.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      728 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en-ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      728 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en-gb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      725 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      827 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/eo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      840 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/es.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      823 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/et.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      841 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/eu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1105 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fa.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      786 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      786 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fo.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      864 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fr-ca.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      946 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      862 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/gl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1527 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/gu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      911 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/he.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1372 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/hi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      757 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/hr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      870 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/hu.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      699 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/is.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      841 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/it.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      988 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ja.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1564 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ka.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1569 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/km.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      850 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ko.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1218 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ku.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      817 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/lt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      899 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/lv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      725 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/mk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1036 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/mn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      788 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ms.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      747 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/nb.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      844 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/nl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      747 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/no.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      798 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/pl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      938 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/pt-br.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      876 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/pt.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      914 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ro.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1320 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ru.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      878 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      792 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sl.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      817 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sr-latn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1136 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      783 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sv.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1307 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/th.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      831 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/tr.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1206 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ug.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1259 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/uk.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1031 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/vi.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      731 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/zh-cn.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      712 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/zh.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2188 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/skins/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.929699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/skins/moono-lisa/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1306 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/skins/moono-lisa/wsc.css
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.929699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/xml/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/xml/plugin.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    13430 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    14341 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_ie.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    14898 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_ie7.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    14513 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_ie8.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    14370 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_iequirks.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    43055 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/editor.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    43136 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_gecko.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    44054 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_ie.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    46078 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_ie7.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    44229 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_ie8.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    44703 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_iequirks.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    20634 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/icons.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    67753 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/icons_hidpi.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      191 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/arrow.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      468 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/close.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1271 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/close.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1329 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/lock-open.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1299 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/lock.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1842 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/refresh.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      349 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/lock-open.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      475 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/lock.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      422 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/refresh.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2984 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/spinner.gif
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2364 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/readme.md
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    13634 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog.css
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    14657 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog_ie.css
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    15206 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog_ie8.css
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    14686 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog_iequirks.css
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    48309 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor.css
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    48390 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_gecko.css
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    49308 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_ie.css
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    50114 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_ie8.css
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    49957 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_iequirks.css
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    12237 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/icons.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    38309 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/icons_hidpi.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      191 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/arrow.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      615 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/close.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1238 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/close.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1071 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/lock-open.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1062 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/lock.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1623 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/refresh.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      511 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/lock-open.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      506 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/lock.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      757 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/refresh.png
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2984 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/spinner.gif
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2284 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/readme.md
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5577 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/styles.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/vendor/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6297 2023-03-22 10:03:03.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/vendor/promise.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1526 2022-12-08 11:14:37.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor-init.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      672 2023-06-23 08:16:02.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor.css
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/file-icons/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2066 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/file-icons/doc.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1270 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/file-icons/file.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1929 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/file-icons/pdf.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1766 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/file-icons/ppt.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1970 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/file-icons/swf.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1898 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/file-icons/txt.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1659 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/file-icons/xls.png
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1043 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/basic.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      865 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/black.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3542 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/caption.png
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3363 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/galleriffic-1.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3166 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/galleriffic-2.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3167 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/galleriffic-3.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3373 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/galleriffic-4.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3451 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/galleriffic-5.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1836 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/jush.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    10453 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/loader.gif
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    10294 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/loaderWhite.gif
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       79 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/nextPageArrow.gif
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       79 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/nextPageArrowWhite.gif
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       78 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/prevPageArrow.gif
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       78 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/prevPageArrowWhite.gif
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      849 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/white.css
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/js/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)   120619 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/js/jquery-1.3.2.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    33266 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/js/jquery.galleriffic.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     6465 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/js/jquery.history.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      937 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/js/jquery.opacityrollover.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)   111151 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/js/jush.js
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor/templates/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor/templates/ckeditor/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      461 2022-05-19 09:30:59.000000 django-ckeditor-6.6.1/ckeditor/templates/ckeditor/widget.html
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     4214 2023-06-23 08:08:18.000000 django-ckeditor-6.6.1/ckeditor/widgets.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor_demo/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor_demo/__init__.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor_demo/demo_application/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/__init__.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      148 2022-04-11 07:31:10.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/admin.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      177 2022-04-11 07:31:10.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/apps.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1938 2022-05-19 09:30:59.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/forms.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor_demo/demo_application/migrations/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1222 2023-06-23 08:08:18.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/migrations/0001_initial.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/migrations/__init__.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      282 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/models.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/__init__.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      431 2022-02-23 10:18:39.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/test_custom_backend.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3304 2022-04-11 07:31:10.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/test_deprecation.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3959 2022-04-11 07:31:10.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/test_dummy.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3390 2022-05-19 09:30:59.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/test_fields.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     7931 2022-04-11 07:31:10.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/test_pillow.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     5299 2022-05-19 09:30:59.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/test_widget_context.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     5181 2022-08-10 12:04:12.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/tests_functional.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2120 2022-04-11 07:31:10.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/utils.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      611 2022-04-11 07:31:10.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/views.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      157 2022-04-11 07:31:10.000000 django-ckeditor-6.6.1/ckeditor_demo/demo_application/widgets.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     4850 2022-04-11 07:31:10.000000 django-ckeditor-6.6.1/ckeditor_demo/settings.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      688 2023-06-23 08:08:18.000000 django-ckeditor-6.6.1/ckeditor_demo/urls.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      405 2022-04-11 07:31:10.000000 django-ckeditor-6.6.1/ckeditor_demo/wsgi.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor_uploader/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      733 2022-04-21 08:48:39.000000 django-ckeditor-6.6.1/ckeditor_uploader/__init__.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor_uploader/backends/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1329 2022-04-21 08:48:39.000000 django-ckeditor-6.6.1/ckeditor_uploader/backends/__init__.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      465 2022-04-21 08:48:39.000000 django-ckeditor-6.6.1/ckeditor_uploader/backends/dummy_backend.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2525 2022-04-21 08:48:39.000000 django-ckeditor-6.6.1/ckeditor_uploader/backends/pillow_backend.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      409 2022-04-21 08:48:39.000000 django-ckeditor-6.6.1/ckeditor_uploader/fields.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      177 2022-04-21 08:48:39.000000 django-ckeditor-6.6.1/ckeditor_uploader/forms.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.939699 django-ckeditor-6.6.1/ckeditor_uploader/management/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-04-21 08:48:39.000000 django-ckeditor-6.6.1/ckeditor_uploader/management/__init__.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.949699 django-ckeditor-6.6.1/ckeditor_uploader/management/commands/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2022-04-21 08:48:39.000000 django-ckeditor-6.6.1/ckeditor_uploader/management/commands/__init__.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1363 2022-05-31 09:45:18.000000 django-ckeditor-6.6.1/ckeditor_uploader/management/commands/generateckeditorthumbnails.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor_uploader/static/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor_uploader/static/ckeditor/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.949699 django-ckeditor-6.6.1/ckeditor_uploader/static/ckeditor/ckeditor_uploader/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1429 2022-04-21 08:48:39.000000 django-ckeditor-6.6.1/ckeditor_uploader/static/ckeditor/ckeditor_uploader/admin_base.css
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.819699 django-ckeditor-6.6.1/ckeditor_uploader/templates/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.949699 django-ckeditor-6.6.1/ckeditor_uploader/templates/ckeditor/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     9963 2022-04-21 08:48:39.000000 django-ckeditor-6.6.1/ckeditor_uploader/templates/ckeditor/browse.html
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      417 2022-04-21 08:48:39.000000 django-ckeditor-6.6.1/ckeditor_uploader/urls.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2542 2022-04-21 08:48:39.000000 django-ckeditor-6.6.1/ckeditor_uploader/utils.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     7951 2022-04-21 08:48:39.000000 django-ckeditor-6.6.1/ckeditor_uploader/views.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      458 2022-04-21 08:48:39.000000 django-ckeditor-6.6.1/ckeditor_uploader/widgets.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2023-06-23 08:17:07.949699 django-ckeditor-6.6.1/django_ckeditor.egg-info/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    32080 2023-06-23 08:17:07.000000 django-ckeditor-6.6.1/django_ckeditor.egg-info/PKG-INFO
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)    83940 2023-06-23 08:17:07.000000 django-ckeditor-6.6.1/django_ckeditor.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2023-06-23 08:17:07.000000 django-ckeditor-6.6.1/django_ckeditor.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-05-19 09:31:28.000000 django-ckeditor-6.6.1/django_ckeditor.egg-info/not-zip-safe
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       33 2023-06-23 08:17:07.000000 django-ckeditor-6.6.1/django_ckeditor.egg-info/requires.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       41 2023-06-23 08:17:07.000000 django-ckeditor-6.6.1/django_ckeditor.egg-info/top_level.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      312 2023-06-23 08:17:07.949699 django-ckeditor-6.6.1/setup.cfg
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1997 2022-12-08 11:14:37.000000 django-ckeditor-6.6.1/setup.py
```

### Comparing `django-ckeditor-6.6.0/AUTHORS.rst` & `django-ckeditor-6.6.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/CHANGELOG.rst` & `django-ckeditor-6.6.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/LICENSE` & `django-ckeditor-6.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/PKG-INFO` & `django-ckeditor-6.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ckeditor
-Version: 6.6.0
+Version: 6.6.1
 Summary: Django admin CKEditor integration.
 Home-page: https://github.com/django-ckeditor/django-ckeditor
 Author: Shaun Sephton & Piotr Malinski
 Author-email: riklaunim@gmail.com
 Project-URL: Documentation, https://django-ckeditor.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/django-ckeditor/django-ckeditor
 Classifier: Programming Language :: Python
```

### Comparing `django-ckeditor-6.6.0/README.rst` & `django-ckeditor-6.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/configs.py` & `django-ckeditor-6.6.1/ckeditor/configs.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/fields.py` & `django-ckeditor-6.6.1/ckeditor/fields.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/CHANGES.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/CHANGES.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/LICENSE.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/README.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/README.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/SECURITY.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/SECURITY.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/adapters/jquery.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/adapters/jquery.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/build-config.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/build-config.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/ckeditor.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/ckeditor.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/contents.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/contents.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/af.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/af.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ar.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ar.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/az.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/az.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/bg.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/bg.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/bn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/bn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/bs.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/bs.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ca.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ca.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/cs.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/cs.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/cy.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/cy.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/da.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/da.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/de-ch.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/de.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/de.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/el.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/el.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/en-au.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/en-ca.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/en-ca.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/en-gb.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/en.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/en.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/eo.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/eo.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/es-mx.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/es-mx.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/es.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/es.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/et.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/et.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/eu.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/eu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/fa.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/fa.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/fi.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/fi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/fo.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/fo.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/fr-ca.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/fr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/fr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/gl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/gl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/gu.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/gu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/he.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/he.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/hi.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/hi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/hr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/hr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/hu.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/hu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/id.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/id.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/is.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/is.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/it.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/it.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ja.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ja.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ka.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ka.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/km.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/km.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ko.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ko.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ku.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ku.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/lt.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/lt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/lv.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/lv.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/mk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/mk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/mn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/mn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ms.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ms.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/nb.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/nb.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/nl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/nl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/no.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/no.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/oc.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/oc.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/pl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/pl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/pt-br.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/pt.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/pt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ro.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ro.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ru.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ru.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/si.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/si.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/sk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/sk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/sl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/sl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/sq.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/sq.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/sr-latn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/sr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/sr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/sv.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/sv.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/th.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/th.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/tr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/tr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/tt.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/tt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/ug.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/ug.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/uk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/uk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/vi.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/vi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/zh-cn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/lang/zh.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/lang/zh.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/a11yhelp.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/a11yhelp.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/_translationstatus.txt` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/_translationstatus.txt`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/af.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/af.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ar.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ar.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/az.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/az.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/bg.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/bg.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ca.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ca.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/cs.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/cs.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/cy.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/cy.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/da.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/da.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/de-ch.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/de.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/de.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/el.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/el.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/en-au.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/en-gb.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/en.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/en.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/eo.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/eo.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/es-mx.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/es-mx.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/es.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/es.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/et.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/et.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/eu.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/eu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fa.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fa.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fi.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fo.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fo.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fr-ca.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/fr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/gl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/gl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/gu.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/gu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/he.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/he.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/hi.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/hi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/hr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/hr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/hu.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/hu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/id.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/id.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/it.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/it.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ja.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ja.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/km.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/km.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ko.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ko.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ku.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ku.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/lt.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/lt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/lv.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/lv.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/mk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/mk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/mn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/mn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/nb.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/nb.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/nl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/nl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/no.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/no.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/oc.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/oc.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/pl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/pl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/pt-br.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/pt.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/pt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ro.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ro.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ru.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ru.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/si.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/si.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sq.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sq.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sr-latn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sv.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/sv.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/th.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/th.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/tr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/tr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/tt.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/tt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ug.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/ug.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/uk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/uk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/vi.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/vi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/zh-cn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/zh.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/a11yhelp/dialogs/lang/zh.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/about.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/about.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/hidpi/logo_ckeditor.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/hidpi/logo_ckeditor.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/logo_ckeditor.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/about/dialogs/logo_ckeditor.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/adobeair/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/adobeair/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/ajax/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/ajax/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autoembed/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autogrow/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autogrow/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/autolink/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/autolink/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/bbcode/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/bbcode/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/clipboard/dialogs/paste.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/clipboard/dialogs/paste.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/codesnippet.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/codesnippet.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/icons/codesnippet.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/icons/codesnippet.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/codesnippet.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/codesnippet.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/el.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lang/el.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/CHANGES.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/CHANGES.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/LICENSE` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.ru.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.ru.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/highlight.pack.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/arta.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/arta.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ascetic.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ascetic.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.dark.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.dark.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.light.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.light.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.dark.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.dark.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.light.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.light.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.dark.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.dark.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.light.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.light.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.dark.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.dark.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.light.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.light.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.dark.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.dark.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.light.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.light.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_paper.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_paper.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_papersq.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_papersq.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/dark.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/dark.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/default.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/default.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/docco.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/docco.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/far.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/far.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/foundation.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/foundation.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/github.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/github.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/googlecode.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/googlecode.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/idea.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/idea.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ir_black.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ir_black.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/magula.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/magula.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/mono-blue.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/mono-blue.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai_sublime.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai_sublime.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/obsidian.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/obsidian.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.dark.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.dark.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.light.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.light.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.jpg` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.jpg`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/railscasts.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/railscasts.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/rainbow.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/rainbow.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_dark.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_dark.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_light.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_light.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/sunburst.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/sunburst.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-blue.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-blue.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-bright.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-bright.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-eighties.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-eighties.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/vs.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/vs.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/xcode.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/xcode.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/zenburn.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/zenburn.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippet/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/codesnippetgeshi/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/codesnippetgeshi/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/colordialog/dialogs/colordialog.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/colordialog/dialogs/colordialog.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/colordialog/dialogs/colordialog.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/colordialog/dialogs/colordialog.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/cursors/cursor-disabled.svg` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/cursors/cursor-disabled.svg`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/cursors/cursor.svg` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/cursors/cursor.svg`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/styles/copyformatting.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/copyformatting/styles/copyformatting.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/_translationstatus.txt` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/lang/_translationstatus.txt`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/devtools/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/devtools/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/div/dialogs/div.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/div/dialogs/div.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/divarea/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/divarea/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/dialogs/docprops.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/dialogs/docprops.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/docprops-rtl.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/docprops-rtl.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/docprops.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/docprops.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/hidpi/docprops-rtl.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/hidpi/docprops-rtl.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/hidpi/docprops.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/icons/hidpi/docprops.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/af.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/af.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ar.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ar.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/bg.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/bg.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/bn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/bn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/bs.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/bs.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ca.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ca.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/cs.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/cs.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/cy.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/cy.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/da.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/da.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/de.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/de.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/el.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/el.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en-au.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en-ca.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en-ca.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en-gb.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/en.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/eo.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/eo.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/es.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/es.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/et.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/et.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/eu.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/eu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fa.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fa.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fi.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fo.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fo.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fr-ca.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/fr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/gl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/gl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/gu.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/gu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/he.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/he.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/hi.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/hi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/hr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/hr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/hu.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/hu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/id.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/id.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/is.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/is.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/it.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/it.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ja.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ja.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ka.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ka.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/km.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/km.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ko.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ko.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ku.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ku.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/lt.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/lt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/lv.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/lv.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/mk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/mk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/mn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/mn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ms.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ms.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/nb.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/nb.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/nl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/nl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/no.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/no.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/pl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/pl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/pt-br.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/pt.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/pt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ro.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ro.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ru.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ru.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/si.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/si.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sq.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sq.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sr-latn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sv.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/sv.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/th.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/th.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/tr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/tr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/tt.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/tt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ug.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/ug.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/uk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/uk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/vi.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/vi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/zh-cn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/zh.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/lang/zh.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/docprops/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/docprops/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embed/icons/hidpi/embed.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embed/icons/hidpi/embed.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embed/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embed/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/dialogs/embedbase.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/dialogs/embedbase.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/de.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/de.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/fr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/fr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/gl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/gl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/it.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/it.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/ko.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/ko.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/ku.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/ku.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/nl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/nl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/pl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/pl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/pt-br.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/ru.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/ru.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/tr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/lang/tr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedbase/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/icons/hidpi/embedsemantic.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/icons/hidpi/embedsemantic.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/embedsemantic/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/CHANGELOG.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/LICENSE.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/README.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/README.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/_helpers/tools.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/_helpers/tools.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/authentication.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/authentication.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/exportpdf.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/exportpdf.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/configfilename.html` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/configfilename.html`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/configfilename.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/configfilename.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/emptyeditor.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/emptyeditor.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integration.html` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integration.html`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integration.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integration.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integrations/easyimage.html` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integrations/easyimage.html`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integrations/easyimage.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/integrations/easyimage.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/notifications.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/notifications.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/notificationsasync.html` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/notificationsasync.html`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/notificationsasync.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/notificationsasync.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/paperformat.html` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/paperformat.html`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/paperformat.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/paperformat.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/readonly.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/readonly.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/stylesheets.html` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/stylesheets.html`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/stylesheets.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/stylesheets.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokenfetching.html` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokenfetching.html`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokenfetching.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokenfetching.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorscorrect.html` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorscorrect.html`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorscorrect.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorscorrect.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorswrong.html` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorswrong.html`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorswrong.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokentwoeditorswrong.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokenwithouturl.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/tokenwithouturl.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/wrongendpoint.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/manual/wrongendpoint.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/notification.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/notification.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/resourcespaths.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/resourcespaths.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/statistics.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/statistics.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/stylesheets.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/exportpdf/tests/stylesheets.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/cs.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/cs.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/da.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/da.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/de.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/de.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/en.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/en.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/eo.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/eo.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/fr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/fr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/gl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/gl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/it.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/it.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/ko.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/ko.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/ku.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/ku.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/nb.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/nb.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/nl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/nl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/pl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/pl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/pt-br.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/ru.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/ru.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/sv.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/sv.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/tr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/tr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/zh-cn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/zh.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/lang/zh.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/filetools/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/filetools/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/find/dialogs/find.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/find/dialogs/find.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/flash/dialogs/flash.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/flash/dialogs/flash.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/button.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/button.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/checkbox.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/checkbox.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/form.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/form.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/hiddenfield.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/hiddenfield.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/radio.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/radio.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/select.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/select.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/textarea.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/textarea.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/textfield.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/forms/dialogs/textfield.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/icons.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/icons.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/icons_hidpi.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/icons_hidpi.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/iframe/dialogs/iframe.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/iframe/dialogs/iframe.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/iframedialog/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/iframedialog/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image/dialogs/image.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image/dialogs/image.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image/images/noimage.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image/images/noimage.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/dialogs/image2.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/dialogs/image2.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/icons/hidpi/image.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/icons/hidpi/image.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/icons/image.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/icons/image.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ar.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ar.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/bg.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/bg.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/bn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/bn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/el.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/el.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/fa.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/fa.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/gu.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/gu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/he.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/he.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/hi.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/hi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ka.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ka.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/km.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/km.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ku.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ku.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/mn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/mn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ru.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ru.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/si.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/si.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/sr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/sr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/th.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/th.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/tt.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/tt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ug.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/ug.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/uk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/lang/uk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/image2/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/image2/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/icons/hidpi/language.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/icons/hidpi/language.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/icons/language.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/icons/language.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/language/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/language/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/lineutils/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/lineutils/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/link/dialogs/anchor.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/link/dialogs/anchor.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/link/dialogs/link.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/link/dialogs/link.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/link/images/anchor.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/link/images/anchor.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/link/images/hidpi/anchor.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/link/images/hidpi/anchor.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/liststyle/dialogs/liststyle.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/liststyle/dialogs/liststyle.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/dialogs/mathjax.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/dialogs/mathjax.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/icons/hidpi/mathjax.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/icons/hidpi/mathjax.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/icons/mathjax.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/icons/mathjax.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/images/loader.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/images/loader.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/mathjax/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/menubutton/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/menubutton/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notification/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notification/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/notificationaggregator/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/notificationaggregator/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastefromgdocs/filter/default.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastefromgdocs/filter/default.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastefromlibreoffice/filter/default.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastefromlibreoffice/filter/default.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastefromword/filter/default.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastefromword/filter/default.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastetools/filter/common.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastetools/filter/common.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/pastetools/filter/image.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/pastetools/filter/image.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/dialogs/placeholder.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/dialogs/placeholder.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/icons/hidpi/placeholder.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/icons/hidpi/placeholder.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/icons/placeholder.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/icons/placeholder.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/el.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/el.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/fa.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/fa.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/km.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/km.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ru.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/ru.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/uk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/lang/uk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/placeholder/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/scayt/LICENSE.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/scayt/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/scayt/README.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/scayt/README.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/scayt/dialogs/options.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/scayt/dialogs/options.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/scayt/dialogs/toolbar.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/scayt/dialogs/toolbar.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sharedspace/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sharedspace/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/dialogs/smiley.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/dialogs/smiley.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angel_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angel_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angel_smile.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angel_smile.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angry_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angry_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angry_smile.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/angry_smile.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/broken_heart.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/broken_heart.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/broken_heart.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/broken_heart.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/confused_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/confused_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/confused_smile.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/confused_smile.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/cry_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/cry_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/cry_smile.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/cry_smile.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/devil_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/devil_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/devil_smile.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/devil_smile.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/embaressed_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/embaressed_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/embarrassed_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/embarrassed_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/embarrassed_smile.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/embarrassed_smile.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/envelope.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/envelope.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/heart.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/heart.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/heart.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/heart.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/kiss.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/kiss.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/kiss.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/kiss.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/lightbulb.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/lightbulb.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/lightbulb.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/lightbulb.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/omg_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/omg_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/omg_smile.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/omg_smile.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/regular_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/regular_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/regular_smile.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/regular_smile.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/sad_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/sad_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/sad_smile.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/sad_smile.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/shades_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/shades_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/shades_smile.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/shades_smile.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/teeth_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/teeth_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/teeth_smile.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/teeth_smile.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_down.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_down.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_down.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_down.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_up.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_up.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_up.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/thumbs_up.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/tongue_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/tongue_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/tongue_smile.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/tongue_smile.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/tounge_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/tounge_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/whatchutalkingabout_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/whatchutalkingabout_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/whatchutalkingabout_smile.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/whatchutalkingabout_smile.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/wink_smile.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/wink_smile.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/wink_smile.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/smiley/images/wink_smile.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/dialogs/sourcedialog.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/dialogs/sourcedialog.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/hidpi/sourcedialog-rtl.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/hidpi/sourcedialog-rtl.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/hidpi/sourcedialog.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/hidpi/sourcedialog.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/sourcedialog-rtl.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/sourcedialog-rtl.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/sourcedialog.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/icons/sourcedialog.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/sourcedialog/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/_translationstatus.txt` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/_translationstatus.txt`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/af.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/af.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ar.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ar.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/az.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/az.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/bg.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/bg.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ca.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ca.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/cs.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/cs.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/cy.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/cy.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/da.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/da.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/de-ch.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/de.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/de.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/el.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/el.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en-au.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en-ca.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en-ca.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en-gb.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/en.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/eo.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/eo.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/es-mx.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/es-mx.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/es.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/es.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/et.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/et.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/eu.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/eu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fa.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fa.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fi.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fr-ca.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/fr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/gl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/gl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/he.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/he.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/hr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/hr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/hu.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/hu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/id.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/id.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/it.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/it.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ja.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ja.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/km.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/km.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ko.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ko.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ku.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ku.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/lt.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/lt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/lv.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/lv.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/nb.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/nb.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/nl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/nl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/no.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/no.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/oc.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/oc.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/pl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/pl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/pt-br.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/pt.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/pt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ro.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ro.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ru.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ru.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/si.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/si.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sq.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sq.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sr-latn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sv.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/sv.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/th.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/th.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/tr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/tr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/tt.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/tt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ug.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/ug.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/uk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/uk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/vi.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/vi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/zh-cn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/zh.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/lang/zh.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/specialchar.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/specialchar/dialogs/specialchar.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/stylesheetparser/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/stylesheetparser/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/table/dialogs/table.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/table/dialogs/table.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/tableresize/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/tableresize/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/tableselection/styles/tableselection.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/tableselection/styles/tableselection.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/tabletools/dialogs/tableCell.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/tabletools/dialogs/tableCell.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/dialogs/templates.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/dialogs/templates.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/dialogs/templates.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/dialogs/templates.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/default.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/default.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/images/template1.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/images/template1.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/images/template3.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/templates/templates/images/template3.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/dialogs/uicolor.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/dialogs/uicolor.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/icons/hidpi/uicolor.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/icons/hidpi/uicolor.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/icons/uicolor.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/icons/uicolor.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/_translationstatus.txt` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/_translationstatus.txt`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/km.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/lang/km.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/hue_bg.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/hue_bg.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/picker_mask.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/picker_mask.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/yui.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/assets/yui.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/yui.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uicolor/yui/yui.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadimage/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadimage/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/fr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/fr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/ko.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/ko.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/ku.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/ku.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/ru.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/lang/ru.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/uploadwidget/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/widget/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/widget/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/LICENSE.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/README.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/README.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/ciframe.html` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/ciframe.html`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/tmpFrameset.html` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/tmpFrameset.html`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/wsc.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/wsc.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/wsc.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/wsc.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/wsc_ie.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/dialogs/wsc_ie.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/icons/hidpi/spellchecker.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/icons/hidpi/spellchecker.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/icons/spellchecker.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/icons/spellchecker.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/af.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/af.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ar.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ar.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/bg.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/bg.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/bn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/bn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/bs.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/bs.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ca.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ca.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/cs.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/cs.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/cy.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/cy.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/da.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/da.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/de.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/de.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/el.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/el.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en-au.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en-ca.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en-ca.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en-gb.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/en.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/eo.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/eo.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/es.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/es.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/et.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/et.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/eu.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/eu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fa.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fa.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fi.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fo.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fo.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fr-ca.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/fr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/gl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/gl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/gu.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/gu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/he.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/he.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/hi.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/hi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/hr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/hr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/hu.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/hu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/is.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/is.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/it.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/it.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ja.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ja.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ka.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ka.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/km.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/km.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ko.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ko.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ku.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ku.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/lt.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/lt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/lv.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/lv.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/mk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/mk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/mn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/mn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ms.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ms.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/nb.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/nb.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/nl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/nl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/no.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/no.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/pl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/pl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/pt-br.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/pt.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/pt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ro.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ro.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ru.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ru.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sl.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sr-latn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sv.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/sv.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/th.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/th.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/tr.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/tr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ug.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/ug.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/uk.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/uk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/vi.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/vi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/zh-cn.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/zh.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/lang/zh.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/wsc/skins/moono-lisa/wsc.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/wsc/skins/moono-lisa/wsc.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/plugins/xml/plugin.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/plugins/xml/plugin.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_ie.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_ie.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_ie7.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_ie7.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_ie8.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_ie8.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_iequirks.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/dialog_iequirks.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/editor.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/editor.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_gecko.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_gecko.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_ie.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_ie.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_ie7.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_ie7.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_ie8.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_ie8.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_iequirks.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/editor_iequirks.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/icons.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/icons.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/icons_hidpi.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/icons_hidpi.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/close.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/close.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/lock-open.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/lock-open.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/lock.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/lock.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/refresh.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/hidpi/refresh.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/images/spinner.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono/readme.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono/readme.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog_ie.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog_ie.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog_ie8.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog_ie8.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog_iequirks.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/dialog_iequirks.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_gecko.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_gecko.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_ie.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_ie.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_ie8.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_ie8.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_iequirks.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/editor_iequirks.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/icons.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/icons.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/icons_hidpi.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/icons_hidpi.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/close.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/close.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/close.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/close.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/lock-open.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/lock-open.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/lock.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/lock.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/refresh.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/hidpi/refresh.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/refresh.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/refresh.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/spinner.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/readme.md` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/skins/moono-lisa/readme.md`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/styles.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/styles.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor/vendor/promise.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor/vendor/promise.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor-init.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor-init.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/ckeditor.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/ckeditor.css`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 /* Fix for Django dark theme background */
 /* See https://github.com/django-ckeditor/django-ckeditor/issues/670 */
 .cke_reset_all tr:nth-child(even),
 .cke_reset_all tr:nth-child(odd),
 .cke_reset_all .row-form-errors,
 .cke_reset_all tr:nth-child(even) .errorlist,
 .cke_reset_all tr:nth-child(odd) + .row-form-errors,
-.cke_reset_all tr:nth-child(odd) + .row-form-errors .errorlist {
-    background: inherit;
+.cke_reset_all tr:nth-child(odd) + .row-form-errors .errorlist,
+.cke_reset_all input[type="text"],
+.cke_reset_all input[type="password"] {
+  background: inherit;
+  color: inherit;
 }
 
 /* Fix for CKEditor source editor with Django dark theme */
 /* See https://github.com/django-ckeditor/django-ckeditor/issues/741 */
 textarea.cke_source {
-    color: revert;
+  color: revert;
 }
```

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/file-icons/doc.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/file-icons/doc.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/file-icons/file.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/file-icons/file.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/file-icons/pdf.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/file-icons/pdf.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/file-icons/ppt.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/file-icons/ppt.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/file-icons/swf.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/file-icons/swf.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/file-icons/txt.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/file-icons/txt.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/file-icons/xls.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/file-icons/xls.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/basic.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/basic.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/black.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/black.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/caption.png` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/caption.png`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/galleriffic-1.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/galleriffic-1.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/galleriffic-2.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/galleriffic-2.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/galleriffic-3.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/galleriffic-3.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/galleriffic-4.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/galleriffic-4.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/galleriffic-5.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/galleriffic-5.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/jush.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/jush.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/loader.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/loader.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/loaderWhite.gif` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/loaderWhite.gif`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/css/white.css` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/css/white.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/js/jquery-1.3.2.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/js/jquery-1.3.2.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/js/jquery.galleriffic.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/js/jquery.galleriffic.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/js/jquery.history.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/js/jquery.history.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/js/jquery.opacityrollover.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/js/jquery.opacityrollover.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/static/ckeditor/galleriffic/js/jush.js` & `django-ckeditor-6.6.1/ckeditor/static/ckeditor/galleriffic/js/jush.js`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor/widgets.py` & `django-ckeditor-6.6.1/ckeditor/widgets.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_demo/demo_application/forms.py` & `django-ckeditor-6.6.1/ckeditor_demo/demo_application/forms.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_demo/demo_application/migrations/0001_initial.py` & `django-ckeditor-6.6.1/ckeditor_demo/demo_application/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/test_deprecation.py` & `django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/test_dummy.py` & `django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/test_fields.py` & `django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/test_pillow.py` & `django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/test_pillow.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/test_widget_context.py` & `django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/test_widget_context.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/tests_functional.py` & `django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/tests_functional.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_demo/demo_application/tests/utils.py` & `django-ckeditor-6.6.1/ckeditor_demo/demo_application/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_demo/demo_application/views.py` & `django-ckeditor-6.6.1/ckeditor_demo/demo_application/views.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_demo/settings.py` & `django-ckeditor-6.6.1/ckeditor_demo/settings.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_demo/urls.py` & `django-ckeditor-6.6.1/ckeditor_demo/urls.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_uploader/__init__.py` & `django-ckeditor-6.6.1/ckeditor_uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_uploader/backends/__init__.py` & `django-ckeditor-6.6.1/ckeditor_uploader/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_uploader/backends/pillow_backend.py` & `django-ckeditor-6.6.1/ckeditor_uploader/backends/pillow_backend.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_uploader/management/commands/generateckeditorthumbnails.py` & `django-ckeditor-6.6.1/ckeditor_uploader/management/commands/generateckeditorthumbnails.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_uploader/static/ckeditor/ckeditor_uploader/admin_base.css` & `django-ckeditor-6.6.1/ckeditor_uploader/static/ckeditor/ckeditor_uploader/admin_base.css`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_uploader/templates/ckeditor/browse.html` & `django-ckeditor-6.6.1/ckeditor_uploader/templates/ckeditor/browse.html`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_uploader/utils.py` & `django-ckeditor-6.6.1/ckeditor_uploader/utils.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/ckeditor_uploader/views.py` & `django-ckeditor-6.6.1/ckeditor_uploader/views.py`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/django_ckeditor.egg-info/PKG-INFO` & `django-ckeditor-6.6.1/django_ckeditor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ckeditor
-Version: 6.6.0
+Version: 6.6.1
 Summary: Django admin CKEditor integration.
 Home-page: https://github.com/django-ckeditor/django-ckeditor
 Author: Shaun Sephton & Piotr Malinski
 Author-email: riklaunim@gmail.com
 Project-URL: Documentation, https://django-ckeditor.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/django-ckeditor/django-ckeditor
 Classifier: Programming Language :: Python
```

### Comparing `django-ckeditor-6.6.0/django_ckeditor.egg-info/SOURCES.txt` & `django-ckeditor-6.6.1/django_ckeditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ckeditor-6.6.0/setup.py` & `django-ckeditor-6.6.1/setup.py`

 * *Files identical despite different names*

