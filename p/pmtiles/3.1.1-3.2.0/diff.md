# Comparing `tmp/pmtiles-3.1.1.tar.gz` & `tmp/pmtiles-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmtiles-3.1.1.tar", last modified: Sun Apr 16 11:41:33 2023, max compression
+gzip compressed data, was "pmtiles-3.2.0.tar", last modified: Fri Jun 23 06:17:20 2023, max compression
```

## Comparing `pmtiles-3.1.1.tar` & `pmtiles-3.2.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-04-16 11:41:33.049441 pmtiles-3.1.1/
--rw-r--r--   0 bdon       (501) staff       (20)       54 2022-09-15 23:32:51.000000 pmtiles-3.1.1/.gitignore
--rw-r--r--   0 bdon       (501) staff       (20)      495 2023-04-16 11:41:33.049313 pmtiles-3.1.1/PKG-INFO
--rw-r--r--   0 bdon       (501) staff       (20)        0 2022-01-20 15:34:15.000000 pmtiles-3.1.1/README.md
-drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-04-16 11:41:33.046278 pmtiles-3.1.1/bin/
--rwxr-xr-x   0 bdon       (501) staff       (20)     1423 2022-11-21 14:51:38.000000 pmtiles-3.1.1/bin/pmtiles-convert
--rwxr-xr-x   0 bdon       (501) staff       (20)      142 2022-11-21 14:51:38.000000 pmtiles-3.1.1/bin/pmtiles-serve
--rwxr-xr-x   0 bdon       (501) staff       (20)      557 2022-11-21 14:51:38.000000 pmtiles-3.1.1/bin/pmtiles-show
-drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-04-16 11:41:33.046436 pmtiles-3.1.1/examples/
--rw-r--r--   0 bdon       (501) staff       (20)     1525 2022-11-21 14:51:38.000000 pmtiles-3.1.1/examples/create_raster_example.py
-drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-04-16 11:41:33.047732 pmtiles-3.1.1/pmtiles/
--rw-r--r--   0 bdon       (501) staff       (20)      111 2022-05-30 02:55:23.000000 pmtiles-3.1.1/pmtiles/__init__.py
--rw-r--r--   0 bdon       (501) staff       (20)     5570 2023-03-12 05:15:04.000000 pmtiles-3.1.1/pmtiles/convert.py
--rw-r--r--   0 bdon       (501) staff       (20)     2451 2022-11-21 14:51:38.000000 pmtiles-3.1.1/pmtiles/reader.py
--rw-r--r--   0 bdon       (501) staff       (20)     7238 2023-02-01 10:17:57.000000 pmtiles-3.1.1/pmtiles/tile.py
--rw-r--r--   0 bdon       (501) staff       (20)     3090 2023-02-01 10:17:57.000000 pmtiles-3.1.1/pmtiles/v2.py
--rw-r--r--   0 bdon       (501) staff       (20)     4474 2022-11-21 14:51:38.000000 pmtiles-3.1.1/pmtiles/writer.py
-drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-04-16 11:41:33.048273 pmtiles-3.1.1/pmtiles.egg-info/
--rw-r--r--   0 bdon       (501) staff       (20)      495 2023-04-16 11:41:32.000000 pmtiles-3.1.1/pmtiles.egg-info/PKG-INFO
--rw-r--r--   0 bdon       (501) staff       (20)      443 2023-04-16 11:41:32.000000 pmtiles-3.1.1/pmtiles.egg-info/SOURCES.txt
--rw-r--r--   0 bdon       (501) staff       (20)        1 2023-04-16 11:41:32.000000 pmtiles-3.1.1/pmtiles.egg-info/dependency_links.txt
--rw-r--r--   0 bdon       (501) staff       (20)       13 2023-04-16 11:41:32.000000 pmtiles-3.1.1/pmtiles.egg-info/top_level.txt
--rw-r--r--   0 bdon       (501) staff       (20)       38 2023-04-16 11:41:33.049479 pmtiles-3.1.1/setup.cfg
--rw-r--r--   0 bdon       (501) staff       (20)      813 2023-04-16 11:40:58.000000 pmtiles-3.1.1/setup.py
-drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-04-16 11:41:33.049096 pmtiles-3.1.1/test/
--rw-r--r--   0 bdon       (501) staff       (20)        0 2022-05-30 02:55:23.000000 pmtiles-3.1.1/test/__init__.py
--rw-r--r--   0 bdon       (501) staff       (20)     3157 2022-11-21 14:51:38.000000 pmtiles-3.1.1/test/test_convert.py
--rw-r--r--   0 bdon       (501) staff       (20)     1206 2022-11-21 14:51:38.000000 pmtiles-3.1.1/test/test_reader.py
--rw-r--r--   0 bdon       (501) staff       (20)     7871 2023-02-01 09:15:14.000000 pmtiles-3.1.1/test/test_tile.py
--rw-r--r--   0 bdon       (501) staff       (20)       16 2022-11-21 14:51:38.000000 pmtiles-3.1.1/test/test_writer.py
+drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-06-23 06:17:20.328653 pmtiles-3.2.0/
+-rw-r--r--   0 bdon       (501) staff       (20)       54 2022-09-15 23:32:51.000000 pmtiles-3.2.0/.gitignore
+-rw-r--r--   0 bdon       (501) staff       (20)      495 2023-06-23 06:17:20.328502 pmtiles-3.2.0/PKG-INFO
+-rw-r--r--   0 bdon       (501) staff       (20)        0 2022-01-20 15:34:15.000000 pmtiles-3.2.0/README.md
+drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-06-23 06:17:20.325884 pmtiles-3.2.0/bin/
+-rwxr-xr-x   0 bdon       (501) staff       (20)     1423 2022-11-21 14:51:38.000000 pmtiles-3.2.0/bin/pmtiles-convert
+-rwxr-xr-x   0 bdon       (501) staff       (20)      142 2022-11-21 14:51:38.000000 pmtiles-3.2.0/bin/pmtiles-serve
+-rwxr-xr-x   0 bdon       (501) staff       (20)      557 2022-11-21 14:51:38.000000 pmtiles-3.2.0/bin/pmtiles-show
+drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-06-23 06:17:20.326029 pmtiles-3.2.0/examples/
+-rw-r--r--   0 bdon       (501) staff       (20)     1525 2022-11-21 14:51:38.000000 pmtiles-3.2.0/examples/create_raster_example.py
+drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-06-23 06:17:20.327009 pmtiles-3.2.0/pmtiles/
+-rw-r--r--   0 bdon       (501) staff       (20)      111 2022-05-30 02:55:23.000000 pmtiles-3.2.0/pmtiles/__init__.py
+-rw-r--r--   0 bdon       (501) staff       (20)     6275 2023-06-23 06:13:40.000000 pmtiles-3.2.0/pmtiles/convert.py
+-rw-r--r--   0 bdon       (501) staff       (20)     2418 2023-06-21 13:08:35.000000 pmtiles-3.2.0/pmtiles/reader.py
+-rw-r--r--   0 bdon       (501) staff       (20)     7524 2023-06-23 04:01:37.000000 pmtiles-3.2.0/pmtiles/tile.py
+-rw-r--r--   0 bdon       (501) staff       (20)     3090 2023-06-21 11:59:52.000000 pmtiles-3.2.0/pmtiles/v2.py
+-rw-r--r--   0 bdon       (501) staff       (20)     4872 2023-06-23 04:01:37.000000 pmtiles-3.2.0/pmtiles/writer.py
+drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-06-23 06:17:20.327469 pmtiles-3.2.0/pmtiles.egg-info/
+-rw-r--r--   0 bdon       (501) staff       (20)      495 2023-06-23 06:17:20.000000 pmtiles-3.2.0/pmtiles.egg-info/PKG-INFO
+-rw-r--r--   0 bdon       (501) staff       (20)      430 2023-06-23 06:17:20.000000 pmtiles-3.2.0/pmtiles.egg-info/SOURCES.txt
+-rw-r--r--   0 bdon       (501) staff       (20)        1 2023-06-23 06:17:20.000000 pmtiles-3.2.0/pmtiles.egg-info/dependency_links.txt
+-rw-r--r--   0 bdon       (501) staff       (20)       13 2023-06-23 06:17:20.000000 pmtiles-3.2.0/pmtiles.egg-info/top_level.txt
+-rw-r--r--   0 bdon       (501) staff       (20)       38 2023-06-23 06:17:20.328693 pmtiles-3.2.0/setup.cfg
+-rw-r--r--   0 bdon       (501) staff       (20)      813 2023-06-23 06:14:25.000000 pmtiles-3.2.0/setup.py
+drwxr-xr-x   0 bdon       (501) staff       (20)        0 2023-06-23 06:17:20.327893 pmtiles-3.2.0/test/
+-rw-r--r--   0 bdon       (501) staff       (20)        0 2022-05-30 02:55:23.000000 pmtiles-3.2.0/test/__init__.py
+-rw-r--r--   0 bdon       (501) staff       (20)     3641 2023-06-23 04:01:37.000000 pmtiles-3.2.0/test/test_convert.py
+-rw-r--r--   0 bdon       (501) staff       (20)     1755 2023-06-23 04:01:37.000000 pmtiles-3.2.0/test/test_reader_writer.py
+-rw-r--r--   0 bdon       (501) staff       (20)     7918 2023-06-21 13:08:35.000000 pmtiles-3.2.0/test/test_tile.py
```

### Comparing `pmtiles-3.1.1/bin/pmtiles-convert` & `pmtiles-3.2.0/bin/pmtiles-convert`

 * *Files identical despite different names*

### Comparing `pmtiles-3.1.1/bin/pmtiles-show` & `pmtiles-3.2.0/bin/pmtiles-show`

 * *Files identical despite different names*

### Comparing `pmtiles-3.1.1/examples/create_raster_example.py` & `pmtiles-3.2.0/examples/create_raster_example.py`

 * *Files identical despite different names*

### Comparing `pmtiles-3.1.1/pmtiles/convert.py` & `pmtiles-3.2.0/pmtiles/convert.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,21 +31,23 @@
         header["tile_type"] = TileType.MVT
     elif tile_format == "png":
         header["tile_type"] = TileType.PNG
     elif tile_format == "jpeg":
         header["tile_type"] = TileType.JPEG
     elif tile_format == "webp":
         header["tile_type"] = TileType.WEBP
