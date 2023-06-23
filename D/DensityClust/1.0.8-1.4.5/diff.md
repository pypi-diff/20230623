# Comparing `tmp/DensityClust-1.0.8.tar.gz` & `tmp/DensityClust-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DensityClust-1.0.8.tar", last modified: Tue Dec  7 02:36:59 2021, max compression
+gzip compressed data, was "DensityClust-1.4.5.tar", last modified: Fri Jun 23 11:18:14 2023, max compression
```

## Comparing `DensityClust-1.0.8.tar` & `DensityClust-1.4.5.tar`

### file list

```diff
@@ -1,15 +1,39 @@
-drwxrwxrwx   0        0        0        0 2021-12-07 02:36:59.714494 DensityClust-1.0.8/
-drwxrwxrwx   0        0        0        0 2021-12-07 02:36:59.694546 DensityClust-1.0.8/DensityClust/
--rw-rw-rw-   0        0        0     2655 2021-11-24 07:22:51.000000 DensityClust-1.0.8/DensityClust/LocalDensityClustering_main.py
--rw-rw-rw-   0        0        0        0 2021-11-08 13:50:19.000000 DensityClust-1.0.8/DensityClust/__init__.py
--rw-rw-rw-   0        0        0    10126 2021-11-24 07:21:41.000000 DensityClust-1.0.8/DensityClust/clustring_subfunc.py
--rw-rw-rw-   0        0        0    18752 2021-12-06 09:20:02.000000 DensityClust-1.0.8/DensityClust/densityCluster_3d.py
--rw-rw-rw-   0        0        0     5269 2021-12-06 09:20:02.000000 DensityClust-1.0.8/DensityClust/make_plot.py
-drwxrwxrwx   0        0        0        0 2021-12-07 02:36:59.713524 DensityClust-1.0.8/DensityClust.egg-info/
--rw-rw-rw-   0        0        0      238 2021-12-07 02:36:58.000000 DensityClust-1.0.8/DensityClust.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2021-12-07 02:36:58.000000 DensityClust-1.0.8/DensityClust.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-07 02:36:58.000000 DensityClust-1.0.8/DensityClust.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2021-12-07 02:36:58.000000 DensityClust-1.0.8/DensityClust.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      238 2021-12-07 02:36:59.714494 DensityClust-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2021-12-07 02:36:59.714494 DensityClust-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      348 2021-12-07 02:35:05.000000 DensityClust-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:18:14.048182 DensityClust-1.4.5/
+drwxrwxrwx   0        0        0        0 2023-06-23 11:18:14.006438 DensityClust-1.4.5/DensityClust/
+-rw-rw-rw-   0        0        0     7105 2023-06-23 10:21:24.000000 DensityClust-1.4.5/DensityClust/LocalDensityClustering_main.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 11:05:30.000000 DensityClust-1.4.5/DensityClust/__init__.py
+-rw-rw-rw-   0        0        0    29426 2023-06-23 04:03:04.000000 DensityClust-1.4.5/DensityClust/clustring_subfunc.py
+-rw-rw-rw-   0        0        0    51177 2023-06-23 10:21:24.000000 DensityClust-1.4.5/DensityClust/localDenClust2.py
+-rw-rw-rw-   0        0        0    11964 2023-06-23 04:03:04.000000 DensityClust-1.4.5/DensityClust/split_cube.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:18:14.026871 DensityClust-1.4.5/DensityClust.egg-info/
+-rw-rw-rw-   0        0        0      341 2023-06-23 11:18:13.000000 DensityClust-1.4.5/DensityClust.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      770 2023-06-23 11:18:13.000000 DensityClust-1.4.5/DensityClust.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 11:18:13.000000 DensityClust-1.4.5/DensityClust.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-06-23 11:18:13.000000 DensityClust-1.4.5/DensityClust.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 11:18:14.030867 DensityClust-1.4.5/Generate/
+-rw-rw-rw-   0        0        0     3381 2023-06-23 04:03:04.000000 DensityClust-1.4.5/Generate/fits_header.py
+-rw-rw-rw-   0        0        0    15795 2023-06-23 04:03:04.000000 DensityClust-1.4.5/Generate/generate.py
+-rw-rw-rw-   0        0        0    13320 2023-06-23 04:03:04.000000 DensityClust-1.4.5/Generate/synthetic_data.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:18:14.034867 DensityClust-1.4.5/LDC_MGM_main/
+-rw-rw-rw-   0        0        0     7159 2023-06-23 11:10:39.000000 DensityClust-1.4.5/LDC_MGM_main/LDC_MGM_main.py
+-rw-rw-rw-   0        0        0     1329 2023-06-23 11:10:39.000000 DensityClust-1.4.5/LDC_MGM_main/LDC_mian.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 04:03:04.000000 DensityClust-1.4.5/LDC_MGM_main/__init__.py
+-rw-rw-rw-   0        0        0     1111 2023-06-23 04:03:04.000000 DensityClust-1.4.5/LICENSE
+-rw-rw-rw-   0        0        0      341 2023-06-23 11:18:14.048182 DensityClust-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4089 2023-06-23 10:23:18.000000 DensityClust-1.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 11:18:14.039902 DensityClust-1.4.5/fit_clump_function/
+-rw-rw-rw-   0        0        0        0 2023-06-23 04:03:04.000000 DensityClust-1.4.5/fit_clump_function/__init__.py
+-rw-rw-rw-   0        0        0     9322 2023-06-23 04:03:04.000000 DensityClust-1.4.5/fit_clump_function/main_fit_gauss_3d.py
+-rw-rw-rw-   0        0        0    26025 2023-06-23 04:03:04.000000 DensityClust-1.4.5/fit_clump_function/multi_gauss_fitting_new.py
+-rw-rw-rw-   0        0        0    11936 2023-06-23 04:03:04.000000 DensityClust-1.4.5/fit_clump_function/touch_clump.py
+-rw-rw-rw-   0        0        0       42 2023-06-23 11:18:14.049187 DensityClust-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-06-23 11:18:01.000000 DensityClust-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:18:14.042039 DensityClust-1.4.5/t_match/
+-rw-rw-rw-   0        0        0        0 2023-06-23 04:03:04.000000 DensityClust-1.4.5/t_match/__init__.py
+-rw-rw-rw-   0        0        0    24986 2023-06-23 04:03:04.000000 DensityClust-1.4.5/t_match/match_6_.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:18:14.046186 DensityClust-1.4.5/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-23 04:03:04.000000 DensityClust-1.4.5/tools/__init__.py
+-rw-rw-rw-   0        0        0     7193 2023-06-23 04:03:04.000000 DensityClust-1.4.5/tools/data_merge.py
+-rw-rw-rw-   0        0        0     8962 2023-06-23 04:03:04.000000 DensityClust-1.4.5/tools/make_plot.py
+-rw-rw-rw-   0        0        0    14792 2023-06-23 04:03:04.000000 DensityClust-1.4.5/tools/show_clumps.py
+-rw-rw-rw-   0        0        0    12625 2023-06-23 04:03:04.000000 DensityClust-1.4.5/tools/ultil_lxy.py
```

### Comparing `DensityClust-1.0.8/DensityClust/clustring_subfunc.py` & `DensityClust-1.4.5/DensityClust/split_cube.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,276 +1,276 @@
+import os
+from tools.show_clumps import make_plot_wcs_1
 import numpy as np
