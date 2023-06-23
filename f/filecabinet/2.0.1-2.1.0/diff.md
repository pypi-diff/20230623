# Comparing `tmp/filecabinet-2.0.1.tar.gz` & `tmp/filecabinet-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filecabinet-2.0.1.tar", last modified: Sat Jun  3 09:11:58 2023, max compression
+gzip compressed data, was "filecabinet-2.1.0.tar", last modified: Fri Jun 23 11:39:10 2023, max compression
```

## Comparing `filecabinet-2.0.1.tar` & `filecabinet-2.1.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:11:58.613384 filecabinet-2.0.1/
--rw-r--r--   0 robert    (1000) robert    (1000)      461 2023-06-03 09:07:55.000000 filecabinet-2.0.1/CHANGELOG.md
--rw-r--r--   0 robert    (1000) robert    (1000)     1500 2022-02-26 07:52:08.000000 filecabinet-2.0.1/LICENSE
--rw-r--r--   0 robert    (1000) robert    (1000)      113 2023-06-03 09:08:18.000000 filecabinet-2.0.1/MANIFEST.in
--rw-r--r--   0 robert    (1000) robert    (1000)     8249 2023-06-03 09:11:58.613384 filecabinet-2.0.1/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     6252 2023-05-19 11:42:35.000000 filecabinet-2.0.1/README.md
--rw-r--r--   0 robert    (1000) robert    (1000)      754 2023-06-03 09:11:05.000000 filecabinet-2.0.1/example.conf
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:11:58.613384 filecabinet-2.0.1/filecabinet/
--rw-r--r--   0 robert    (1000) robert    (1000)       62 2022-02-26 07:52:09.000000 filecabinet-2.0.1/filecabinet/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)    10047 2023-06-03 08:59:25.000000 filecabinet-2.0.1/filecabinet/cabinet.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3247 2023-05-19 11:33:18.000000 filecabinet-2.0.1/filecabinet/configuration.py
--rw-r--r--   0 robert    (1000) robert    (1000)     9911 2023-05-27 07:35:00.000000 filecabinet-2.0.1/filecabinet/main.py
--rw-r--r--   0 robert    (1000) robert    (1000)     7892 2023-06-03 08:49:18.000000 filecabinet-2.0.1/filecabinet/manager.py
--rw-r--r--   0 robert    (1000) robert    (1000)      313 2022-02-26 07:52:09.000000 filecabinet-2.0.1/filecabinet/meta.py
--rw-r--r--   0 robert    (1000) robert    (1000)     8605 2023-05-19 11:38:06.000000 filecabinet-2.0.1/filecabinet/shell.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4058 2023-05-28 07:40:25.000000 filecabinet-2.0.1/filecabinet/utils.py
--rw-r--r--   0 robert    (1000) robert    (1000)       19 2023-06-03 09:06:34.000000 filecabinet-2.0.1/filecabinet/version.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:11:58.613384 filecabinet-2.0.1/filecabinet.egg-info/
--rw-r--r--   0 robert    (1000) robert    (1000)     8249 2023-06-03 09:11:58.000000 filecabinet-2.0.1/filecabinet.egg-info/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)      522 2023-06-03 09:11:58.000000 filecabinet-2.0.1/filecabinet.egg-info/SOURCES.txt
--rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-06-03 09:11:58.000000 filecabinet-2.0.1/filecabinet.egg-info/dependency_links.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       53 2023-06-03 09:11:58.000000 filecabinet-2.0.1/filecabinet.egg-info/entry_points.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       37 2023-06-03 09:11:58.000000 filecabinet-2.0.1/filecabinet.egg-info/requires.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       12 2023-06-03 09:11:58.000000 filecabinet-2.0.1/filecabinet.egg-info/top_level.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       22 2022-02-26 07:52:09.000000 filecabinet-2.0.1/requirements.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-06-03 09:11:58.613384 filecabinet-2.0.1/setup.cfg
--rw-r--r--   0 robert    (1000) robert    (1000)     1059 2023-06-03 09:05:46.000000 filecabinet-2.0.1/setup.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:11:58.613384 filecabinet-2.0.1/tests/
--rw-r--r--   0 robert    (1000) robert    (1000)     5290 2022-02-26 07:52:09.000000 filecabinet-2.0.1/tests/test_processing.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 11:39:10.660357 filecabinet-2.1.0/
+-rw-r--r--   0 robert    (1000) robert    (1000)      663 2023-06-23 11:34:50.000000 filecabinet-2.1.0/CHANGELOG.md
+-rw-r--r--   0 robert    (1000) robert    (1000)     1500 2023-06-23 11:38:00.000000 filecabinet-2.1.0/LICENSE
+-rw-r--r--   0 robert    (1000) robert    (1000)      113 2023-06-23 10:59:34.000000 filecabinet-2.1.0/MANIFEST.in
+-rw-r--r--   0 robert    (1000) robert    (1000)    10629 2023-06-23 11:39:10.660357 filecabinet-2.1.0/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     8632 2023-06-23 11:37:21.000000 filecabinet-2.1.0/README.md
+-rw-r--r--   0 robert    (1000) robert    (1000)     1016 2023-06-23 11:11:22.000000 filecabinet-2.1.0/example.conf
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 11:39:10.660357 filecabinet-2.1.0/filecabinet/
+-rw-r--r--   0 robert    (1000) robert    (1000)        0 2023-06-23 10:59:34.000000 filecabinet-2.1.0/filecabinet/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    11584 2023-06-23 11:38:09.000000 filecabinet-2.1.0/filecabinet/cabinet.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3247 2023-05-19 11:33:18.000000 filecabinet-2.1.0/filecabinet/configuration.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     9911 2023-05-27 07:35:00.000000 filecabinet-2.1.0/filecabinet/main.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     7971 2023-06-23 10:59:34.000000 filecabinet-2.1.0/filecabinet/manager.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      313 2022-02-26 07:52:09.000000 filecabinet-2.1.0/filecabinet/meta.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     8605 2023-06-23 10:59:34.000000 filecabinet-2.1.0/filecabinet/shell.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4058 2023-06-23 10:59:34.000000 filecabinet-2.1.0/filecabinet/utils.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       19 2023-06-23 11:34:31.000000 filecabinet-2.1.0/filecabinet/version.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 11:39:10.660357 filecabinet-2.1.0/filecabinet.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)    10629 2023-06-23 11:39:10.000000 filecabinet-2.1.0/filecabinet.egg-info/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)      537 2023-06-23 11:39:10.000000 filecabinet-2.1.0/filecabinet.egg-info/SOURCES.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-06-23 11:39:10.000000 filecabinet-2.1.0/filecabinet.egg-info/dependency_links.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       53 2023-06-23 11:39:10.000000 filecabinet-2.1.0/filecabinet.egg-info/entry_points.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       37 2023-06-23 11:39:10.000000 filecabinet-2.1.0/filecabinet.egg-info/requires.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       12 2023-06-23 11:39:10.000000 filecabinet-2.1.0/filecabinet.egg-info/top_level.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       50 2023-06-23 11:01:25.000000 filecabinet-2.1.0/pyproject.toml
+-rw-r--r--   0 robert    (1000) robert    (1000)       22 2022-02-26 07:52:09.000000 filecabinet-2.1.0/requirements.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-06-23 11:39:10.660357 filecabinet-2.1.0/setup.cfg
+-rw-r--r--   0 robert    (1000) robert    (1000)     1059 2023-06-23 11:00:45.000000 filecabinet-2.1.0/setup.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 11:39:10.660357 filecabinet-2.1.0/tests/
+-rw-r--r--   0 robert    (1000) robert    (1000)     5290 2022-02-26 07:52:09.000000 filecabinet-2.1.0/tests/test_processing.py
```

### Comparing `filecabinet-2.0.1/LICENSE` & `filecabinet-2.1.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-Copyright 2019 Robert Labudda All Rights Reserved.
+Copyright 2023 Robert Labudda All Rights Reserved.
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
    * Redistribution of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
    * Redistribution in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
    * Neither the name of Robert Labudda or the names of contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 This software is provided "AS IS," without a warranty of any kind. ALL EXPRESS OR IMPLIED CONDITIONS, REPRESENTATIONS AND WARRANTIES, INCLUDING ANY IMPLIED WARRANTY OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE OR NON-INFRINGEMENT, ARE HEREBY EXCLUDED. ROBERT LABUDDA ("RL") AND ITS LICENSORS SHALL NOT BE LIABLE FOR ANY DAMAGES SUFFERED BY LICENSEE AS A RESULT OF USING, MODIFYING OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES. IN NO EVENT WILL RL OR ITS LICENSORS BE LIABLE FOR ANY LOST REVENUE, PROFIT OR DATA, OR FOR DIRECT, INDIRECT, SPECIAL, CONSEQUENTIAL, INCIDENTAL OR PUNITIVE DAMAGES, HOWEVER CAUSED AND REGARDLESS OF THE THEORY OF LIABILITY, ARISING OUT OF THE USE OF OR INABILITY TO USE THIS SOFTWARE, EVEN IF RL HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