+    elif tile_format == "avif":
+        header["tile_type"] = TileType.AVIF
     else:
         header["tile_type"] = TileType.UNKNOWN
 
-    if mbtiles_metadata.get("compression") == "gzip":
-        header["tile_compression"] = Compression.GZIP  # TODO: does this ever matter?
+    if tile_format == "pbf" or mbtiles_metadata.get("compression") == "gzip":
+        header["tile_compression"] = Compression.GZIP
     else:
-        header["tile_compression"] = Compression.UNKNOWN
+        header["tile_compression"] = Compression.NONE
 
     return header, mbtiles_metadata
 
 
 def mbtiles_to_pmtiles(input, output, maxzoom):
     conn = sqlite3.connect(input)
     cursor = conn.cursor()
@@ -59,33 +61,37 @@
             (maxzoom or 99,),
         ):
             flipped = (1 << row[0]) - 1 - row[2]
             tileid_set.append(zxy_to_tileid(row[0], row[1], flipped))
 
         tileid_set.sort()
 
+        mbtiles_metadata = {}
+        for row in cursor.execute("SELECT name,value FROM metadata"):
+            mbtiles_metadata[row[0]] = row[1]
+        is_pbf = mbtiles_metadata["format"] == "pbf"
+
         # query the db in ascending tile order
         for tileid in tileid_set:
             z, x, y = tileid_to_zxy(tileid)
             flipped = (1 << z) - 1 - y
             res = cursor.execute(
                 "SELECT tile_data FROM tiles WHERE zoom_level = ? AND tile_column = ? AND tile_row = ?",
                 (z, x, flipped),
             )
             data = res.fetchone()[0]
             # force gzip compression only for vector