-import time
-from astropy import wcs
-from tabulate import tabulate
-import astropy.io.fits as fits
 import pandas as pd
+import matplotlib.pyplot as plt
+from spectral_cube import SpectralCube
+from DensityClust.localDenClust2 import LocalDensityCluster as LDC
+from DensityClust.localDenClust2 import Data
+from t_match.match_6_ import match_simu_detect_new
+
+
+split_list = [[0, 150, 0, 150], [0, 150, 90, 271], [0, 150, 210, 361],
+              [90, 241, 0, 150], [90, 241, 90, 271], [90, 241, 210, 361]]
+
+
+def split_cube_lxy(data_path, save_folder_all):
+
+    split_list = [[0, 150, 0, 150], [0, 150, 90, 271], [0, 150, 210, 361],
+                  [90, 241, 0, 150], [90, 241, 90, 271], [90, 241, 210, 361]]
+    data_cube = SpectralCube.read(data_path)
+    sub_cube_path_list = []
+    for i, item in enumerate(split_list):
+        sub_cude = data_cube[:, item[0]: item[1], item[2]: item[3]]
+        # 更换文件路径
+        sub_cube_path = os.path.join(save_folder_all, os.path.basename(data_path))
+        sub_cube_path = sub_cube_path.replace('.fits', '_%02d.fits' % i)
+        if not os.path.exists(sub_cube_path):
+            sub_cude.write(sub_cube_path)
+        sub_cube_path_list.append(sub_cube_path)
+    return sub_cube_path_list
+
+
+def get_outcat_i(outcat, i):
+    outcat_split = [[0, 120, 0, 120], [0, 120, 30, 150], [0, 120, 30, 150],
+                    [30, 150, 0, 120], [30, 150, 30, 150], [30, 150, 30, 150]]
+    [cen2_min, cen2_max, cen1_min, cen1_max] = outcat_split[i]
+    aa = outcat.loc[outcat['Cen1'] > cen1_min]
+    aa = aa.loc[outcat['Cen1'] <= cen1_max]
 
