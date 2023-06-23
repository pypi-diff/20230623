# Comparing `tmp/AcraNetwork-0.7.4.tar.gz` & `tmp/AcraNetwork-0.7.5.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AcraNetwork-0.7.4.tar", last modified: Mon Oct 24 19:41:21 2016, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