-            if data[0:2] != b"\x1f\x8b":
+            if is_pbf and data[0:2] != b"\x1f\x8b":
                 data = gzip.compress(data)
             writer.write_tile(tileid, data)
 
-        mbtiles_metadata = {}
-        for row in cursor.execute("SELECT name,value FROM metadata"):
-            mbtiles_metadata[row[0]] = row[1]
-
         pmtiles_header, pmtiles_metadata = mbtiles_to_header_json(mbtiles_metadata)
+        if maxzoom:
+            pmtiles_header["max_zoom"] = int(maxzoom)
+            mbtiles_metadata["maxzoom"] = maxzoom
         result = writer.finalize(pmtiles_header, pmtiles_metadata)
 
     conn.close()
 
 
 def pmtiles_to_mbtiles(input, output):
     conn = sqlite3.connect(output)
@@ -121,19 +127,32 @@
             center_zoom = header["center_zoom"]
             metadata["center"] = f"{center_lon},{center_lat},{center_zoom}"
 
         if "format" not in metadata:
             if header["tile_type"] == TileType.MVT:
                 metadata["format"] = "pbf"
 
+        json_metadata = {}
         for k, v in metadata.items():
-            if not isinstance(v, str):
+            if k == "vector_layers":
+                json_metadata["vector_layers"] = v
+                continue
+            elif k == "tilestats":
+                json_metadata["tilestats"] = v
+                continue
+            elif not isinstance(v, str):
                 v = json.dumps(v, ensure_ascii=False)
             cursor.execute("INSERT INTO metadata VALUES(?,?)", (k, v))
 
