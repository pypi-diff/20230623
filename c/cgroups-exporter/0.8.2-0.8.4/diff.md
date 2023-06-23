# Comparing `tmp/cgroups_exporter-0.8.2.tar.gz` & `tmp/cgroups_exporter-0.8.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgroups_exporter-0.8.2.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