-
-def setdiff_nd(a1, a2):
-    """
-    python 使用numpy求二维数组的差集
-    :param a1:
-    :param a2:
-    :return:
-    """
-    # a1 = index_value
-    # a2 = np.array([point_ii_xy])
-    a1_rows = a1.view([('', a1.dtype)] * a1.shape[1])
-    a2_rows = a2.view([('', a2.dtype)] * a2.shape[1])
-
-    a3 = np.setdiff1d(a1_rows, a2_rows).view(a1.dtype).reshape(-1, a1.shape[1])
-    return a3
-
-
-def get_xyz(data):
-    """
-    :param data: 3D data
-    :return: 3D data coordinates
-    第1,2,3维数字依次递增
-
-     :param data: 2D data
-    :return: 2D data coordinates
-    第1,2维数字依次递增
-
-    """
-    nim = data.ndim
-    if nim == 3:
-        size_x, size_y, size_z = data.shape
-        x_arange = np.arange(1, size_x+1)
-        y_arange = np.arange(1, size_y+1)
-        z_arange = np.arange(1, size_z+1)
-        [xx, yy, zz] = np.meshgrid(x_arange, y_arange, z_arange, indexing='ij')
-        xyz = np.column_stack([zz.flatten(), yy.flatten(), xx.flatten()])
-
-    else:
-        size_x, size_y = data.shape
-        x_arange = np.arange(1, size_x + 1)
-        y_arange = np.arange(1, size_y + 1)
-        [xx, yy] = np.meshgrid(x_arange, y_arange, indexing='ij')
-        xyz = np.column_stack([yy.flatten(), xx.flatten()])
-    return xyz
-
-
-def kc_coord_3d(point_ii_xy, xm, ym, zm, r):
-    """
-    :param point_ii_xy: 当前点坐标(x,y,z)
-    :param xm: size_x
-    :param ym: size_y
-    :param zm: size_z
-    :param r: 2 * r + 1
-    :return:
-    返回delta_ii_xy点r邻域的点坐标
-    """
-    it = point_ii_xy[0]
-    jt = point_ii_xy[1]
-    kt = point_ii_xy[2]
-
-    xyz_min = np.array([[1, it - r], [1, jt - r], [1, kt - r]])
-    xyz_min = xyz_min.max(axis=1)
-
-    xyz_max = np.array([[xm, it + r], [ym, jt + r], [zm, kt + r]])
-    xyz_max = xyz_max.min(axis=1)
-
-    x_arange = np.arange(xyz_min[0], xyz_max[0] + 1)
-    y_arange = np.arange(xyz_min[1], xyz_max[1] + 1)
-    v_arange = np.arange(xyz_min[2], xyz_max[2] + 1)
-
-    [p_k, p_i, p_j] = np.meshgrid(x_arange, y_arange, v_arange, indexing='ij')
-    Index_value = np.column_stack([p_k.flatten(), p_i.flatten(), p_j.flatten()])
-    Index_value = setdiff_nd(Index_value, np.array([point_ii_xy]))
-
-    ordrho_jj = np.matmul(Index_value - 1, np.array([[1], [xm], [ym * xm]]))
-    ordrho_jj.reshape([1, ordrho_jj.shape[0]])
-
-    return ordrho_jj[:, 0], Index_value
+    aa = aa.loc[outcat['Cen2'] > cen2_min]
+    loc_outcat = aa.loc[outcat['Cen2'] <= cen2_max]
+    return loc_outcat
 
 
-def kc_coord_2d(point_ii_xy, xm, ym, r):
+def get_outcat_wcs_all(save_path, data_all_path):
     """
-    :param point_ii_xy: 当前点坐标(x,y)
-    :param xm: size_x
-    :param ym: size_y
-    :param r: 2 * r + 1
+    对分块检测结果的整合
+    :param save_path: LDC分块检测结果保存位置
+    :param data_all_path: 原始待检测数据位置
     :return:
-    返回point_ii_xy点r邻域的点坐标
     """
