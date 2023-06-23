# Comparing `tmp/lanablas-0.0.2.tar.gz` & `tmp/lanablas-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanablas-0.0.2.tar", last modified: Thu Jun 22 21:42:02 2023, max compression
+gzip compressed data, was "lanablas-0.0.3.tar", last modified: Fri Jun 23 12:26:03 2023, max compression
```

## Comparing `lanablas-0.0.2.tar` & `lanablas-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-22 21:42:02.201899 lanablas-0.0.2/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-06-20 12:16:48.000000 lanablas-0.0.2/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1189 2023-06-22 21:42:02.201431 lanablas-0.0.2/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      777 2023-06-20 12:15:53.000000 lanablas-0.0.2/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-22 21:42:02.198089 lanablas-0.0.2/lanablas/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-06-22 21:00:47.000000 lanablas-0.0.2/lanablas/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5451 2023-06-22 21:41:55.000000 lanablas-0.0.2/lanablas/matrix.c
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-22 21:42:02.200688 lanablas-0.0.2/lanablas.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1189 2023-06-22 21:42:01.000000 lanablas-0.0.2/lanablas.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-06-22 21:42:02.000000 lanablas-0.0.2/lanablas.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-22 21:42:01.000000 lanablas-0.0.2/lanablas.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-22 21:42:01.000000 lanablas-0.0.2/lanablas.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-22 21:42:02.202044 lanablas-0.0.2/setup.cfg
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1116 2023-06-22 20:54:30.000000 lanablas-0.0.2/setup.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-23 12:26:03.619114 lanablas-0.0.3/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-06-20 12:16:48.000000 lanablas-0.0.3/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1196 2023-06-23 12:26:03.618590 lanablas-0.0.3/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      784 2023-06-23 08:02:14.000000 lanablas-0.0.3/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-23 12:26:03.614433 lanablas-0.0.3/lanablas/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1113 2023-06-23 12:12:41.000000 lanablas-0.0.3/lanablas/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     7218 2023-06-23 10:48:17.000000 lanablas-0.0.3/lanablas/matrix.c
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-23 12:26:03.616330 lanablas-0.0.3/lanablas.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1196 2023-06-23 12:26:02.000000 lanablas-0.0.3/lanablas.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-06-23 12:26:03.000000 lanablas-0.0.3/lanablas.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-23 12:26:02.000000 lanablas-0.0.3/lanablas.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-23 12:26:03.000000 lanablas-0.0.3/lanablas.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-23 12:26:03.619299 lanablas-0.0.3/setup.cfg
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1116 2023-06-23 10:12:39.000000 lanablas-0.0.3/setup.py
```

### Comparing `lanablas-0.0.2/LICENSE` & `lanablas-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lanablas-0.0.2/PKG-INFO` & `lanablas-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanablas
-Version: 0.0.2
+Version: 0.0.3
 Summary: Extension module for matrix multiplication
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,12 +23,12 @@
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas
+pip install lanablas==0.0.2
 ```
```

### Comparing `lanablas-0.0.2/README.md` & `lanablas-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas
+pip install lanablas==0.0.2
 ```
```

### Comparing `lanablas-0.0.2/lanablas/matrix.c` & `lanablas-0.0.3/lanablas/matrix.c`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,54 @@
     PyObject_HEAD
     int rows;
     int cols;
     double** data;
 } MatrixObject;
 
 
+static PyObject* Matrix_new(PyTypeObject* type, PyObject* args) {
+
+    PyObject* pyList;
+    if (!PyArg_ParseTuple(args, "O", &pyList)) {
+        PyErr_SetString(PyExc_TypeError, "Invalid argument: expected a list");
+        return NULL;
+    }
+
+    if (!PyList_Check(pyList)) {
+        PyErr_SetString(PyExc_TypeError, "Invalid argument: expected a list");
+        return NULL;
+    }
+
+    int rows = PyList_Size(pyList);
+    int cols = PyList_Size(PyList_GetItem(pyList, 0));
+
+    MatrixObject* matrix = (MatrixObject*)type->tp_alloc(type, 0);
+    if (matrix == NULL) {
+        PyErr_SetString(PyExc_RuntimeError, "Failed to allocate memory for matrix");
+        return NULL;
+    }
+
+    matrix->rows = rows;
+    matrix->cols = cols;
+    matrix->data = malloc(rows * sizeof(double*));
+
+    for (int i = 0; i < rows; i++) {
+        matrix->data[i] = malloc(cols * sizeof(double));
+        PyObject* row = PyList_GetItem(pyList, i);
+
+        for (int j = 0; j < cols; j++) {
+            PyObject* value = PyList_GetItem(row, j);
+            matrix->data[i][j] = PyFloat_AsDouble(value);
+        }
+    }
+
+    return (PyObject*)matrix;
+}
+
+
 static PyObject* Matrix_zeros(PyTypeObject* type, PyObject* args) {
     
     int rows, cols;
     if (!PyArg_ParseTuple(args, "ii", &rows, &cols)) {
         PyErr_SetString(PyExc_TypeError, "Invalid arguments");
         return NULL;
     }
@@ -93,37 +133,54 @@
             }
         }
     }
 
     return (PyObject*)matrix;
 }
 
