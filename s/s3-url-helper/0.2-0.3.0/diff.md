# Comparing `tmp/s3_url_helper-0.2.tar.gz` & `tmp/s3_url_helper-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\s3_url_helper-0.2.tar", last modified: Thu Jun 22 09:43:16 2023, max compression
+gzip compressed data, was "s3_url_helper-0.3.0.tar", last modified: Fri Jun 23 12:35:59 2023, max compression
```

## Comparing `s3_url_helper-0.2.tar` & `s3_url_helper-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 09:43:16.372484 s3_url_helper-0.2/
--rw-rw-rw-   0        0        0     1074 2023-06-22 08:47:58.000000 s3_url_helper-0.2/LICENSE
--rw-rw-rw-   0        0        0     2299 2023-06-22 09:43:16.371484 s3_url_helper-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2016 2023-06-22 09:39:05.000000 s3_url_helper-0.2/README.md
--rw-rw-rw-   0        0        0       88 2023-06-22 08:43:19.000000 s3_url_helper-0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-22 09:43:16.357402 s3_url_helper-0.2/s3_url/
--rw-rw-rw-   0        0        0       33 2023-06-22 08:46:47.000000 s3_url_helper-0.2/s3_url/__init__.py
--rw-rw-rw-   0        0        0     6773 2023-06-22 09:20:52.000000 s3_url_helper-0.2/s3_url/s3_url.py
-drwxrwxrwx   0        0        0        0 2023-06-22 09:43:16.367484 s3_url_helper-0.2/s3_url_helper.egg-info/
--rw-rw-rw-   0        0        0     2299 2023-06-22 09:43:16.000000 s3_url_helper-0.2/s3_url_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-06-22 09:43:16.000000 s3_url_helper-0.2/s3_url_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 09:43:16.000000 s3_url_helper-0.2/s3_url_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-06-22 09:43:16.000000 s3_url_helper-0.2/s3_url_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-22 09:43:16.000000 s3_url_helper-0.2/s3_url_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 09:43:16.372484 s3_url_helper-0.2/setup.cfg
--rw-rw-rw-   0        0        0      917 2023-06-22 09:40:33.000000 s3_url_helper-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 09:43:16.369487 s3_url_helper-0.2/tests/
--rw-rw-rw-   0        0        0    16984 2023-06-22 09:34:59.000000 s3_url_helper-0.2/tests/test_s3_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:35:59.749047 s3_url_helper-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:35:59.749047 s3_url_helper-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:35:59.749047 s3_url_helper-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-23 12:35:45.000000 s3_url_helper-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-23 12:35:45.000000 s3_url_helper-0.3.0/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-23 12:35:45.000000 s3_url_helper-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-23 12:35:59.749047 s3_url_helper-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-23 12:35:45.000000 s3_url_helper-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-23 12:35:45.000000 s3_url_helper-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:35:59.749047 s3_url_helper-0.3.0/s3_url/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 12:35:45.000000 s3_url_helper-0.3.0/s3_url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-06-23 12:35:45.000000 s3_url_helper-0.3.0/s3_url/s3_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:35:59.749047 s3_url_helper-0.3.0/s3_url_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-23 12:35:59.000000 s3_url_helper-0.3.0/s3_url_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-23 12:35:59.000000 s3_url_helper-0.3.0/s3_url_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 12:35:59.000000 s3_url_helper-0.3.0/s3_url_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-23 12:35:59.000000 s3_url_helper-0.3.0/s3_url_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 12:35:59.000000 s3_url_helper-0.3.0/s3_url_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 12:35:59.749047 s3_url_helper-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:35:59.749047 s3_url_helper-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:35:45.000000 s3_url_helper-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-23 12:35:45.000000 s3_url_helper-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:35:59.749047 s3_url_helper-0.3.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 12:35:45.000000 s3_url_helper-0.3.0/tests/resources/test_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16502 2023-06-23 12:35:45.000000 s3_url_helper-0.3.0/tests/test_s3_url.py
```

### Comparing `s3_url_helper-0.2/LICENSE` & `s3_url_helper-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2023 Nikolai Orlov
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2023 Nikolai Orlov
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `s3_url_helper-0.2/PKG-INFO` & `s3_url_helper-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,73 @@
-Metadata-Version: 2.1
-Name: s3_url_helper
-Version: 0.2
-Summary: S3 Url Helper
-Home-page: https://github.com/n-orlov/s3-url-helper
-Author: Nikolai Orlov
-Author-email: nikolaiorl@gmail.com
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-## Overview
-S3Url is a helper class that can help with simple operations on AWS S3 objects.<br>
-### Installation
-`pip install s3-url-helper==0.1`<br>
-### Usage
-    from s3_url import S3Url
-
-    file_url = S3Url(f's3://test-bucket/prefix/file.json')
-
-    # url component properties
-    assert file_url.bucket == 'test-bucket'
-    assert file_url.key == 'prefix/file.json'
-
-    # factory methods
-    file_url = S3Url.from_url('s3://test-bucket/prefix/file.json')
-    file_url = S3Url.from_bucket_key(bucket='test-bucket', key='prefix/file.json')
-
-    # access underlying boto3 s3 resource object
-    boto3_obj = file_url.object
-
-    # return url string
-    url_str: str = file_url.url
-    url_str: str = str(file_url)
-    assert url_str == 's3://test-bucket/prefix/file.json'
-
-    # check if file exists
-    exists: bool = file_url.exists()
-    assert exists
-
-    # check if any files exist in prefix (url should end with /)
-    prefix_exists = S3Url('s3://test-bucket/prefix/').prefix_exists()
-    assert prefix_exists
-
-    # read text/json
-    file_content: str = file_url.read_text()
-    file_content_json: json = file_url.read_json()
-
-    # delete file
-    file_url.delete()
-    assert not file_url.exists()
-
-    # write text/json
-    file_url.write_text("test data")
-    file_url.write_json({"testEntry": "test data"})
-    assert file_url.exists()
-
-    # copy to another object
-    file_url.copy_to('s3://test-bucket/prefix/file-copy.json')
-    S3Url('s3://test-bucket/prefix/another-file-copy.json').copy_from(file_url)
-
-    # delete all filed in prefix
-    prefix_url = S3Url('s3://test-bucket/prefix/')
-    prefix_url.delete_dir()
-
-    assert not prefix_url.prefix_exists()
-    assert not file_url.exists()
-
-    # see tests for more examples
-
-## Development notes
-init deps:
-    
-    install dev dependencies: pip install -e ".[dev]" 
-
-build/upload:
-
-    py -m build
-    py -m twine upload --repository pypi dist/*  
-
-todo - write docstrings
+[![Coverage Badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/n-orlov/f26292d8b498fa22b87e6425ddc7d235/raw/9624db6266b021187ae76483eb2aa7d9f5ed5a75/s3_url_helper_coverage_badge__master.json)](https://gist.github.com/n-orlov/f26292d8b498fa22b87e6425ddc7d235#file-code-coverage-results-md)
+
+## Overview
+S3Url is a helper class that can help with simple operations on AWS S3 objects.<br>
+### Installation
+Get from https://pypi.org/project/s3-url-helper/
+<br> e.g `pip install s3-url-helper`<br>
+### Usage
+    from s3_url import S3Url
+
+    file_url = S3Url(f's3://test-bucket/prefix/file.json')
+
+    # url component properties
+    assert file_url.bucket == 'test-bucket'
+    assert file_url.key == 'prefix/file.json'
+
+    # factory methods
+    file_url = S3Url.from_url('s3://test-bucket/prefix/file.json')
+    file_url = S3Url.from_bucket_key(bucket='test-bucket', key='prefix/file.json')
+
+    # access underlying boto3 s3 resource object
+    boto3_obj = file_url.object
+
+    # return url string
+    url_str: str = file_url.url
+    url_str: str = str(file_url)
+    assert url_str == 's3://test-bucket/prefix/file.json'
+
+    # check if file exists
+    exists: bool = file_url.exists()
+    assert exists
+
+    # check if any files exist in prefix (url should end with /)
+    prefix_exists = S3Url('s3://test-bucket/prefix/').prefix_exists()
+    assert prefix_exists
+
+    # read text/json
+    file_content: str = file_url.read_text()
+    file_content_json: json = file_url.read_json()
+
+    # delete file
+    file_url.delete()
+    assert not file_url.exists()
+
+    # write text/json
+    file_url.write_text("test data")
+    file_url.write_json({"testEntry": "test data"})
+    assert file_url.exists()
+
+    # copy to another object
+    file_url.copy_to('s3://test-bucket/prefix/file-copy.json')
+    S3Url('s3://test-bucket/prefix/another-file-copy.json').copy_from(file_url)
+
+    # delete all filed in prefix
+    prefix_url = S3Url('s3://test-bucket/prefix/')
+    prefix_url.delete_dir()
+
+    assert not prefix_url.prefix_exists()
+    assert not file_url.exists()
+
+    # see tests for more examples
+
+## Development notes
+Install dev dependencies: 
+    pip install .[dev]
+    pip install .[build]
+
+build/upload:
+
+    py -m build
+    py -m twine upload --repository pypi dist/*  
+
+todo - write docstrings
```