-    it = point_ii_xy[0]
-    jt = point_ii_xy[1]
 
-    xyz_min = np.array([[1, it - r], [1, jt - r]])
-    xyz_min = xyz_min.max(axis=1)
+    outcat_wcs_all = pd.DataFrame([])
+    outcat_wcs_path = os.path.join(save_path, 'LDC_auto_outcat_wcs.csv')
+    outcat_path = os.path.join(save_path, 'LDC_auto_outcat.csv')
+
+    file_name = os.path.basename(data_all_path).replace('.fits', '')
+    for i in range(6):
+        # i = 1
+        # outcat_i_path = r'test_data/synthetic/synthetic_model_0000_%02d/LDC_auto_outcat.csv' % i
+        outcat_i_path = os.path.join(save_path, file_name + r'_%02d\LDC_auto_outcat.csv' % i)
+        outcat_i = pd.read_csv(outcat_i_path, sep='\t')
+        loc_outcat_i = get_outcat_i(outcat_i, i)
+
+        origin_data_name = os.path.join(save_path, file_name + r'_%02d.fits' % i)
+        data = Data(data_path=origin_data_name)
+        ldc = LDC(data=data, para=None)
+        outcat_wcs = ldc.change_pix2world(loc_outcat_i)
+        outcat_wcs_all = pd.concat([outcat_wcs_all, outcat_wcs], axis=0)
+
+    outcat_wcs_all.to_csv(outcat_wcs_path, sep='\t', index=False)
+    data = Data(data_path=data_path)
+    ldc = LDC(data=data, para=None)
+    data_wcs = ldc.data.wcs
+    outcat_wcs_all = pd.read_csv(outcat_wcs_path, sep='\t')
+
+    outcat_all = change_world2pix(outcat_wcs_all, data_wcs)
+    outcat_all.to_csv(outcat_path, sep='\t', index=False)
+    fig_name = os.path.join(save_path, 'LDC_auto_detect_result.png')
+    make_plot_wcs_1(outcat_wcs_all, data_wcs, data.data_cube, fig_name=fig_name)
+
+
+def make_plot_wcs_data_outcat(data_name, outcat_wcs_path):
+    """
+    将银经银纬核表绘制在数据块上
+    :param data_name：分子云核数据块路径
+    :param outcat_wcs_path：银经银纬核表路径
+    """
+    data = Data(data_path=data_name)
+    outcat_wcs_all = pd.read_csv(outcat_wcs_path, sep='\t')
+    data_wcs = data.wcs
+    data_cube = data.data_cube
+    make_plot_wcs_1(outcat_wcs_all, data_wcs, data_cube)
+
+
+def make_plot_ij(match_outcat_path, col_names_g=None, col_names_s=None):
+    """
+    将匹配结果进行绘制
+        :param match_outcat_path：匹配核表
+        :param col_names_g：检测核表要比较的列名，如：['Cen1', 'Cen2', 'Cen3']
+        :param col_names_s：仿真核表要比较的列名，如：['Cen1', 'Cen2', 'Cen3']
+    return:
+        绘制的1*3的图片
+    """
+    match_outcat = pd.read_csv(match_outcat_path, sep='\t')
+    if col_names_s is None:
+        col_names_s = ['Cen1', 'Cen2', 'Cen3']
+    if col_names_g is None:
+        col_names_g = ['Cen1', 'Cen2', 'Cen3']
+    fig = plt.figure(figsize=[15, 4])
+    ii = 1
+    for c_n_g, c_n_s in zip(col_names_g, col_names_s):
+        col_name_g = 'f_' + c_n_g
+        col_name_s = 's_' + c_n_s
+        data_g = match_outcat[col_name_g].values
+        data_s = match_outcat[col_name_s].values
+        ax = fig.add_subplot(1, 3, ii)
+        ax.scatter(data_g, data_s)
+        ax.set_xlabel(col_name_g)
+        ax.set_ylabel(col_name_s)
+        ii += 1
+    plt.show()
+
+
+def compare_version(sop, dop, msp, s_cen=None, s_szie=None, g_cen=None):
+    """
+    将仿真核表和检测核表进行匹配，并把匹配结果的中心坐标散点图画出来.
+    其他参数如要绘制，请调用make_plot_ij()函数
+        :param sop：仿真核表路径(也可以是其他作为标准的核表)
+        :param dop：检测核表路径
+        :param msp：匹配核表保存路径
+        :param s_cen：仿真核表的质心列名，默认为：['Cen1', 'Cen2', 'Cen3']
+        :param s_cen：仿真核表的轴长列名，默认为：['Size1', 'Size2', 'Size3']
+        :param g_cen：检测核表的质心列名，默认为：['Cen1', 'Cen2', 'Cen3']
+    return:
+        None
+    """
+
+    if g_cen is None:
+        g_cen = ['Cen1', 'Cen2', 'Cen3']
+    if s_szie is None:
+        s_szie = ['Size1', 'Size2', 'Size3']
+    if s_cen is None:
+        s_cen = ['Cen1', 'Cen2', 'Cen3']
+    match_cfg = match_simu_detect_new(sop, dop, msp, s_cen=s_cen, s_size=s_szie, g_cen=g_cen)
 
