# Comparing `tmp/ckanext-geodatagov-0.1.8.tar.gz` & `tmp/ckanext-geodatagov-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-geodatagov-0.1.8.tar", last modified: Mon Oct  3 16:14:30 2022, max compression
+gzip compressed data, was "ckanext-geodatagov-0.1.9.tar", last modified: Wed Oct  5 20:29:24 2022, max compression
```

## Comparing `ckanext-geodatagov-0.1.8.tar` & `ckanext-geodatagov-0.1.9.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.362466 ckanext-geodatagov-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7210 2022-10-03 16:14:30.362466 ckanext-geodatagov-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5922 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (121)    11139 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    42703 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/harvesters/
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/harvesters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15250 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/harvesters/arcgis.py
--rw-r--r--   0 runner    (1001) docker     (121)    10218 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/harvesters/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4648 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/harvesters/waf_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3817 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/harvesters/z3950.py
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    19670 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/logic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    24420 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/saml2/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/saml2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/saml2/pkitestcrt/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/saml2/pkitestcrt/mycert.pem
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/saml2/pkitestcrt/mykey.pem
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/search.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.346466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/templates/organization/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/templates/organization/read.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/templates/organization/snippets/
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/templates/organization/snippets/organization_form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/templates/package/
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/templates/package/read.html
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/templates/package/search.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/templates/snippets/
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/templates/snippets/related_collection.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/templates/source/
--rw-r--r--   0 runner    (1001) docker     (121)     5494 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/templates/source/geodatagov_source_form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.346466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.346466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/tests/data-samples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/tests/data-samples/waf-collection1/
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/tests/data-samples/waf-collection1/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/tests/data-samples/waf-collection2/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/tests/data-samples/waf-collection2/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/tests/data-samples/waf-fgdc/
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/tests/data-samples/waf-fgdc/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/tests/data-samples/waf-gmi/
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/tests/data-samples/waf-gmi/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/tests/data-samples/waf-trim-tags/
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/tests/data-samples/waf-trim-tags/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/tests/data-samples/waf1/
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/tests/data-samples/waf1/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/
--rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.346466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.350466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/
--rw-r--r--   0 runner    (1001) docker     (121)    12555 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect03.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    69938 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect04.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    17854 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect05.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    10195 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect10.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    50490 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect01.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    27105 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect02.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    35634 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect06.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    10500 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect07.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    10304 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect08.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    12185 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect09.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.358466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/
--rw-r--r--   0 runner    (1001) docker     (121)    12555 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect03.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    69938 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect04.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    17854 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect05.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    26698 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect06.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     9938 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect08.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    10195 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect10.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    31196 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect01.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    31779 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect02.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    10267 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect07.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     7137 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect09.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6691 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.358466 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/
--rw-r--r--   0 runner    (1001) docker     (121)     9878 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect01.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     7751 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect02.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     5135 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect03.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    24168 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect04.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6327 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect05.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     9012 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect06.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    10276 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect07.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     9938 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect08.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6915 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect09.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    10195 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect10.xsd
--rw-r--r--   0 runner    (1001) docker     (121)   101010 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-instinfo.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6622 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-locainfo.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    20687 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-plmiinfo.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    22569 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect01.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    27195 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect02.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     5683 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect03.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    35720 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect04.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6537 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect05.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     7967 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 16:14:30.358466 ckanext-geodatagov-0.1.8/ckanext_geodatagov.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7210 2022-10-03 16:14:30.000000 ckanext-geodatagov-0.1.8/ckanext_geodatagov.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5188 2022-10-03 16:14:30.000000 ckanext-geodatagov-0.1.8/ckanext_geodatagov.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 16:14:30.000000 ckanext-geodatagov-0.1.8/ckanext_geodatagov.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-10-03 16:14:30.000000 ckanext-geodatagov-0.1.8/ckanext_geodatagov.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-10-03 16:14:30.000000 ckanext-geodatagov-0.1.8/ckanext_geodatagov.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 16:14:30.000000 ckanext-geodatagov-0.1.8/ckanext_geodatagov.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-03 16:14:30.000000 ckanext-geodatagov-0.1.8/ckanext_geodatagov.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-03 16:14:30.000000 ckanext-geodatagov-0.1.8/ckanext_geodatagov.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-10-03 16:14:30.362466 ckanext-geodatagov-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-10-03 16:14:29.000000 ckanext-geodatagov-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.587268 ckanext-geodatagov-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7210 2022-10-05 20:29:24.587268 ckanext-geodatagov-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5922 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.571268 ckanext-geodatagov-0.1.9/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.571268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10427 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42703 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15250 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/arcgis.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10218 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4648 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/waf_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3817 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/z3950.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19670 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/logic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24420 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/saml2/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/saml2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/saml2/pkitestcrt/
+-rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/saml2/pkitestcrt/mycert.pem
+-rw-r--r--   0 runner    (1001) docker     (121)      887 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/saml2/pkitestcrt/mykey.pem
+-rw-r--r--   0 runner    (1001) docker     (121)     1787 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/search.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.567268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/organization/
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/organization/read.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/organization/snippets/
+-rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/organization/snippets/organization_form.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/package/
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/package/read.html
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/package/search.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/snippets/
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/snippets/related_collection.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/source/
+-rw-r--r--   0 runner    (1001) docker     (121)     5494 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/source/geodatagov_source_form.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.567268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.567268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-collection1/
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-collection1/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-collection2/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-collection2/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.579268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-fgdc/
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-fgdc/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.579268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-gmi/
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-gmi/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.579268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-trim-tags/
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-trim-tags/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.579268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf1/
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf1/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.579268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/
+-rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.567268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.583268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/
+-rw-r--r--   0 runner    (1001) docker     (121)    12555 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect03.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    69938 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect04.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    17854 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect05.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    10195 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect10.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    50490 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect01.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    27105 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect02.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    35634 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect06.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    10500 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect07.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    10304 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect08.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    12185 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect09.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999.xsd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.583268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/
+-rw-r--r--   0 runner    (1001) docker     (121)    12555 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect03.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    69938 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect04.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    17854 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect05.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    26698 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect06.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     9938 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect08.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    10195 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect10.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    31196 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect01.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    31779 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect02.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    10267 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect07.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     7137 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect09.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     6691 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001.xsd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.587268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/
+-rw-r--r--   0 runner    (1001) docker     (121)     9878 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect01.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     7751 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect02.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     5135 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect03.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    24168 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect04.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     6327 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect05.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     9012 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect06.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    10276 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect07.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     9938 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect08.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     6915 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect09.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    10195 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect10.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)   101010 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-instinfo.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     6622 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-locainfo.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    20687 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-plmiinfo.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    22569 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect01.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    27195 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect02.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     5683 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect03.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)    35720 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect04.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     6537 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect05.xsd
+-rw-r--r--   0 runner    (1001) docker     (121)     7967 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002.xsd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.587268 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7210 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5188 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      855 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      814 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-10-05 20:29:24.587268 ckanext-geodatagov-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/setup.py
```

### Comparing `ckanext-geodatagov-0.1.8/LICENSE.md` & `ckanext-geodatagov-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/PKG-INFO` & `ckanext-geodatagov-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-geodatagov
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/GSA/ckanext-geodatagov
 Author: Data.gov
 Author-email: datagovhelp@gsa.gov
 License: UNKNOWN
 Description: [![Github Actions](https://github.com/GSA/ckanext-geodatagov/actions/workflows/test.yml/badge.svg)](https://github.com/GSA/ckanext-geodatagov/actions)
         [![PyPI version](https://badge.fury.io/py/ckanext-geodatagov.svg)](https://badge.fury.io/py/ckanext-geodatagov)
```

### Comparing `ckanext-geodatagov-0.1.8/README.md` & `ckanext-geodatagov-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/blueprint.py` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/blueprint.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/cli.py` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import datetime
 import io
 import json
 import logging
 
 import boto3
-import ckan.logic as logic
 import ckan.model as model
 import click
 from botocore.exceptions import ClientError
 from ckan.common import config
+from ckan.lib.search import rebuild
 from ckan.lib.search.common import make_connection
 from ckan.lib.search.index import NoopSearchIndex, PackageSearchIndex
 
 from ckanext.geodatagov.search import GeoPackageSearchQuery
 
 _INDICES = {
     'package': PackageSearchIndex
@@ -20,17 +20,14 @@
 
 # default constants
 DEFAULT_LOG = "ckanext.geodatagov"
 #   for sitemap_to_s3
 UPLOAD_TO_S3 = True
 PAGE_SIZE = 1000
 MAX_PER_PAGE = 50000
-DEFAULT_DRYRUN = False
-DEFAULT_CLEANUP_SOLR = False
-DEFAULT_UPDATE_SOLR = False
 
 log = logging.getLogger(DEFAULT_LOG)
 
 
 @click.group()
 def geodatagov():
     pass
@@ -239,80 +236,70 @@
     conn = make_connection()
     data = conn.search(query, fq=fq, rows=max_results, fl='id, metadata_modified')
 
     return [(r.get('id'), r.get('metadata_modified')) for r in data.docs]
 
 
 @geodatagov.command()
-@click.option("--dryrun", default=DEFAULT_DRYRUN, type=click.BOOL, help='inspect what will be updated')
-@click.option("--cleanup_solr", default=DEFAULT_CLEANUP_SOLR, type=click.BOOL, help='Only remove orphaned entries in Solr')
-@click.option("--update_solr", default=DEFAULT_UPDATE_SOLR, type=click.BOOL, help=(
+@click.option("--dryrun", is_flag=True, help='inspect what will be updated')
+@click.option("--cleanup_solr", is_flag=True, help='Only remove orphaned entries in Solr')
+@click.option("--update_solr", is_flag=True, help=(
     '(Update solr entries with new data from DB) OR (Add DB data to Solr that is missing)'))
 def db_solr_sync(dryrun, cleanup_solr, update_solr):
     ''' db solr sync '''
     if dryrun:
         log.info('Starting dryrun to update index.')
 
     package_index = index_for(model.Package)
-    context = {'model': model, 'ignore_auth': True, 'validate': False, 'use_cache': False}
 
     # get active packages from DB
     active_package = [(r[0], r[1].replace(microsecond=0)) for r in model.Session.query(model.Package.id,
                       model.Package.metadata_modified).filter(model.Package.state != 'deleted').all()]
     log.info(f"total {len(active_package)} DB active_package")
 
     # get indexed packages from solr
     indexed_package = set(get_all_entity_ids_and_date(max_results=2000000))
     log.info(f"total {len(indexed_package)} solr indexed_package")
 
     solr_package = indexed_package - set(active_package)
     db_package = set(active_package) - indexed_package
 
     work_list = {}
-    for id, date in (solr_package):
-        work_list[id] = {"solr": date}
-    for id, date in (db_package):
+    for id, _ in (solr_package):
+        work_list[id] = "solr"
+    for id, _ in (db_package):
         if id in work_list:
-            work_list[id].update({"db": date})
+            work_list[id] = "solr-db"
         else:
-            work_list[id] = {"db": date}
+            work_list[id] = "db"
 
     both = cleanup_solr == update_solr
-    count_to_cleanup = sum([1 if list(work_list[i].keys()) == ["solr"] else 0 for i in work_list])
-    count_to_update = len(work_list) - count_to_cleanup
+    set_cleanup = {i if work_list[i] == "solr" else None for i in work_list} - {None}
+    set_update = work_list.keys() - set_cleanup
+    log.info(f"{len(set_cleanup)} packages need to be removed from Solr")
+    log.info(f"{len(set_update)} packages need to be updated/added to Solr")
+
+    if not dryrun and set_cleanup and (cleanup_solr or both):
+        for id in set_cleanup:
+            log.info(f"deleting index with {id} \n")
+            try:
+                package_index.remove_dict({'id': id})
+            except Exception as e:
+                log.error(u'Error while delete index %s: %s' % (id, repr(e)))
+        package_index.commit()
+        log.info('Finished cleaning solr entries.')
 
-    if len(work_list) > 0:
-        if cleanup_solr or both:
-            log.info(f"{count_to_cleanup} packages need to be removed from Solr")
-        if update_solr or both:
-            log.info(f"{count_to_update} packages need to be updated/added to Solr")
-
-        for id in work_list:
-            if list(work_list[id].keys()) == ["solr"] and (cleanup_solr or both):
-                log.info(f"deleting index with {id} \n")
-                try:
-                    if not dryrun:
-                        package_index.remove_dict({'id': id})
-                except Exception as e:
-                    log.error(u'Error while delete index %s: %s' % (id, repr(e)))
-            elif list(work_list[id].keys()) in [["solr", "db"], ["db"]] and (update_solr or both):
-                log.info(f"updating index with {id} \n")
-                pkg_dict = logic.get_action('package_show')(context, {'id': id})
-                try:
-                    if not dryrun:
-                        package_index.remove_dict(pkg_dict)
-                        package_index.insert_dict(pkg_dict)
-                except Exception as e:
-                    log.error(u'Error while rebuild index %s: %s' % (id, repr(e)))
-    else:
-        log.info('Solr is good.')
-        return
-
-    model.Session.commit()
-    log.info('Finished updating solr entries.')
+    if not dryrun and set_update and (update_solr or both):
+        log.info("rebuilding indexes\n")
+        try:
+            rebuild(package_ids=set_update, defer_commit=True)
+        except Exception as e:
+            log.error(u'Error while rebuild index %s: %s' % (id, repr(e)))
+        package_index.commit()
+        log.info('Finished updating solr entries.')
 
 
 @geodatagov.command()
 def test_command():
     ''' Basic cli command with normal result '''
     print("This is a good test!")
     return True
```

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/commands.py` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/commands.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/harvesters/__init__.py` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/harvesters/arcgis.py` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/arcgis.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/harvesters/base.py` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/base.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/harvesters/waf_collection.py` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/waf_collection.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/harvesters/z3950.py` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/z3950.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/helpers.py` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/logic.py` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/logic.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/model.py` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/model.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/plugin.py` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/saml2/pkitestcrt/mycert.pem` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/saml2/pkitestcrt/mycert.pem`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/saml2/pkitestcrt/mykey.pem` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/saml2/pkitestcrt/mykey.pem`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/search.py` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/search.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/templates/organization/snippets/organization_form.html` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/organization/snippets/organization_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/templates/package/read.html` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/package/read.html`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/templates/source/geodatagov_source_form.html` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/source/geodatagov_source_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/tests/data-samples/waf1/index.html` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf1/index.html`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/__init__.py` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect03.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect03.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect04.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect04.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect05.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect05.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect10.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect10.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect01.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect01.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect02.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect02.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect06.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect06.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect07.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect07.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect08.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect08.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect09.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect09.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect03.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect03.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect04.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect04.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect05.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect05.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect06.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect06.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect08.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect08.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect10.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect10.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect01.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect01.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect02.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect02.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect07.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect07.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect09.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect09.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect01.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect01.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect02.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect02.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect03.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect03.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect04.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect04.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect05.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect05.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect06.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect06.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect07.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect07.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect08.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect08.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect09.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect09.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect10.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect10.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-instinfo.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-instinfo.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-locainfo.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-locainfo.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-plmiinfo.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-plmiinfo.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect01.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect01.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect02.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect02.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect03.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect03.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect04.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect04.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect05.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect05.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002.xsd` & `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext_geodatagov.egg-info/PKG-INFO` & `ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-geodatagov
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/GSA/ckanext-geodatagov
 Author: Data.gov
 Author-email: datagovhelp@gsa.gov
 License: UNKNOWN
 Description: [![Github Actions](https://github.com/GSA/ckanext-geodatagov/actions/workflows/test.yml/badge.svg)](https://github.com/GSA/ckanext-geodatagov/actions)
         [![PyPI version](https://badge.fury.io/py/ckanext-geodatagov.svg)](https://badge.fury.io/py/ckanext-geodatagov)
```

### Comparing `ckanext-geodatagov-0.1.8/ckanext_geodatagov.egg-info/SOURCES.txt` & `ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/ckanext_geodatagov.egg-info/entry_points.txt` & `ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/requirements.txt` & `ckanext-geodatagov-0.1.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.8/setup.py` & `ckanext-geodatagov-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the relevant file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="ckanext-geodatagov",
-    version="0.1.8",
+    version="0.1.9",
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python :: 3'
     ],  # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     keywords='',
```