+
 static PyObject* Matrix_shape(MatrixObject* self) {
     PyObject* shape = PyTuple_New(2);
     PyObject* rows = PyLong_FromLong(self->rows);
     PyObject* cols = PyLong_FromLong(self->cols);
     PyTuple_SetItem(shape, 0, rows);
     PyTuple_SetItem(shape, 1, cols);
     return shape;
 }
 
 
+static PyObject* Matrix_to_list(MatrixObject* self) {
+    PyObject* result = PyList_New(self->rows);
+    for (int i = 0; i < self->rows; i++) {
+        PyObject* row = PyList_New(self->cols);
+        for (int j = 0; j < self->cols; j++) {
+            PyObject* value = PyFloat_FromDouble(self->data[i][j]);
+            PyList_SetItem(row, j, value);
+        }
+        PyList_SetItem(result, i, row);
+    }
+    return result;
+}
+
+
 static void Matrix_dealloc(MatrixObject* self) {
     for (int i = 0; i < self->rows; i++) {
         free(self->data[i]);
     }
     free(self->data);
     Py_TYPE(self)->tp_free((PyObject*)self);
 }
 
 
 static PyMethodDef MatrixExtensionMethods[] = {
     {"zeros", (PyCFunction)Matrix_zeros, METH_VARARGS | METH_CLASS, "Create a matrix of zeros"},
     {"ones", (PyCFunction)Matrix_ones, METH_VARARGS | METH_CLASS, "Create a matrix of ones"},
     {"eye", (PyCFunction)Matrix_eye, METH_VARARGS | METH_CLASS, "Create an identity matrix"},
+    {"new", (PyCFunction)Matrix_new, METH_VARARGS | METH_CLASS, "Create a matrix from a Python list"},
+    {"to_list", (PyCFunction)Matrix_to_list, METH_NOARGS, "Convert the matrix to a list of lists"},
     {NULL, NULL, 0, NULL}
 };
 
 
 static PyGetSetDef Matrix_getsetters[] = {
     {"shape", (getter)Matrix_shape, NULL, "Return the shape of the matrix as a tuple", NULL},
     {NULL}
@@ -152,15 +209,14 @@
             PyUnicode_AppendAndDel(&result, PyUnicode_FromString("])"));
         }
     }
     return result;
 }
 
 
-
 static PyTypeObject MatrixType = {
     PyVarObject_HEAD_INIT(NULL, 0)
     .tp_name = "Matrix",
     .tp_doc = "Matrix object",
     .tp_basicsize = sizeof(MatrixObject),
     .tp_itemsize = 0,
     .tp_flags = Py_TPFLAGS_DEFAULT,
```

### Comparing `lanablas-0.0.2/lanablas.egg-info/PKG-INFO` & `lanablas-0.0.3/lanablas.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanablas
-Version: 0.0.2
+Version: 0.0.3
 Summary: Extension module for matrix multiplication
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,12 +23,12 @@
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas
+pip install lanablas==0.0.2
 ```
```

### Comparing `lanablas-0.0.2/setup.py` & `lanablas-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     extra_compile_args=['-std=c11'],  # Set the C standard to C11
     include_dirs=['/usr/local/opt/openblas/include'],  # BLAS include directory
     library_dirs=['/usr/local/opt/openblas/lib'],  # BLAS library directory
 )
 
 setup(
 name='lanablas',
-    version='0.0.2',
+    version='0.0.3',
     description='Extension module for matrix multiplication',
     author='Marco Salvalaggio',
     author_email='mar.salvalaggio@gmail.com',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['lanablas'],
```