+        if len(json_metadata) > 0:
+            cursor.execute(
+                "INSERT INTO metadata VALUES(?,?)",
+                ("json", json.dumps(json_metadata, ensure_ascii=False)),
+            )
+
         for zxy, tile_data in all_tiles(source):
             flipped_y = (1 << zxy[0]) - 1 - zxy[2]
             cursor.execute(
                 "INSERT INTO tiles VALUES(?,?,?,?)",
                 (zxy[0], zxy[1], flipped_y, tile_data),
             )
```

### Comparing `pmtiles-3.1.1/pmtiles/reader.py` & `pmtiles-3.2.0/pmtiles/reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     find_tile,
     Compression,
 )
 import gzip
 
 
 def MmapSource(f):
-    mapping = mmap.mmap(f.fileno(), 0)
+    mapping = mmap.mmap(f.fileno(), 0, access=mmap.ACCESS_READ)
 
     def get_bytes(offset, length):
         return mapping[offset : offset + length]
 
     return get_bytes
 
 
@@ -31,23 +31,23 @@
     def __init__(self, get_bytes):
         self.get_bytes = get_bytes
 
     def header(self):
         return deserialize_header(self.get_bytes(0, 127))
 
     def metadata(self):
-        header = deserialize_header(self.get_bytes(0, 127))
+        header = self.header()
         metadata = self.get_bytes(header["metadata_offset"], header["metadata_length"])
         if header["internal_compression"] == Compression.GZIP:
             metadata = gzip.decompress(metadata)
         return json.loads(metadata)
 
     def get(self, z, x, y):
         tile_id = zxy_to_tileid(z, x, y)
-        header = deserialize_header(self.get_bytes(0, 127))
+        header = self.header()
         dir_offset = header["root_offset"]
         dir_length = header["root_length"]
         for depth in range(0, 4):  # max depth
             directory = deserialize_directory(self.get_bytes(dir_offset, dir_length))
             result = find_tile(directory, tile_id)
             if result:
                 if result.run_length == 0:
```

### Comparing `pmtiles-3.1.1/pmtiles/tile.py` & `pmtiles-3.2.0/pmtiles/tile.py`

 * *Files 7% similar despite different names*

```diff
@@ -138,14 +138,15 @@
 
 class TileType(Enum):
     UNKNOWN = 0
     MVT = 1
     PNG = 2
     JPEG = 3
     WEBP = 4
+    AVIF = 5
 
 
 def deserialize_directory(buf):
     b_io = io.BytesIO(gzip.decompress(buf))
     entries = []
     num_entries = read_varint(b_io)
 