-    xyz_max = np.array([[xm, it + r], [ym, jt + r]])
-    xyz_max = xyz_max.min(axis=1)
+    mop = match_cfg['Match_table_name']
+    make_plot_ij(mop, col_names_g=g_cen, col_names_s=s_cen)
 
-    x_arrange = np.arange(xyz_min[0], xyz_max[0] + 1)
-    y_arrange = np.arange(xyz_min[1], xyz_max[1] + 1)
 
-    [p_k, p_i] = np.meshgrid(x_arrange, y_arrange, indexing='ij')
-    Index_value = np.column_stack([p_k.flatten(), p_i.flatten()])
-    Index_value = setdiff_nd(Index_value, np.array([point_ii_xy]))
-
-    return Index_value
-
-
-def to_fwf(df, fname):
-    content = tabulate(df.values.tolist(), list(df.columns), tablefmt="plain")
-    open(fname, "w").write(content)
-
-
-def save_outcat(outcat_name, outcat):
+def change_world2pix(outcat, data_wcs):
     """
-    # 保存LDC检测的直接结果，即单位为像素
-    :param outcat_name: 核表的路径
-    :param outcat: 核表数据
+    将算法检测的结果(像素单位)转换到天空坐标系上去
     :return:
-    """
-
-    outcat_colums = outcat.shape[1]
-    pd.DataFrame.to_fwf = to_fwf
-    if outcat_colums == 10:
-        # 2d result
-        table_title = ['ID', 'Peak1', 'Peak2', 'Cen1', 'Cen2', 'Size1', 'Size2', 'Peak', 'Sum', 'Volume']
-        dataframe = pd.DataFrame(outcat, columns=table_title)
-        dataframe = dataframe.round({'ID': 0, 'Peak1': 0, 'Peak2': 0, 'Cen1': 3, 'Cen2': 3,
-                                     'Size1': 3, 'Size2': 3, 'Peak': 3, 'Sum': 3, 'Volume': 3})
-        dataframe.to_csv(outcat_name, sep='\t', index=False)
-        # dataframe.to_fwf(detected_outcat_name)
-    elif outcat_colums == 13:
-        # 3d result
-        table_title = ['ID', 'Peak1', 'Peak2', 'Peak3', 'Cen1', 'Cen2', 'Cen3', 'Size1', 'Size2', 'Size3', 'Peak', 'Sum',
-                       'Volume']
-        dataframe = pd.DataFrame(outcat, columns=table_title)
-        dataframe = dataframe.round({'ID': 0, 'Peak1': 0, 'Peak2': 0, 'Peak3': 0, 'Cen1': 3, 'Cen2': 3, 'Cen3': 3,
-                                     'Size1': 3, 'Size2': 3, 'Size3': 3, 'Peak': 3, 'Sum': 3, 'Volume': 3})
-        dataframe.to_csv(outcat_name, sep='\t', index=False)
-        # dataframe.to_fwf(detected_outcat_name)
-
-    elif outcat_colums == 11:
-        # fitting 2d data result
-        fit_outcat_name = outcat_name
-        fit_outcat = outcat
-        table_title = ['ID', 'Peak1', 'Peak2', 'Cen1', 'Cen2', 'Size1', 'Size2', 'theta', 'Peak',
-                       'Sum', 'Volume']
-        dataframe = pd.DataFrame(fit_outcat, columns=table_title)
-        dataframe = dataframe.round(
-            {'ID': 0, 'Peak1': 3, 'Peak2': 3, 'Cen1': 3, 'Cen2': 3, 'Size1': 3, 'Size2': 3, 'theta': 3, 'Peak': 3,
-             'Sum': 3, 'Volume': 3})
-        dataframe.to_csv(fit_outcat_name, sep='\t', index=False)
-        # dataframe.to_fwf(fit_outcat_name)
-    else:
-        print('outcat columns is %d' % outcat_colums)
-
+    outcat_wcs
+    ['ID', 'Peak1', 'Peak2', 'Peak3', 'Cen1', 'Cen2', 'Cen3', 'Size1', 'Size2', 'Size3', 'Peak', 'Sum', 'Volume']
+    -->3d
 
