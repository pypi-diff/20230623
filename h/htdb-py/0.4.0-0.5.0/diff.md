# Comparing `tmp/htdb-py-0.4.0.tar.gz` & `tmp/htdb-py-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htdb-py-0.4.0.tar", last modified: Thu Jun 22 11:10:29 2023, max compression
+gzip compressed data, was "htdb-py-0.5.0.tar", last modified: Fri Jun 23 08:05:21 2023, max compression
```

## Comparing `htdb-py-0.4.0.tar` & `htdb-py-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 11:10:30.000000 htdb-py-0.4.0/
--rw-rw-rw-   0        0        0    11558 2023-06-17 09:16:02.000000 htdb-py-0.4.0/LICENSE
--rw-rw-rw-   0        0        0       18 2023-06-17 09:35:40.000000 htdb-py-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0      123 2023-06-22 11:10:30.000000 htdb-py-0.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 11:10:30.000000 htdb-py-0.4.0/htdb/
--rw-rw-rw-   0        0        0    13075 2023-06-19 14:03:48.000000 htdb-py-0.4.0/htdb/dict.c
--rw-rw-rw-   0        0        0     2705 2023-06-17 08:31:04.000000 htdb-py-0.4.0/htdb/dict.h
--rw-rw-rw-   0        0        0     8066 2023-06-18 10:00:50.000000 htdb-py-0.4.0/htdb/htdb.c
--rw-rw-rw-   0        0        0     1672 2023-06-17 08:31:04.000000 htdb-py-0.4.0/htdb/htdb.h
--rw-rw-rw-   0        0        0    14397 2023-06-14 11:09:50.000000 htdb-py-0.4.0/htdb/siphash.c
--rw-rw-rw-   0        0        0      254 2023-06-15 13:51:52.000000 htdb-py-0.4.0/htdb/siphash.h
-drwxrwxrwx   0        0        0        0 2023-06-22 11:10:30.000000 htdb-py-0.4.0/htdb_py.egg-info/
--rw-rw-rw-   0        0        0      123 2023-06-22 11:10:30.000000 htdb-py-0.4.0/htdb_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-06-22 11:10:30.000000 htdb-py-0.4.0/htdb_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 11:10:30.000000 htdb-py-0.4.0/htdb_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 09:04:40.000000 htdb-py-0.4.0/htdb_py.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-06-22 11:10:30.000000 htdb-py-0.4.0/htdb_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-22 11:10:30.000000 htdb-py-0.4.0/htdb_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2023-06-17 09:30:36.000000 htdb-py-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 11:10:30.000000 htdb-py-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      548 2023-06-22 11:07:56.000000 htdb-py-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 11:10:30.000000 htdb-py-0.4.0/src/
--rw-rw-rw-   0        0        0     6109 2023-06-21 13:56:08.000000 htdb-py-0.4.0/src/bindings.cpp
+drwxrwxrwx   0        0        0        0 2023-06-23 08:05:20.000000 htdb-py-0.5.0/
+-rw-rw-rw-   0        0        0    11558 2023-06-17 09:16:02.000000 htdb-py-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-06-17 09:35:40.000000 htdb-py-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      123 2023-06-23 08:05:22.000000 htdb-py-0.5.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-23 08:05:20.000000 htdb-py-0.5.0/htdb/
+-rw-rw-rw-   0        0        0    13075 2023-06-19 14:03:48.000000 htdb-py-0.5.0/htdb/dict.c
+-rw-rw-rw-   0        0        0     2705 2023-06-17 08:31:04.000000 htdb-py-0.5.0/htdb/dict.h
+-rw-rw-rw-   0        0        0     9059 2023-06-23 07:58:26.000000 htdb-py-0.5.0/htdb/htdb.c
+-rw-rw-rw-   0        0        0     1842 2023-06-23 08:02:18.000000 htdb-py-0.5.0/htdb/htdb.h
+-rw-rw-rw-   0        0        0    14397 2023-06-14 11:09:50.000000 htdb-py-0.5.0/htdb/siphash.c
+-rw-rw-rw-   0        0        0      254 2023-06-15 13:51:52.000000 htdb-py-0.5.0/htdb/siphash.h
+drwxrwxrwx   0        0        0        0 2023-06-23 08:05:20.000000 htdb-py-0.5.0/htdb_py.egg-info/
+-rw-rw-rw-   0        0        0      123 2023-06-23 08:05:20.000000 htdb-py-0.5.0/htdb_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-06-23 08:05:20.000000 htdb-py-0.5.0/htdb_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 08:05:20.000000 htdb-py-0.5.0/htdb_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 09:04:40.000000 htdb-py-0.5.0/htdb_py.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-06-23 08:05:20.000000 htdb-py-0.5.0/htdb_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-23 08:05:20.000000 htdb-py-0.5.0/htdb_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2023-06-17 09:30:36.000000 htdb-py-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 08:05:22.000000 htdb-py-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      548 2023-06-23 08:00:08.000000 htdb-py-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:05:20.000000 htdb-py-0.5.0/src/
+-rw-rw-rw-   0        0        0     6303 2023-06-23 08:01:22.000000 htdb-py-0.5.0/src/bindings.cpp
```

### Comparing `htdb-py-0.4.0/LICENSE` & `htdb-py-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `htdb-py-0.4.0/htdb/dict.c` & `htdb-py-0.5.0/htdb/dict.c`

 * *Files identical despite different names*