@@ -210,14 +211,15 @@
     def read_uint64(pos):
         return int.from_bytes(buf[pos : pos + 8], byteorder="little")
 
     def read_int32(pos):
         return int.from_bytes(buf[pos : pos + 4], byteorder="little", signed=True)
 
     return {
+        "version": buf[7],
         "root_offset": read_uint64(8),
         "root_length": read_uint64(16),
         "metadata_offset": read_uint64(24),
         "metadata_length": read_uint64(32),
         "leaf_directory_offset": read_uint64(40),
         "leaf_directory_length": read_uint64(48),
         "tile_data_offset": read_uint64(56),
@@ -268,16 +270,20 @@
     write_uint64(h.get("tile_contents_count", 0))
     b_io.write(b"\x01" if h["clustered"] else b"\x00")
     write_uint8(h["internal_compression"].value)
     write_uint8(h["tile_compression"].value)
     write_uint8(h["tile_type"].value)
     write_uint8(h["min_zoom"])
     write_uint8(h["max_zoom"])
-    write_int32(h["min_lon_e7"])
-    write_int32(h["min_lat_e7"])
-    write_int32(h["max_lon_e7"])
-    write_int32(h["max_lat_e7"])
-    write_uint8(h["center_zoom"])
-    write_int32(h["center_lon_e7"])
-    write_int32(h["center_lat_e7"])
+    min_lon_e7 = h.get("min_lon_e7",-180)
+    write_int32(min_lon_e7)
+    min_lat_e7 = h.get("min_lat_e7",-90)
+    write_int32(min_lat_e7)
+    max_lon_e7 = h.get("max_lon_e7",180)
+    write_int32(max_lon_e7)
+    max_lat_e7 = h.get("max_lat_e7",90)
+    write_int32(max_lat_e7)
+    write_uint8(h.get("center_zoom",h["min_zoom"]))
+    write_int32(h.get("center_lon_e7", round((min_lon_e7 + max_lon_e7) / 2)))
+    write_int32(h.get("center_lat_e7", round((min_lat_e7 + max_lat_e7) / 2)))
 
     return b_io.getvalue()
```

### Comparing `pmtiles-3.1.1/pmtiles/v2.py` & `pmtiles-3.2.0/pmtiles/v2.py`

 * *Files identical despite different names*

### Comparing `pmtiles-3.1.1/pmtiles/writer.py` & `pmtiles-3.2.0/pmtiles/writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import json
 import tempfile
 import gzip
 import shutil
 from contextlib import contextmanager
-from .tile import Entry, serialize_directory, Compression, serialize_header
+from .tile import (
+    Entry,
+    serialize_directory,
+    Compression,
+    serialize_header,
+    tileid_to_zxy,
+)
 
 
 @contextmanager
 def write(fname):
     f = open(fname, "wb")
     w = Writer(f)
     try:
@@ -51,17 +57,20 @@
     def __init__(self, f):
         self.f = f
         self.tile_entries = []
         self.hash_to_offset = {}
         self.tile_f = tempfile.TemporaryFile()
         self.offset = 0
         self.addressed_tiles = 0
+        self.clustered = True
 
-    # TODO enforce ordered writes
     def write_tile(self, tileid, data):
+        if len(self.tile_entries) > 0 and tileid < self.tile_entries[-1].tile_id:
+            self.clustered = False
+
         hsh = hash(data)
         if hsh in self.hash_to_offset:
             last = self.tile_entries[-1]
             found = self.hash_to_offset[hsh]
             if tileid == last.tile_id + last.run_length and last.offset == found:
                 self.tile_entries[-1].run_length += 1
             else:
@@ -79,14 +88,19 @@
         print("# of tile entries (after RLE):", len(self.tile_entries))
         print("# of tile contents:", len(self.hash_to_offset))
 
         header["addressed_tiles_count"] = self.addressed_tiles
         header["tile_entries_count"] = len(self.tile_entries)
         header["tile_contents_count"] = len(self.hash_to_offset)
 
+        self.tile_entries = sorted(self.tile_entries, key=lambda e: e.tile_id)
+
+        header["min_zoom"] = tileid_to_zxy(self.tile_entries[0].tile_id)[0]
+        header["max_zoom"] = tileid_to_zxy(self.tile_entries[-1].tile_id)[0]
+
         root_bytes, leaves_bytes, num_leaves = optimize_directories(
             self.tile_entries, 16384 - 127
         )
 
         if num_leaves > 0:
             print("Root dir bytes:", len(root_bytes))
             print("Leaves dir bytes:", len(leaves_bytes))
@@ -101,15 +115,15 @@
             print("Total dir bytes:", len(root_bytes))
             print(
                 "Average bytes per addressed tile:",
                 len(root_bytes) / self.addressed_tiles,
             )
 
         compressed_metadata = gzip.compress(json.dumps(metadata).encode())
-        header["clustered"] = True
+        header["clustered"] = self.clustered
         header["internal_compression"] = Compression.GZIP
         header["root_offset"] = 127
         header["root_length"] = len(root_bytes)
         header["metadata_offset"] = header["root_offset"] + header["root_length"]
         header["metadata_length"] = len(compressed_metadata)
         header["leaf_directory_offset"] = (
             header["metadata_offset"] + header["metadata_length"]
```

### Comparing `pmtiles-3.1.1/setup.py` & `pmtiles-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pmtiles",
-    version="3.1.1",
+    version="3.2.0",
     author="Brandon Liu",
     author_email="brandon@protomaps.com",
     description="Library and utilities to write and read PMTiles files - cloud-optimized archives of map tiles.",
     license="BSD-3-Clause",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/protomaps/pmtiles",
```

### Comparing `pmtiles-3.1.1/test/test_convert.py` & `pmtiles-3.2.0/test/test_convert.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import unittest
+import sqlite3
 from io import BytesIO
 import os
+import json
 from pmtiles.writer import Writer
 from pmtiles.reader import Reader, MemorySource
 from pmtiles.convert import (
     pmtiles_to_mbtiles,
     mbtiles_to_pmtiles,
     mbtiles_to_header_json,
 )
@@ -47,18 +49,27 @@
                     "max_lon_e7": 0,
                     "min_lat_e7": 0,
                     "max_lat_e7": 0,
                     "center_zoom": 0,
                     "center_lon_e7": 0,
                     "center_lat_e7": 0,
                 },
-                {"": "value"},
+                {"vector_layers": ['vector','layers'],
+                "tilestats":{'tile':'stats'}},
             )
 
         pmtiles_to_mbtiles("test_tmp.pmtiles", "test_tmp.mbtiles")