```

### Comparing `filecabinet-2.0.1/PKG-INFO` & `filecabinet-2.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: filecabinet
-Version: 2.0.1
+Version: 2.1.0
 Summary: A local, offline document archive
 Home-page: https://vonshednob.cc/filecabinet
 Author: R
 Author-email: dev+filecabinet-this-is-spam@vonshednob.cc
-License: Copyright 2019 Robert Labudda All Rights Reserved.
+License: Copyright 2023 Robert Labudda All Rights Reserved.
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
            * Redistribution of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
            * Redistribution in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
            * Neither the name of Robert Labudda or the names of contributors may be used to endorse or promote products derived from this software without specific prior written permission.
         This software is provided "AS IS," without a warranty of any kind. ALL EXPRESS OR IMPLIED CONDITIONS, REPRESENTATIONS AND WARRANTIES, INCLUDING ANY IMPLIED WARRANTY OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE OR NON-INFRINGEMENT, ARE HEREBY EXCLUDED. ROBERT LABUDDA ("RL") AND ITS LICENSORS SHALL NOT BE LIABLE FOR ANY DAMAGES SUFFERED BY LICENSEE AS A RESULT OF USING, MODIFYING OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES. IN NO EVENT WILL RL OR ITS LICENSORS BE LIABLE FOR ANY LOST REVENUE, PROFIT OR DATA, OR FOR DIRECT, INDIRECT, SPECIAL, CONSEQUENTIAL, INCIDENTAL OR PUNITIVE DAMAGES, HOWEVER CAUSED AND REGARDLESS OF THE THEORY OF LIABILITY, ARISING OUT OF THE USE OF OR INABILITY TO USE THIS SOFTWARE, EVEN IF RL HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
         
 Classifier: Development Status :: 3 - Alpha
