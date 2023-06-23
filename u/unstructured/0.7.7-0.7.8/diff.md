# Comparing `tmp/unstructured-0.7.7.tar.gz` & `tmp/unstructured-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.7.7.tar", last modified: Tue Jun 20 19:15:00 2023, max compression
+gzip compressed data, was "unstructured-0.7.8.tar", last modified: Fri Jun 23 02:24:47 2023, max compression
```

## Comparing `unstructured-0.7.7.tar` & `unstructured-0.7.8.tar`

### file list

```diff
@@ -1,131 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.988214 unstructured-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-20 19:14:47.000000 unstructured-0.7.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-20 19:14:47.000000 unstructured-0.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18269 2023-06-20 19:15:00.988214 unstructured-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-06-20 19:14:47.000000 unstructured-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.960214 unstructured-0.7.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-20 19:14:47.000000 unstructured-0.7.7/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 19:14:47.000000 unstructured-0.7.7/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 19:14:47.000000 unstructured-0.7.7/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 19:14:47.000000 unstructured-0.7.7/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-20 19:14:47.000000 unstructured-0.7.7/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 19:14:47.000000 unstructured-0.7.7/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 19:14:47.000000 unstructured-0.7.7/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 19:14:47.000000 unstructured-0.7.7/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 19:14:47.000000 unstructured-0.7.7/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 19:14:47.000000 unstructured-0.7.7/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 19:14:47.000000 unstructured-0.7.7/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 19:14:47.000000 unstructured-0.7.7/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-20 19:15:00.988214 unstructured-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-20 19:14:47.000000 unstructured-0.7.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.960214 unstructured-0.7.7/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:14:47.000000 unstructured-0.7.7/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.964214 unstructured-0.7.7/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:14:47.000000 unstructured-0.7.7/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-20 19:14:47.000000 unstructured-0.7.7/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-20 19:14:47.000000 unstructured-0.7.7/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-20 19:14:47.000000 unstructured-0.7.7/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-20 19:14:47.000000 unstructured-0.7.7/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.964214 unstructured-0.7.7/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.968214 unstructured-0.7.7/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.972214 unstructured-0.7.7/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/documents/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.972214 unstructured-0.7.7/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    16722 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.972214 unstructured-0.7.7/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.976214 unstructured-0.7.7/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.976214 unstructured-0.7.7/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25155 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.976214 unstructured-0.7.7/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.984214 unstructured-0.7.7/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.988214 unstructured-0.7.7/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13432 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.988214 unstructured-0.7.7/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-20 19:14:47.000000 unstructured-0.7.7/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:15:00.964214 unstructured-0.7.7/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18269 2023-06-20 19:15:00.000000 unstructured-0.7.7/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-20 19:15:00.000000 unstructured-0.7.7/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:15:00.000000 unstructured-0.7.7/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 19:15:00.000000 unstructured-0.7.7/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-20 19:15:00.000000 unstructured-0.7.7/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 19:15:00.000000 unstructured-0.7.7/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.132688 unstructured-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-23 02:24:36.000000 unstructured-0.7.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-23 02:24:36.000000 unstructured-0.7.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-06-23 02:24:47.132688 unstructured-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-06-23 02:24:36.000000 unstructured-0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.120688 unstructured-0.7.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-gcs.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 02:24:36.000000 unstructured-0.7.8/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-23 02:24:47.132688 unstructured-0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-23 02:24:36.000000 unstructured-0.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.120688 unstructured-0.7.8/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.120688 unstructured-0.7.8/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-23 02:24:37.000000 unstructured-0.7.8/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-23 02:24:37.000000 unstructured-0.7.8/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-23 02:24:37.000000 unstructured-0.7.8/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-23 02:24:37.000000 unstructured-0.7.8/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.120688 unstructured-0.7.8/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/documents/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16722 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25924 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.132688 unstructured-0.7.8/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.132688 unstructured-0.7.8/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14138 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.132688 unstructured-0.7.8/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-23 02:24:37.000000 unstructured-0.7.8/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:24:47.124688 unstructured-0.7.8/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-06-23 02:24:46.000000 unstructured-0.7.8/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-23 02:24:47.000000 unstructured-0.7.8/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 02:24:46.000000 unstructured-0.7.8/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 02:24:46.000000 unstructured-0.7.8/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-23 02:24:46.000000 unstructured-0.7.8/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 02:24:46.000000 unstructured-0.7.8/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.7.7/LICENSE.md` & `unstructured-0.7.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/PKG-INFO` & `unstructured-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.7
+Version: 0.7.8
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -78,15 +78,15 @@
           use the instructions [here](https://github.com/Unstructured-IO/unstructured-inference#detectron2).
         
         At this point, you should be able to run the following code:
         
         ```python
         from unstructured.partition.auto import partition
         
-        elements = partition(filename="example-docs/fake-email.eml")
+        elements = partition(filename="example-docs/eml/fake-email.eml")
         print("\n\n".join([str(el) for el in elements]))
         ```
         
         The following table shows the document types the `unstructured` library currently supports.
         `partition` will recognize each of these document types and route the document to the
         appropriate partitioning function. If you already know your document type, you can use
         the partitioning function listed in the table directly.
@@ -299,7 +299,8 @@
 Provides-Extra: discord
 Provides-Extra: github
 Provides-Extra: gitlab
 Provides-Extra: reddit
 Provides-Extra: slack
 Provides-Extra: wikipedia
 Provides-Extra: google-drive
+Provides-Extra: gcs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.7 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.8 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -44,31 +44,31 @@
 and PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs)
 - If you are parsing PDFs and want to use a model from the [layoutparser model
 zoo](https://github.com/Unstructured-IO/unstructured-inference#using-models-
 from-the-layoutparser-model-zoo), use the instructions [here](https://
 github.com/Unstructured-IO/unstructured-inference#detectron2). At this point,
 you should be able to run the following code: ```python from
 unstructured.partition.auto import partition elements = partition
-(filename="example-docs/fake-email.eml") print("\n\n".join([str(el) for el in
-elements])) ``` The following table shows the document types the `unstructured`
-library currently supports. `partition` will recognize each of these document
-types and route the document to the appropriate partitioning function. If you
-already know your document type, you can use the partitioning function listed
-in the table directly. See our [documentation page](https://unstructured-
-io.github.io/unstructured/) for more details about the library. | Document Type
-| Partition Function | Strategies | Table Support | Options | | --- | --- | --
-- | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None | |
-E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails (`.msg`) |
-`partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) | `partition_epub` |
-N/A | Yes | Include Page Breaks | | Excel Documents (`.xlsx`/`.xls`) |
-`partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`) | `partition_html`
-| N/A | No | Encoding; Include Page Breaks | | Images (`.png`/`.jpg`) |
-`partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding;
-Include Page Breaks; Infer Table Structure; OCR Languages, Strategy | |
-Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Open
+(filename="example-docs/eml/fake-email.eml") print("\n\n".join([str(el) for el
+in elements])) ``` The following table shows the document types the
+`unstructured` library currently supports. `partition` will recognize each of
+these document types and route the document to the appropriate partitioning
+function. If you already know your document type, you can use the partitioning
+function listed in the table directly. See our [documentation page](https://
+unstructured-io.github.io/unstructured/) for more details about the library. |
+Document Type | Partition Function | Strategies | Table Support | Options | | -
+-- | --- | --- | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes
+| None | | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails
+(`.msg`) | `partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) |
+`partition_epub` | N/A | Yes | Include Page Breaks | | Excel Documents
+(`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`)
+| `partition_html` | N/A | No | Encoding; Include Page Breaks | | Images
+(`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes
+| Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
+| | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
 Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
 Breaks | | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include
@@ -197,7 +197,8 @@
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown Provides-Extra: huggingface Provides-
 Extra: local-inference Provides-Extra: s3 Provides-Extra: azure Provides-Extra:
 discord Provides-Extra: github Provides-Extra: gitlab Provides-Extra: reddit
 Provides-Extra: slack Provides-Extra: wikipedia Provides-Extra: google-drive
+Provides-Extra: gcs
```

### Comparing `unstructured-0.7.7/README.md` & `unstructured-0.7.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
   use the instructions [here](https://github.com/Unstructured-IO/unstructured-inference#detectron2).
 
 At this point, you should be able to run the following code:
 
 ```python
 from unstructured.partition.auto import partition
 
-elements = partition(filename="example-docs/fake-email.eml")
+elements = partition(filename="example-docs/eml/fake-email.eml")
 print("\n\n".join([str(el) for el in elements]))
 ```
 
 The following table shows the document types the `unstructured` library currently supports.
 `partition` will recognize each of these document types and route the document to the
 appropriate partitioning function. If you already know your document type, you can use
 the partitioning function listed in the table directly.
```

#### html2text {}

```diff
@@ -40,31 +40,31 @@
 and PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs)
 - If you are parsing PDFs and want to use a model from the [layoutparser model
 zoo](https://github.com/Unstructured-IO/unstructured-inference#using-models-
 from-the-layoutparser-model-zoo), use the instructions [here](https://
 github.com/Unstructured-IO/unstructured-inference#detectron2). At this point,
 you should be able to run the following code: ```python from
 unstructured.partition.auto import partition elements = partition
-(filename="example-docs/fake-email.eml") print("\n\n".join([str(el) for el in
-elements])) ``` The following table shows the document types the `unstructured`
-library currently supports. `partition` will recognize each of these document
-types and route the document to the appropriate partitioning function. If you
-already know your document type, you can use the partitioning function listed
-in the table directly. See our [documentation page](https://unstructured-
-io.github.io/unstructured/) for more details about the library. | Document Type
-| Partition Function | Strategies | Table Support | Options | | --- | --- | --
-- | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None | |
-E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails (`.msg`) |
-`partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) | `partition_epub` |
-N/A | Yes | Include Page Breaks | | Excel Documents (`.xlsx`/`.xls`) |
-`partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`) | `partition_html`
-| N/A | No | Encoding; Include Page Breaks | | Images (`.png`/`.jpg`) |
-`partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding;
-Include Page Breaks; Infer Table Structure; OCR Languages, Strategy | |
-Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Open
+(filename="example-docs/eml/fake-email.eml") print("\n\n".join([str(el) for el
+in elements])) ``` The following table shows the document types the
+`unstructured` library currently supports. `partition` will recognize each of
+these document types and route the document to the appropriate partitioning
+function. If you already know your document type, you can use the partitioning
+function listed in the table directly. See our [documentation page](https://
+unstructured-io.github.io/unstructured/) for more details about the library. |
+Document Type | Partition Function | Strategies | Table Support | Options | | -
+-- | --- | --- | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes
+| None | | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails
+(`.msg`) | `partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) |
+`partition_epub` | N/A | Yes | Include Page Breaks | | Excel Documents
+(`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`)
+| `partition_html` | N/A | No | Encoding; Include Page Breaks | | Images
+(`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes
+| Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
+| | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
 Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
 Breaks | | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include
```

### Comparing `unstructured-0.7.7/setup.py` & `unstructured-0.7.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,11 +77,12 @@
         "discord": load_requirements("requirements/ingest-discord.in"),
         "github": load_requirements("requirements/ingest-github.in"),
         "gitlab": load_requirements("requirements/ingest-gitlab.in"),
         "reddit": load_requirements("requirements/ingest-reddit.in"),
         "slack": load_requirements("requirements/ingest-slack.in"),
         "wikipedia": load_requirements("requirements/ingest-wikipedia.in"),
         "google-drive": load_requirements("requirements/ingest-google-drive.in"),
+        "gcs": load_requirements("requirements/ingest-gcs.in"),
     },
     package_dir={"unstructured": "unstructured"},
     package_data={"unstructured": ["nlp/*.txt"]},
 )
