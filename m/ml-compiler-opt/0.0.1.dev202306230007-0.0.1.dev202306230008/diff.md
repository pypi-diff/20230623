# Comparing `tmp/ml-compiler-opt-0.0.1.dev202306230007.tar.gz` & `tmp/ml_compiler_opt-0.0.1.dev202306230008-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-compiler-opt-0.0.1.dev202306230007.tar", last modified: Fri Jun 23 00:07:53 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