@@ -79,28 +79,46 @@
 ```bash
     filecabinet add ~/some_scanned_document.jpg
 ```
 
 To get a basic overview of documents, you can use the Shell.
 
 
+# Workflow / Use cases
+
+Here’s the usual worflow with filecabinet:
+
+ 1. Put some documents (PDF, scanned documents, etc) into the `inbox`
+    folder of your cabinet
+ 2. Run `filecabinet pickup`
+ 3. List all new documents with `filecabinet list new`
+
+Other use cases are:
+
+ * **Search** for a specific document with `filecabinet find "searchterm" "other search term"`
+ * **Edit** the metadata of a document through the shell `filecabinet shell` (see next section)
+
+
 # Shell
 
 There’s a basic shell that allows you to inspect indexed documents, edit
 their metadata (by means of an external text editor), or view the
 documents.
 
 To open the shell, run
 
 ```bash
     filecabinet shell
 ```
 
 Try `help` inside the shell to see what your options are.
 
+
+## Metadata editing
+
 If you want to use a specific text editor to modify metadata, consider
 updating your configuration file’s `Shell` section and add a
 `document_editor`, like this:
 
 ```ini
     [Shell]
     editor = subl -w
@@ -137,26 +155,76 @@
 
 The title contains "brain", is from author "Gumby" and it was set to some time
 before August 2005: `title:brain author:gumby date:2015-08-01`
 
 Looking for a newly added document with the title "The Larch": `title:larch tag:new`
 
 
+# Grouping of pages
+
+Sometimes you will have a scanned document in form of multiple pages, each
+page a `.jpg` file, like `page1.jpg`, `page2.jpg`, `page3.jpg`.
+
+Of course all these pages form the same document.
+
+To tell filecabinet that these files all belong to the same document, you
+can put them in a folder inside the inbox before running `pickup`:
+
+ * `inbox/doc/page1.jpg`
+ * `inbox/doc/page2.jpg`
+ * `inbox/doc/page3.jpg`
+
+This will tell filecabinet that they all belong to the same
+document.
+
+Here’s also where you can hint to the language of the document
+for OCR (see *Language hinting* in the next section) by calling the folder,
+for example, `doc-nl` to indicate that all pages are written in the dutch
+language.
+
+
 # OCR
 
 filecabinet can use Tesseract OCR to do character recognition on pictures and
 scanned PDFs, so you can search the text of images.
 
 In order for that to work, you have to install Tesseract and some language
 packages, depending on the languages of the documents you wish to scan.
 
 If you don't have Tesseract OCR installed, filecabinet will still work, but
 be much less useful.
 
 
+## Language hinting
+
+You can tell filecabinet what language a document has even as it is in the
+inbox by adding its language as a suffix: hyphen followed by language code
+(ISO-639).
+
+A few examples will help. Consider these files:
+
+ * `page-1.jpg`
+ * `contract.png`
+
+Suppose your default language is set to english (`default-lanugage = eng` in
+the configuration file); `page-1.jpg` is in English but `contract.png` is
+in German.
+
+OCR will likely have difficulties with letters like `öäü` in `contract.png`
+unless you tell it what language the document is in:
+
+ * `contract-ger.png`
+
+`ger` is one of the ISO-639 language codes for German (others are `de` and
+`deu`; see [wikipedia](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for the long listing).
+
+With this `-ger` suffix, filecabinet will use the correct language packet
+(if you have it installed) and the OCR will yield much better results.
+
+
 # Rule based tagging
 
 By using metaindex, filecabinet inherits the powerful rule based
 tagging. This allows you to automatically add metadata tags to documents
 based on their text (which might have come from OCR).
 
 Rules are defined in text files and you have to point filecabinet to the
@@ -215,24 +283,32 @@
  * `<document id>.yaml` contains the metadata
  * `<document id>.<suffix>` is the original document (usually a PDF)
  * `<document id>.txt` is the extracted full text, if it could be extracted
  * `metaindex.conf`, the configuration file for filecabinet's metaindexserver
  * `metaindex.log`, the log file of file cabinet's metaindexserver
 
 
+# Configuration
+
+filecabinet itself as well as each individual cabinet can be configured
+through the user’s configuration file (usually in `~/.config/filecabinet/filecabinet.conf`).
+
+See `example.conf` for all configuration options!
+
+
 # Usage from Python
 
 To use `filecabinet` from Python, you can use this boilerplate:
 
 ```python