-def get_wcs(data_name):
-    """
-    得到wcs信息
-    :param data_name: fits文件
-    :return:
-    data_wcs
+     ['ID', 'Peak1', 'Peak2', 'Cen1', 'Cen2',  'Size1', 'Size2', 'Peak', 'Sum', 'Volume']
+     -->2d
     """
-    data_header = fits.getheader(data_name)
-    keys = data_header.keys()
-    key = [k for k in keys if k.endswith('4')]
-    [data_header.remove(k) for k in key]
-
-    try:
-        data_header.remove('VELREF')
-    except:
-        pass
-    data_wcs = wcs.WCS(data_header)
-
-    return data_wcs
+    # outcat_record = self.result.outcat_record
+    table_title = outcat.keys()
+    if outcat is None:
+        return None
+    else:
+        if 'Cen3' not in table_title:
+            # 2d result
+            peak1, peak2 = data_wcs.all_world2pix(outcat['Peak1'], outcat['Peak2'], 1)
+            cen1, cen2 = data_wcs.all_pix2world(outcat['Cen1'], outcat['Cen2'], 1)
+            size1, size2 = np.array([outcat['Size1'] * 30, outcat['Size2'] * 30])
+
+            clump_Peak = np.column_stack([peak1, peak2])
+            clump_Cen = np.column_stack([cen1, cen2])
+            clustSize = np.column_stack([size1, size2])
+            clustPeak, clustSum, clustVolume = np.array([outcat['Peak'], outcat['Sum'], outcat['Volume']])
+
+            id_clumps = []  # MWSIP017.558+00.150+020.17  分别表示：银经：17.558°， 银纬：0.15°，速度：20.17km/s
+            for item_l, item_b in zip(cen1, cen2):
+                str_l = 'MWSIP' + ('%.03f' % item_l).rjust(7, '0')
+                if item_b < 0:
+                    str_b = '-' + ('%.03f' % abs(item_b)).rjust(6, '0')
+                else:
+                    str_b = '+' + ('%.03f' % abs(item_b)).rjust(6, '0')
+                id_clumps.append(str_l + str_b)
+            id_clumps = np.array(id_clumps)
+
+        elif 'Cen3' in table_title:
+            # 3d result
+            peak1, peak2, peak3 = data_wcs.all_world2pix(outcat['Peak1'], outcat['Peak2'], outcat['Peak3']*1000, 1)
+            cen1, cen2, cen3 = data_wcs.all_world2pix(outcat['Cen1'], outcat['Cen2'], outcat['Cen3']*1000, 1)
+            size1, size2, size3 = np.array([outcat['Size1'] / 30, outcat['Size2'] / 30, outcat['Size3'] / 0.166])
+            clustPeak, clustSum, clustVolume = np.array([outcat['Peak'], outcat['Sum'], outcat['Volume']])
+
+            clump_Peak = np.column_stack([peak1, peak2, peak3])
+            clump_Cen = np.column_stack([cen1, cen2, cen3])
+            clustSize = np.column_stack([size1, size2, size3])
+            id_clumps = outcat['ID']
+        else:
+            print('outcat_record columns name are: ' % table_title)
+            return None
+
+        outcat = np.column_stack(
+            (id_clumps, clump_Peak, clump_Cen, clustSize, clustPeak, clustSum, clustVolume))
+        outcat = pd.DataFrame(outcat, columns=table_title)
+        return outcat
 
 
-def change_pix2word(data_wcs, outcat):
+def change_world2pix_fit(outcat, data_wcs):
     """
     将算法检测的结果(像素单位)转换到天空坐标系上去
-    :param data_wcs: 头文件得到的wcs
-    :param outcat: 算法检测核表
     :return:
     outcat_wcs
-    ['ID', 'Peak1', 'Peak2', 'Peak3', 'Cen1', 'Cen2', 'Cen3', 'Size1', 'Size2', 'Size3', 'Peak', 'Sum', 'Volume'] -->3d
-     ['ID', 'Peak1', 'Peak2', 'Cen1', 'Cen2',  'Size1', 'Size2', 'Peak', 'Sum', 'Volume']-->2d
-    """
-    outcat_column = outcat.shape[1]
-
-    if outcat_column == 10:
-        # 2d result
-        peak1, peak2 = data_wcs.all_pix2world(outcat['Peak1'], outcat['Peak2'], 1)
-        clump_Peak = np.column_stack([peak1, peak2])
-        cen1, cen2 = data_wcs.all_pix2world(outcat['Cen1'], outcat['Cen2'], 1)
-        clump_Cen = np.column_stack([cen1, cen2])
-        size1, size2 = np.array([outcat['Size1'] * 30, outcat['Size2'] * 30])
-        clustSize = np.column_stack([size1, size2])
-        clustPeak, clustSum, clustVolume = np.array([outcat['Peak'], outcat['Sum'], outcat['Volume']])
-        id_clumps = []  # MWSIP017.558+00.150+020.17  分别表示：银经：17.558°， 银纬：0.15°，速度：20.17km/s
-        for item_l, item_b in zip(cen1, cen2):
-            str_l = 'MWSIP' + ('%.03f' % item_l).rjust(7, '0')
-            if item_b < 0:
-                str_b = '-' + ('%.03f' % abs(item_b)).rjust(6, '0')
-            else:
-                str_b = '+' + ('%.03f' % abs(item_b)).rjust(6, '0')
-            id_clumps.append(str_l + str_b)
-        id_clumps = np.array(id_clumps)
-
-    elif outcat_column == 13:
-        # 3d result
-        peak1, peak2, peak3 = data_wcs.all_pix2world(outcat['Peak1'], outcat['Peak2'], outcat['Peak3'], 1)
-        clump_Peak = np.column_stack([peak1, peak2, peak3 / 1000])
-        cen1, cen2, cen3 = data_wcs.all_pix2world(outcat['Cen1'], outcat['Cen2'], outcat['Cen3'], 1)
-        clump_Cen = np.column_stack([cen1, cen2, cen3 / 1000])
-        size1, size2, size3 = np.array([outcat['Size1'] * 30, outcat['Size2'] * 30, outcat['Size3'] * 0.166])
-        clustSize = np.column_stack([size1, size2, size3])
-        clustPeak, clustSum, clustVolume = np.array([outcat['Peak'], outcat['Sum'], outcat['Volume']])
-
-        id_clumps = []  # G017.558+00.150+020.17  分别表示：银经：17.558°， 银纬：0.15°，速度：20.17km/s
-        for item_l, item_b, item_v in zip(cen1, cen2, cen3 / 1000):
-            str_l = 'MWISP' + ('%.03f' % item_l).rjust(7, '0')
-            if item_b < 0:
-                str_b = '-' + ('%.03f' % abs(item_b)).rjust(6, '0')
-            else:
-                str_b = '+' + ('%.03f' % abs(item_b)).rjust(6, '0')
-            if item_v < 0:
-                str_v = '-' + ('%.03f' % abs(item_v)).rjust(6, '0')
-            else:
-                str_v = '+' + ('%.03f' % abs(item_v)).rjust(6, '0')
-            id_clumps.append(str_l + str_b + str_v)
-        id_clumps = np.array(id_clumps)
-    else:
-        print('outcat columns is %d' % outcat_column)
+    ['ID', 'Galactic_Longitude', 'Galactic_Latitude', 'Velocity',
+       'Size_major', 'Size_minor', 'Size_velocity', 'Theta', 'Peak', 'Flux',
+       'Flux_SNR', 'Peak_SNR', 'Success', 'Cost']
+    -->3d
+
+     ['ID', 'Peak1', 'Peak2', 'Cen1', 'Cen2',  'Size1', 'Size2', 'Peak', 'Sum', 'Volume']
+     -->2d
+    """
+    # outcat_record = self.result.outcat_record
+    table_title = outcat.keys()
+    Theta = outcat['Theta'].values
+    Flux_SNR_Cost = outcat[['Flux_SNR', 'Peak_SNR', 'Success', 'Cost']]
+    if outcat is None:
         return None
-
-    outcat_wcs = np.column_stack((id_clumps, clump_Peak, clump_Cen, clustSize, clustPeak, clustSum, clustVolume))
-    return outcat_wcs
-
-
-def get_outcat_local(outcat):
-    """
-    返回局部区域的检测结果：
-    原始图为120*120  局部区域为30-->90, 30-->90 左开右闭
-    :param outcat:
-    :return:
-    """
-    # outcat = pd.read_csv(txt_name, sep='\t')
-    cen1_min = 30
-    cen1_max = 90
-    cen2_min = 30
-    cen2_max = 90
-    aa = outcat.loc[outcat['Cen1'] > cen1_min]
-    aa = aa.loc[outcat['Cen1'] <= cen1_max]
-    aa = aa.loc[outcat['Cen2'] > cen2_min]
-    aa = aa.loc[outcat['Cen2'] <= cen2_max]
-    return aa
+    else:
+        if 'Velocity' not in table_title:
+            # 2d result
+            peak1, peak2 = data_wcs.all_world2pix(outcat['Peak1'], outcat['Peak2'], 1)
+            cen1, cen2 = data_wcs.all_pix2world(outcat['Cen1'], outcat['Cen2'], 1)
+            size1, size2 = np.array([outcat['Size1'] * 30, outcat['Size2'] * 30])
+
+            clump_Peak = np.column_stack([peak1, peak2])
+            clump_Cen = np.column_stack([cen1, cen2])
+            clustSize = np.column_stack([size1, size2])
+            clustPeak, clustSum, clustVolume = np.array([outcat['Peak'], outcat['Sum'], outcat['Volume']])
+
+            id_clumps = []  # MWSIP017.558+00.150+020.17  分别表示：银经：17.558°， 银纬：0.15°，速度：20.17km/s
+            for item_l, item_b in zip(cen1, cen2):
+                str_l = 'MWSIP' + ('%.03f' % item_l).rjust(7, '0')
+                if item_b < 0:
+                    str_b = '-' + ('%.03f' % abs(item_b)).rjust(6, '0')
+                else:
+                    str_b = '+' + ('%.03f' % abs(item_b)).rjust(6, '0')
+                id_clumps.append(str_l + str_b)
+            id_clumps = np.array(id_clumps)
+
+        elif 'Velocity' in table_title:
+            # 3d result
+            cen1, cen2, cen3 = data_wcs.all_world2pix(outcat['Galactic_Longitude'], outcat['Galactic_Latitude'],
+                                                      outcat['Velocity'] * 1000, 1)
+            size1, size2, size3 = np.array(
+                [outcat['Size_major'] / 30, outcat['Size_minor'] / 30, outcat['Size_velocity'] / 0.166])
+            clustPeak, clustSum = np.array([outcat['Peak'], outcat['Flux']])
+
+            clump_Cen = np.column_stack([cen1, cen2, cen3])
+            clustSize = np.column_stack([size1, size2, size3])
+            id_clumps = outcat['ID']
+        else:
+            print('outcat_record columns name are: ' % table_title)
+            return None
+
+        outcat = np.column_stack(
+            (id_clumps, clump_Cen, clustSize, Theta, clustPeak, clustSum, Flux_SNR_Cost))
+        outcat = pd.DataFrame(outcat, columns=table_title)
+        return outcat
 
 
 if __name__ == '__main__':
-    xm, ym, zm = 100, 80, 120
-    r = 3
-    delta_ii_xy = np.array([43, 22, 109])
-    t0 = time.time()
-    index, index_value = kc_coord_3d(delta_ii_xy, xm, ym, zm, r)
-    t1 = time.time()
-    print((t1-t0) * 10000000)
-    delta_ii_xy = np.array([43, 22])
-    aa1 = kc_coord_2d(delta_ii_xy, xm, ym, r)
+    data_path = r'D:\LDC\test_data\R2_R16_region\0145-005_L.fits'
+    save_path = r'D:\LDC\test_data\R2_R16_region\0145-005_L13_noise_2_rho_3'
+    outcat_all = get_outcat_wcs_all(save_path, data_path)
+    outcat_all.to_csv(os.path.join(save_path, 'LDC_auto_outcat.csv'), index=False)
+
```

