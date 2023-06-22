# Comparing `tmp/clickhouse-connect-0.6.3.tar.gz` & `tmp/clickhouse_connect-0.6.4-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-connect-0.6.3.tar", last modified: Fri Jun 16 15:34:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