-from filecabinet import Manager
+    from filecabinet import Manager
 
 
-manager = Manager()
-manager.launch_server()
+    manager = Manager()
+    manager.launch_server()
 
-session = manager.new_session()
+    session = manager.new_session()
 ```
 
 `session` will be an instance of `Session` which, together with `manager`,
 allows manipulation of metadata and querying of documents.
```

### Comparing `filecabinet-2.0.1/README.md` & `filecabinet-2.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -58,28 +58,46 @@
 ```bash
     filecabinet add ~/some_scanned_document.jpg
 ```
 
 To get a basic overview of documents, you can use the Shell.
 
 
+# Workflow / Use cases
+
+Here’s the usual worflow with filecabinet:
+
+ 1. Put some documents (PDF, scanned documents, etc) into the `inbox`
+    folder of your cabinet
+ 2. Run `filecabinet pickup`
+ 3. List all new documents with `filecabinet list new`
+
+Other use cases are:
+
+ * **Search** for a specific document with `filecabinet find "searchterm" "other search term"`
+ * **Edit** the metadata of a document through the shell `filecabinet shell` (see next section)
+
+
 # Shell
 
 There’s a basic shell that allows you to inspect indexed documents, edit
 their metadata (by means of an external text editor), or view the
 documents.
 
 To open the shell, run
 
 ```bash
     filecabinet shell
 ```
 
 Try `help` inside the shell to see what your options are.
 
+
+## Metadata editing
+
 If you want to use a specific text editor to modify metadata, consider
 updating your configuration file’s `Shell` section and add a
 `document_editor`, like this:
 
 ```ini
     [Shell]
     editor = subl -w
@@ -116,26 +134,76 @@
 
 The title contains "brain", is from author "Gumby" and it was set to some time
 before August 2005: `title:brain author:gumby date:2015-08-01`
 
 Looking for a newly added document with the title "The Larch": `title:larch tag:new`
 
 
+# Grouping of pages
+
+Sometimes you will have a scanned document in form of multiple pages, each
+page a `.jpg` file, like `page1.jpg`, `page2.jpg`, `page3.jpg`.
+
+Of course all these pages form the same document.
+
+To tell filecabinet that these files all belong to the same document, you
+can put them in a folder inside the inbox before running `pickup`:
+
+ * `inbox/doc/page1.jpg`
+ * `inbox/doc/page2.jpg`
+ * `inbox/doc/page3.jpg`
+
+This will tell filecabinet that they all belong to the same
+document.
+
+Here’s also where you can hint to the language of the document
+for OCR (see *Language hinting* in the next section) by calling the folder,
+for example, `doc-nl` to indicate that all pages are written in the dutch
+language.
+
+
 # OCR
 
 filecabinet can use Tesseract OCR to do character recognition on pictures and
 scanned PDFs, so you can search the text of images.
 
 In order for that to work, you have to install Tesseract and some language
 packages, depending on the languages of the documents you wish to scan.
 
 If you don't have Tesseract OCR installed, filecabinet will still work, but
 be much less useful.
 
 
+## Language hinting
+
+You can tell filecabinet what language a document has even as it is in the
+inbox by adding its language as a suffix: hyphen followed by language code
+(ISO-639).
+
+A few examples will help. Consider these files:
+
+ * `page-1.jpg`
+ * `contract.png`
+
+Suppose your default language is set to english (`default-lanugage = eng` in
+the configuration file); `page-1.jpg` is in English but `contract.png` is
+in German.
+
+OCR will likely have difficulties with letters like `öäü` in `contract.png`
+unless you tell it what language the document is in:
+
+ * `contract-ger.png`
+
+`ger` is one of the ISO-639 language codes for German (others are `de` and
+`deu`; see [wikipedia](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for the long listing).
+
+With this `-ger` suffix, filecabinet will use the correct language packet
+(if you have it installed) and the OCR will yield much better results.
+
+
 # Rule based tagging
 
 By using metaindex, filecabinet inherits the powerful rule based
 tagging. This allows you to automatically add metadata tags to documents
 based on their text (which might have come from OCR).
 
 Rules are defined in text files and you have to point filecabinet to the
@@ -194,24 +262,32 @@
  * `<document id>.yaml` contains the metadata
  * `<document id>.<suffix>` is the original document (usually a PDF)
  * `<document id>.txt` is the extracted full text, if it could be extracted
  * `metaindex.conf`, the configuration file for filecabinet's metaindexserver
  * `metaindex.log`, the log file of file cabinet's metaindexserver
 
 
+# Configuration
+
+filecabinet itself as well as each individual cabinet can be configured
+through the user’s configuration file (usually in `~/.config/filecabinet/filecabinet.conf`).
+
+See `example.conf` for all configuration options!
+
+
 # Usage from Python
 
 To use `filecabinet` from Python, you can use this boilerplate:
 
 ```python
