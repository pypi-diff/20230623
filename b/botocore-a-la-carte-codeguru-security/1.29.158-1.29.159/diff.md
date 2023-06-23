# Comparing `tmp/botocore-a-la-carte-codeguru-security-1.29.158.tar.gz` & `tmp/botocore_a_la_carte_codeguru_security-1.29.159-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-codeguru-security-1.29.158.tar", last modified: Thu Jun 22 01:25:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

