# Comparing `tmp/pyngres-0.1.1.tar.gz` & `tmp/pyngres-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyngres-0.1.1.tar", last modified: Tue May 16 12:27:33 2023, max compression
+gzip compressed data, was "pyngres-0.1.4.tar", last modified: Fri Jun 23 16:31:35 2023, max compression
```

## Comparing `pyngres-0.1.1.tar` & `pyngres-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 12:27:25.000000 pyngres-0.1.1/
--rw-rw-rw-   0        0        0     1086 2023-05-02 12:46:41.000000 pyngres-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      320 2023-05-16 12:27:25.000000 pyngres-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2357 2023-05-02 12:46:41.000000 pyngres-0.1.1/README.md
--rw-rw-rw-   0        0        0      444 2023-05-16 12:27:25.000000 pyngres-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-05-02 12:46:41.000000 pyngres-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:27:25.000000 pyngres-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 12:27:25.000000 pyngres-0.1.1/src/pyngres/
--rw-rw-rw-   0        0        0    18990 2023-05-02 13:35:29.000000 pyngres-0.1.1/src/pyngres/IIAPI_CONSTANTS.py
--rw-rw-rw-   0        0        0    19585 2023-05-02 13:41:37.000000 pyngres-0.1.1/src/pyngres/IIAPI_PARM.py
--rw-rw-rw-   0        0        0     9061 2023-05-16 12:07:00.000000 pyngres-0.1.1/src/pyngres/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:27:25.000000 pyngres-0.1.1/src/pyngres.egg-info/
--rw-rw-rw-   0        0        0      320 2023-05-16 12:27:24.000000 pyngres-0.1.1/src/pyngres.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-05-16 12:27:25.000000 pyngres-0.1.1/src/pyngres.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 12:27:24.000000 pyngres-0.1.1/src/pyngres.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-16 12:27:24.000000 pyngres-0.1.1/src/pyngres.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 12:27:24.000000 pyngres-0.1.1/src/pyngres.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 16:31:17.000000 pyngres-0.1.4/
+-rw-rw-rw-   0        0        0     1086 2023-05-02 12:46:41.000000 pyngres-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      320 2023-06-23 16:31:17.000000 pyngres-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2357 2023-05-02 12:46:41.000000 pyngres-0.1.4/README.md
+-rw-rw-rw-   0        0        0      433 2023-06-23 16:31:17.000000 pyngres-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-05-02 12:46:41.000000 pyngres-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:31:17.000000 pyngres-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 16:31:17.000000 pyngres-0.1.4/src/pyngres/
+-rw-rw-rw-   0        0        0    19020 2023-06-22 09:48:17.000000 pyngres-0.1.4/src/pyngres/IIAPI_CONSTANTS.py
+-rw-rw-rw-   0        0        0    21164 2023-06-01 12:39:59.000000 pyngres-0.1.4/src/pyngres/IIAPI_PARM.py
+-rw-rw-rw-   0        0        0     9061 2023-05-16 12:07:00.000000 pyngres-0.1.4/src/pyngres/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:31:17.000000 pyngres-0.1.4/src/pyngres.egg-info/
+-rw-rw-rw-   0        0        0      320 2023-06-23 16:31:17.000000 pyngres-0.1.4/src/pyngres.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-06-23 16:31:17.000000 pyngres-0.1.4/src/pyngres.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 16:31:17.000000 pyngres-0.1.4/src/pyngres.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 16:31:17.000000 pyngres-0.1.4/src/pyngres.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 16:31:17.000000 pyngres-0.1.4/src/pyngres.egg-info/top_level.txt
```

### Comparing `pyngres-0.1.1/LICENSE` & `pyngres-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyngres-0.1.1/README.md` & `pyngres-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyngres-0.1.1/src/pyngres/IIAPI_CONSTANTS.py` & `pyngres-0.1.4/src/pyngres/IIAPI_CONSTANTS.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,14 +252,15 @@
 IIAPI_EPV_DFRMT_DMY = 7
 IIAPI_EPV_DFRMT_FINNISH = 2
 IIAPI_EPV_DFRMT_GERMAN = 4
 IIAPI_EPV_DFRMT_ISO = 3
 IIAPI_EPV_DFRMT_ISO4 = 9
 IIAPI_EPV_DFRMT_ISO4T = 11
 IIAPI_EPV_DFRMT_ISO4TC = 12
+IIAPI_EPV_DFRMT_ISO8601 = 13
 IIAPI_EPV_DFRMT_MDY = 6
 IIAPI_EPV_DFRMT_MLT4 = 8
 IIAPI_EPV_DFRMT_MULTI = 1
 IIAPI_EPV_DFRMT_US = 0
 IIAPI_EPV_DFRMT_YMD = 5
 IIAPI_EPV_EXPONENTIAL = 'e'
 IIAPI_EPV_FLOATDEC = 'n'
```

### Comparing `pyngres-0.1.1/src/pyngres/IIAPI_PARM.py` & `pyngres-0.1.4/src/pyngres/IIAPI_PARM.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,64 @@
                 struct_name = self.__class__.__name__
                 diagnostic = '{struct_name} object has no attribute "{name}"'
                 raise AttributeError(diagnostic)
             super().__setattr__(name, value)
 
     display_trim = ''
 