-from filecabinet import Manager
+    from filecabinet import Manager
 
 
-manager = Manager()
-manager.launch_server()
+    manager = Manager()
+    manager.launch_server()
 
-session = manager.new_session()
+    session = manager.new_session()
 ```
 
 `session` will be an instance of `Session` which, together with `manager`,
 allows manipulation of metadata and querying of documents.
```

### Comparing `filecabinet-2.0.1/example.conf` & `filecabinet-2.1.0/example.conf`

 * *Files 23% similar despite different names*

```diff
@@ -5,26 +5,37 @@
 
 ## The path to the cache database
 ## You shouldn’t have to change this from its default:
 # database = ~/.cache/filecabinet
 
 [Shell]
 ## What program to use when attempting to open files from the shell
-# document_opener = rifle
+## Defaults to:
+# document_opener = xdg-open
+
+## What program to use when editing metadata YAML files
+## Will fall back to environment variables VISUAL and EDITOR if not set
+# editor =
 
 [OCR]
 ## Whether or not to try and run tesseract to extract text from images
+## Defaults to:
 # enabled = yes
 
 ## The default language if there is not hint from the filename.
 ## Make sure you have at least this language packet installed.
+## Defaults to:
 # default-language = eng
 
 ## Any other section is considered one of your file cabinets
 ## Like this:
 
 # [cabinet1]
 ## A more convenient name
 # name = My file cabinet
 
 ## The folder where the cabinet is stored.
 # path = ~/Documents/cabinet
+
+## Keep the original document's name
+## Defaults to:
+# keep-name = no
```

### Comparing `filecabinet-2.0.1/filecabinet/cabinet.py` & `filecabinet-2.1.0/filecabinet/cabinet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Package for Cabinet and related classes"""
 import logging
 import shutil
 import subprocess
 import mimetypes
 import tempfile
+import hashlib
 from pathlib import Path
 
 from pypdf import PdfWriter
 
 import metaindex.shared
 from metaindex import yaml
 from metaindex import indexers
@@ -37,14 +38,15 @@
 
 
 class Document(CacheEntry):
     """Representing a document in a filecabinet"""
     def __init__(self, *args, cabinet=None, **kwargs):
         super().__init__(*args, **kwargs)
         self.cabinet = cabinet
+        self._sha256 = None
 
     @classmethod
     def wrap(cls, cabinet, entry):
         """Create a new Document based on ``entry``
         """
         if isinstance(entry, Document):
             entry.cabinet = cabinet
@@ -54,30 +56,55 @@
         that.metadata = entry.metadata
         that.last_modified = entry.last_modified
         that.mimetype = entry.mimetype
         that.rel_path = entry.rel_path
         that.storage_label = entry.storage_label
         return that
 
+    def sha256(self):
+        shafile = self.path.parent / (self.path.stem + '.sha256')
+
+        if 'sha256' in self:
+            self._sha256 = self.get('sha256')[0]
+            self.delete('sha256')
+
+        elif shafile.is_file():
+            self._sha256 = shafile.read_text(encoding='ascii').strip()
+
+        if self._sha256 is None or not shafile.is_file():
+            # ensure the sha256 file is in place
+            if self._sha256 is None:
+                self.create_checksum()
+            assert self._sha256 is not None
+            shafile.write_text(self._sha256, encoding='ascii')
+
+        return self._sha256
+
+    def create_checksum(self):
+        self._sha256 = hashlib.sha256(self.path.read_bytes()).hexdigest()
+        return self._sha256
+
     def copy(self):
         that = super().copy()
         that.cabinet = self.cabinet
+        that._sha256 = self._sha256
         return that
 
     def is_new(self):
         return any(v == 'new' for v in self.get('extra.tag'))
 
 
 class Cabinet:
     """Represents a filecabinet as a container of documents"""
     def __init__(self, name, manager):
         self.manager = manager
         self.config = manager.config
         self.name = name
         self.description = self.config[name].get('description', name)
