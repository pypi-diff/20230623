# Comparing `tmp/django-deep-link-0.2.6.tar.gz` & `tmp/django_deep_link-0.3.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-deep-link-0.2.6.tar", last modified: Wed Aug  4 15:13:08 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