### Comparing `htdb-py-0.4.0/htdb/dict.h` & `htdb-py-0.5.0/htdb/dict.h`

 * *Files identical despite different names*

### Comparing `htdb-py-0.4.0/htdb/htdb.c` & `htdb-py-0.5.0/htdb/htdb.c`

 * *Files 16% similar despite different names*

```diff
@@ -197,14 +197,23 @@
     xobj *valobj = xobjNew(XOBJ_TYPE_BYTES, (char *)value_, value_len);
 
     dictSet(db->table, (void *)keyobj, (void *)valobj);
 
     return 1;
 }
 
+int _xdbSetBytesInt(xdb *db, const char *key_, xobjlen_t key_len, uint64_t value_) {
+    xobj *keyobj = xobjNew(XOBJ_TYPE_BYTES, (char *)key_, key_len);
+    xobj *valobj = xobjNew(XOBJ_TYPE_INT, (char *)&value_, sizeof(value_));
+
+    dictSet(db->table, (void *)keyobj, (void *)valobj);
+
+    return 1;
+}
+
 int _xdbGetIntBytes(xdb *db, uint64_t key_, char **value_, xobjlen_t *value_len) {
     xobjlen_t key_len = sizeof(key_);
 
     xobj *keyobj = xobjNew(XOBJ_TYPE_INT, (char *)&key_, key_len);
 
     if (!dictHas(db->table, keyobj)) {
         return -1;
@@ -243,14 +252,38 @@
 
     if (!dictHas(db->table, keyobj)) {
         return -1;
     }
     xobj *valobj = (xobj *)dictGet(db->table, keyobj);
 
     if (valobj->len == 1) {
+        *value = *(uint8_t *)valobj->data;
+    } else if (valobj->len == 2) {
+        *value = *(uint16_t *)valobj->data;
+    } else if (valobj->len == 4) {
+        *value = *(uint32_t *)valobj->data;
+    } else if (valobj->len == 8) {
+        *value = *(uint64_t *)valobj->data;
+    } else {
+        assert(0);
+    }
+
+    free(keyobj);
+    return 0;
+}
+
+int _xdbGetBytesInt(xdb *db, const char *key_, xobjlen_t key_len, uint64_t *value) {
+    xobj *keyobj = xobjNew(XOBJ_TYPE_BYTES, (char *)key_, key_len);
+
+    if (!dictHas(db->table, keyobj)) {
+        return -1;
+    }
+    xobj *valobj = (xobj *)dictGet(db->table, keyobj);
+
+    if (valobj->len == 1) {
         *value = *(uint8_t *)valobj->data;
     } else if (valobj->len == 2) {
         *value = *(uint16_t *)valobj->data;
     } else if (valobj->len == 4) {
         *value = *(uint32_t *)valobj->data;
     } else if (valobj->len == 8) {
         *value = *(uint64_t *)valobj->data;
```

### Comparing `htdb-py-0.4.0/htdb/htdb.h` & `htdb-py-0.5.0/htdb/htdb.h`

 * *Files 7% similar despite different names*

