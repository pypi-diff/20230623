# Comparing `tmp/lanablas-0.0.3.tar.gz` & `tmp/lanablas-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanablas-0.0.3.tar", last modified: Fri Jun 23 12:26:03 2023, max compression
+gzip compressed data, was "lanablas-0.0.4.tar", last modified: Fri Jun 23 13:29:59 2023, max compression
```

## Comparing `lanablas-0.0.3.tar` & `lanablas-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-23 12:26:03.619114 lanablas-0.0.3/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-06-20 12:16:48.000000 lanablas-0.0.3/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1196 2023-06-23 12:26:03.618590 lanablas-0.0.3/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      784 2023-06-23 08:02:14.000000 lanablas-0.0.3/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-23 12:26:03.614433 lanablas-0.0.3/lanablas/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1113 2023-06-23 12:12:41.000000 lanablas-0.0.3/lanablas/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     7218 2023-06-23 10:48:17.000000 lanablas-0.0.3/lanablas/matrix.c
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-23 12:26:03.616330 lanablas-0.0.3/lanablas.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1196 2023-06-23 12:26:02.000000 lanablas-0.0.3/lanablas.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-06-23 12:26:03.000000 lanablas-0.0.3/lanablas.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-23 12:26:02.000000 lanablas-0.0.3/lanablas.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-23 12:26:03.000000 lanablas-0.0.3/lanablas.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-23 12:26:03.619299 lanablas-0.0.3/setup.cfg
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1116 2023-06-23 10:12:39.000000 lanablas-0.0.3/setup.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-23 13:29:59.231470 lanablas-0.0.4/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-06-20 12:16:48.000000 lanablas-0.0.4/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-06-23 13:29:59.231239 lanablas-0.0.4/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1047 2023-06-23 12:38:32.000000 lanablas-0.0.4/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-23 13:29:59.229360 lanablas-0.0.4/lanablas/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1113 2023-06-23 13:22:23.000000 lanablas-0.0.4/lanablas/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8357 2023-06-23 13:26:46.000000 lanablas-0.0.4/lanablas/matrix.c
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-23 13:29:59.230884 lanablas-0.0.4/lanablas.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-06-23 13:29:58.000000 lanablas-0.0.4/lanablas.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-06-23 13:29:59.000000 lanablas-0.0.4/lanablas.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-23 13:29:58.000000 lanablas-0.0.4/lanablas.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-23 13:29:58.000000 lanablas-0.0.4/lanablas.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-23 13:29:59.231561 lanablas-0.0.4/setup.cfg
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1116 2023-06-23 13:22:17.000000 lanablas-0.0.4/setup.py
```

### Comparing `lanablas-0.0.3/LICENSE` & `lanablas-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lanablas-0.0.3/PKG-INFO` & `lanablas-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanablas
-Version: 0.0.3
+Version: 0.0.4
 Summary: Extension module for matrix multiplication
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,12 +23,24 @@
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.2
+pip install lanablas==0.0.3
 ```
 
+## Example 
+
+```python
+from lanablas import Matrix
+
+zeros = Matrix.zeros(3,3)
+print(zeros)
+print(type(zeros), zeros.shape)
+```
+
+For more comprehensive examples, please visit the [examples](https://github.com/marcosalvalaggio/lana-blas/tree/main/examples) folder
+
```

### Comparing `lanablas-0.0.3/README.md` & `lanablas-0.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -9,10 +9,22 @@
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.2
+pip install lanablas==0.0.3
 ```
 
+## Example 
+
+```python
+from lanablas import Matrix
+
+zeros = Matrix.zeros(3,3)
+print(zeros)
+print(type(zeros), zeros.shape)
+```
+
+For more comprehensive examples, please visit the [examples](https://github.com/marcosalvalaggio/lana-blas/tree/main/examples) folder
+
```