### Comparing `s3_url_helper-0.2/s3_url/s3_url.py` & `s3_url_helper-0.3.0/s3_url/s3_url.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,207 +1,207 @@
-import json
-import threading
-from typing import Union, Iterable
-from urllib.parse import urlparse
-
-import boto3
-from botocore.exceptions import ClientError
-
-
-class S3Url():
-    _local = threading.local()
-
-    def __init__(self, url: Union[str, 'S3Url']):
-        '''
-        Creates object instance
-        :param url: "s3://"-shaped url or another S3Url object
-        '''
-
-        if not hasattr(self._local, 's3_res'):
-            self._local.s3_res = boto3.resource('s3')
-        if isinstance(url, S3Url):
-            url = url.url
-        else:
-            if not url.startswith('s3://'):
-                raise Exception(f'Unsupported URL: {url}. It must start with s3://')
-        self._parsed = urlparse(url, allow_fragments=False)
-        self._object = self._local.s3_res.Object(self.bucket, self.key)
-
-    @classmethod
-    def from_url(cls, url: Union[str, 'S3Url']) -> 'S3Url':
-        return S3Url(url)
-
-    @classmethod
-    def from_bucket_key(cls, bucket: str, key: str) -> 'S3Url':
-        return S3Url(f's3://{bucket}/{key}')
-
-
-
-    def __repr__(self) -> str:
-        return self.url
-
-    def __eq__(self, o: object) -> bool:
-        return isinstance(o, S3Url) and o.url == self.url
-
-    def __hash__(self) -> int:
-        return self.url.__hash__()
-
-    @property
-    def bucket(self) -> str:
-        return self._parsed.netloc
-
-    @property
-    def key(self) -> str:
-        return self._parsed.path.lstrip('/')
-
-    @property
-    def object(self):
-        return self._object
-
-    @property
-    def url(self) -> str:
-        return self._parsed.geturl()
-
-    def exists(self) -> bool:
-        try:
-            self.object.load()
-            return True
-        except ClientError as cerr:
-            if '404' in str(cerr):
-                return False
-            else:
-                raise cerr
-
-    def prefix_exists(self) -> bool:
-        try:
-            next(iter(self._object.Bucket().objects.filter(Prefix=self.key)))
-            return True
-        except StopIteration:
-            return False
-        except ClientError as cerr:
-            if '404' in str(cerr):
-                return False
-            else:
-                raise cerr
-
-    def read_text(self, encoding="utf-8-sig") -> str:
-        return self.object.get()['Body'].read().decode(encoding)
-
-    def read_json(self, encoding="utf-8-sig") -> json:
-        return json.loads(self.read_text(encoding))
-
-    def delete(self) -> None:
-        self.object.delete()
-
-    def write_text(self, body: str, encryption=None) -> None:
-        if encryption:
-            self.object.put(Body=body, ServerSideEncryption=encryption)
-        else:
-            self.object.put(Body=body)
-
-    def write_json(self, body: json, encryption=None) -> None:
-        self.write_text(json.dumps(body), encryption)
-
-    def upload_file(self, fileobj, encryption=None):
-        if encryption:
-            self.object.upload_fileobj(fileobj, ExtraArgs={
-                'ServerSideEncryption': encryption
-            })
-        else:
-            self.object.upload_fileobj(fileobj)
-
-    def delete_dir(self):
-        for obj in self._local.s3_res.Bucket(self.bucket).objects.filter(Prefix=self.key):
-            obj.delete()
-
-    def write_tags(self, tags: dict) -> None:
-        if tags:
-            tag_set = [{'Key': k, 'Value': v} for k, v in tags.items()]
-            self._local.s3_res.meta.client.put_object_tagging(
-                Bucket=self.bucket,
-                Key=self.key,
-                Tagging={
-                    'TagSet': tag_set
-                }
-            )
-
-    def read_tags(self) -> dict:
-        tags_dict = {}
-        tags = self._local.s3_res.meta.client.get_object_tagging(
-            Bucket=self.bucket,
-            Key=self.key,
-        )
-        if tags:
-            tags_dict = {x['Key']: x['Value'] for x in tags['TagSet']}
-
-        return tags_dict
-
-    def transition_to_storage_tier(self, storage_tier: str):
-        return self._local.s3_res.meta.client.copy_object(
-            CopySource={
-                'Bucket': self.bucket,
-                'Key': self.key
-            },
-            Bucket=self.bucket,
-            Key=self.key,
-            StorageClass=storage_tier,
-            MetadataDirective='COPY')
-
-    def restore_to_storage_tier(self, days: int, retrieval_tier: str = "Standard"):
-        return self._local.s3_res.meta.client.restore_object(
-            Bucket=self.bucket,
-            Key=self.key,
-            RestoreRequest={'Days': days, 'GlacierJobParameters': {'Tier': retrieval_tier}})
-
-    def copy_to(self, target_url: Union[str, 'S3Url']) -> None:
-        if isinstance(target_url, S3Url):
-            target_obj = target_url
-        else:
-            target_obj = S3Url(target_url)
-        self._local.s3_res.meta.client.copy({
-            'Bucket': self.bucket,
-            'Key': self.key
-        }, target_obj.bucket, target_obj.key)
-
-    def copy_from(self, source_url: Union[str, 'S3Url']) -> None:
-        if isinstance(source_url, S3Url):
-            source_obj = source_url
-        else:
-            source_obj = S3Url(source_url)
-        self._local.s3_res.meta.client.copy({
-            'Bucket': source_obj.bucket,
-            'Key': source_obj.key
-        }, self.bucket, self.key)
-
-    def copy_tags_to(self, target_url: Union[str, 'S3Url']) -> None:
-        source_tags = self.read_tags()
-        if isinstance(target_url, S3Url):
-            target_obj = target_url
-        else:
-            target_obj = S3Url(target_url)
-        target_obj.write_tags(source_tags)
-
-    def copy_tags_from(self, source_url: Union[str, 'S3Url']) -> None:
-        if isinstance(source_url, S3Url):
-            source_obj = source_url
-        else:
-            source_obj = S3Url(source_url)
-        source_tags = source_obj.read_tags()
-        self.write_tags(source_tags)
-
-    def list_prefix_objects(self) -> Iterable['S3Url']:
-        for s3_obj in self._object.Bucket().objects.filter(Prefix=self.key):
-            yield S3Url(f's3://{s3_obj.bucket_name}/{s3_obj.key}')
-
-    def generate_presigned_url_get(self, timeout=3600) -> str:
-        return self._local.s3_res.meta.client.generate_presigned_url(
-            ClientMethod='get_object',
-            Params={'Bucket': self.bucket, 'Key': self.key},
-            ExpiresIn=timeout
-        )
-
-    def generate_presigned_url_put(self, timeout=3600) -> str:
-        return self._local.s3_res.meta.client.generate_presigned_url(
-            ClientMethod='put_object',
-            Params={'Bucket': self.bucket, 'Key': self.key},
-            ExpiresIn=timeout
-        )
+import json
+import threading
+from typing import Union, Iterable
+from urllib.parse import urlparse
+
+import boto3
+from botocore.exceptions import ClientError
+
+
+class S3Url():
+    _local = threading.local()
+
+    def __init__(self, url: Union[str, 'S3Url']):
+        '''
+        Creates object instance
+        :param url: "s3://"-shaped url or another S3Url object
+        '''
+
+        if not hasattr(self._local, 's3_res'):
+            self._local.s3_res = boto3.resource('s3')
+        if isinstance(url, S3Url):
+            url = url.url
+        else:
+            if not url.startswith('s3://'):
+                raise Exception(f'Unsupported URL: {url}. It must start with s3://')
+        self._parsed = urlparse(url, allow_fragments=False)
+        self._object = self._local.s3_res.Object(self.bucket, self.key)
+
+    @classmethod
+    def from_url(cls, url: Union[str, 'S3Url']) -> 'S3Url':
+        return S3Url(url)
+
+    @classmethod
+    def from_bucket_key(cls, bucket: str, key: str) -> 'S3Url':
+        return S3Url(f's3://{bucket}/{key}')
+
+
+
+    def __repr__(self) -> str:
+        return self.url
+
+    def __eq__(self, o: object) -> bool:
+        return isinstance(o, S3Url) and o.url == self.url
+
+    def __hash__(self) -> int:
+        return self.url.__hash__()
+
+    @property
+    def bucket(self) -> str:
+        return self._parsed.netloc
+
+    @property
+    def key(self) -> str:
+        return self._parsed.path.lstrip('/')
+
+    @property
+    def object(self):
+        return self._object
+
+    @property
+    def url(self) -> str:
+        return self._parsed.geturl()
+
+    def exists(self) -> bool:
+        try:
+            self.object.load()
+            return True
+        except ClientError as cerr:
+            if '404' in str(cerr):
+                return False
+            else:
+                raise cerr
+
+    def prefix_exists(self) -> bool:
+        try:
+            next(iter(self._object.Bucket().objects.filter(Prefix=self.key)))
+            return True
+        except StopIteration:
+            return False
+        except ClientError as cerr:
+            if '404' in str(cerr):
+                return False
+            else:
+                raise cerr
+
+    def read_text(self, encoding="utf-8-sig") -> str:
+        return self.object.get()['Body'].read().decode(encoding)
+
+    def read_json(self, encoding="utf-8-sig") -> json:
+        return json.loads(self.read_text(encoding))
+
+    def delete(self) -> None:
+        self.object.delete()
+
+    def write_text(self, body: str, encryption=None) -> None:
+        if encryption:
+            self.object.put(Body=body, ServerSideEncryption=encryption)
+        else:
+            self.object.put(Body=body)
+
+    def write_json(self, body: json, encryption=None) -> None:
+        self.write_text(json.dumps(body), encryption)
+
+    def upload_file(self, fileobj, encryption=None):
+        if encryption:
+            self.object.upload_fileobj(fileobj, ExtraArgs={
+                'ServerSideEncryption': encryption
+            })
+        else:
+            self.object.upload_fileobj(fileobj)
+
+    def delete_dir(self):
+        for obj in self._local.s3_res.Bucket(self.bucket).objects.filter(Prefix=self.key):
+            obj.delete()
+
+    def write_tags(self, tags: dict) -> None:
+        if tags:
+            tag_set = [{'Key': k, 'Value': v} for k, v in tags.items()]
+            self._local.s3_res.meta.client.put_object_tagging(
+                Bucket=self.bucket,
+                Key=self.key,
+                Tagging={
+                    'TagSet': tag_set
+                }
+            )
+
+    def read_tags(self) -> dict:
+        tags_dict = {}
+        tags = self._local.s3_res.meta.client.get_object_tagging(
+            Bucket=self.bucket,
+            Key=self.key,
+        )
+        if tags:
+            tags_dict = {x['Key']: x['Value'] for x in tags['TagSet']}
+
+        return tags_dict
+
+    def transition_to_storage_tier(self, storage_tier: str):
+        return self._local.s3_res.meta.client.copy_object(
+            CopySource={
+                'Bucket': self.bucket,
+                'Key': self.key
+            },
+            Bucket=self.bucket,
+            Key=self.key,
+            StorageClass=storage_tier,
+            MetadataDirective='COPY')
+
+    def restore_to_storage_tier(self, days: int, retrieval_tier: str = "Standard"):
+        return self._local.s3_res.meta.client.restore_object(
+            Bucket=self.bucket,
+            Key=self.key,
+            RestoreRequest={'Days': days, 'GlacierJobParameters': {'Tier': retrieval_tier}})
+
+    def copy_to(self, target_url: Union[str, 'S3Url']) -> None:
+        if isinstance(target_url, S3Url):
+            target_obj = target_url
+        else:
+            target_obj = S3Url(target_url)
+        self._local.s3_res.meta.client.copy({
+            'Bucket': self.bucket,
+            'Key': self.key
+        }, target_obj.bucket, target_obj.key)
+
+    def copy_from(self, source_url: Union[str, 'S3Url']) -> None:
+        if isinstance(source_url, S3Url):
+            source_obj = source_url
+        else:
+            source_obj = S3Url(source_url)
+        self._local.s3_res.meta.client.copy({
+            'Bucket': source_obj.bucket,
+            'Key': source_obj.key
+        }, self.bucket, self.key)
+
+    def copy_tags_to(self, target_url: Union[str, 'S3Url']) -> None:
+        source_tags = self.read_tags()
+        if isinstance(target_url, S3Url):
+            target_obj = target_url
+        else:
+            target_obj = S3Url(target_url)
+        target_obj.write_tags(source_tags)
+
+    def copy_tags_from(self, source_url: Union[str, 'S3Url']) -> None:
+        if isinstance(source_url, S3Url):
+            source_obj = source_url
+        else:
+            source_obj = S3Url(source_url)
+        source_tags = source_obj.read_tags()
+        self.write_tags(source_tags)
+
+    def list_prefix_objects(self) -> Iterable['S3Url']:
+        for s3_obj in self._object.Bucket().objects.filter(Prefix=self.key):
+            yield S3Url(f's3://{s3_obj.bucket_name}/{s3_obj.key}')
+
+    def generate_presigned_url_get(self, timeout=3600) -> str:
+        return self._local.s3_res.meta.client.generate_presigned_url(
+            ClientMethod='get_object',
+            Params={'Bucket': self.bucket, 'Key': self.key},
+            ExpiresIn=timeout
+        )
+
+    def generate_presigned_url_put(self, timeout=3600) -> str:
+        return self._local.s3_res.meta.client.generate_presigned_url(
+            ClientMethod='put_object',
+            Params={'Bucket': self.bucket, 'Key': self.key},
+            ExpiresIn=timeout
+        )
```

### Comparing `s3_url_helper-0.2/tests/test_s3_url.py` & `s3_url_helper-0.3.0/tests/test_s3_url.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,482 +1,482 @@
-import json
-from pathlib import Path
-
-import boto3
-import pytest
-import requests
-from assertpy import assert_that
-from boto3 import s3
-from botocore.exceptions import ClientError
-from s3_url import S3Url
-from tests.conftest import TEST_BUCKET, assert_with_timeout
-
-
-def test_demo(s3_test_bucket, s3_demo_file):
-    file_url = S3Url(f's3://test-bucket/prefix/file.json')
-
-    # url component properties
-    assert file_url.bucket == 'test-bucket'
-    assert file_url.key == 'prefix/file.json'
-
-    # factory methods
-    file_url = S3Url.from_url('s3://test-bucket/prefix/file.json')
-    file_url = S3Url.from_bucket_key(bucket='test-bucket', key='prefix/file.json')
-
-    # access underlying boto3 s3 resource object
-    boto3_obj = file_url.object
-
-    # return url string
-    url_str: str = file_url.url
-    url_str: str = str(file_url)
-    assert url_str == 's3://test-bucket/prefix/file.json'
-
-    # check if file exists
-    exists: bool = file_url.exists()
-    assert exists
-
-    # check if any files exist in prefix (url should end with /)
-    prefix_exists = S3Url('s3://test-bucket/prefix/').prefix_exists()
-    assert prefix_exists
-
-    # read text/json
-    file_content: str = file_url.read_text()
-    file_content_json: json = file_url.read_json()
-
-    # delete file
-    file_url.delete()
-    assert not file_url.exists()
-
-    # write text/json
-    file_url.write_text("test data")
-    file_url.write_json({"testEntry": "test data"})
-    assert file_url.exists()
-
-    # copy to another object
-    file_url.copy_to('s3://test-bucket/prefix/file-copy.json')
-    S3Url('s3://test-bucket/prefix/another-file-copy.json').copy_from(file_url)
-
-    # delete all filed in prefix
-    prefix_url = S3Url('s3://test-bucket/prefix/')
-    prefix_url.delete_dir()
-
-    assert not prefix_url.prefix_exists()
-    assert not file_url.exists()
-
-
-def test_s3_url_parts(s3_test_bucket, s3_test_file):
-    url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    assert_that(url.url).is_equal_to(f's3://{TEST_BUCKET}/SomeFolder/test_file.json')
-    assert_that(url.bucket).is_equal_to(TEST_BUCKET)
-    assert_that(url.key).is_equal_to('SomeFolder/test_file.json')
-
-
-def test_factory_methods(s3_test_bucket, s3_test_file):
-    url = S3Url.from_url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    assert_that(url.url).is_equal_to(f's3://{TEST_BUCKET}/SomeFolder/test_file.json')
-    assert_that(url.bucket).is_equal_to(TEST_BUCKET)
-    assert_that(url.key).is_equal_to('SomeFolder/test_file.json')
-
-    url = S3Url.from_bucket_key(s3_test_bucket.name, s3_test_file)
-    assert_that(url.url).is_equal_to(f's3://{TEST_BUCKET}/SomeFolder/test_file.json')
-    assert_that(url.bucket).is_equal_to(TEST_BUCKET)
-    assert_that(url.key).is_equal_to('SomeFolder/test_file.json')
-
-
-def test_unsupported_url(s3_test_bucket):
-    with pytest.raises(Exception) as err:
-        S3Url(f'https://{s3_test_bucket.name}/some/path')
-    assert_that(str(err)).contains('Unsupported URL')
-
-
-def test_s3_url_exists(s3_test_bucket, s3_test_file):
-    existing_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    assert_that(existing_url.exists()).is_true()
-    non_existing_url = S3Url(f's3://{s3_test_bucket.name}/non_existing_file.txt')
-    assert_that(non_existing_url.exists()).is_false()
-
-
-def test_generate_presigned_url_get(s3_test_bucket, s3_test_file):
-    existing_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    get_url = existing_url.generate_presigned_url_get()
-    assert_that(requests.get(get_url).content.decode()).is_equal_to(existing_url.read_text())
-
-
-def test_generate_presigned_url_put(s3_test_bucket, s3_test_file):
-    non_existing_url = S3Url(f's3://{s3_test_bucket.name}/non_existing_file.txt')
-    get_url = non_existing_url.generate_presigned_url_put()
-    requests.put(get_url, data="test text file".encode()).raise_for_status()
-    assert_that(non_existing_url.read_text()).is_equal_to("test text file")
-
-
-def test_s3_url_exists_access_denied(s3_test_bucket, s3_test_file, monkeypatch):
-    existing_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    expected_exc = ClientError({'Error': {'Code': '403', 'Message': 'Forbidden'},
-                                'ResponseMetadata': {'HTTPStatusCode': 403, 'RetryAttempts': 0}}, 'HeadObject')
-
-    def raise_exc(*args, **kwargs):
-        raise expected_exc
-
-    monkeypatch.setattr(existing_url.object.meta.client, '_make_api_call', raise_exc)
-    assert_that(existing_url.exists).raises(ClientError).when_called_with()
-
-
-def test_s3_url_exists_for_a_path(s3_test_bucket, s3_test_file_3):
-    existing_url = S3Url(f's3://{s3_test_bucket.name}/a/path/to/')
-    assert_that(existing_url.prefix_exists()).is_true()
-    existing_url = S3Url(f's3://{s3_test_bucket.name}/a/path/to/the/file')
-    assert_that(existing_url.prefix_exists()).is_true()
-
-    non_existing_url = S3Url(f's3://{s3_test_bucket.name}/unknown/path/to/the/file')
-    assert_that(non_existing_url.prefix_exists()).is_false()
-
-
-def test_list_prefix_objects(s3_test_bucket):
-    file_1 = S3Url(f's3://{s3_test_bucket.name}/some_prefix/some_file_1.txt')
-    file_2 = S3Url(f's3://{s3_test_bucket.name}/some_prefix/some_file_2.txt')
-    file_3 = S3Url(f's3://{s3_test_bucket.name}/some_prefix/some_file_3.txt')
-
-    file_1.write_text("1")
-    file_2.write_text("2")
-    file_3.write_text("3")
-
-    existing_prefix_url = S3Url(f's3://{s3_test_bucket.name}/some_prefix/')
-    assert_that(list(existing_prefix_url.list_prefix_objects())).is_length(3).contains_only(file_1, file_2, file_3)
-
-
-def test_s3_url_exists_for_a_path_access_denied(s3_test_bucket, s3_test_file_3, monkeypatch):
-    existing_url = S3Url(f's3://{s3_test_bucket.name}/a/path/to/')
-    expected_exc = ClientError({'Error': {'Code': '403', 'Message': 'Forbidden'},
-                                'ResponseMetadata': {'HTTPStatusCode': 403, 'RetryAttempts': 0}}, 'ListObjects')
-
-    def raise_exc(*args, **kwargs):
-        raise expected_exc
-
-    monkeypatch.setattr(existing_url.object.meta.client, '_make_api_call', raise_exc)
-    assert_that(existing_url.prefix_exists).raises(ClientError).when_called_with()
-
-
-def test_s3_url_delete(s3_test_bucket, s3_test_file):
-    existing_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    assert_that(existing_url.exists()).is_true()
-    existing_url.delete()
-    assert_that(existing_url.exists()).is_false()
-    # should not fail if not exists
-    existing_url.delete()
-
-
-def test_s3_url_delete_dir(s3_test_bucket, s3_test_file):
-    existing_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    assert_that(existing_url.exists()).is_true()
-    prefix = S3Url(f's3://{s3_test_bucket.name}/SomeFolder/')
-    prefix.delete_dir()
-    assert_that(existing_url.exists()).is_false()
-
-
-def test_s3_url_read_write(s3_test_bucket, s3_test_file):
-    url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    assert_that(json.loads(url.read_text())).is_equal_to({
-        "testEntry1": "value1"
-    })
-    url.write_text(json.dumps({
-        "newField": "newValue"
-    }))
-    assert_that(url.object.server_side_encryption).is_none()
-
-    assert_that(json.loads(url.read_text())).is_equal_to({
-        "newField": "newValue"
-    })
-    url.write_text(json.dumps({
-        "newField": "newValue"
-    }), encryption='AES256')
-    assert_that(url.object.server_side_encryption).is_equal_to('AES256')
-
-
-def test_s3_url_read_write_json(s3_test_bucket, s3_test_file):
-    url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    assert_that(url.read_json()).is_equal_to({
-        "testEntry1": "value1"
-    })
-    url.write_json({
-        "newField": "newValue"
-    })
-    assert_that(url.object.server_side_encryption).is_none()
-
-    assert_that(url.read_json()).is_equal_to({
-        "newField": "newValue"
-    })
-    url.write_json({
-        "newField": "newValue"
-    }, encryption='AES256')
-    assert_that(url.object.server_side_encryption).is_equal_to('AES256')
-
-
-def test_s3_url_read_non_existing(s3_test_bucket):
-    non_existing_url = S3Url(f's3://{s3_test_bucket.name}/non_existing_file.txt')
-    with pytest.raises(ClientError) as err:
-        non_existing_url.read_text()
-    assert_that(str(err.value)).contains('NoSuchKey')
-    assert_that(str(err.value)).contains('The specified key does not exist')
-
-
-def test_s3_url_upload_file(s3_test_bucket):
-    url = S3Url(f's3://{s3_test_bucket.name}/some_new_file.json')
-    current_path = Path(__file__).resolve().parent
-    img_path = current_path / "resources" / "test_file.json"
-    with img_path.open(mode='rb') as fobj:
-        url.upload_file(fobj)
-    assert_that(json.loads(url.read_text())).is_equal_to({
-        "testEntry1": "value1"
-    })
-    assert_that(url.object.server_side_encryption).is_none()
-
-
-def test_s3_url_upload_file_encryption(s3_test_bucket):
-    url = S3Url(f's3://{s3_test_bucket.name}/some_new_file.json')
-    current_path = Path(__file__).resolve().parent
-    img_path = current_path / "resources" / "test_file.json"
-    with img_path.open(mode='rb') as fobj:
-        url.upload_file(fobj, encryption='AES256')
-    assert_that(json.loads(url.read_text())).is_equal_to({
-        "testEntry1": "value1"
-    })
-    assert_that(url.object.server_side_encryption).is_equal_to('AES256')
-
-
-def test_copy_to_url(s3_test_bucket, s3_test_file):
-    # Given
-    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    target_url = S3Url(f's3://{s3_test_bucket.name}/copied/{s3_test_file}')
-    assert_that(target_url).s3_file_does_not_exist()
-
-    # When
-    source_url.copy_to(target_url)
-
-    # Then
-    assert_that(target_url).s3_file_exists()
-
-
-def test_copy_to_str(s3_test_bucket, s3_test_file):
-    # Given
-    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    target_url = S3Url(f's3://{s3_test_bucket.name}/copied/{s3_test_file}')
-    assert_that(target_url).s3_file_does_not_exist()
-
-    # When
-    source_url.copy_to(target_url.url)
-
-    # Then
-    assert_that(target_url).s3_file_exists()
-
-
-def test_copy_from_url(s3_test_bucket, s3_test_file):
-    # Given
-    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    target_url = S3Url(f's3://{s3_test_bucket.name}/copied/{s3_test_file}')
-    assert_that(target_url).s3_file_does_not_exist()
-
-    # When
-    target_url.copy_from(source_url)
-
-    # Then
-    assert_that(target_url).s3_file_exists()
-
-
-def test_copy_from_str(s3_test_bucket, s3_test_file):
-    # Given
-    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    target_url = S3Url(f's3://{s3_test_bucket.name}/copied/{s3_test_file}')
-    assert_that(target_url).s3_file_does_not_exist()
-
-    # When
-    target_url.copy_from(source_url.url)
-
-    # Then
-    assert_that(target_url).s3_file_exists()
-
-
-def test_should_read_tags_to_s3_file(s3_test_bucket, s3_test_file):
-    # Given
-    url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    s3_test_bucket.meta.client.put_object_tagging(
-        Bucket=s3_test_bucket.name,
-        Key=s3_test_file,
-        Tagging={
-            'TagSet': [
-                {'Key': 'tag1', 'Value': 'value1'},
-                {'Key': 'tag2', 'Value': 'value2'},
-            ]
-        }
-    )
-
-    # Then
-    assert_that(url).has_s3_tags_equal_to({'tag1': 'value1', 'tag2': 'value2'})
-
-
-def test_should_add_and_read_no_tags_to_s3_file(s3_test_bucket, s3_test_file):
-    # Given
-    input_tags = {}
-    url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-
-    # When
-    url.write_tags(input_tags)
-
-    # Then
-    assert_that(url).has_s3_tags_equal_to({})
-
-
-def test_should_add_and_read_none_tags_to_s3_file(s3_test_bucket, s3_test_file):
-    # Given
-    input_tags = None
-
-    url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-
-    # When
-    url.write_tags(input_tags)
-
-    # Then
-    assert_that(url).has_s3_tags_equal_to({})
-
-
-def test_should_copy_s3_file_with_tags(s3_test_bucket, s3_test_file):
-    # Given
-    source_s3_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    target_s3_url = S3Url(f's3://{s3_test_bucket.name}/copied/{s3_test_file}')
-    s3_test_bucket.meta.client.put_object_tagging(
-        Bucket=s3_test_bucket.name,
-        Key=s3_test_file,
-        Tagging={
-            'TagSet': [
-                {'Key': 'tag1', 'Value': 'value1'},
-                {'Key': 'tag2', 'Value': 'value2'},
-            ]
-        }
-    )
-
-    # When
-    source_s3_url.copy_to(target_s3_url)
-
-    # Then
-    assert_that(target_s3_url).s3_file_exists()
-    assert_that(target_s3_url).has_s3_tags_equal_to({'tag1': 'value1', 'tag2': 'value2'})
-
-
-def test_should_copy_tags_to_url(s3_test_bucket, s3_test_file, s3_test_file_2):
-    # Given
-    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    target_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file_2}')
-
-    assert_that(source_url).has_s3_tags_equal_to({})
-    assert_that(target_url).has_s3_tags_equal_to({})
-
-    # When
-    source_url.write_tags({'tag1': 'value1', 'tag2': 'value2'})
-    source_url.copy_tags_to(target_url)
-
-    # Then
-    assert_that(target_url).s3_file_exists()
-    assert_that(target_url).has_s3_tags_equal_to({'tag1': 'value1', 'tag2': 'value2'})
-
-
-def test_should_copy_tags_to_str(s3_test_bucket, s3_test_file, s3_test_file_2):
-    # Given
-    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    target_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file_2}')
-
-    assert_that(source_url).has_s3_tags_equal_to({})
-    assert_that(target_url).has_s3_tags_equal_to({})
-
-    # When
-    source_url.write_tags({'tag1': 'value1', 'tag2': 'value2'})
-    source_url.copy_tags_to(target_url.url)
-
-    # Then
-    assert_that(target_url).has_s3_tags_equal_to({'tag1': 'value1', 'tag2': 'value2'})
-
-
-def test_should_copy_s3_file_with_no_tags(s3_test_bucket, s3_test_file, s3_test_file_2):
-    # Given
-    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    target_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file_2}')
-
-    assert_that(source_url).has_s3_tags_equal_to({})
-    assert_that(target_url).has_s3_tags_equal_to({})
-
-    # When
-    source_url.copy_tags_to(target_url)
-
-    # Then
-    assert_that(target_url.exists()).is_true()
-    assert_that(target_url).has_s3_tags_equal_to({})
-
-
-def test_transition_to_glacier(s3_test_bucket, s3_test_file):
-    # Given
-    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-
-    # When
-    source_url.transition_to_storage_tier("GLACIER")
-
-    # Then
-    assert_that(source_url.object.storage_class).is_equal_to("GLACIER")
-
-
-def test_shouldnt_transition_from_glacier(s3_test_bucket, s3_test_file):
-    # Given
-    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    source_url.transition_to_storage_tier("GLACIER")
-
-    # When
-    with pytest.raises(Exception):
-        source_url.transition_to_storage_tier("STANDARD")
-
-
-def test_transition_from_int_tiering(s3_test_bucket, s3_test_file):
-    # Given
-    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    source_url.transition_to_storage_tier("INTELLIGENT_TIERING")
-
-    # When
-    source_url.transition_to_storage_tier("STANDARD")
-
-
-def test_transition_from_onezone(s3_test_bucket, s3_test_file):
-    # Given
-    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    source_url.transition_to_storage_tier("ONEZONE_IA")
-
-    # When
-    source_url.transition_to_storage_tier("STANDARD")
-
-
-def test_transition_to_storage_tier(s3_test_bucket, s3_test_file):
-    # Given
-    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-
-    # When
-    source_url.transition_to_storage_tier("STANDARD_IA")
-
-    # Then
-    assert_that(source_url.object.storage_class).is_equal_to("STANDARD_IA")
-
-
-def test_restore_from_glacier(s3_test_bucket, s3_test_file):
-    # Given
-    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
-    source_url.transition_to_storage_tier("GLACIER")
-
-    # When
-    source_url.restore_to_storage_tier(1)
-
-    def assert_object_restored():
-        obj = source_url.object
-        assert_that(obj.restore).is_not_none().starts_with('ongoing-request="false"')
-
-    assert_with_timeout(assert_object_restored, 100, 1)
-    assert_that(source_url.object.storage_class).is_equal_to("GLACIER")
-    assert_that(source_url.object.restore).is_not_none().starts_with('ongoing-request="false"')
-
-    # When
-    source_url.restore_to_storage_tier(1, "Expedited")
-
-    assert_with_timeout(assert_object_restored, 100, 1)
-    assert_that(source_url.object.storage_class).is_equal_to("GLACIER")
+import json
+from pathlib import Path
+
+import boto3
+import pytest
+import requests
+from assertpy import assert_that
+from boto3 import s3
+from botocore.exceptions import ClientError
+from s3_url import S3Url
+from tests.conftest import TEST_BUCKET, assert_with_timeout
+
+
+def test_demo(s3_test_bucket, s3_demo_file):
+    file_url = S3Url(f's3://test-bucket/prefix/file.json')
+
+    # url component properties
+    assert file_url.bucket == 'test-bucket'
+    assert file_url.key == 'prefix/file.json'
+
+    # factory methods
+    file_url = S3Url.from_url('s3://test-bucket/prefix/file.json')
+    file_url = S3Url.from_bucket_key(bucket='test-bucket', key='prefix/file.json')
+
+    # access underlying boto3 s3 resource object
+    boto3_obj = file_url.object
+
+    # return url string
+    url_str: str = file_url.url
+    url_str: str = str(file_url)
+    assert url_str == 's3://test-bucket/prefix/file.json'
+
+    # check if file exists
+    exists: bool = file_url.exists()
+    assert exists
+
+    # check if any files exist in prefix (url should end with /)
+    prefix_exists = S3Url('s3://test-bucket/prefix/').prefix_exists()
+    assert prefix_exists
+
+    # read text/json
+    file_content: str = file_url.read_text()
+    file_content_json: json = file_url.read_json()
+
+    # delete file
+    file_url.delete()
+    assert not file_url.exists()
+
+    # write text/json
+    file_url.write_text("test data")
+    file_url.write_json({"testEntry": "test data"})
+    assert file_url.exists()
+
+    # copy to another object
+    file_url.copy_to('s3://test-bucket/prefix/file-copy.json')
+    S3Url('s3://test-bucket/prefix/another-file-copy.json').copy_from(file_url)
+
+    # delete all filed in prefix
+    prefix_url = S3Url('s3://test-bucket/prefix/')
+    prefix_url.delete_dir()
+
+    assert not prefix_url.prefix_exists()
+    assert not file_url.exists()
+
+
+def test_s3_url_parts(s3_test_bucket, s3_test_file):
+    url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    assert_that(url.url).is_equal_to(f's3://{TEST_BUCKET}/SomeFolder/test_file.json')
+    assert_that(url.bucket).is_equal_to(TEST_BUCKET)
+    assert_that(url.key).is_equal_to('SomeFolder/test_file.json')
+
+
+def test_factory_methods(s3_test_bucket, s3_test_file):
+    url = S3Url.from_url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    assert_that(url.url).is_equal_to(f's3://{TEST_BUCKET}/SomeFolder/test_file.json')
+    assert_that(url.bucket).is_equal_to(TEST_BUCKET)
+    assert_that(url.key).is_equal_to('SomeFolder/test_file.json')
+
+    url = S3Url.from_bucket_key(s3_test_bucket.name, s3_test_file)
+    assert_that(url.url).is_equal_to(f's3://{TEST_BUCKET}/SomeFolder/test_file.json')
+    assert_that(url.bucket).is_equal_to(TEST_BUCKET)
+    assert_that(url.key).is_equal_to('SomeFolder/test_file.json')
+
+
+def test_unsupported_url(s3_test_bucket):
+    with pytest.raises(Exception) as err:
+        S3Url(f'https://{s3_test_bucket.name}/some/path')
+    assert_that(str(err)).contains('Unsupported URL')
+
+
+def test_s3_url_exists(s3_test_bucket, s3_test_file):
+    existing_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    assert_that(existing_url.exists()).is_true()
+    non_existing_url = S3Url(f's3://{s3_test_bucket.name}/non_existing_file.txt')
+    assert_that(non_existing_url.exists()).is_false()
+
+
+def test_generate_presigned_url_get(s3_test_bucket, s3_test_file):
+    existing_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    get_url = existing_url.generate_presigned_url_get()
+    assert_that(requests.get(get_url).content.decode()).is_equal_to(existing_url.read_text())
+
+
+def test_generate_presigned_url_put(s3_test_bucket, s3_test_file):
+    non_existing_url = S3Url(f's3://{s3_test_bucket.name}/non_existing_file.txt')
+    get_url = non_existing_url.generate_presigned_url_put()
+    requests.put(get_url, data="test text file".encode()).raise_for_status()
+    assert_that(non_existing_url.read_text()).is_equal_to("test text file")
+
+
+def test_s3_url_exists_access_denied(s3_test_bucket, s3_test_file, monkeypatch):
+    existing_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    expected_exc = ClientError({'Error': {'Code': '403', 'Message': 'Forbidden'},
+                                'ResponseMetadata': {'HTTPStatusCode': 403, 'RetryAttempts': 0}}, 'HeadObject')
+
+    def raise_exc(*args, **kwargs):
+        raise expected_exc
+
+    monkeypatch.setattr(existing_url.object.meta.client, '_make_api_call', raise_exc)
+    assert_that(existing_url.exists).raises(ClientError).when_called_with()
+
+
+def test_s3_url_exists_for_a_path(s3_test_bucket, s3_test_file_3):
+    existing_url = S3Url(f's3://{s3_test_bucket.name}/a/path/to/')
+    assert_that(existing_url.prefix_exists()).is_true()
+    existing_url = S3Url(f's3://{s3_test_bucket.name}/a/path/to/the/file')
+    assert_that(existing_url.prefix_exists()).is_true()
+
+    non_existing_url = S3Url(f's3://{s3_test_bucket.name}/unknown/path/to/the/file')
+    assert_that(non_existing_url.prefix_exists()).is_false()
+
+
+def test_list_prefix_objects(s3_test_bucket):
+    file_1 = S3Url(f's3://{s3_test_bucket.name}/some_prefix/some_file_1.txt')
+    file_2 = S3Url(f's3://{s3_test_bucket.name}/some_prefix/some_file_2.txt')
+    file_3 = S3Url(f's3://{s3_test_bucket.name}/some_prefix/some_file_3.txt')
+
+    file_1.write_text("1")
+    file_2.write_text("2")
+    file_3.write_text("3")
+
+    existing_prefix_url = S3Url(f's3://{s3_test_bucket.name}/some_prefix/')
+    assert_that(list(existing_prefix_url.list_prefix_objects())).is_length(3).contains_only(file_1, file_2, file_3)
+
+
+def test_s3_url_exists_for_a_path_access_denied(s3_test_bucket, s3_test_file_3, monkeypatch):
+    existing_url = S3Url(f's3://{s3_test_bucket.name}/a/path/to/')
+    expected_exc = ClientError({'Error': {'Code': '403', 'Message': 'Forbidden'},
+                                'ResponseMetadata': {'HTTPStatusCode': 403, 'RetryAttempts': 0}}, 'ListObjects')
+
+    def raise_exc(*args, **kwargs):
+        raise expected_exc
+
+    monkeypatch.setattr(existing_url.object.meta.client, '_make_api_call', raise_exc)
+    assert_that(existing_url.prefix_exists).raises(ClientError).when_called_with()
+
+
+def test_s3_url_delete(s3_test_bucket, s3_test_file):
+    existing_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    assert_that(existing_url.exists()).is_true()
+    existing_url.delete()
+    assert_that(existing_url.exists()).is_false()
+    # should not fail if not exists
+    existing_url.delete()
+
+
+def test_s3_url_delete_dir(s3_test_bucket, s3_test_file):
+    existing_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    assert_that(existing_url.exists()).is_true()
+    prefix = S3Url(f's3://{s3_test_bucket.name}/SomeFolder/')
+    prefix.delete_dir()
+    assert_that(existing_url.exists()).is_false()
+
+
+def test_s3_url_read_write(s3_test_bucket, s3_test_file):
+    url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    assert_that(json.loads(url.read_text())).is_equal_to({
+        "testEntry1": "value1"
+    })
+    url.write_text(json.dumps({
+        "newField": "newValue"
+    }))
+    assert_that(url.object.server_side_encryption).is_none()
+
+    assert_that(json.loads(url.read_text())).is_equal_to({
+        "newField": "newValue"
+    })
+    url.write_text(json.dumps({
+        "newField": "newValue"
+    }), encryption='AES256')
+    assert_that(url.object.server_side_encryption).is_equal_to('AES256')
+
+
+def test_s3_url_read_write_json(s3_test_bucket, s3_test_file):
+    url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    assert_that(url.read_json()).is_equal_to({
+        "testEntry1": "value1"
+    })
+    url.write_json({
+        "newField": "newValue"
+    })
+    assert_that(url.object.server_side_encryption).is_none()
+
+    assert_that(url.read_json()).is_equal_to({
+        "newField": "newValue"
+    })
+    url.write_json({
+        "newField": "newValue"
+    }, encryption='AES256')
+    assert_that(url.object.server_side_encryption).is_equal_to('AES256')
+
+
+def test_s3_url_read_non_existing(s3_test_bucket):
+    non_existing_url = S3Url(f's3://{s3_test_bucket.name}/non_existing_file.txt')
+    with pytest.raises(ClientError) as err:
+        non_existing_url.read_text()
+    assert_that(str(err.value)).contains('NoSuchKey')
+    assert_that(str(err.value)).contains('The specified key does not exist')
+
+
+def test_s3_url_upload_file(s3_test_bucket):
+    url = S3Url(f's3://{s3_test_bucket.name}/some_new_file.json')
+    current_path = Path(__file__).resolve().parent
+    img_path = current_path / "resources" / "test_file.json"
+    with img_path.open(mode='rb') as fobj:
+        url.upload_file(fobj)
+    assert_that(json.loads(url.read_text())).is_equal_to({
+        "testEntry1": "value1"
+    })
+    assert_that(url.object.server_side_encryption).is_none()
+
+
+def test_s3_url_upload_file_encryption(s3_test_bucket):
+    url = S3Url(f's3://{s3_test_bucket.name}/some_new_file.json')
+    current_path = Path(__file__).resolve().parent
+    img_path = current_path / "resources" / "test_file.json"
+    with img_path.open(mode='rb') as fobj:
+        url.upload_file(fobj, encryption='AES256')
+    assert_that(json.loads(url.read_text())).is_equal_to({
+        "testEntry1": "value1"
+    })
+    assert_that(url.object.server_side_encryption).is_equal_to('AES256')
+
+
+def test_copy_to_url(s3_test_bucket, s3_test_file):
+    # Given
+    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    target_url = S3Url(f's3://{s3_test_bucket.name}/copied/{s3_test_file}')
+    assert_that(target_url).s3_file_does_not_exist()
+
+    # When
+    source_url.copy_to(target_url)
+
+    # Then
+    assert_that(target_url).s3_file_exists()
+
+
+def test_copy_to_str(s3_test_bucket, s3_test_file):
+    # Given
+    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    target_url = S3Url(f's3://{s3_test_bucket.name}/copied/{s3_test_file}')
+    assert_that(target_url).s3_file_does_not_exist()
+
+    # When
+    source_url.copy_to(target_url.url)
+
+    # Then
+    assert_that(target_url).s3_file_exists()
+
+
+def test_copy_from_url(s3_test_bucket, s3_test_file):
+    # Given
+    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    target_url = S3Url(f's3://{s3_test_bucket.name}/copied/{s3_test_file}')
+    assert_that(target_url).s3_file_does_not_exist()
+
+    # When
+    target_url.copy_from(source_url)
+
+    # Then
+    assert_that(target_url).s3_file_exists()
+
+
+def test_copy_from_str(s3_test_bucket, s3_test_file):
+    # Given
+    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    target_url = S3Url(f's3://{s3_test_bucket.name}/copied/{s3_test_file}')
+    assert_that(target_url).s3_file_does_not_exist()
+
+    # When
+    target_url.copy_from(source_url.url)
+
+    # Then
+    assert_that(target_url).s3_file_exists()
+
+
+def test_should_read_tags_to_s3_file(s3_test_bucket, s3_test_file):
+    # Given
+    url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    s3_test_bucket.meta.client.put_object_tagging(
+        Bucket=s3_test_bucket.name,
+        Key=s3_test_file,
+        Tagging={
+            'TagSet': [
+                {'Key': 'tag1', 'Value': 'value1'},
+                {'Key': 'tag2', 'Value': 'value2'},
+            ]
+        }
+    )
+
+    # Then
+    assert_that(url).has_s3_tags_equal_to({'tag1': 'value1', 'tag2': 'value2'})
+
+
+def test_should_add_and_read_no_tags_to_s3_file(s3_test_bucket, s3_test_file):
+    # Given
+    input_tags = {}
+    url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+
+    # When
+    url.write_tags(input_tags)
+
+    # Then
+    assert_that(url).has_s3_tags_equal_to({})
+
+
+def test_should_add_and_read_none_tags_to_s3_file(s3_test_bucket, s3_test_file):
+    # Given
+    input_tags = None
+
+    url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+
+    # When
+    url.write_tags(input_tags)
+
+    # Then
+    assert_that(url).has_s3_tags_equal_to({})
+
+
+def test_should_copy_s3_file_with_tags(s3_test_bucket, s3_test_file):
+    # Given
+    source_s3_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    target_s3_url = S3Url(f's3://{s3_test_bucket.name}/copied/{s3_test_file}')
+    s3_test_bucket.meta.client.put_object_tagging(
+        Bucket=s3_test_bucket.name,
+        Key=s3_test_file,
+        Tagging={
+            'TagSet': [
+                {'Key': 'tag1', 'Value': 'value1'},
+                {'Key': 'tag2', 'Value': 'value2'},
+            ]
+        }
+    )
+
+    # When
+    source_s3_url.copy_to(target_s3_url)
+
+    # Then
+    assert_that(target_s3_url).s3_file_exists()
+    assert_that(target_s3_url).has_s3_tags_equal_to({'tag1': 'value1', 'tag2': 'value2'})
+
+
+def test_should_copy_tags_to_url(s3_test_bucket, s3_test_file, s3_test_file_2):
+    # Given
+    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    target_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file_2}')
+
+    assert_that(source_url).has_s3_tags_equal_to({})
+    assert_that(target_url).has_s3_tags_equal_to({})
+
+    # When
+    source_url.write_tags({'tag1': 'value1', 'tag2': 'value2'})
+    source_url.copy_tags_to(target_url)
+
+    # Then
+    assert_that(target_url).s3_file_exists()
+    assert_that(target_url).has_s3_tags_equal_to({'tag1': 'value1', 'tag2': 'value2'})
+
+
+def test_should_copy_tags_to_str(s3_test_bucket, s3_test_file, s3_test_file_2):
+    # Given
+    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    target_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file_2}')
+
+    assert_that(source_url).has_s3_tags_equal_to({})
+    assert_that(target_url).has_s3_tags_equal_to({})
+
+    # When
+    source_url.write_tags({'tag1': 'value1', 'tag2': 'value2'})
+    source_url.copy_tags_to(target_url.url)
+
+    # Then
+    assert_that(target_url).has_s3_tags_equal_to({'tag1': 'value1', 'tag2': 'value2'})
+
+
+def test_should_copy_s3_file_with_no_tags(s3_test_bucket, s3_test_file, s3_test_file_2):
+    # Given
+    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    target_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file_2}')
+
+    assert_that(source_url).has_s3_tags_equal_to({})
+    assert_that(target_url).has_s3_tags_equal_to({})
+
+    # When
+    source_url.copy_tags_to(target_url)
+
+    # Then
+    assert_that(target_url.exists()).is_true()
+    assert_that(target_url).has_s3_tags_equal_to({})
+
+
+def test_transition_to_glacier(s3_test_bucket, s3_test_file):
+    # Given
+    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+
+    # When
+    source_url.transition_to_storage_tier("GLACIER")
+
+    # Then
+    assert_that(source_url.object.storage_class).is_equal_to("GLACIER")
+
+
+def test_shouldnt_transition_from_glacier(s3_test_bucket, s3_test_file):
+    # Given
+    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    source_url.transition_to_storage_tier("GLACIER")
+
+    # When
+    with pytest.raises(Exception):
+        source_url.transition_to_storage_tier("STANDARD")
+
+
+def test_transition_from_int_tiering(s3_test_bucket, s3_test_file):
+    # Given
+    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    source_url.transition_to_storage_tier("INTELLIGENT_TIERING")
+
+    # When
+    source_url.transition_to_storage_tier("STANDARD")
+
+
+def test_transition_from_onezone(s3_test_bucket, s3_test_file):
+    # Given
+    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    source_url.transition_to_storage_tier("ONEZONE_IA")
+
+    # When
+    source_url.transition_to_storage_tier("STANDARD")
+
+
+def test_transition_to_storage_tier(s3_test_bucket, s3_test_file):
+    # Given
+    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+
+    # When
+    source_url.transition_to_storage_tier("STANDARD_IA")
+
+    # Then
+    assert_that(source_url.object.storage_class).is_equal_to("STANDARD_IA")
+
+
+def test_restore_from_glacier(s3_test_bucket, s3_test_file):
+    # Given
+    source_url = S3Url(f's3://{s3_test_bucket.name}/{s3_test_file}')
+    source_url.transition_to_storage_tier("GLACIER")
+
+    # When
+    source_url.restore_to_storage_tier(1)
+
+    def assert_object_restored():
+        obj = source_url.object
+        assert_that(obj.restore).is_not_none().starts_with('ongoing-request="false"')
+
+    assert_with_timeout(assert_object_restored, 100, 1)
+    assert_that(source_url.object.storage_class).is_equal_to("GLACIER")
+    assert_that(source_url.object.restore).is_not_none().starts_with('ongoing-request="false"')
+
+    # When
+    source_url.restore_to_storage_tier(1, "Expedited")
+
+    assert_with_timeout(assert_object_restored, 100, 1)
+    assert_that(source_url.object.storage_class).is_equal_to("GLACIER")
```