```

### Comparing `unstructured-0.7.7/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.7.8/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.7.8/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/test_unstructured/test_utils.py` & `unstructured-0.7.8/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/cleaners/core.py` & `unstructured-0.7.8/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/cleaners/extract.py` & `unstructured-0.7.8/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/cleaners/translate.py` & `unstructured-0.7.8/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/documents/base.py` & `unstructured-0.7.8/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/documents/coordinates.py` & `unstructured-0.7.8/unstructured/documents/coordinates.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/documents/elements.py` & `unstructured-0.7.8/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/documents/email_elements.py` & `unstructured-0.7.8/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/documents/html.py` & `unstructured-0.7.8/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/documents/xml.py` & `unstructured-0.7.8/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/file_utils/encoding.py` & `unstructured-0.7.8/unstructured/file_utils/encoding.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import IO, Optional, Tuple, Union
 
 import chardet
 
+from unstructured.partition.common import convert_to_bytes
+
 ENCODE_REC_THRESHOLD = 0.5
 
 # popular encodings from https://en.wikipedia.org/wiki/Popularity_of_text_encodings
 COMMON_ENCODINGS = [
     "utf_8",
     "iso_8859_1",
     "ascii",
@@ -42,22 +44,15 @@
     filename: str = "",
     file: Optional[Union[bytes, IO]] = None,
 ) -> Tuple[str, str]:
     if filename:
         with open(filename, "rb") as f:
             byte_data = f.read()
     elif file:
-        if isinstance(file, bytes):
-            byte_data = file
-        else:
-            if not hasattr(file, "mode") or "b" in file.mode:
-                byte_data = file.read()
-            else:
-                with open(file.name, "rb") as f:
-                    byte_data = f.read()
+        byte_data = convert_to_bytes(file)
     else:
         raise FileNotFoundError("No filename nor file were specified")
 
     result = chardet.detect(byte_data)
     encoding = result["encoding"]
     confidence = result["confidence"]
```

### Comparing `unstructured-0.7.7/unstructured/file_utils/exploration.py` & `unstructured-0.7.8/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/file_utils/file_conversion.py` & `unstructured-0.7.8/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/file_utils/filetype.py` & `unstructured-0.7.8/unstructured/file_utils/filetype.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/file_utils/metadata.py` & `unstructured-0.7.8/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/ingest/connector/azure.py` & `unstructured-0.7.8/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/ingest/connector/biomed.py` & `unstructured-0.7.8/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/ingest/connector/discord.py` & `unstructured-0.7.8/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/ingest/connector/fsspec.py` & `unstructured-0.7.8/unstructured/ingest/connector/fsspec.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,23 +11,27 @@
     BaseIngestDoc,
     StandardConnectorConfig,
 )
 from unstructured.ingest.logger import logger
 
 SUPPORTED_REMOTE_FSSPEC_PROTOCOLS = [
     "s3",
+    "s3a",
     "abfs",
     "az",
+    "gs",
+    "gcs",
 ]
 
 
 @dataclass
 class SimpleFsspecConfig(BaseConnectorConfig):
     # fsspec specific options
     path: str
+    recursive: bool
     access_kwargs: dict = field(default_factory=dict)
     protocol: str = field(init=False)
     path_without_protocol: str = field(init=False)
     dir_path: str = field(init=False)
     file_path: str = field(init=False)
 
     def __post_init__(self):
@@ -77,15 +81,17 @@
         return (
             Path(self.standard_config.output_dir)
             / f"{self.remote_file_path.replace(f'{self.config.dir_path}/', '')}.json"
         )
 
     def has_output(self):
         """Determine if structured output for this doc already exists."""
-        return self._output_filename().is_file() and os.path.getsize(self._output_filename())
+        return self._output_filename().is_file() and os.path.getsize(
+            self._output_filename(),
+        )
 
     def _create_full_tmp_dir_path(self):
         """Includes "directories" in the object path"""
         self._tmp_download_file().parent.mkdir(parents=True, exist_ok=True)
 
     def get_file(self):
         """Fetches the file from the current filesystem and stores it locally."""
@@ -110,27 +116,32 @@
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
         if self.standard_config.download_only:
             return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w") as output_f:
-            output_f.write(json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2))
+            output_f.write(
+                json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2),
+            )
         logger.info(f"Wrote {output_filename}")
 
     @property
     def filename(self):