+        self.keep_name = self.config.bool(name, 'keep-name', 'no')
         self.basedir = self.config.path(name, 'path')
         self.inbox = self.basedir / self.config[name].get('inbox', 'inbox')
         self.documents = self.basedir / self.config[name].get('documents', 'documents')
 
         self.documents.mkdir(exist_ok=True, parents=True)
         self.inbox.mkdir(exist_ok=True, parents=True)
 
@@ -133,26 +160,39 @@
 
         for result in generator:
             if not result.success:
                 logging.warning(f"Unknown file: {result.filename}")
                 continue
 
             result.info.last_modified = metaindex.shared.get_last_modified(result.filename)
-            info = result.info
+            info = Document.wrap(self, result.info)
+
+            # verify that the document doesn't exist yet
+            checksum = info.create_checksum()
+            duplicates = session.find('sha256:'+checksum)
+            if len(duplicates) > 0:
+                logging.info(f"{info.path} has already been added as {duplicates[0].path}")
+                continue
 
             # new document ID
             prefix, docid = self.next_doc_id()
+            basename = docid
+            if self.keep_name:
+                basename = result.filename.stem
             docdir = self.documents / prefix / docid
             docdir.mkdir(parents=True)
-            docpath = docdir / (docid + info.path.suffix)
+            docpath = docdir / (basename + info.path.suffix)
 
             # move to new location
             shutil.move(result.filename, docpath)
             info.path = docpath
 
+            # create checksum sidecar
+            info.add('sha256', info.sha256())
+
             # mark as 'new'
             info.add('extra.tag', 'new')
 
             # index metadata in cache
             session.cache.reduce(info)
             session.cache.insert(info)
 
@@ -160,28 +200,27 @@
             fulltext = ("\n".join([str(v) for v in info.get('extra.fulltext')])).strip()
 
             # create the sidecar file
             self.save_metadata(info)
 
             # write out full text, if there was any
             if len(fulltext) > 0:
-                text = docdir / (docid + ".txt")
+                text = docdir / (basename + ".txt")
                 text.write_text(fulltext, encoding='utf-8')
 
     def save_metadata(self, document):
         """Save the metadata of 'document' to its respective sidecar file"""
         docdir = document.path.parent
-        docid = document.path.stem
-        assert docdir.stem == docid
+        basename = document.path.stem
 
         to_save = document.copy()
         to_save.delete('extra.fulltext')
 
         # create sidecar file
-        sidecar = docdir / (docid + ".yaml")
+        sidecar = docdir / (basename + ".yaml")
         yaml.store(to_save, sidecar)
 
     def merge_files(self, dirpath):
         """Try and merge all files in ``dirpath`` into one PDF at ``dirpath/../dirpath.pdf``
 
         Returns the full path to the merged file on success, otherwise ``None``
         """
@@ -248,15 +287,17 @@
 
     def files(self):
         """Iterate over all document files in this cabinet"""
         paths = sum([list(d.iterdir())
                      for d in self.documents.iterdir()], start=[])
 
         for path in paths:
-            candidates = [fn for fn in path.iterdir() if fn.suffix != '.yaml']
+            candidates = [fn
+                          for fn in path.iterdir()
+                          if fn.suffix not in ['.yaml', '.sha256']]
             if len(candidates) == 0:
                 logging.info(f"Abandoned folder {path}")
                 continue
             if len(candidates) == 1:
                 yield candidates[0]
                 continue
             candidates = [c for c in candidates if c.suffix != '.txt']
@@ -277,21 +318,22 @@
         files = [fn for fn in files
                  if fn.is_relative_to(self.documents)]
 
         for filepath in files:
             sidecar = filepath.parent / (filepath.stem + '.yaml')
             fulltext = filepath.parent / (filepath.stem + '.txt')
 
-            entry = yaml.get(sidecar)
-            entry.path = filepath
+            doc = Document.wrap(self, yaml.get(sidecar))
+            doc.path = filepath
+            doc.add('sha256', doc.sha256())
 
             if fulltext.is_file():
-                entry.add('extra.fulltext', fulltext.read_text(encoding='utf-8'))
+                doc.add('extra.fulltext', fulltext.read_text(encoding='utf-8'))
 
-            session.cache.insert(entry)
+            session.cache.insert(doc)
 
     def update(self, session, documents):
         """Update the metadata information of these documents"""
         for document in documents:
             if not document.path.is_relative_to(self.documents):
                 continue
             self.save_metadata(document)