### Comparing `lanablas-0.0.3/lanablas/__init__.py` & `lanablas-0.0.4/lanablas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union, List
 from matrix import Matrix
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 
 def inject(data: Union[float, int, List, List[List]]) -> List[List[float]]:
     """
     Injects the input data into a matrix.
 
     Args:
```

### Comparing `lanablas-0.0.3/lanablas/matrix.c` & `lanablas-0.0.4/lanablas/matrix.c`

 * *Files 9% similar despite different names*

```diff
@@ -134,14 +134,52 @@
         }
     }
 
     return (PyObject*)matrix;
 }
 
 
+static PyObject* Matrix_fill(PyTypeObject* type, PyObject* args) {
+    
+    PyObject* sizeTuple;
+    double fill_value;
+
+    if (!PyArg_ParseTuple(args, "Od", &sizeTuple, &fill_value)) {
+        PyErr_SetString(PyExc_TypeError, "Invalid arguments: (rows, cols), fill_value");
+        return NULL;
+    }
+
+    int rows, cols;
+    if (!PyArg_ParseTuple(sizeTuple, "ii", &rows, &cols)) {
+        PyErr_SetString(PyExc_TypeError, "Invalid size tuple: (rows, cols)");
+        return NULL;
+    }
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
+    for (int i = 0; i < rows; i++) {
+        matrix->data[i] = malloc(cols * sizeof(double));
+        for (int j = 0; j < cols; j++) {
+            matrix->data[i][j] = fill_value;
+        }
+    }
+
+    return (PyObject*)matrix;
+
+}
+
+
+
 static PyObject* Matrix_shape(MatrixObject* self) {
     PyObject* shape = PyTuple_New(2);
     PyObject* rows = PyLong_FromLong(self->rows);
     PyObject* cols = PyLong_FromLong(self->cols);
     PyTuple_SetItem(shape, 0, rows);
     PyTuple_SetItem(shape, 1, cols);
     return shape;
@@ -172,14 +210,15 @@
 
 
 static PyMethodDef MatrixExtensionMethods[] = {
     {"zeros", (PyCFunction)Matrix_zeros, METH_VARARGS | METH_CLASS, "Create a matrix of zeros"},
     {"ones", (PyCFunction)Matrix_ones, METH_VARARGS | METH_CLASS, "Create a matrix of ones"},
     {"eye", (PyCFunction)Matrix_eye, METH_VARARGS | METH_CLASS, "Create an identity matrix"},
     {"new", (PyCFunction)Matrix_new, METH_VARARGS | METH_CLASS, "Create a matrix from a Python list"},
+    {"fill", (PyCFunction)Matrix_fill, METH_VARARGS | METH_CLASS, "Fill the matrix with a specified value"},
     {"to_list", (PyCFunction)Matrix_to_list, METH_NOARGS, "Convert the matrix to a list of lists"},
     {NULL, NULL, 0, NULL}
 };
 
 
 static PyGetSetDef Matrix_getsetters[] = {
     {"shape", (getter)Matrix_shape, NULL, "Return the shape of the matrix as a tuple", NULL},
```

### Comparing `lanablas-0.0.3/lanablas.egg-info/PKG-INFO` & `lanablas-0.0.4/lanablas.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanablas
-Version: 0.0.3
+Version: 0.0.4
 Summary: Extension module for matrix multiplication
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,12 +23,24 @@
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.2
+pip install lanablas==0.0.3
 ```
 
+## Example 
+
+```python
+from lanablas import Matrix
+
+zeros = Matrix.zeros(3,3)
+print(zeros)
+print(type(zeros), zeros.shape)
+```
+
+For more comprehensive examples, please visit the [examples](https://github.com/marcosalvalaggio/lana-blas/tree/main/examples) folder
+
```

### Comparing `lanablas-0.0.3/setup.py` & `lanablas-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     extra_compile_args=['-std=c11'],  # Set the C standard to C11
     include_dirs=['/usr/local/opt/openblas/include'],  # BLAS include directory
     library_dirs=['/usr/local/opt/openblas/lib'],  # BLAS library directory
 )
 
 setup(
 name='lanablas',
-    version='0.0.3',
+    version='0.0.4',
     description='Extension module for matrix multiplication',
     author='Marco Salvalaggio',
     author_email='mar.salvalaggio@gmail.com',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['lanablas'],
```