-        """The filename of the file after downloading from s3"""
+        """The filename of the file after downloading from cloud"""
         return self._tmp_download_file()
 
     def cleanup_file(self):
         """Removes the local copy of the file after successful processing."""
         if not self.standard_config.preserve_downloads and not self.standard_config.download_only:
             logger.debug(f"Cleaning up {self}")
-            os.unlink(self._tmp_download_file())
+            try:
+                os.unlink(self._tmp_download_file())
+            except OSError as e:  # Don't think we need to raise an exception
+                logger.debug(f"Failed to remove {self._tmp_download_file()} due to {e}")
 
 
 class FsspecConnector(BaseConnector):
     """Objects of this class support fetching document(s) from"""
 
     config: SimpleFsspecConfig
     ingest_doc_cls: Type[FsspecIngestDoc] = FsspecIngestDoc
@@ -147,15 +158,15 @@
             **self.config.access_kwargs,
         )
         self.cleanup_files = (
             not standard_config.preserve_downloads and not standard_config.download_only
         )
 
     def cleanup(self, cur_dir=None):
-        """cleanup linginering empty sub-dirs from s3 paths, but leave remaining files
+        """cleanup linginering empty sub-dirs from cloud paths, but leave remaining files
         (and their paths) in tact as that indicates they were not processed"""
         if not self.cleanup_files:
             return
 
         if cur_dir is None:
             cur_dir = self.standard_config.download_dir
         sub_dirs = os.listdir(cur_dir)
@@ -173,15 +184,34 @@
         ls_output = self.fs.ls(self.config.path_without_protocol)
         if len(ls_output) < 1:
             raise ValueError(
                 f"No objects found in {self.config.path}.",
             )
 
     def _list_files(self):
-        return self.fs.ls(self.config.path_without_protocol)
+        if not self.config.recursive:
+            # fs.ls does not walk directories
+            # directories that are listed in cloud storage can cause problems
+            # because they are seen as 0 byte files
+            return [
+                x.get("name")
+                for x in self.fs.ls(self.config.path_without_protocol, detail=True)
+                if x.get("size") > 0
+            ]
+        else:
+            # fs.find will recursively walk directories
+            # "size" is a common key for all the cloud protocols with fs
+            return [
+                k
+                for k, v in self.fs.find(
+                    self.config.path_without_protocol,
+                    detail=True,
+                ).items()
+                if v.get("size") > 0
+            ]
 
     def get_ingest_docs(self):
         return [
             self.ingest_doc_cls(
                 self.standard_config,
                 self.config,
                 file,
```

### Comparing `unstructured-0.7.7/unstructured/ingest/connector/git.py` & `unstructured-0.7.8/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/ingest/connector/github.py` & `unstructured-0.7.8/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/ingest/connector/gitlab.py` & `unstructured-0.7.8/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/ingest/connector/google_drive.py` & `unstructured-0.7.8/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/ingest/connector/local.py` & `unstructured-0.7.8/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/ingest/connector/reddit.py` & `unstructured-0.7.8/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/ingest/connector/s3.py` & `unstructured-0.7.8/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/ingest/connector/slack.py` & `unstructured-0.7.8/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.7.8/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.7.8/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/ingest/interfaces.py` & `unstructured-0.7.8/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/ingest/main.py` & `unstructured-0.7.8/unstructured/ingest/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,30 +158,31 @@
 )
 @click.option(
     "--local-input-path",
     default=None,
     help="Path to the location in the local file system that will be processed.",
 )
 @click.option(
-    "--local-recursive",
-    is_flag=True,
-    default=False,
-    help="Support recursive local file processing.",
-)
-@click.option(
     "--local-file-glob",
     default=None,
     help="A comma-separated list of file globs to limit which types of local files are accepted,"
     " e.g. '*.html,*.txt'",
 )
 @click.option(
     "--remote-url",
     default=None,
     help="Remote fsspec URL formatted as `protocol://dir/path`, it can contain both "
-    "a directory or a single file. Supported protocols are: `s3`, `s3a`, `abfs`, and `az`.",
+    "a directory or a single file. Supported protocols are: `gcs`, `gs`, `s3`, `s3a`, `abfs` "
+    "and `az`.",
+)
+@click.option(
+    "--gcs-token",
+    default=None,
+    help="Token used to access Google Cloud. GCSFS will attempt to use your default gcloud creds"
+    "or get creds from the google metadata service or fall back to anonymous access.",
 )
 @click.option(
     "--s3-anonymous",
     is_flag=True,
     default=False,
     help="Connect to s3 without local AWS credentials.",
 )
@@ -208,21 +209,14 @@
 )
 @click.option(
     "--drive-service-account-key",
     default=None,
     help="Path to the Google Drive service account json file.",
 )
 @click.option(
-    "--drive-recursive",
-    is_flag=True,
-    default=False,
-    help="Recursively download files in folders from the Google Drive ID, "
-    "otherwise stop at the files in provided folder level.",
-)
-@click.option(
     "--drive-extension",
     default=None,
     help="Filters the files to be processed based on extension e.g. .jpg, .docx, etc.",
 )
 @click.option(
     "--biomed-path",
     default=None,
@@ -408,25 +402,34 @@
 )
 @click.option(
     "--num-processes",
     default=2,
     show_default=True,
     help="Number of parallel processes to process docs in.",
 )
+@click.option(
+    "--recursive",
+    is_flag=True,
+    default=False,
+    help="Recursively download files in their respective folders"
+    "otherwise stop at the files in provided folder level."
+    " Supported protocols are: `gcs`, `gs`, `s3`, `s3a`, `abfs` "
+    "`az`, `google drive` and `local`.",
+)
 @click.option("-v", "--verbose", is_flag=True, default=False)
 def main(
     ctx,
     remote_url,
     s3_anonymous,
+    gcs_token,
     azure_account_name,
     azure_account_key,
     azure_connection_string,
     drive_id,
     drive_service_account_key,
-    drive_recursive,
     drive_extension,
     biomed_path,
     biomed_api_id,
     biomed_api_from,
     biomed_api_until,
     biomed_max_retries,
     biomed_max_request_time,
@@ -453,26 +456,26 @@
     discord_token,
     discord_period,
     download_dir,
     preserve_downloads,
     structured_output_dir,
     reprocess,
     num_processes,
+    recursive,
     verbose,
     metadata_include,
     metadata_exclude,
     fields_include,
     flatten_metadata,
     max_docs,
     partition_by_api,
     partition_endpoint,
     partition_strategy,
     api_key,
     local_input_path,
-    local_recursive,
     local_file_glob,
     download_only,
 ):
     default_values = collections.Counter([option.default for option in ctx.command.params])
     passed_values = collections.Counter(ctx.params.values())
     if default_values == passed_values:
         return click.echo(ctx.get_help())
@@ -576,17 +579,29 @@
         if protocol in ("s3", "s3a"):
             from unstructured.ingest.connector.s3 import S3Connector, SimpleS3Config
 
             doc_connector = S3Connector(  # type: ignore
                 standard_config=standard_config,
                 config=SimpleS3Config(
                     path=remote_url,
+                    recursive=recursive,
                     access_kwargs={"anon": s3_anonymous},
                 ),
             )
+        elif protocol in ("gs", "gcs"):
+            from unstructured.ingest.connector.gcs import GcsConnector, SimpleGcsConfig
+
+            doc_connector = GcsConnector(  # type: ignore
+                standard_config=standard_config,
+                config=SimpleGcsConfig(
+                    path=remote_url,
+                    recursive=recursive,
+                    access_kwargs={"token": gcs_token},
+                ),
+            )
         elif protocol in ("abfs", "az"):
             from unstructured.ingest.connector.azure import (
                 AzureBlobStorageConnector,
                 SimpleAzureBlobStorageConfig,
             )
 
             if azure_account_name:
@@ -598,34 +613,36 @@
                 access_kwargs = {"connection_string": azure_connection_string}
             else:
                 access_kwargs = {}
             doc_connector = AzureBlobStorageConnector(  # type: ignore
                 standard_config=standard_config,
                 config=SimpleAzureBlobStorageConfig(
                     path=remote_url,
+                    recursive=recursive,
                     access_kwargs=access_kwargs,
                 ),
             )
         else:
             warnings.warn(
                 f"`fsspec` protocol {protocol} is not directly supported by `unstructured`,"
-                " so use it at your own risk. Supported protocols are `s3`, `s3a`, `abfs`,"
-                " and `az`.",
+                " so use it at your own risk. Supported protocols are `gcs`, `gs`, `s3`, `s3a`,"
+                "`abfs` and `az`.",
                 UserWarning,
             )
 
             from unstructured.ingest.connector.fsspec import (
                 FsspecConnector,
                 SimpleFsspecConfig,
             )
 
             doc_connector = FsspecConnector(  # type: ignore
                 standard_config=standard_config,
                 config=SimpleFsspecConfig(
                     path=remote_url,
+                    recursive=recursive,
                 ),
             )
     elif github_url:
         from unstructured.ingest.connector.github import (
             GitHubConnector,
             SimpleGitHubConfig,
         )
@@ -717,15 +734,15 @@
         )
 
         doc_connector = GoogleDriveConnector(  # type: ignore
             standard_config=standard_config,
             config=SimpleGoogleDriveConfig(
                 drive_id=drive_id,
                 service_account_key=drive_service_account_key,
-                recursive=drive_recursive,
+                recursive=recursive,
                 extension=drive_extension,
             ),
         )
     elif biomed_path or biomed_api_id or biomed_api_from or biomed_api_until:
         from unstructured.ingest.connector.biomed import (
             BiomedConnector,
             SimpleBiomedConfig,
@@ -749,15 +766,15 @@
             SimpleLocalConfig,
         )
 
         doc_connector = LocalConnector(  # type: ignore
             standard_config=standard_config,
             config=SimpleLocalConfig(
                 input_path=local_input_path,
-                recursive=local_recursive,
+                recursive=recursive,
                 file_glob=local_file_glob,
             ),
         )
     # Check for other connector-specific options here and define the doc_connector object
     # e.g. "elif azure_container:  ..."
 
     else:
```

### Comparing `unstructured-0.7.7/unstructured/nlp/english-words.txt` & `unstructured-0.7.8/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/nlp/english_words.py` & `unstructured-0.7.8/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/nlp/patterns.py` & `unstructured-0.7.8/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/nlp/tokenize.py` & `unstructured-0.7.8/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/__init__.py` & `unstructured-0.7.8/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/api.py` & `unstructured-0.7.8/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/auto.py` & `unstructured-0.7.8/unstructured/partition/auto.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/common.py` & `unstructured-0.7.8/unstructured/partition/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import subprocess
-from io import BytesIO
+from io import BufferedReader, BytesIO, TextIOWrapper
 from tempfile import SpooledTemporaryFile
-from typing import TYPE_CHECKING, Any, BinaryIO, Dict, List, Optional, Tuple, Union
+from typing import IO, TYPE_CHECKING, Any, BinaryIO, Dict, List, Optional, Tuple, Union
 
 from docx import table as docxtable
 from tabulate import tabulate
 
 from unstructured.documents.elements import (
     TYPE_TO_TEXT_ELEMENT_MAP,
     CheckBox,
@@ -180,14 +180,33 @@
         contents = file_obj.read()
         return BytesIO(contents)
     else:
         # Return the original file object if it's not a SpooledTemporaryFile
         return file_obj
 
 
+def convert_to_bytes(
+    file: Optional[Union[bytes, SpooledTemporaryFile, IO]] = None,
+) -> bytes:
+    if isinstance(file, bytes):
+        f_bytes = file
+    elif isinstance(file, SpooledTemporaryFile):
+        file.seek(0)
+        f_bytes = file.read()
+    elif isinstance(file, BytesIO):
+        f_bytes = file.getvalue()
+    elif isinstance(file, (TextIOWrapper, BufferedReader)):
+        with open(file.name, "rb") as f:
+            f_bytes = f.read()
+    else:
+        raise ValueError("Invalid file-like object type")
+
+    return f_bytes
+
+
 def convert_ms_office_table_to_text(table: docxtable.Table, as_html: bool = True):
     """
     Convert a table object from a Word document to an HTML table string using the tabulate library.
 
     Args:
         table (Table): A Table object.
         as_html (bool): Whether to return the table as an HTML string (True) or a