```

### Comparing `filecabinet-2.0.1/filecabinet/configuration.py` & `filecabinet-2.1.0/filecabinet/configuration.py`

 * *Files identical despite different names*

### Comparing `filecabinet-2.0.1/filecabinet/main.py` & `filecabinet-2.1.0/filecabinet/main.py`

 * *Files identical despite different names*

### Comparing `filecabinet-2.0.1/filecabinet/manager.py` & `filecabinet-2.1.0/filecabinet/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 fulltext = pdf.fulltext, extra.fulltext
 issuer = extra.issuer
 creator = extra.creator
 subject = extra.subject
 tag = extra.tag, extra.tags, rules.tag, rules.tags
 language = extra.language, rules.language
 date = extra.date, rules.date
+checksum = sha256
 
 [Server]
 loglevel = warning
 logfile = {logfile}
 index-new-tags = yes
 '''
 
@@ -52,15 +53,17 @@
         self.manager = manager
 
     def reduce(self, entry):
         for key in set(entry.metadata.keys()):
             values = entry.metadata[key]
             skey = None
 
-            if key in self.config.synonymized and any(len(str(v.raw_value)) > 0 for v in values):
+            if key == 'sha256':
+                skey = key
+            elif key in self.config.synonymized and any(len(str(v.raw_value)) > 0 for v in values):
                 skey = 'extra.' + self.config.synonymized[key]
             elif key.startswith('extra.'):
                 skey = key.lower()
             elif key.startswith('rules.') and len(key.strip()) > 6:
                 skey = 'extra.' + key.strip()[6:]
 
             if skey is not None:
```

### Comparing `filecabinet-2.0.1/filecabinet/shell.py` & `filecabinet-2.1.0/filecabinet/shell.py`

 * *Files identical despite different names*

### Comparing `filecabinet-2.0.1/filecabinet/utils.py` & `filecabinet-2.1.0/filecabinet/utils.py`

 * *Files identical despite different names*

### Comparing `filecabinet-2.0.1/filecabinet.egg-info/PKG-INFO` & `filecabinet-2.1.0/filecabinet.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: filecabinet
-Version: 2.0.1
+Version: 2.1.0
 Summary: A local, offline document archive
 Home-page: https://vonshednob.cc/filecabinet
 Author: R
 Author-email: dev+filecabinet-this-is-spam@vonshednob.cc
-License: Copyright 2019 Robert Labudda All Rights Reserved.
+License: Copyright 2023 Robert Labudda All Rights Reserved.
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
            * Redistribution of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
            * Redistribution in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
            * Neither the name of Robert Labudda or the names of contributors may be used to endorse or promote products derived from this software without specific prior written permission.
         This software is provided "AS IS," without a warranty of any kind. ALL EXPRESS OR IMPLIED CONDITIONS, REPRESENTATIONS AND WARRANTIES, INCLUDING ANY IMPLIED WARRANTY OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE OR NON-INFRINGEMENT, ARE HEREBY EXCLUDED. ROBERT LABUDDA ("RL") AND ITS LICENSORS SHALL NOT BE LIABLE FOR ANY DAMAGES SUFFERED BY LICENSEE AS A RESULT OF USING, MODIFYING OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES. IN NO EVENT WILL RL OR ITS LICENSORS BE LIABLE FOR ANY LOST REVENUE, PROFIT OR DATA, OR FOR DIRECT, INDIRECT, SPECIAL, CONSEQUENTIAL, INCIDENTAL OR PUNITIVE DAMAGES, HOWEVER CAUSED AND REGARDLESS OF THE THEORY OF LIABILITY, ARISING OUT OF THE USE OF OR INABILITY TO USE THIS SOFTWARE, EVEN IF RL HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
         
 Classifier: Development Status :: 3 - Alpha
@@ -79,28 +79,46 @@
 ```bash
     filecabinet add ~/some_scanned_document.jpg
 ```
 
 To get a basic overview of documents, you can use the Shell.
 
 
+# Workflow / Use cases
+
+Here’s the usual worflow with filecabinet:
+
+ 1. Put some documents (PDF, scanned documents, etc) into the `inbox`
+    folder of your cabinet
+ 2. Run `filecabinet pickup`
+ 3. List all new documents with `filecabinet list new`
+
+Other use cases are:
+
+ * **Search** for a specific document with `filecabinet find "searchterm" "other search term"`
+ * **Edit** the metadata of a document through the shell `filecabinet shell` (see next section)
+
+
 # Shell
 
 There’s a basic shell that allows you to inspect indexed documents, edit
 their metadata (by means of an external text editor), or view the
 documents.
 
 To open the shell, run
 
 ```bash
     filecabinet shell
 ```
 
 Try `help` inside the shell to see what your options are.
 
+
+## Metadata editing
+
 If you want to use a specific text editor to modify metadata, consider
 updating your configuration file’s `Shell` section and add a
 `document_editor`, like this:
 
 ```ini
     [Shell]
     editor = subl -w
@@ -137,26 +155,76 @@
 
 The title contains "brain", is from author "Gumby" and it was set to some time
 before August 2005: `title:brain author:gumby date:2015-08-01`
 
 Looking for a newly added document with the title "The Larch": `title:larch tag:new`
 
 
+# Grouping of pages
+
+Sometimes you will have a scanned document in form of multiple pages, each
+page a `.jpg` file, like `page1.jpg`, `page2.jpg`, `page3.jpg`.
+
+Of course all these pages form the same document.
+
+To tell filecabinet that these files all belong to the same document, you
+can put them in a folder inside the inbox before running `pickup`:
+
+ * `inbox/doc/page1.jpg`
+ * `inbox/doc/page2.jpg`
+ * `inbox/doc/page3.jpg`
+
+This will tell filecabinet that they all belong to the same
+document.
+
+Here’s also where you can hint to the language of the document
+for OCR (see *Language hinting* in the next section) by calling the folder,
+for example, `doc-nl` to indicate that all pages are written in the dutch
+language.
+
+
 # OCR
 
 filecabinet can use Tesseract OCR to do character recognition on pictures and
 scanned PDFs, so you can search the text of images.
 
 In order for that to work, you have to install Tesseract and some language
 packages, depending on the languages of the documents you wish to scan.
 
 If you don't have Tesseract OCR installed, filecabinet will still work, but
 be much less useful.
 
 
+## Language hinting
+
+You can tell filecabinet what language a document has even as it is in the
+inbox by adding its language as a suffix: hyphen followed by language code
+(ISO-639).
+
+A few examples will help. Consider these files:
+
+ * `page-1.jpg`
+ * `contract.png`
+
+Suppose your default language is set to english (`default-lanugage = eng` in
+the configuration file); `page-1.jpg` is in English but `contract.png` is
+in German.
+
+OCR will likely have difficulties with letters like `öäü` in `contract.png`
+unless you tell it what language the document is in:
+
+ * `contract-ger.png`
+
+`ger` is one of the ISO-639 language codes for German (others are `de` and
+`deu`; see [wikipedia](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for the long listing).
+
+With this `-ger` suffix, filecabinet will use the correct language packet
+(if you have it installed) and the OCR will yield much better results.
+
+
 # Rule based tagging
 
 By using metaindex, filecabinet inherits the powerful rule based
 tagging. This allows you to automatically add metadata tags to documents
 based on their text (which might have come from OCR).
 
 Rules are defined in text files and you have to point filecabinet to the
@@ -215,24 +283,32 @@
  * `<document id>.yaml` contains the metadata
  * `<document id>.<suffix>` is the original document (usually a PDF)
  * `<document id>.txt` is the extracted full text, if it could be extracted
  * `metaindex.conf`, the configuration file for filecabinet's metaindexserver
  * `metaindex.log`, the log file of file cabinet's metaindexserver
 
 
+# Configuration
+
+filecabinet itself as well as each individual cabinet can be configured
+through the user’s configuration file (usually in `~/.config/filecabinet/filecabinet.conf`).
+
+See `example.conf` for all configuration options!
+
+
 # Usage from Python
 
 To use `filecabinet` from Python, you can use this boilerplate:
 
 ```python
-from filecabinet import Manager
+    from filecabinet import Manager
 
 
-manager = Manager()
-manager.launch_server()
+    manager = Manager()
+    manager.launch_server()
 
-session = manager.new_session()
+    session = manager.new_session()
 ```
 
 `session` will be an instance of `Session` which, together with `manager`,
 allows manipulation of metadata and querying of documents.
```

### Comparing `filecabinet-2.0.1/filecabinet.egg-info/SOURCES.txt` & `filecabinet-2.1.0/filecabinet.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 example.conf
+pyproject.toml
 requirements.txt
 setup.py
 filecabinet/__init__.py
 filecabinet/cabinet.py
 filecabinet/configuration.py
 filecabinet/main.py
 filecabinet/manager.py
```

### Comparing `filecabinet-2.0.1/setup.py` & `filecabinet-2.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,13 +20,13 @@
       author_email="dev+filecabinet-this-is-spam@vonshednob.cc",
       license=licensetext,
       entry_points={'console_scripts': ['filecabinet=filecabinet.main:run']},
       packages=['filecabinet',
                 ],
       package_data={},
       data_files=[],
-      install_requires=['pyyaml', 'pypdf', 'Pillow', 'metaindex >= 2.2.2'],
+      install_requires=['pyyaml', 'pypdf', 'Pillow', 'metaindex >= 2.3.0'],
       python_requires='>=3.7',
       classifiers=['Development Status :: 3 - Alpha',
                    'License :: OSI Approved :: BSD License',
                    'Programming Language :: Python :: 3',
                    ])
```

### Comparing `filecabinet-2.0.1/tests/test_processing.py` & `filecabinet-2.1.0/tests/test_processing.py`

 * *Files identical despite different names*