```diff
@@ -39,17 +39,19 @@
 void xdbFree(xdb *db);
 size_t xdbSize(xdb *db);
 void xdbDump(xdb *db, FILE *stream);
 void xdbLoad(xdb *db, FILE *stream);
 int _xdbSetIntBytes(xdb *db, uint64_t key_, const char *value_, xobjlen_t value_len);
 int _xdbSetIntInt(xdb *db, uint64_t key_, uint64_t value_);
 int _xdbSetBytesBytes(xdb *db, const char *key_, xobjlen_t key_len, const char *value_, xobjlen_t value_len);
+int _xdbSetBytesInt(xdb *db, const char *key_, xobjlen_t key_len, uint64_t value_);
 int _xdbGetIntBytes(xdb *db, uint64_t key_, char **value_, xobjlen_t *value_len);
 int _xdbGetBytesBytes(xdb *db, const char *key_, xobjlen_t key_len, char **value_, xobjlen_t *value_len);
 int _xdbGetIntInt(xdb *db, uint64_t key_, uint64_t *value);
+int _xdbGetBytesInt(xdb *db, const char *key_, xobjlen_t key_len, uint64_t *value);
 
 xobj *xdbGetByInt(xdb *db, uint64_t key_);
 xobj *xdbGetByBytes(xdb *db, const char *key_, xobjlen_t key_len);
 bool xdbHasInt(xdb *db, uint64_t key_);
 bool xdbHasBytes(xdb *db, const char *key_, xobjlen_t key_len);
 bool xdbDelInt(xdb *db, uint64_t key_);
 bool xdbDelBytes(xdb *db, const char *key_, xobjlen_t key_len);
```

### Comparing `htdb-py-0.4.0/htdb/siphash.c` & `htdb-py-0.5.0/htdb/siphash.c`

 * *Files identical despite different names*

### Comparing `htdb-py-0.4.0/setup.py` & `htdb-py-0.5.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import glob
 
 from setuptools import setup
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 
 ext_modules=[
     Pybind11Extension(
         name="htdb",
         sources=sorted(glob.glob("htdb/*.c")) + sorted(glob.glob("src/*.cpp")),
         include_dirs=["htdb/"],
```

### Comparing `htdb-py-0.4.0/src/bindings.cpp` & `htdb-py-0.5.0/src/bindings.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,17 @@
 
         } else if (py::isinstance<py::bytes>(key_) || py::isinstance<py::str>(key_)) {
             std::string key = key_.cast<std::string>();
 
             if (py::isinstance<py::bytes>(value_) || py::isinstance<py::str>(value_)) {
                 std::string value = value_.cast<std::string>();
                 _xdbSetBytesBytes(_db, key.c_str(), static_cast<xobjlen_t>(key.length()), value.c_str(), static_cast<xobjlen_t>(value.length()));
+            } else if (py::isinstance<py::int_>(value_)) {
+                uint64_t value = value_.cast<uint64_t>();
+                _xdbSetBytesInt(_db, key.c_str(), static_cast<xobjlen_t>(key.length()), value);
             } else {
                 throw py::type_error("invalid value type");
             }
 
         } else {
             throw py::type_error("key must be int, bytes or str");
         }
@@ -65,19 +68,17 @@
 
     auto get(py::object key_) -> py::object {
         xobj *valobj = NULL;
 
         if (py::isinstance<py::int_>(key_)) {
             uint64_t key = key_.cast<uint64_t>();
             valobj = xdbGetByInt(_db, key);
-
         } else if (py::isinstance<py::bytes>(key_) || py::isinstance<py::str>(key_)) {
             std::string key = key_.cast<std::string>();
             valobj = xdbGetByBytes(_db, key.c_str(), static_cast<xobjlen_t>(key.length()));
-
         } else {
             throw py::type_error("invalid key type");
         }
 
         if (valobj == NULL) {
             throw py::key_error("Key not found");
         }
@@ -90,27 +91,28 @@
             return py::bytes(value);
         } else {
             throw std::runtime_error("err: unknown value type");
         }
     }
 
     auto has(py::object key_) -> bool {
+        bool ret;
         if (py::isinstance<py::int_>(key_)) {
             uint64_t key = key_.cast<uint64_t>();
-            bool ret = static_cast<bool>(xdbHasInt(_db, key));
-            return ret;
+            ret = static_cast<bool>(xdbHasInt(_db, key));
 
         } else if (py::isinstance<py::bytes>(key_) || py::isinstance<py::str>(key_)) {
             std::string key = key_.cast<std::string>();
-            bool ret = static_cast<bool>(xdbHasBytes(_db, key.c_str(), static_cast<xobjlen_t>(key.length())));
-            return ret;
+            ret = static_cast<bool>(xdbHasBytes(_db, key.c_str(), static_cast<xobjlen_t>(key.length())));
 
         } else {
             throw py::type_error("invalid key type");
         }
+
+        return ret;
     }
 
     auto remove(py::object key_) -> void {
         if (py::isinstance<py::int_>(key_)) {
             uint64_t key = key_.cast<uint64_t>();
             xdbDelInt(_db, key);
```