+
+    ##  all the OpenAPI structure member names have a structure-specific
+    ##  prefix (e.g. co_genParm, qy_genparm, etc). The following methods
+    ##  facilitate access when the prefix is not known, using only the
+    ##  suffix (e.g. genParm)
+
+    def _field_name_prefix(self):
+        '''return the field name prefix used in the structure'''
+
+        prefix = None
+        field = self._fields_[0]
+        name = field[0]
+        prefix = name[0:2]
+        return prefix
+
+
+    def field_by_suffix(self,suffix):
+        '''get a structure field using only its name-suffix'''
+
+        prefix = self._field_name_prefix()
+        full_name = prefix + '_' + suffix
+        ##  don't use try/except here; let it be fatal
+        field = getattr(self,full_name)
+        return field
+
+
+    def genParm(self):
+        '''return the genParm field (if any)'''
+
+        return self.field_by_suffix('genParm')
+
+
+    def connHandle(self):
+        '''return the connHandle field (if any)'''
+
+        return self.field_by_suffix('connHandle')
+
+
+    def tranHandle(self):
+        '''return the tranHandle field (if any)'''
+
+        return self.field_by_suffix('tranHandle')
+
+
+    def stmtHandle(self):
+        '''return the stmtHandle field (if any)'''
+
+        return self.field_by_suffix('stmtHandle')
+
+
     def __repr__(self):
         struct_name = self.__class__.__name__
         repr = []
         repr.append('')
         repr.append(f'{struct_name}:')
         for name, type in self._fields_:
             value = getattr(self, name)
@@ -72,14 +122,17 @@
 
 class IIAPI_MEMBER(IIAPI):
     '''data structures used as members by the OpenAPI'''
 
     display_trim = '||  '
 
 
+class IIAPI_GENERIC(object):
+    '''mixin class to return *_genParm, *_connHandle, etc'''
+
 class IIAPI_GENPARM(IIAPI_MEMBER):
     '''common parameter member for Ingres OpenAPI'''
 
     _fields_ = [
         ('gp_callback', II_PTR),
         ('gp_closure', II_PTR),
         ('gp_completed', II_BOOL),
@@ -102,15 +155,19 @@
         ('ds_columnName', II_STR),
     ]
 
 
 class IIAPI_DATAVALUE(IIAPI_MEMBER):
     '''generic column data'''
 
-    _fields_ = [('dv_null', II_BOOL), ('dv_length', II_UINT2), ('dv_value', II_PTR)]
+    _fields_ = [
+        ('dv_null', II_BOOL), 
+        ('dv_length', II_UINT2), 
+        ('dv_value', II_PTR)
+    ]
 
 
 class IIAPI_FDATADESCR(IIAPI_MEMBER):
     '''
     This data type describes the data in a copy file. It also describes
     how the file should be formatted.
     '''
@@ -175,15 +232,18 @@
         ('svr_parmValue', ctypes.POINTER(IIAPI_DATAVALUE)),
     ]
 
 
 class IIAPI_II_TRAN_ID(IIAPI_MEMBER):
     '''Ingres transaction ID'''
 
-    _fields_ = [('it_highTran', II_UINT4), ('it_lowTran', II_UINT4)]
+    _fields_ = [
+        ('it_highTran', II_UINT4), 
+        ('it_lowTran', II_UINT4)
+    ]
 
 
 class IIAPI_II_DIS_TRAN_ID(IIAPI_MEMBER):
     '''"conventional" 2PC transaction identifier'''
 
     _fields_ = [
         ('ii_tranID', IIAPI_II_TRAN_ID),
@@ -212,24 +272,30 @@
     ]
 
 
 ##  NB this is a union not a struct
 class IIAPI_2PC_TRAN_ID(ctypes.Union):
     '''2PC transaction identifier'''
 
-    _fields_ = [('iiXID', IIAPI_II_DIS_TRAN_ID), ('xaXID', IIAPI_XA_DIS_TRAN_ID)]
+    _fields_ = [
+        ('iiXID', IIAPI_II_DIS_TRAN_ID), 
+        ('xaXID', IIAPI_XA_DIS_TRAN_ID)
+    ]
 
 
 class IIAPI_TRAN_ID(IIAPI_MEMBER):
     '''
     The IIAPI_TRAN_ID data type specifies and names an OpenAPI
     transaction
     '''
 
-    _fields_ = [('ti_type', II_ULONG), ('ti_value', IIAPI_2PC_TRAN_ID)]
+    _fields_ = [
+        ('ti_type', II_ULONG), 
+        ('ti_value', IIAPI_2PC_TRAN_ID)
+    ]
 
 
 class IIAPI_PARM(IIAPI):
     '''parameter block for the Ingres OpenAPI'''
 
     ##  I suspect, but don't yet know for sure, that PARM blocks should
     ##  be treated as context managers; they don't do anything (yet) but
@@ -245,15 +311,18 @@
     def __exit__(self):
         pass
 
 
 class IIAPI_ABORTPARM(IIAPI_PARM):
     '''parameter block for IIapi_abort'''
 
-    _fields_ = [('ab_genParm', IIAPI_GENPARM), ('ab_connHandle', ctypes.c_void_p)]
+    _fields_ = [
+        ('ab_genParm', IIAPI_GENPARM), 
+        ('ab_connHandle', ctypes.c_void_p)
+    ]
 
 
 class IIAPI_AUTOPARM(IIAPI_PARM):
     '''parameter block for IIapi_autocommit'''
 
     _fields_ = [
         ('ac_genParm', IIAPI_GENPARM),
```

### Comparing `pyngres-0.1.1/src/pyngres/__init__.py` & `pyngres-0.1.4/src/pyngres/__init__.py`

 * *Files identical despite different names*