```

### Comparing `unstructured-0.7.7/unstructured/partition/csv.py` & `unstructured-0.7.8/unstructured/partition/csv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/doc.py` & `unstructured-0.7.8/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/docx.py` & `unstructured-0.7.8/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/email.py` & `unstructured-0.7.8/unstructured/partition/email.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import datetime
 import email
 import re
 import sys
 from email.message import Message
 from functools import partial
+from tempfile import SpooledTemporaryFile
 from typing import IO, Dict, List, Optional, Tuple, Union
 
 from unstructured.file_utils.encoding import (
     COMMON_ENCODINGS,
     format_encoding_str,
     read_txt_file,
 )
-from unstructured.partition.common import exactly_one
+from unstructured.partition.common import (
+    convert_to_bytes,
+    exactly_one,
+)
 
 if sys.version_info < (3, 8):
     from typing_extensions import Final
 else:
     from typing import Final
 
 from unstructured.cleaners.core import clean_extra_whitespace, replace_mime_encodings
@@ -185,22 +189,22 @@
     element.text = element.text.replace("[image: " + image_info[:-1] + "]", "")
 
     return Image(text=image_info[:-1]), element
 
 
 def parse_email(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[Union[IO, SpooledTemporaryFile]] = None,
 ) -> Tuple[Optional[str], Message]:
     if filename is not None:
         with open(filename, "rb") as f:
             msg = email.message_from_binary_file(f)
     elif file is not None:
-        with open(file.name, "rb") as f:
-            msg = email.message_from_binary_file(f)
+        f_bytes = convert_to_bytes(file)
+        msg = email.message_from_bytes(f_bytes)
     else:
         raise ValueError("Either 'filename' or 'file' must be provided.")
 
     encoding = None
     charsets = msg.get_charsets() or []
     for charset in charsets:
         if charset and charset.strip():
@@ -212,15 +216,15 @@
     return formatted_encoding, msg
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.EML)
 def partition_email(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[Union[IO, SpooledTemporaryFile]] = None,
     text: Optional[str] = None,
     content_source: str = "text/html",
     encoding: Optional[str] = None,
     include_headers: bool = False,
     **kwargs,
 ) -> List[Element]:
     """Partitions an .eml documents into its constituent elements.
@@ -279,17 +283,17 @@
         if part.get_content_disposition() is not None:
             continue
         content_type = part.get_content_type()
         content_map[content_type] = part.get_payload()
 
     content = content_map.get(content_source, "")
     if not content:
-        raise ValueError(f"{content_source} content not found in email")
+        elements = []
 
-    if content_source == "text/html":
+    elif content_source == "text/html":
         # NOTE(robinson) - In the .eml files, the HTML content gets stored in a format that
         # looks like the following, resulting in extraneous "=" characters in the output if
         # you don't clean it up
         # <ul> =
         #    <li>Item 1</li>=
         #    <li>Item 2<li>=
         # </ul>
@@ -312,14 +316,15 @@
                     for enc in common_encodings:
                         try:
                             _replace_mime_encodings = partial(replace_mime_encodings, encoding=enc)
                             element.apply(_replace_mime_encodings)
                             break
                         except (UnicodeDecodeError, UnicodeError):
                             continue
+
     elif content_source == "text/plain":
         list_content = split_by_paragraph(content)
         elements = partition_text(text=content, encoding=encoding)
 
     for idx, element in enumerate(elements):
         indices = has_embedded_image(element)
         if (isinstance(element, (NarrativeText, Title))) and indices:
```

### Comparing `unstructured-0.7.7/unstructured/partition/epub.py` & `unstructured-0.7.8/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/html.py` & `unstructured-0.7.8/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/image.py` & `unstructured-0.7.8/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/json.py` & `unstructured-0.7.8/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/md.py` & `unstructured-0.7.8/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/msg.py` & `unstructured-0.7.8/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/odt.py` & `unstructured-0.7.8/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/pdf.py` & `unstructured-0.7.8/unstructured/partition/pdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 import warnings
 from tempfile import SpooledTemporaryFile
 from typing import BinaryIO, List, Optional, Union, cast
 
 import pdf2image
 from pdfminer.high_level import extract_pages
+from pdfminer.layout import LTContainer, LTImage, LTItem, LTTextBox
 from pdfminer.utils import open_filename
 from PIL import Image
 
 from unstructured.cleaners.core import clean_extra_whitespace
 from unstructured.documents.coordinates import PixelSpace
 from unstructured.documents.elements import (
     Element,
@@ -260,14 +261,33 @@
             filename=filename,
             include_page_breaks=include_page_breaks,
         )
 
     return elements
 
 
+def _extract_text(item: LTItem) -> str:
+    """Recursively extracts text from PDFMiner objects to account
+    for scenarios where the text is in a sub-container."""
+    if hasattr(item, "get_text"):
+        return item.get_text()
+
+    elif isinstance(item, LTContainer):
+        text = ""
+        for child in item:
+            text += _extract_text(child) or ""
+        return text
+
+    elif isinstance(item, (LTTextBox, LTImage)):
+        # TODO(robinson) - Support pulling text out of images
+        # https://github.com/pdfminer/pdfminer.six/blob/master/pdfminer/image.py#L90
+        return "\n"
+    return "\n"
+
+
 def _process_pdfminer_pages(
     fp: BinaryIO,
     filename: str = "",
     include_page_breaks: bool = False,
 ):
     """Uses PDF miner to split a document into pages and process them."""
     elements: List[Element] = []
@@ -279,31 +299,32 @@
         text_segments = []
         page_elements = []
         for obj in page:
             x1, y2, x2, y1 = obj.bbox
             y1 = height - y1
             y2 = height - y2
 
-            # NOTE(robinson) - "Figure" is an example of an object type that does
-            # not have a get_text method
-            if not hasattr(obj, "get_text"):
-                continue
-            _text = obj.get_text()
-            _text = re.sub(PARAGRAPH_PATTERN, " ", _text)
-            _text = clean_extra_whitespace(_text)
-            if _text.strip():
-                text_segments.append(_text)
-                element = element_from_text(_text)
-                element._coordinate_system = PixelSpace(
-                    width=width,
-                    height=height,
-                )
-                element.coordinates = ((x1, y1), (x1, y2), (x2, y2), (x2, y1))
-                element.metadata = metadata
-                page_elements.append(element)
+            if hasattr(obj, "get_text"):
+                _text_snippets = [obj.get_text()]
+            else:
+                _text = _extract_text(obj)
+                _text_snippets = re.split(PARAGRAPH_PATTERN, _text)
+
+            for _text in _text_snippets:
+                _text = clean_extra_whitespace(_text)
+                if _text.strip():
+                    text_segments.append(_text)
+                    element = element_from_text(_text)
+                    element._coordinate_system = PixelSpace(
+                        width=width,
+                        height=height,
+                    )
+                    element.coordinates = ((x1, y1), (x1, y2), (x2, y2), (x2, y1))
+                    element.metadata = metadata
+                    page_elements.append(element)
 
         sorted_page_elements = sorted(
             page_elements,
             key=lambda el: (
                 el.coordinates[0][1] if el.coordinates else float("inf"),
                 el.coordinates[0][0] if el.coordinates else float("inf"),
             ),
```

### Comparing `unstructured-0.7.7/unstructured/partition/ppt.py` & `unstructured-0.7.8/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/pptx.py` & `unstructured-0.7.8/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/rst.py` & `unstructured-0.7.8/unstructured/partition/rst.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/rtf.py` & `unstructured-0.7.8/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/strategies.py` & `unstructured-0.7.8/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/text.py` & `unstructured-0.7.8/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/text_type.py` & `unstructured-0.7.8/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/tsv.py` & `unstructured-0.7.8/unstructured/partition/tsv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/xlsx.py` & `unstructured-0.7.8/unstructured/partition/xlsx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/partition/xml.py` & `unstructured-0.7.8/unstructured/partition/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/staging/argilla.py` & `unstructured-0.7.8/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/staging/base.py` & `unstructured-0.7.8/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/staging/baseplate.py` & `unstructured-0.7.8/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/staging/datasaur.py` & `unstructured-0.7.8/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/staging/huggingface.py` & `unstructured-0.7.8/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/staging/label_box.py` & `unstructured-0.7.8/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/staging/label_studio.py` & `unstructured-0.7.8/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/staging/prodigy.py` & `unstructured-0.7.8/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/staging/weaviate.py` & `unstructured-0.7.8/unstructured/staging/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.7/unstructured/utils.py` & `unstructured-0.7.8/unstructured/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             for dep in dependencies:
                 if not dependency_exists(dep):
                     missing_deps.append(dep)
             if len(missing_deps) > 0:
                 raise ImportError(
                     f"Following dependencies are missing: {', '.join(missing_deps)}. "
                     + (
-                        f"Please install them using `pip install unstructured[{extras}]`."
+                        f"""Please install them using `pip install "unstructured[{extras}]"`."""
                         if extras
                         else f"Please install them using `pip install {' '.join(missing_deps)}`."
                     ),
                 )
             return func(*args, **kwargs)
 
         return wrapper
```

### Comparing `unstructured-0.7.7/unstructured.egg-info/PKG-INFO` & `unstructured-0.7.8/unstructured.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.7
+Version: 0.7.8
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -78,15 +78,15 @@
           use the instructions [here](https://github.com/Unstructured-IO/unstructured-inference#detectron2).
         
         At this point, you should be able to run the following code:
         
         ```python
         from unstructured.partition.auto import partition
         
-        elements = partition(filename="example-docs/fake-email.eml")
+        elements = partition(filename="example-docs/eml/fake-email.eml")
         print("\n\n".join([str(el) for el in elements]))
         ```
         
         The following table shows the document types the `unstructured` library currently supports.
         `partition` will recognize each of these document types and route the document to the
         appropriate partitioning function. If you already know your document type, you can use
         the partitioning function listed in the table directly.
@@ -299,7 +299,8 @@
 Provides-Extra: discord
 Provides-Extra: github
 Provides-Extra: gitlab
 Provides-Extra: reddit
 Provides-Extra: slack
 Provides-Extra: wikipedia
 Provides-Extra: google-drive
+Provides-Extra: gcs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.7 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.8 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -44,31 +44,31 @@
 and PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs)
 - If you are parsing PDFs and want to use a model from the [layoutparser model
 zoo](https://github.com/Unstructured-IO/unstructured-inference#using-models-
 from-the-layoutparser-model-zoo), use the instructions [here](https://
 github.com/Unstructured-IO/unstructured-inference#detectron2). At this point,
 you should be able to run the following code: ```python from
 unstructured.partition.auto import partition elements = partition
-(filename="example-docs/fake-email.eml") print("\n\n".join([str(el) for el in
-elements])) ``` The following table shows the document types the `unstructured`
-library currently supports. `partition` will recognize each of these document
-types and route the document to the appropriate partitioning function. If you
-already know your document type, you can use the partitioning function listed
-in the table directly. See our [documentation page](https://unstructured-
-io.github.io/unstructured/) for more details about the library. | Document Type
-| Partition Function | Strategies | Table Support | Options | | --- | --- | --
-- | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes | None | |
-E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails (`.msg`) |
-`partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) | `partition_epub` |
-N/A | Yes | Include Page Breaks | | Excel Documents (`.xlsx`/`.xls`) |
-`partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`) | `partition_html`
-| N/A | No | Encoding; Include Page Breaks | | Images (`.png`/`.jpg`) |
-`partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding;
-Include Page Breaks; Infer Table Structure; OCR Languages, Strategy | |
-Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Open
+(filename="example-docs/eml/fake-email.eml") print("\n\n".join([str(el) for el
+in elements])) ``` The following table shows the document types the
+`unstructured` library currently supports. `partition` will recognize each of
+these document types and route the document to the appropriate partitioning
+function. If you already know your document type, you can use the partitioning
+function listed in the table directly. See our [documentation page](https://
+unstructured-io.github.io/unstructured/) for more details about the library. |
+Document Type | Partition Function | Strategies | Table Support | Options | | -
+-- | --- | --- | --- | --- | | CSV Files (`.csv`) | `partition_csv` | N/A | Yes
+| None | | E-mails (`.eml`) | `partition_eml` | N/A | No | Encoding | | E-mails
+(`.msg`) | `partition_msg` | N/A | No | Encoding | | EPubs (`.epub`) |
+`partition_epub` | N/A | Yes | Include Page Breaks | | Excel Documents
+(`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None | | HTML Pages (`.html`)
+| `partition_html` | N/A | No | Encoding; Include Page Breaks | | Images
+(`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes
+| Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
+| | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
 Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
 Breaks | | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include
@@ -197,7 +197,8 @@
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown Provides-Extra: huggingface Provides-
 Extra: local-inference Provides-Extra: s3 Provides-Extra: azure Provides-Extra:
 discord Provides-Extra: github Provides-Extra: gitlab Provides-Extra: reddit
 Provides-Extra: slack Provides-Extra: wikipedia Provides-Extra: google-drive
+Provides-Extra: gcs
```

### Comparing `unstructured-0.7.7/unstructured.egg-info/SOURCES.txt` & `unstructured-0.7.8/unstructured.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 setup.cfg
 setup.py
 requirements/base.in
 requirements/huggingface.in
 requirements/ingest-azure.in
 requirements/ingest-discord.in
+requirements/ingest-gcs.in
 requirements/ingest-github.in
 requirements/ingest-gitlab.in
 requirements/ingest-google-drive.in
 requirements/ingest-reddit.in
 requirements/ingest-s3.in
 requirements/ingest-slack.in
 requirements/ingest-wikipedia.in
@@ -54,14 +55,15 @@
 unstructured/ingest/logger.py
 unstructured/ingest/main.py
 unstructured/ingest/connector/__init__.py
 unstructured/ingest/connector/azure.py
 unstructured/ingest/connector/biomed.py
 unstructured/ingest/connector/discord.py
 unstructured/ingest/connector/fsspec.py
+unstructured/ingest/connector/gcs.py
 unstructured/ingest/connector/git.py
 unstructured/ingest/connector/github.py
 unstructured/ingest/connector/gitlab.py
 unstructured/ingest/connector/google_drive.py
 unstructured/ingest/connector/local.py
 unstructured/ingest/connector/reddit.py
 unstructured/ingest/connector/s3.py
```

