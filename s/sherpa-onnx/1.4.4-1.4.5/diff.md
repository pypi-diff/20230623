# Comparing `tmp/sherpa-onnx-1.4.4.tar.gz` & `tmp/sherpa_onnx-1.4.5-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-onnx-1.4.4.tar", last modified: Thu Jun  8 02:04:47 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

