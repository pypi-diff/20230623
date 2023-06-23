# Comparing `tmp/scPANTHEON-0.3.2.tar.gz` & `tmp/scPANTHEON-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scPANTHEON-0.3.2.tar", last modified: Thu Jun 22 15:09:25 2023, max compression
+gzip compressed data, was "scPANTHEON-0.3.3.tar", last modified: Fri Jun 23 01:54:13 2023, max compression
```

## Comparing `scPANTHEON-0.3.2.tar` & `scPANTHEON-0.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 15:09:25.516600 scPANTHEON-0.3.2/
--rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0      261 2023-06-22 15:09:25.516600 scPANTHEON-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 15:09:25.503556 scPANTHEON-0.3.2/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      261 2023-06-22 15:09:25.000000 scPANTHEON-0.3.2/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-06-22 15:09:25.000000 scPANTHEON-0.3.2/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 15:09:25.000000 scPANTHEON-0.3.2/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-22 15:09:25.000000 scPANTHEON-0.3.2/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      100 2023-06-22 15:09:25.000000 scPANTHEON-0.3.2/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-22 15:09:25.000000 scPANTHEON-0.3.2/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-22 15:09:25.515600 scPANTHEON-0.3.2/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.3.2/scpantheon/__init__.py
--rw-rw-rw-   0        0        0     2519 2023-06-08 07:21:40.000000 scPANTHEON-0.3.2/scpantheon/bokeh_qt.py
--rw-rw-rw-   0        0        0     4162 2023-05-08 07:39:20.000000 scPANTHEON-0.3.2/scpantheon/data_qt.py
--rw-rw-rw-   0        0        0     1154 2023-06-22 15:08:18.000000 scPANTHEON-0.3.2/scpantheon/main.py
--rw-rw-rw-   0        0        0     5627 2023-05-08 06:44:29.000000 scPANTHEON-0.3.2/scpantheon/qt.py
--rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.3.2/scpantheon/run.py
--rw-rw-rw-   0        0        0     3270 2023-05-12 02:45:41.000000 scPANTHEON-0.3.2/scpantheon/save_qt.py
--rw-rw-rw-   0        0        0    60638 2023-06-22 14:44:00.000000 scPANTHEON-0.3.2/scpantheon/source.py
--rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.3.2/scpantheon/transform.py
--rw-rw-rw-   0        0        0       42 2023-06-22 15:09:25.516600 scPANTHEON-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-06-22 15:08:50.000000 scPANTHEON-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 01:54:13.640333 scPANTHEON-0.3.3/
+-rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      261 2023-06-23 01:54:13.639807 scPANTHEON-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 01:54:13.625711 scPANTHEON-0.3.3/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-06-23 01:54:13.000000 scPANTHEON-0.3.3/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-06-23 01:54:13.000000 scPANTHEON-0.3.3/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 01:54:13.000000 scPANTHEON-0.3.3/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-23 01:54:13.000000 scPANTHEON-0.3.3/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       86 2023-06-23 01:54:13.000000 scPANTHEON-0.3.3/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-23 01:54:13.000000 scPANTHEON-0.3.3/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 01:54:13.638266 scPANTHEON-0.3.3/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.3.3/scpantheon/__init__.py
+-rw-rw-rw-   0        0        0     2519 2023-06-08 07:21:40.000000 scPANTHEON-0.3.3/scpantheon/bokeh_qt.py
+-rw-rw-rw-   0        0        0     4162 2023-05-08 07:39:20.000000 scPANTHEON-0.3.3/scpantheon/data_qt.py
+-rw-rw-rw-   0        0        0     1154 2023-06-22 15:08:18.000000 scPANTHEON-0.3.3/scpantheon/main.py
+-rw-rw-rw-   0        0        0     5627 2023-05-08 06:44:29.000000 scPANTHEON-0.3.3/scpantheon/qt.py
+-rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.3.3/scpantheon/run.py
+-rw-rw-rw-   0        0        0     3272 2023-06-23 01:41:05.000000 scPANTHEON-0.3.3/scpantheon/save_qt.py
+-rw-rw-rw-   0        0        0    60639 2023-06-23 01:41:16.000000 scPANTHEON-0.3.3/scpantheon/source.py
+-rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.3.3/scpantheon/transform.py
+-rw-rw-rw-   0        0        0       42 2023-06-23 01:54:13.640333 scPANTHEON-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1070 2023-06-23 01:54:05.000000 scPANTHEON-0.3.3/setup.py
```

### Comparing `scPANTHEON-0.3.2/scpantheon/bokeh_qt.py` & `scPANTHEON-0.3.3/scpantheon/bokeh_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.2/scpantheon/data_qt.py` & `scPANTHEON-0.3.3/scpantheon/data_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.2/scpantheon/main.py` & `scPANTHEON-0.3.3/scpantheon/main.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.2/scpantheon/qt.py` & `scPANTHEON-0.3.3/scpantheon/qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.2/scpantheon/save_qt.py` & `scPANTHEON-0.3.3/scpantheon/save_qt.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         font.setPointSize(20)
         font.setWeight(20)
 
         # render help text
         self.text_brow = QTextBrowser()
 
         # choose path button
-        self.btn_save = QPushButton("save", self)  
+        self.btn_save = QPushButton("output", self)  
         self.btn_save.setObjectName("btn_save")  
         self.btn_save.clicked.connect(self.slot_btn_save)
         self.btn_save.setFont(font)
         self.btn_save.setFixedWidth(400)
         
         self.layout1 = QVBoxLayout()
         self.layout1.addWidget(self.btn_save)
```

### Comparing `scPANTHEON-0.3.2/scpantheon/source.py` & `scPANTHEON-0.3.3/scpantheon/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
         self.button_disabled()
         def next_save(self):
             if save_qt.main() == 'app closed':
                 print('choosing finished')
             path = get_save_path(dir) + '/'
             text_cover(dir, path + 'result.h5ad') # write the output anndata to cover the data
             print("path covered to " + path + "result.h5ad")
-            try:
+            try: 
                 self.adata.write_h5ad(path+'result.h5ad') 
                 self.adata.obs.to_csv(path+'cluster.csv')
             except:
                 os.makedirs(path)
                 self.adata.write_h5ad(path+'result.h5ad') 
                 self.adata.obs.to_csv(path+'cluster.csv')
             # for cate in list(self.adata.uns['category_dict'].keys()):
```

### Comparing `scPANTHEON-0.3.2/scpantheon/transform.py` & `scPANTHEON-0.3.3/scpantheon/transform.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.2/setup.py` & `scPANTHEON-0.3.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.3.2',#版本
+    version='0.3.3',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
-    install_requires=['bokeh==2.4.3','pandas','anndata','colorcet','scanpy','numpy','PyQt5','PyQtWebEngine',
-                        'appdirs==1.4.4'], # 依赖包,如果没有,可以不要
+    install_requires=['bokeh','pandas','anndata','colorcet','scanpy','numpy','PyQt5','PyQtWebEngine',
+                        'appdirs'], # 依赖包,如果没有,可以不要
     extras_require={
         'tomas': ['tomas'],
     }, # 依赖包,深度使用需手动安装
     entry_points={
         'console_scripts': [
             'sc-pantheon = scpantheon.main:main' # scripts -> multiprocessing
         ]
```