+        conn = sqlite3.connect('test_tmp.mbtiles')
+        cursor = conn.cursor()
+        res = cursor.execute("SELECT value from metadata where name = 'json'")
+        data = res.fetchone()[0]
+        json_metadata = json.loads(data)
+        self.assertEqual(json_metadata['vector_layers'], ['vector', 'layers'])
+        self.assertEqual(json_metadata['tilestats'], {'tile':'stats'})
+
         mbtiles_to_pmtiles("test_tmp.mbtiles", "test_tmp_2.pmtiles", 3)
 
     def test_mbtiles_header(self):
         header, json_metadata = mbtiles_to_header_json(
             {
                 "name": "test_name",
                 "format": "pbf",
```

### Comparing `pmtiles-3.1.1/test/test_tile.py` & `pmtiles-3.2.0/test/test_tile.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,15 @@
             "max_lat_e7": int(2.2 * 10000000),
             "center_zoom": 3,
             "center_lon_e7": int(3.1 * 10000000),
             "center_lat_e7": int(3.2 * 10000000),
         }
         serialized = serialize_header(header)
         result = deserialize_header(serialized)
+        self.assertEqual(result['version'], 3)
         self.assertEqual(result["root_offset"], 1)
         self.assertEqual(result["root_length"], 2)
         self.assertEqual(result["metadata_offset"], 3)
         self.assertEqual(result["metadata_length"], 4)
         self.assertEqual(result["leaf_directory_offset"], 5)
         self.assertEqual(result["leaf_directory_length"], 6)
         self.assertEqual(result["tile_data_offset"], 7)
```

