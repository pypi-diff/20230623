# Comparing `tmp/phonenumbers-8.9.8.tar.gz` & `tmp/phonenumbers-8.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phonenumbers-8.9.8.tar", last modified: Sat Jun 16 06:53:18 2018, max compression
+gzip compressed data, was "dist/phonenumbers-8.9.9.tar", last modified: Fri Jun 29 07:35:41 2018, max compression
```

## Comparing `phonenumbers-8.9.8.tar` & `phonenumbers-8.9.9.tar`

### file list

```diff
@@ -1,671 +1,671 @@
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/
--rw-r--r--   0 dmd        (501) staff       (20)      115 2014-12-16 15:23:29.000000 phonenumbers-8.9.8/MANIFEST.in
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/phonenumbers/
--rw-r--r--   0 dmd        (501) staff       (20)     9853 2018-06-16 06:46:56.000000 phonenumbers-8.9.8/phonenumbers/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)    31975 2017-04-19 13:38:31.000000 phonenumbers-8.9.8/phonenumbers/asyoutypeformatter.py
--rw-r--r--   0 dmd        (501) staff       (20)     6352 2013-11-15 12:19:09.000000 phonenumbers-8.9.8/phonenumbers/carrier.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/phonenumbers/carrierdata/
--rw-r--r--   0 dmd        (501) staff       (20)      936 2018-06-16 06:46:07.000000 phonenumbers-8.9.8/phonenumbers/carrierdata/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)   308533 2018-06-16 06:46:07.000000 phonenumbers-8.9.8/phonenumbers/carrierdata/data0.py
--rw-r--r--   0 dmd        (501) staff       (20)   346243 2018-06-16 06:46:07.000000 phonenumbers-8.9.8/phonenumbers/carrierdata/data1.py
--rw-r--r--   0 dmd        (501) staff       (20)   140640 2018-06-16 06:46:07.000000 phonenumbers-8.9.8/phonenumbers/carrierdata/data2.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/phonenumbers/data/
--rw-r--r--   0 dmd        (501) staff       (20)    10295 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)      339 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_255.py
--rw-r--r--   0 dmd        (501) staff       (20)      232 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_27.py
--rw-r--r--   0 dmd        (501) staff       (20)      228 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_30.py
--rw-r--r--   0 dmd        (501) staff       (20)      436 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_31.py
--rw-r--r--   0 dmd        (501) staff       (20)      348 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_34.py
--rw-r--r--   0 dmd        (501) staff       (20)      217 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_350.py
--rw-r--r--   0 dmd        (501) staff       (20)      454 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_351.py
--rw-r--r--   0 dmd        (501) staff       (20)      199 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_352.py
--rw-r--r--   0 dmd        (501) staff       (20)      360 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_358.py
--rw-r--r--   0 dmd        (501) staff       (20)      482 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_359.py
--rw-r--r--   0 dmd        (501) staff       (20)      328 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_36.py
--rw-r--r--   0 dmd        (501) staff       (20)      572 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_372.py
--rw-r--r--   0 dmd        (501) staff       (20)      353 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_373.py
--rw-r--r--   0 dmd        (501) staff       (20)      493 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_380.py
--rw-r--r--   0 dmd        (501) staff       (20)      754 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_381.py
--rw-r--r--   0 dmd        (501) staff       (20)      545 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_385.py
--rw-r--r--   0 dmd        (501) staff       (20)      377 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_39.py
--rw-r--r--   0 dmd        (501) staff       (20)     1480 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_43.py
--rw-r--r--   0 dmd        (501) staff       (20)      689 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_44.py
--rw-r--r--   0 dmd        (501) staff       (20)     7207 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_49.py
--rw-r--r--   0 dmd        (501) staff       (20)      226 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_505.py
--rw-r--r--   0 dmd        (501) staff       (20)      241 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_506.py
--rw-r--r--   0 dmd        (501) staff       (20)      404 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_52.py
--rw-r--r--   0 dmd        (501) staff       (20)      343 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_54.py
--rw-r--r--   0 dmd        (501) staff       (20)      224 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_55.py
--rw-r--r--   0 dmd        (501) staff       (20)      197 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_58.py
--rw-r--r--   0 dmd        (501) staff       (20)      500 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_595.py
--rw-r--r--   0 dmd        (501) staff       (20)      589 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_61.py
--rw-r--r--   0 dmd        (501) staff       (20)      589 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_62.py
--rw-r--r--   0 dmd        (501) staff       (20)      215 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_63.py
--rw-r--r--   0 dmd        (501) staff       (20)      348 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_64.py
--rw-r--r--   0 dmd        (501) staff       (20)      216 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_66.py
--rw-r--r--   0 dmd        (501) staff       (20)      230 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_675.py
--rw-r--r--   0 dmd        (501) staff       (20)      230 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_676.py
--rw-r--r--   0 dmd        (501) staff       (20)      227 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_679.py
--rw-r--r--   0 dmd        (501) staff       (20)      696 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_7.py
--rw-r--r--   0 dmd        (501) staff       (20)      479 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_81.py
--rw-r--r--   0 dmd        (501) staff       (20)      343 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_84.py
--rw-r--r--   0 dmd        (501) staff       (20)      213 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_855.py
--rw-r--r--   0 dmd        (501) staff       (20)      415 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_856.py
--rw-r--r--   0 dmd        (501) staff       (20)      269 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_90.py
--rw-r--r--   0 dmd        (501) staff       (20)      973 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_91.py
--rw-r--r--   0 dmd        (501) staff       (20)      431 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_94.py
--rw-r--r--   0 dmd        (501) staff       (20)      224 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_95.py
--rw-r--r--   0 dmd        (501) staff       (20)      236 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_971.py
--rw-r--r--   0 dmd        (501) staff       (20)      248 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_972.py
--rw-r--r--   0 dmd        (501) staff       (20)      254 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/alt_format_995.py
--rw-r--r--   0 dmd        (501) staff       (20)      509 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_800.py
--rw-r--r--   0 dmd        (501) staff       (20)      511 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_808.py
--rw-r--r--   0 dmd        (501) staff       (20)      544 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_870.py
--rw-r--r--   0 dmd        (501) staff       (20)      527 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_878.py
--rw-r--r--   0 dmd        (501) staff       (20)      557 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_881.py
--rw-r--r--   0 dmd        (501) staff       (20)     1650 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_882.py
--rw-r--r--   0 dmd        (501) staff       (20)      838 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_883.py
--rw-r--r--   0 dmd        (501) staff       (20)      522 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_888.py
--rw-r--r--   0 dmd        (501) staff       (20)      522 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_979.py
--rw-r--r--   0 dmd        (501) staff       (20)      674 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1310 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AD.py
--rw-r--r--   0 dmd        (501) staff       (20)     1871 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AE.py
--rw-r--r--   0 dmd        (501) staff       (20)      902 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AF.py
--rw-r--r--   0 dmd        (501) staff       (20)     1556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1231 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AI.py
--rw-r--r--   0 dmd        (501) staff       (20)     1981 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AL.py
--rw-r--r--   0 dmd        (501) staff       (20)     1951 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AM.py
--rw-r--r--   0 dmd        (501) staff       (20)      670 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AO.py
--rw-r--r--   0 dmd        (501) staff       (20)     7150 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1235 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AS.py
--rw-r--r--   0 dmd        (501) staff       (20)     3044 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AT.py
--rw-r--r--   0 dmd        (501) staff       (20)     3275 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AU.py
--rw-r--r--   0 dmd        (501) staff       (20)     1075 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AW.py
--rw-r--r--   0 dmd        (501) staff       (20)     1611 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AX.py
--rw-r--r--   0 dmd        (501) staff       (20)     1611 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_AZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1889 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1728 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BB.py
--rw-r--r--   0 dmd        (501) staff       (20)     3300 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BD.py
--rw-r--r--   0 dmd        (501) staff       (20)     1940 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BE.py
--rw-r--r--   0 dmd        (501) staff       (20)      757 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BF.py
--rw-r--r--   0 dmd        (501) staff       (20)     2554 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1235 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BH.py
--rw-r--r--   0 dmd        (501) staff       (20)      675 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BI.py
--rw-r--r--   0 dmd        (501) staff       (20)      951 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      699 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BL.py
--rw-r--r--   0 dmd        (501) staff       (20)     1251 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BM.py
--rw-r--r--   0 dmd        (501) staff       (20)      717 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BN.py
--rw-r--r--   0 dmd        (501) staff       (20)     1494 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BO.py
--rw-r--r--   0 dmd        (501) staff       (20)      656 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BQ.py
--rw-r--r--   0 dmd        (501) staff       (20)     3258 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1711 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BS.py
--rw-r--r--   0 dmd        (501) staff       (20)      931 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1280 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BW.py
--rw-r--r--   0 dmd        (501) staff       (20)     3067 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BY.py
--rw-r--r--   0 dmd        (501) staff       (20)      971 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_BZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1627 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1633 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1313 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CD.py
--rw-r--r--   0 dmd        (501) staff       (20)      780 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CF.py
--rw-r--r--   0 dmd        (501) staff       (20)     1059 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CG.py
--rw-r--r--   0 dmd        (501) staff       (20)     2082 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CH.py
--rw-r--r--   0 dmd        (501) staff       (20)      767 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CI.py
--rw-r--r--   0 dmd        (501) staff       (20)      645 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CK.py
--rw-r--r--   0 dmd        (501) staff       (20)     3573 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CL.py
--rw-r--r--   0 dmd        (501) staff       (20)      963 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CM.py
--rw-r--r--   0 dmd        (501) staff       (20)     7253 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CN.py
--rw-r--r--   0 dmd        (501) staff       (20)     2114 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1448 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1208 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CU.py
--rw-r--r--   0 dmd        (501) staff       (20)      710 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CV.py
--rw-r--r--   0 dmd        (501) staff       (20)     1144 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CW.py
--rw-r--r--   0 dmd        (501) staff       (20)     1644 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CX.py
--rw-r--r--   0 dmd        (501) staff       (20)     1281 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CY.py
--rw-r--r--   0 dmd        (501) staff       (20)     1951 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_CZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     5878 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_DE.py
--rw-r--r--   0 dmd        (501) staff       (20)      665 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_DJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      983 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_DK.py
--rw-r--r--   0 dmd        (501) staff       (20)     1266 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_DM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1569 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_DO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1711 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_DZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1900 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_EC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1876 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_EE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1682 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_EG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1055 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_EH.py
--rw-r--r--   0 dmd        (501) staff       (20)      850 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_ER.py
--rw-r--r--   0 dmd        (501) staff       (20)     1724 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_ES.py
--rw-r--r--   0 dmd        (501) staff       (20)     1500 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_ET.py
--rw-r--r--   0 dmd        (501) staff       (20)     2484 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_FI.py
--rw-r--r--   0 dmd        (501) staff       (20)     1021 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_FJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_FK.py
--rw-r--r--   0 dmd        (501) staff       (20)      672 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_FM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1137 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_FO.py
--rw-r--r--   0 dmd        (501) staff       (20)     2032 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_FR.py
--rw-r--r--   0 dmd        (501) staff       (20)      850 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GA.py
--rw-r--r--   0 dmd        (501) staff       (20)     5117 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GB.py
--rw-r--r--   0 dmd        (501) staff       (20)     1331 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GD.py
--rw-r--r--   0 dmd        (501) staff       (20)     1664 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GE.py
--rw-r--r--   0 dmd        (501) staff       (20)      868 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GF.py
--rw-r--r--   0 dmd        (501) staff       (20)     1706 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1483 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GH.py
--rw-r--r--   0 dmd        (501) staff       (20)      728 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GI.py
--rw-r--r--   0 dmd        (501) staff       (20)      915 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GL.py
--rw-r--r--   0 dmd        (501) staff       (20)      732 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GM.py
--rw-r--r--   0 dmd        (501) staff       (20)      979 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GN.py
--rw-r--r--   0 dmd        (501) staff       (20)      980 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GP.py
--rw-r--r--   0 dmd        (501) staff       (20)     1089 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GQ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1837 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1044 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1602 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GU.py
--rw-r--r--   0 dmd        (501) staff       (20)      929 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GW.py
--rw-r--r--   0 dmd        (501) staff       (20)      971 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_GY.py
--rw-r--r--   0 dmd        (501) staff       (20)     2482 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_HK.py
--rw-r--r--   0 dmd        (501) staff       (20)      882 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_HN.py
--rw-r--r--   0 dmd        (501) staff       (20)     2452 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_HR.py
--rw-r--r--   0 dmd        (501) staff       (20)      924 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_HT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1719 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_HU.py
--rw-r--r--   0 dmd        (501) staff       (20)     3599 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_ID.py
--rw-r--r--   0 dmd        (501) staff       (20)     3599 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_IE.py
--rw-r--r--   0 dmd        (501) staff       (20)     3179 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_IL.py
--rw-r--r--   0 dmd        (501) staff       (20)     1564 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_IM.py
--rw-r--r--   0 dmd        (501) staff       (20)     8650 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_IN.py
--rw-r--r--   0 dmd        (501) staff       (20)      621 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_IO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1210 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_IQ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1843 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_IR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1780 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_IS.py
--rw-r--r--   0 dmd        (501) staff       (20)     3308 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_IT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1830 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_JE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1505 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_JM.py
--rw-r--r--   0 dmd        (501) staff       (20)     2482 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_JO.py
--rw-r--r--   0 dmd        (501) staff       (20)    12833 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_JP.py
--rw-r--r--   0 dmd        (501) staff       (20)     1542 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_KE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1537 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_KG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1563 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_KH.py
--rw-r--r--   0 dmd        (501) staff       (20)      935 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_KI.py
--rw-r--r--   0 dmd        (501) staff       (20)      761 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_KM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1245 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_KN.py
--rw-r--r--   0 dmd        (501) staff       (20)     1339 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_KP.py
--rw-r--r--   0 dmd        (501) staff       (20)     5194 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_KR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1175 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_KW.py
--rw-r--r--   0 dmd        (501) staff       (20)     1514 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_KY.py
--rw-r--r--   0 dmd        (501) staff       (20)     1799 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_KZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1267 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_LA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1322 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_LB.py
--rw-r--r--   0 dmd        (501) staff       (20)     1291 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_LC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1661 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_LI.py
--rw-r--r--   0 dmd        (501) staff       (20)     1082 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_LK.py
--rw-r--r--   0 dmd        (501) staff       (20)     1319 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_LR.py
--rw-r--r--   0 dmd        (501) staff       (20)      751 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_LS.py
--rw-r--r--   0 dmd        (501) staff       (20)     2129 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_LT.py
--rw-r--r--   0 dmd        (501) staff       (20)     3066 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_LU.py
--rw-r--r--   0 dmd        (501) staff       (20)     1069 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_LV.py
--rw-r--r--   0 dmd        (501) staff       (20)      873 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_LY.py
--rw-r--r--   0 dmd        (501) staff       (20)     2112 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1558 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1793 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MD.py
--rw-r--r--   0 dmd        (501) staff       (20)     1487 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_ME.py
--rw-r--r--   0 dmd        (501) staff       (20)      723 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MF.py
--rw-r--r--   0 dmd        (501) staff       (20)     1051 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MG.py
--rw-r--r--   0 dmd        (501) staff       (20)      832 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MH.py
--rw-r--r--   0 dmd        (501) staff       (20)     1741 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MK.py
--rw-r--r--   0 dmd        (501) staff       (20)     1287 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_ML.py
--rw-r--r--   0 dmd        (501) staff       (20)     3206 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1778 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MN.py
--rw-r--r--   0 dmd        (501) staff       (20)      749 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1370 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MP.py
--rw-r--r--   0 dmd        (501) staff       (20)      893 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MQ.py
--rw-r--r--   0 dmd        (501) staff       (20)      845 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1184 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MS.py
--rw-r--r--   0 dmd        (501) staff       (20)     1417 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1368 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MU.py
--rw-r--r--   0 dmd        (501) staff       (20)     1312 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MV.py
--rw-r--r--   0 dmd        (501) staff       (20)     1423 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MW.py
--rw-r--r--   0 dmd        (501) staff       (20)     3655 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MX.py
--rw-r--r--   0 dmd        (501) staff       (20)    10145 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MY.py
--rw-r--r--   0 dmd        (501) staff       (20)      946 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_MZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1865 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_NA.py
--rw-r--r--   0 dmd        (501) staff       (20)      849 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_NC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1131 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_NE.py
--rw-r--r--   0 dmd        (501) staff       (20)      877 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_NF.py
--rw-r--r--   0 dmd        (501) staff       (20)     2676 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_NG.py
--rw-r--r--   0 dmd        (501) staff       (20)      830 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_NI.py
--rw-r--r--   0 dmd        (501) staff       (20)     2894 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_NL.py
--rw-r--r--   0 dmd        (501) staff       (20)     1842 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_NO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1351 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_NP.py
--rw-r--r--   0 dmd        (501) staff       (20)      639 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_NR.py
--rw-r--r--   0 dmd        (501) staff       (20)      544 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_NU.py
--rw-r--r--   0 dmd        (501) staff       (20)     2373 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_NZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1220 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_OM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1561 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_PA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1894 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_PE.py
--rw-r--r--   0 dmd        (501) staff       (20)      964 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_PF.py
--rw-r--r--   0 dmd        (501) staff       (20)     1158 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_PG.py
--rw-r--r--   0 dmd        (501) staff       (20)     2440 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_PH.py
--rw-r--r--   0 dmd        (501) staff       (20)     3443 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_PK.py
--rw-r--r--   0 dmd        (501) staff       (20)     2278 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_PL.py
--rw-r--r--   0 dmd        (501) staff       (20)      796 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_PM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1244 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_PR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1469 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_PS.py
--rw-r--r--   0 dmd        (501) staff       (20)     1847 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_PT.py
--rw-r--r--   0 dmd        (501) staff       (20)      732 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_PW.py
--rw-r--r--   0 dmd        (501) staff       (20)     2353 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_PY.py
--rw-r--r--   0 dmd        (501) staff       (20)     1062 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_QA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1335 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_RE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1919 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_RO.py
--rw-r--r--   0 dmd        (501) staff       (20)     2300 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_RS.py
--rw-r--r--   0 dmd        (501) staff       (20)     2121 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_RU.py
--rw-r--r--   0 dmd        (501) staff       (20)     1277 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_RW.py
--rw-r--r--   0 dmd        (501) staff       (20)     1819 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1060 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SB.py
--rw-r--r--   0 dmd        (501) staff       (20)      971 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SC.py
--rw-r--r--   0 dmd        (501) staff       (20)      775 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SD.py
--rw-r--r--   0 dmd        (501) staff       (20)     5804 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1596 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SG.py
--rw-r--r--   0 dmd        (501) staff       (20)      717 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SH.py
--rw-r--r--   0 dmd        (501) staff       (20)     1896 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SI.py
--rw-r--r--   0 dmd        (501) staff       (20)     1464 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SJ.py
--rw-r--r--   0 dmd        (501) staff       (20)     2668 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SK.py
--rw-r--r--   0 dmd        (501) staff       (20)      858 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SL.py
--rw-r--r--   0 dmd        (501) staff       (20)     1662 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1381 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SN.py
--rw-r--r--   0 dmd        (501) staff       (20)     1477 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1047 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SR.py
--rw-r--r--   0 dmd        (501) staff       (20)      754 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SS.py
--rw-r--r--   0 dmd        (501) staff       (20)      658 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_ST.py
--rw-r--r--   0 dmd        (501) staff       (20)     1172 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SV.py
--rw-r--r--   0 dmd        (501) staff       (20)     1233 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SX.py
--rw-r--r--   0 dmd        (501) staff       (20)     1195 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SY.py
--rw-r--r--   0 dmd        (501) staff       (20)     1270 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_SZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      425 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1402 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TC.py
--rw-r--r--   0 dmd        (501) staff       (20)      748 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TD.py
--rw-r--r--   0 dmd        (501) staff       (20)      735 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1570 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TH.py
--rw-r--r--   0 dmd        (501) staff       (20)     1583 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      590 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TK.py
--rw-r--r--   0 dmd        (501) staff       (20)     1162 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TL.py
--rw-r--r--   0 dmd        (501) staff       (20)     1247 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1103 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TN.py
--rw-r--r--   0 dmd        (501) staff       (20)     1057 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TO.py
--rw-r--r--   0 dmd        (501) staff       (20)     2448 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1509 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TT.py
--rw-r--r--   0 dmd        (501) staff       (20)      569 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TV.py
--rw-r--r--   0 dmd        (501) staff       (20)     2303 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TW.py
--rw-r--r--   0 dmd        (501) staff       (20)     1755 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_TZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     2242 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_UA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1657 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_UG.py
--rw-r--r--   0 dmd        (501) staff       (20)     2859 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_US.py
--rw-r--r--   0 dmd        (501) staff       (20)     1439 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_UY.py
--rw-r--r--   0 dmd        (501) staff       (20)     2430 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_UZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1604 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_VA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1309 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_VC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1162 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_VE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1310 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_VG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1412 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_VI.py
--rw-r--r--   0 dmd        (501) staff       (20)     3191 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_VN.py
--rw-r--r--   0 dmd        (501) staff       (20)      869 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_VU.py
--rw-r--r--   0 dmd        (501) staff       (20)      778 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_WF.py
--rw-r--r--   0 dmd        (501) staff       (20)     1030 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_WS.py
--rw-r--r--   0 dmd        (501) staff       (20)     1347 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_XK.py
--rw-r--r--   0 dmd        (501) staff       (20)     1088 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_YE.py
--rw-r--r--   0 dmd        (501) staff       (20)      833 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_YT.py
--rw-r--r--   0 dmd        (501) staff       (20)     2008 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_ZA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1370 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_ZM.py
--rw-r--r--   0 dmd        (501) staff       (20)     3290 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/data/region_ZW.py
--rw-r--r--   0 dmd        (501) staff       (20)    10966 2018-05-17 08:38:10.000000 phonenumbers-8.9.8/phonenumbers/geocoder.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/phonenumbers/geodata/
--rw-r--r--   0 dmd        (501) staff       (20)     2255 2018-06-16 06:46:07.000000 phonenumbers-8.9.8/phonenumbers/geodata/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)   355683 2018-06-16 06:46:03.000000 phonenumbers-8.9.8/phonenumbers/geodata/data0.py
--rw-r--r--   0 dmd        (501) staff       (20)   358303 2018-06-16 06:46:03.000000 phonenumbers-8.9.8/phonenumbers/geodata/data1.py
--rw-r--r--   0 dmd        (501) staff       (20)   327894 2018-06-16 06:46:04.000000 phonenumbers-8.9.8/phonenumbers/geodata/data10.py
--rw-r--r--   0 dmd        (501) staff       (20)   342087 2018-06-16 06:46:04.000000 phonenumbers-8.9.8/phonenumbers/geodata/data11.py
--rw-r--r--   0 dmd        (501) staff       (20)   466008 2018-06-16 06:46:04.000000 phonenumbers-8.9.8/phonenumbers/geodata/data12.py
--rw-r--r--   0 dmd        (501) staff       (20)   919549 2018-06-16 06:46:04.000000 phonenumbers-8.9.8/phonenumbers/geodata/data13.py
--rw-r--r--   0 dmd        (501) staff       (20)   915475 2018-06-16 06:46:04.000000 phonenumbers-8.9.8/phonenumbers/geodata/data14.py
--rw-r--r--   0 dmd        (501) staff       (20)   901730 2018-06-16 06:46:05.000000 phonenumbers-8.9.8/phonenumbers/geodata/data15.py
--rw-r--r--   0 dmd        (501) staff       (20)   913040 2018-06-16 06:46:05.000000 phonenumbers-8.9.8/phonenumbers/geodata/data16.py
--rw-r--r--   0 dmd        (501) staff       (20)   917750 2018-06-16 06:46:05.000000 phonenumbers-8.9.8/phonenumbers/geodata/data17.py
--rw-r--r--   0 dmd        (501) staff       (20)   921018 2018-06-16 06:46:05.000000 phonenumbers-8.9.8/phonenumbers/geodata/data18.py
--rw-r--r--   0 dmd        (501) staff       (20)   923238 2018-06-16 06:46:05.000000 phonenumbers-8.9.8/phonenumbers/geodata/data19.py
--rw-r--r--   0 dmd        (501) staff       (20)   358619 2018-06-16 06:46:03.000000 phonenumbers-8.9.8/phonenumbers/geodata/data2.py
--rw-r--r--   0 dmd        (501) staff       (20)   920700 2018-06-16 06:46:05.000000 phonenumbers-8.9.8/phonenumbers/geodata/data20.py
--rw-r--r--   0 dmd        (501) staff       (20)   919835 2018-06-16 06:46:06.000000 phonenumbers-8.9.8/phonenumbers/geodata/data21.py
--rw-r--r--   0 dmd        (501) staff       (20)   927988 2018-06-16 06:46:06.000000 phonenumbers-8.9.8/phonenumbers/geodata/data22.py
--rw-r--r--   0 dmd        (501) staff       (20)   908636 2018-06-16 06:46:06.000000 phonenumbers-8.9.8/phonenumbers/geodata/data23.py
--rw-r--r--   0 dmd        (501) staff       (20)   914964 2018-06-16 06:46:06.000000 phonenumbers-8.9.8/phonenumbers/geodata/data24.py
--rw-r--r--   0 dmd        (501) staff       (20)   920951 2018-06-16 06:46:06.000000 phonenumbers-8.9.8/phonenumbers/geodata/data25.py
--rw-r--r--   0 dmd        (501) staff       (20)   914124 2018-06-16 06:46:06.000000 phonenumbers-8.9.8/phonenumbers/geodata/data26.py
--rw-r--r--   0 dmd        (501) staff       (20)   923203 2018-06-16 06:46:07.000000 phonenumbers-8.9.8/phonenumbers/geodata/data27.py
--rw-r--r--   0 dmd        (501) staff       (20)   582151 2018-06-16 06:46:07.000000 phonenumbers-8.9.8/phonenumbers/geodata/data28.py
--rw-r--r--   0 dmd        (501) staff       (20)   390404 2018-06-16 06:46:03.000000 phonenumbers-8.9.8/phonenumbers/geodata/data3.py
--rw-r--r--   0 dmd        (501) staff       (20)   861636 2018-06-16 06:46:03.000000 phonenumbers-8.9.8/phonenumbers/geodata/data4.py
--rw-r--r--   0 dmd        (501) staff       (20)   609339 2018-06-16 06:46:03.000000 phonenumbers-8.9.8/phonenumbers/geodata/data5.py
--rw-r--r--   0 dmd        (501) staff       (20)   726827 2018-06-16 06:46:04.000000 phonenumbers-8.9.8/phonenumbers/geodata/data6.py
--rw-r--r--   0 dmd        (501) staff       (20)   461462 2018-06-16 06:46:04.000000 phonenumbers-8.9.8/phonenumbers/geodata/data7.py
--rw-r--r--   0 dmd        (501) staff       (20)   338194 2018-06-16 06:46:04.000000 phonenumbers-8.9.8/phonenumbers/geodata/data8.py
--rw-r--r--   0 dmd        (501) staff       (20)   330259 2018-06-16 06:46:04.000000 phonenumbers-8.9.8/phonenumbers/geodata/data9.py
--rw-r--r--   0 dmd        (501) staff       (20)   610934 2018-06-16 06:46:09.000000 phonenumbers-8.9.8/phonenumbers/geodata/locale.py
--rw-r--r--   0 dmd        (501) staff       (20)    32671 2018-05-17 08:40:03.000000 phonenumbers-8.9.8/phonenumbers/phonemetadata.py
--rw-r--r--   0 dmd        (501) staff       (20)    12452 2018-05-17 08:40:03.000000 phonenumbers-8.9.8/phonenumbers/phonenumber.py
--rw-r--r--   0 dmd        (501) staff       (20)    38746 2018-05-17 08:40:03.000000 phonenumbers-8.9.8/phonenumbers/phonenumbermatcher.py
--rw-r--r--   0 dmd        (501) staff       (20)   155085 2018-05-17 08:40:03.000000 phonenumbers-8.9.8/phonenumbers/phonenumberutil.py
--rw-r--r--   0 dmd        (501) staff       (20)     3650 2013-11-15 12:19:10.000000 phonenumbers-8.9.8/phonenumbers/prefix.py
--rw-r--r--   0 dmd        (501) staff       (20)     1428 2018-05-17 08:38:26.000000 phonenumbers-8.9.8/phonenumbers/re_util.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/phonenumbers/shortdata/
--rw-r--r--   0 dmd        (501) staff       (20)     2180 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AC.py
--rw-r--r--   0 dmd        (501) staff       (20)      558 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AD.py
--rw-r--r--   0 dmd        (501) staff       (20)      696 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AE.py
--rw-r--r--   0 dmd        (501) staff       (20)      807 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AF.py
--rw-r--r--   0 dmd        (501) staff       (20)      791 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AG.py
--rw-r--r--   0 dmd        (501) staff       (20)      773 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AI.py
--rw-r--r--   0 dmd        (501) staff       (20)     1131 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AL.py
--rw-r--r--   0 dmd        (501) staff       (20)      822 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AM.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1006 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AR.py
--rw-r--r--   0 dmd        (501) staff       (20)      676 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AS.py
--rw-r--r--   0 dmd        (501) staff       (20)      737 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1360 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AU.py
--rw-r--r--   0 dmd        (501) staff       (20)      788 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AW.py
--rw-r--r--   0 dmd        (501) staff       (20)      578 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AX.py
--rw-r--r--   0 dmd        (501) staff       (20)      826 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_AZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      786 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BA.py
--rw-r--r--   0 dmd        (501) staff       (20)      565 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BB.py
--rw-r--r--   0 dmd        (501) staff       (20)     1089 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BD.py
--rw-r--r--   0 dmd        (501) staff       (20)     1212 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BE.py
--rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BF.py
--rw-r--r--   0 dmd        (501) staff       (20)      717 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1146 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BH.py
--rw-r--r--   0 dmd        (501) staff       (20)      966 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BI.py
--rw-r--r--   0 dmd        (501) staff       (20)      822 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      541 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BL.py
--rw-r--r--   0 dmd        (501) staff       (20)      777 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BM.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BN.py
--rw-r--r--   0 dmd        (501) staff       (20)      684 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BO.py
--rw-r--r--   0 dmd        (501) staff       (20)      788 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BQ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1494 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BR.py
--rw-r--r--   0 dmd        (501) staff       (20)      554 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BS.py
--rw-r--r--   0 dmd        (501) staff       (20)      684 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BT.py
--rw-r--r--   0 dmd        (501) staff       (20)      801 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BW.py
--rw-r--r--   0 dmd        (501) staff       (20)      612 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BY.py
--rw-r--r--   0 dmd        (501) staff       (20)      568 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_BZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1044 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CA.py
--rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CC.py
--rw-r--r--   0 dmd        (501) staff       (20)      826 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CD.py
--rw-r--r--   0 dmd        (501) staff       (20)      580 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CF.py
--rw-r--r--   0 dmd        (501) staff       (20)      661 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1354 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CH.py
--rw-r--r--   0 dmd        (501) staff       (20)      814 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CI.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CK.py
--rw-r--r--   0 dmd        (501) staff       (20)     1650 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CL.py
--rw-r--r--   0 dmd        (501) staff       (20)      804 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CM.py
--rw-r--r--   0 dmd        (501) staff       (20)      734 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CN.py
--rw-r--r--   0 dmd        (501) staff       (20)      875 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CO.py
--rw-r--r--   0 dmd        (501) staff       (20)      891 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CR.py
--rw-r--r--   0 dmd        (501) staff       (20)      581 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CU.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CV.py
--rw-r--r--   0 dmd        (501) staff       (20)      788 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CW.py
--rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CX.py
--rw-r--r--   0 dmd        (501) staff       (20)      705 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CY.py
--rw-r--r--   0 dmd        (501) staff       (20)      768 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_CZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      706 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_DE.py
--rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_DJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      746 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_DK.py
--rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_DM.py
--rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_DO.py
--rw-r--r--   0 dmd        (501) staff       (20)      785 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_DZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      579 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_EC.py
--rw-r--r--   0 dmd        (501) staff       (20)     2417 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_EE.py
--rw-r--r--   0 dmd        (501) staff       (20)      824 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_EG.py
--rw-r--r--   0 dmd        (501) staff       (20)      572 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_EH.py
--rw-r--r--   0 dmd        (501) staff       (20)      678 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_ER.py
--rw-r--r--   0 dmd        (501) staff       (20)     1620 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_ES.py
--rw-r--r--   0 dmd        (501) staff       (20)      588 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_ET.py
--rw-r--r--   0 dmd        (501) staff       (20)      707 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_FI.py
--rw-r--r--   0 dmd        (501) staff       (20)      749 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_FJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_FK.py
--rw-r--r--   0 dmd        (501) staff       (20)      576 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_FM.py
--rw-r--r--   0 dmd        (501) staff       (20)      591 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_FO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1553 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_FR.py
--rw-r--r--   0 dmd        (501) staff       (20)      588 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1338 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GB.py
--rw-r--r--   0 dmd        (501) staff       (20)      773 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GD.py
--rw-r--r--   0 dmd        (501) staff       (20)      844 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GE.py
--rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GF.py
--rw-r--r--   0 dmd        (501) staff       (20)      636 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GG.py
--rw-r--r--   0 dmd        (501) staff       (20)      856 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GH.py
--rw-r--r--   0 dmd        (501) staff       (20)     1286 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GI.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GL.py
--rw-r--r--   0 dmd        (501) staff       (20)      566 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GM.py
--rw-r--r--   0 dmd        (501) staff       (20)      676 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GN.py
--rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GP.py
--rw-r--r--   0 dmd        (501) staff       (20)      719 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GR.py
--rw-r--r--   0 dmd        (501) staff       (20)      829 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GT.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GU.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GW.py
--rw-r--r--   0 dmd        (501) staff       (20)      860 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_GY.py
--rw-r--r--   0 dmd        (501) staff       (20)     1155 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_HK.py
--rw-r--r--   0 dmd        (501) staff       (20)      793 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_HN.py
--rw-r--r--   0 dmd        (501) staff       (20)     1134 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_HR.py
--rw-r--r--   0 dmd        (501) staff       (20)      799 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_HT.py
--rw-r--r--   0 dmd        (501) staff       (20)      727 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_HU.py
--rw-r--r--   0 dmd        (501) staff       (20)      831 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_ID.py
--rw-r--r--   0 dmd        (501) staff       (20)     1249 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_IE.py
--rw-r--r--   0 dmd        (501) staff       (20)      848 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_IL.py
--rw-r--r--   0 dmd        (501) staff       (20)      720 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_IM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1625 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_IN.py
--rw-r--r--   0 dmd        (501) staff       (20)      860 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_IQ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1368 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_IR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1007 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_IS.py
--rw-r--r--   0 dmd        (501) staff       (20)     1220 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_IT.py
--rw-r--r--   0 dmd        (501) staff       (20)      658 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_JE.py
--rw-r--r--   0 dmd        (501) staff       (20)      796 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_JM.py
--rw-r--r--   0 dmd        (501) staff       (20)      860 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_JO.py
--rw-r--r--   0 dmd        (501) staff       (20)      554 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_JP.py
--rw-r--r--   0 dmd        (501) staff       (20)     1594 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_KE.py
--rw-r--r--   0 dmd        (501) staff       (20)      796 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_KG.py
--rw-r--r--   0 dmd        (501) staff       (20)      810 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_KH.py
--rw-r--r--   0 dmd        (501) staff       (20)      725 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_KI.py
--rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_KM.py
--rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_KN.py
--rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_KP.py
--rw-r--r--   0 dmd        (501) staff       (20)      929 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_KR.py
--rw-r--r--   0 dmd        (501) staff       (20)      686 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_KW.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_KY.py
--rw-r--r--   0 dmd        (501) staff       (20)      841 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_KZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_LA.py
--rw-r--r--   0 dmd        (501) staff       (20)      579 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_LB.py
--rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_LC.py
--rw-r--r--   0 dmd        (501) staff       (20)      602 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_LI.py
--rw-r--r--   0 dmd        (501) staff       (20)      560 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_LK.py
--rw-r--r--   0 dmd        (501) staff       (20)      837 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_LR.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_LS.py
--rw-r--r--   0 dmd        (501) staff       (20)      760 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_LT.py
--rw-r--r--   0 dmd        (501) staff       (20)      712 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_LU.py
--rw-r--r--   0 dmd        (501) staff       (20)     1143 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_LV.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_LY.py
--rw-r--r--   0 dmd        (501) staff       (20)      572 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MA.py
--rw-r--r--   0 dmd        (501) staff       (20)      579 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MC.py
--rw-r--r--   0 dmd        (501) staff       (20)      786 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MD.py
--rw-r--r--   0 dmd        (501) staff       (20)      697 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_ME.py
--rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MF.py
--rw-r--r--   0 dmd        (501) staff       (20)      564 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MG.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MH.py
--rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MK.py
--rw-r--r--   0 dmd        (501) staff       (20)     1470 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_ML.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MM.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MN.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MO.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MP.py
--rw-r--r--   0 dmd        (501) staff       (20)      574 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MQ.py
--rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MR.py
--rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MS.py
--rw-r--r--   0 dmd        (501) staff       (20)      705 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MT.py
--rw-r--r--   0 dmd        (501) staff       (20)      594 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MU.py
--rw-r--r--   0 dmd        (501) staff       (20)      726 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MV.py
--rw-r--r--   0 dmd        (501) staff       (20)      810 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MW.py
--rw-r--r--   0 dmd        (501) staff       (20)      761 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MX.py
--rw-r--r--   0 dmd        (501) staff       (20)      952 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MY.py
--rw-r--r--   0 dmd        (501) staff       (20)      594 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_MZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      599 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_NA.py
--rw-r--r--   0 dmd        (501) staff       (20)      904 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_NC.py
--rw-r--r--   0 dmd        (501) staff       (20)      813 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_NE.py
--rw-r--r--   0 dmd        (501) staff       (20)      568 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_NF.py
--rw-r--r--   0 dmd        (501) staff       (20)      793 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_NG.py
--rw-r--r--   0 dmd        (501) staff       (20)      739 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_NI.py
--rw-r--r--   0 dmd        (501) staff       (20)     1035 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_NL.py
--rw-r--r--   0 dmd        (501) staff       (20)      743 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_NO.py
--rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_NP.py
--rw-r--r--   0 dmd        (501) staff       (20)      566 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_NR.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_NU.py
--rw-r--r--   0 dmd        (501) staff       (20)      901 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_NZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      552 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_OM.py
--rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_PA.py
--rw-r--r--   0 dmd        (501) staff       (20)      568 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_PE.py
--rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_PF.py
--rw-r--r--   0 dmd        (501) staff       (20)      741 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_PG.py
--rw-r--r--   0 dmd        (501) staff       (20)      565 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_PH.py
--rw-r--r--   0 dmd        (501) staff       (20)      599 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_PK.py
--rw-r--r--   0 dmd        (501) staff       (20)      773 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_PL.py
--rw-r--r--   0 dmd        (501) staff       (20)      678 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_PM.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_PR.py
--rw-r--r--   0 dmd        (501) staff       (20)      675 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_PS.py
--rw-r--r--   0 dmd        (501) staff       (20)      699 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_PT.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_PW.py
--rw-r--r--   0 dmd        (501) staff       (20)      565 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_PY.py
--rw-r--r--   0 dmd        (501) staff       (20)      589 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_QA.py
--rw-r--r--   0 dmd        (501) staff       (20)      574 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_RE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1043 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_RO.py
--rw-r--r--   0 dmd        (501) staff       (20)      602 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_RS.py
--rw-r--r--   0 dmd        (501) staff       (20)      595 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_RU.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_RW.py
--rw-r--r--   0 dmd        (501) staff       (20)     1045 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SA.py
--rw-r--r--   0 dmd        (501) staff       (20)      650 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SB.py
--rw-r--r--   0 dmd        (501) staff       (20)      638 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SC.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SD.py
--rw-r--r--   0 dmd        (501) staff       (20)     1316 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SE.py
--rw-r--r--   0 dmd        (501) staff       (20)      748 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SG.py
--rw-r--r--   0 dmd        (501) staff       (20)      582 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SH.py
--rw-r--r--   0 dmd        (501) staff       (20)      711 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SI.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      747 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SK.py
--rw-r--r--   0 dmd        (501) staff       (20)      808 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SL.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1279 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SN.py
--rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SO.py
--rw-r--r--   0 dmd        (501) staff       (20)      561 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SR.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_ST.py
--rw-r--r--   0 dmd        (501) staff       (20)      793 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SV.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SX.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SY.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_SZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_TC.py
--rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_TD.py
--rw-r--r--   0 dmd        (501) staff       (20)      587 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_TG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1672 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_TH.py
--rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_TJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      581 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_TL.py
--rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_TM.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_TN.py
--rw-r--r--   0 dmd        (501) staff       (20)      574 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_TO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1767 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_TR.py
--rw-r--r--   0 dmd        (501) staff       (20)      554 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_TT.py
--rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_TV.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_TW.py
--rw-r--r--   0 dmd        (501) staff       (20)      808 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_TZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      956 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_UA.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_UG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1618 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_US.py
--rw-r--r--   0 dmd        (501) staff       (20)      707 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_UY.py
--rw-r--r--   0 dmd        (501) staff       (20)      833 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_UZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      558 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_VA.py
--rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_VC.py
--rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_VE.py
--rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_VG.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_VI.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_VN.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_VU.py
--rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_WF.py
--rw-r--r--   0 dmd        (501) staff       (20)      710 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_WS.py
--rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_XK.py
--rw-r--r--   0 dmd        (501) staff       (20)      558 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_YE.py
--rw-r--r--   0 dmd        (501) staff       (20)      567 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_YT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1188 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_ZA.py
--rw-r--r--   0 dmd        (501) staff       (20)      575 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_ZM.py
--rw-r--r--   0 dmd        (501) staff       (20)      976 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/phonenumbers/shortdata/region_ZW.py
--rw-r--r--   0 dmd        (501) staff       (20)    20748 2018-05-17 08:40:03.000000 phonenumbers-8.9.8/phonenumbers/shortnumberinfo.py
--rw-r--r--   0 dmd        (501) staff       (20)     4947 2018-05-17 08:38:10.000000 phonenumbers-8.9.8/phonenumbers/timezone.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/phonenumbers/tzdata/
--rw-r--r--   0 dmd        (501) staff       (20)      824 2018-06-16 06:46:07.000000 phonenumbers-8.9.8/phonenumbers/tzdata/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)   244375 2018-06-16 06:46:07.000000 phonenumbers-8.9.8/phonenumbers/tzdata/data0.py
--rw-r--r--   0 dmd        (501) staff       (20)    18939 2013-11-15 12:19:10.000000 phonenumbers-8.9.8/phonenumbers/unicode_util.py
--rw-r--r--   0 dmd        (501) staff       (20)     5865 2016-01-29 10:59:27.000000 phonenumbers-8.9.8/phonenumbers/util.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/phonenumbers.egg-info/
--rw-r--r--   0 dmd        (501) staff       (20)        1 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/phonenumbers.egg-info/dependency_links.txt
--rw-r--r--   0 dmd        (501) staff       (20)      924 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/phonenumbers.egg-info/PKG-INFO
--rw-r--r--   0 dmd        (501) staff       (20)    21478 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/phonenumbers.egg-info/SOURCES.txt
--rw-r--r--   0 dmd        (501) staff       (20)       13 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/phonenumbers.egg-info/top_level.txt
--rw-r--r--   0 dmd        (501) staff       (20)      924 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/PKG-INFO
--rw-r--r--   0 dmd        (501) staff       (20)       67 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/setup.cfg
--rwxr-xr-x   0 dmd        (501) staff       (20)     3319 2017-09-15 12:46:57.000000 phonenumbers-8.9.8/setup.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/tests/
--rw-r--r--   0 dmd        (501) staff       (20)      585 2013-10-11 17:19:49.000000 phonenumbers-8.9.8/tests/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)    67545 2018-05-17 08:38:10.000000 phonenumbers-8.9.8/tests/asyoutypetest.py
--rw-r--r--   0 dmd        (501) staff       (20)     5419 2013-11-15 12:19:10.000000 phonenumbers-8.9.8/tests/carriertest.py
--rw-r--r--   0 dmd        (501) staff       (20)    18579 2018-05-17 08:40:03.000000 phonenumbers-8.9.8/tests/examplenumberstest.py
--rw-r--r--   0 dmd        (501) staff       (20)    11403 2018-05-17 08:40:03.000000 phonenumbers-8.9.8/tests/geocodertest.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/tests/pb2/
--rw-r--r--   0 dmd        (501) staff       (20)      127 2015-10-07 18:13:06.000000 phonenumbers-8.9.8/tests/pb2/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)     2564 2018-05-19 06:37:56.000000 phonenumbers-8.9.8/tests/pb2/converttest.py
--rw-r--r--   0 dmd        (501) staff       (20)    49214 2018-05-17 08:40:03.000000 phonenumbers-8.9.8/tests/phonenumbermatchertest.py
--rwxr-xr-x   0 dmd        (501) staff       (20)     7615 2018-05-17 08:38:10.000000 phonenumbers-8.9.8/tests/phonenumbertest.py
--rwxr-xr-x   0 dmd        (501) staff       (20)   187153 2018-05-17 14:56:20.000000 phonenumbers-8.9.8/tests/phonenumberutiltest.py
--rw-r--r--   0 dmd        (501) staff       (20)    19975 2018-05-17 08:40:03.000000 phonenumbers-8.9.8/tests/shortnumberinfotest.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/tests/testcarrierdata/
--rw-r--r--   0 dmd        (501) staff       (20)      847 2018-06-16 06:46:07.000000 phonenumbers-8.9.8/tests/testcarrierdata/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)     1056 2018-06-16 06:46:07.000000 phonenumbers-8.9.8/tests/testcarrierdata/data0.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/tests/testdata/
--rw-r--r--   0 dmd        (501) staff       (20)     2186 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)      520 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_800.py
--rw-r--r--   0 dmd        (501) staff       (20)      527 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_882.py
--rw-r--r--   0 dmd        (501) staff       (20)      533 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_979.py
--rw-r--r--   0 dmd        (501) staff       (20)      436 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_AD.py
--rw-r--r--   0 dmd        (501) staff       (20)      440 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_AE.py
--rw-r--r--   0 dmd        (501) staff       (20)      731 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_AM.py
--rw-r--r--   0 dmd        (501) staff       (20)      746 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_AO.py
--rw-r--r--   0 dmd        (501) staff       (20)     2450 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_AR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1247 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_AU.py
--rw-r--r--   0 dmd        (501) staff       (20)      420 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_BB.py
--rw-r--r--   0 dmd        (501) staff       (20)      511 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_BR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1072 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_BS.py
--rw-r--r--   0 dmd        (501) staff       (20)      945 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_BY.py
--rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_CA.py
--rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_CC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1083 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_CN.py
--rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_CX.py
--rw-r--r--   0 dmd        (501) staff       (20)     2079 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_DE.py
--rw-r--r--   0 dmd        (501) staff       (20)      671 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_FR.py
--rw-r--r--   0 dmd        (501) staff       (20)     2140 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_GB.py
--rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_GG.py
--rw-r--r--   0 dmd        (501) staff       (20)      502 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_HU.py
--rw-r--r--   0 dmd        (501) staff       (20)     1308 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_IT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1990 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_JP.py
--rw-r--r--   0 dmd        (501) staff       (20)     3617 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_KR.py
--rw-r--r--   0 dmd        (501) staff       (20)     2808 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_MX.py
--rw-r--r--   0 dmd        (501) staff       (20)     1503 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_NZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      909 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_PL.py
--rw-r--r--   0 dmd        (501) staff       (20)     1091 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_RE.py
--rw-r--r--   0 dmd        (501) staff       (20)      382 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_SE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1221 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_SG.py
--rw-r--r--   0 dmd        (501) staff       (20)      668 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_TA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1640 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_US.py
--rw-r--r--   0 dmd        (501) staff       (20)      921 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_UZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      777 2018-06-16 06:46:01.000000 phonenumbers-8.9.8/tests/testdata/region_YT.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/tests/testgeodata/
--rw-r--r--   0 dmd        (501) staff       (20)      847 2018-06-16 06:46:07.000000 phonenumbers-8.9.8/tests/testgeodata/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)     1881 2018-06-16 06:46:07.000000 phonenumbers-8.9.8/tests/testgeodata/data0.py
--rw-r--r--   0 dmd        (501) staff       (20)     2317 2017-07-24 12:06:48.000000 phonenumbers-8.9.8/tests/testmetadatatest.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:53:18.000000 phonenumbers-8.9.8/tests/testtzdata/
--rw-r--r--   0 dmd        (501) staff       (20)      835 2018-06-16 06:46:08.000000 phonenumbers-8.9.8/tests/testtzdata/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)     1112 2018-06-16 06:46:08.000000 phonenumbers-8.9.8/tests/testtzdata/data0.py
--rw-r--r--   0 dmd        (501) staff       (20)     5914 2013-11-15 12:19:10.000000 phonenumbers-8.9.8/tests/timezonetest.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/
+-rw-r--r--   0 dmd        (501) staff       (20)      115 2014-12-16 15:23:29.000000 phonenumbers-8.9.9/MANIFEST.in
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/phonenumbers/
+-rw-r--r--   0 dmd        (501) staff       (20)     9853 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)    31975 2017-04-19 13:38:31.000000 phonenumbers-8.9.9/phonenumbers/asyoutypeformatter.py
+-rw-r--r--   0 dmd        (501) staff       (20)     6352 2013-11-15 12:19:09.000000 phonenumbers-8.9.9/phonenumbers/carrier.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/phonenumbers/carrierdata/
+-rw-r--r--   0 dmd        (501) staff       (20)      936 2018-06-29 07:25:43.000000 phonenumbers-8.9.9/phonenumbers/carrierdata/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)   308533 2018-06-29 07:25:43.000000 phonenumbers-8.9.9/phonenumbers/carrierdata/data0.py
+-rw-r--r--   0 dmd        (501) staff       (20)   346159 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/carrierdata/data1.py
+-rw-r--r--   0 dmd        (501) staff       (20)   140817 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/carrierdata/data2.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/phonenumbers/data/
+-rw-r--r--   0 dmd        (501) staff       (20)    10295 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)      339 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_255.py
+-rw-r--r--   0 dmd        (501) staff       (20)      232 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_27.py
+-rw-r--r--   0 dmd        (501) staff       (20)      228 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_30.py
+-rw-r--r--   0 dmd        (501) staff       (20)      436 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_31.py
+-rw-r--r--   0 dmd        (501) staff       (20)      348 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_34.py
+-rw-r--r--   0 dmd        (501) staff       (20)      217 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_350.py
+-rw-r--r--   0 dmd        (501) staff       (20)      454 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_351.py
+-rw-r--r--   0 dmd        (501) staff       (20)      199 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_352.py
+-rw-r--r--   0 dmd        (501) staff       (20)      360 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_358.py
+-rw-r--r--   0 dmd        (501) staff       (20)      482 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_359.py
+-rw-r--r--   0 dmd        (501) staff       (20)      328 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_36.py
+-rw-r--r--   0 dmd        (501) staff       (20)      572 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_372.py
+-rw-r--r--   0 dmd        (501) staff       (20)      353 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_373.py
+-rw-r--r--   0 dmd        (501) staff       (20)      493 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_380.py
+-rw-r--r--   0 dmd        (501) staff       (20)      754 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_381.py
+-rw-r--r--   0 dmd        (501) staff       (20)      545 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_385.py
+-rw-r--r--   0 dmd        (501) staff       (20)      377 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_39.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1480 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_43.py
+-rw-r--r--   0 dmd        (501) staff       (20)      689 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_44.py
+-rw-r--r--   0 dmd        (501) staff       (20)     7207 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_49.py
+-rw-r--r--   0 dmd        (501) staff       (20)      226 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_505.py
+-rw-r--r--   0 dmd        (501) staff       (20)      241 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_506.py
+-rw-r--r--   0 dmd        (501) staff       (20)      404 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_52.py
+-rw-r--r--   0 dmd        (501) staff       (20)      343 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_54.py
+-rw-r--r--   0 dmd        (501) staff       (20)      224 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_55.py
+-rw-r--r--   0 dmd        (501) staff       (20)      197 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_58.py
+-rw-r--r--   0 dmd        (501) staff       (20)      500 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_595.py
+-rw-r--r--   0 dmd        (501) staff       (20)      589 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_61.py
+-rw-r--r--   0 dmd        (501) staff       (20)      589 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_62.py
+-rw-r--r--   0 dmd        (501) staff       (20)      215 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_63.py
+-rw-r--r--   0 dmd        (501) staff       (20)      348 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_64.py
+-rw-r--r--   0 dmd        (501) staff       (20)      216 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_66.py
+-rw-r--r--   0 dmd        (501) staff       (20)      230 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_675.py
+-rw-r--r--   0 dmd        (501) staff       (20)      230 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_676.py
+-rw-r--r--   0 dmd        (501) staff       (20)      227 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_679.py
+-rw-r--r--   0 dmd        (501) staff       (20)      696 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_7.py
+-rw-r--r--   0 dmd        (501) staff       (20)      479 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_81.py
+-rw-r--r--   0 dmd        (501) staff       (20)      343 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_84.py
+-rw-r--r--   0 dmd        (501) staff       (20)      213 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_855.py
+-rw-r--r--   0 dmd        (501) staff       (20)      415 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_856.py
+-rw-r--r--   0 dmd        (501) staff       (20)      269 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_90.py
+-rw-r--r--   0 dmd        (501) staff       (20)      973 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_91.py
+-rw-r--r--   0 dmd        (501) staff       (20)      431 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_94.py
+-rw-r--r--   0 dmd        (501) staff       (20)      224 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_95.py
+-rw-r--r--   0 dmd        (501) staff       (20)      236 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_971.py
+-rw-r--r--   0 dmd        (501) staff       (20)      248 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_972.py
+-rw-r--r--   0 dmd        (501) staff       (20)      254 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/alt_format_995.py
+-rw-r--r--   0 dmd        (501) staff       (20)      509 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_800.py
+-rw-r--r--   0 dmd        (501) staff       (20)      511 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_808.py
+-rw-r--r--   0 dmd        (501) staff       (20)      544 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_870.py
+-rw-r--r--   0 dmd        (501) staff       (20)      527 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_878.py
+-rw-r--r--   0 dmd        (501) staff       (20)      557 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_881.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1650 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_882.py
+-rw-r--r--   0 dmd        (501) staff       (20)      838 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_883.py
+-rw-r--r--   0 dmd        (501) staff       (20)      522 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_888.py
+-rw-r--r--   0 dmd        (501) staff       (20)      522 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_979.py
+-rw-r--r--   0 dmd        (501) staff       (20)      674 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1310 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AD.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1871 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      902 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1556 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1231 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1981 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AL.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1951 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      670 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     7150 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1235 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3044 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3275 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1075 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1611 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AX.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1611 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_AZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1889 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1728 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BB.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3300 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BD.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1940 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      757 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2554 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1235 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      675 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      951 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      699 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BL.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1251 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      717 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BN.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1494 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      656 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BQ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3258 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1711 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      931 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1280 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3067 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      971 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_BZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1627 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1633 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1313 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      780 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1059 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2082 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      767 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      645 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3573 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      963 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     7253 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CN.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2114 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1448 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1208 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      710 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CV.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1144 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1644 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CX.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1281 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1951 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_CZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     5878 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_DE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      665 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_DJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      983 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_DK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1266 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_DM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1569 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_DO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1711 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_DZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1900 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_EC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1876 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_EE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1682 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_EG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1055 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_EH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      850 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_ER.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1724 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_ES.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1500 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_ET.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2484 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_FI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1021 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_FJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_FK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      672 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_FM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1137 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_FO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2032 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_FR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      850 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     5117 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GB.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1331 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GD.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1664 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      868 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1706 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1483 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      728 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      915 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      732 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      979 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      980 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GP.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1089 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GQ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1837 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1044 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1602 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      929 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      971 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_GY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2482 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_HK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      882 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_HN.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2452 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_HR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      924 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_HT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1719 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_HU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3599 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_ID.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3599 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_IE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3179 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_IL.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1564 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_IM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     8650 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_IN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      621 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_IO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1210 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_IQ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1843 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_IR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1780 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_IS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3308 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_IT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1830 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_JE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1505 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_JM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2482 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_JO.py
+-rw-r--r--   0 dmd        (501) staff       (20)    12833 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_JP.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1542 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_KE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1545 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/data/region_KG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1563 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_KH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      935 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_KI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      761 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_KM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1245 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_KN.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1339 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_KP.py
+-rw-r--r--   0 dmd        (501) staff       (20)     5194 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_KR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1175 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_KW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1514 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_KY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1799 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_KZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1267 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_LA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1322 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_LB.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1291 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_LC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1661 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_LI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1082 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_LK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1319 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_LR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      751 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_LS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2129 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_LT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3066 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_LU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1069 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_LV.py
+-rw-r--r--   0 dmd        (501) staff       (20)      873 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_LY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2112 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1558 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1793 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MD.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1487 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_ME.py
+-rw-r--r--   0 dmd        (501) staff       (20)      723 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1051 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      832 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MH.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1741 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1287 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_ML.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3206 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1778 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      749 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1370 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MP.py
+-rw-r--r--   0 dmd        (501) staff       (20)      893 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MQ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      845 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1184 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1417 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1368 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1312 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MV.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1423 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3655 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MX.py
+-rw-r--r--   0 dmd        (501) staff       (20)    10145 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      946 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_MZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1865 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_NA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      849 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_NC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1131 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_NE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      877 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_NF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2676 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_NG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      830 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_NI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2894 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_NL.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1842 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_NO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1351 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_NP.py
+-rw-r--r--   0 dmd        (501) staff       (20)      639 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_NR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      666 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/data/region_NU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2373 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_NZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1220 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_OM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1561 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_PA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1894 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_PE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      964 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_PF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1158 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_PG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2440 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_PH.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3443 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_PK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2278 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_PL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      796 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_PM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1244 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_PR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1469 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_PS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1847 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_PT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      732 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_PW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2353 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_PY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1062 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_QA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1335 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_RE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1919 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_RO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2300 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_RS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2121 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_RU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1277 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_RW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1819 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1060 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SB.py
+-rw-r--r--   0 dmd        (501) staff       (20)      971 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      775 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SD.py
+-rw-r--r--   0 dmd        (501) staff       (20)     5794 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/data/region_SE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1596 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      717 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SH.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1896 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1464 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2668 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      858 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SL.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1662 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1381 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SN.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1477 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1047 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      754 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      658 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_ST.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1172 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SV.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1233 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SX.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1195 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1270 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_SZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      425 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1402 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      748 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      735 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1570 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TH.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1583 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      590 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1162 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TL.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1247 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1103 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TN.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1057 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2448 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1509 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      569 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TV.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2303 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1755 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_TZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2242 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_UA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1657 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_UG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2859 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_US.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1439 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_UY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2430 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_UZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1604 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_VA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1309 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_VC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1162 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_VE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1310 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_VG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1412 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_VI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3319 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/data/region_VN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      869 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_VU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      778 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_WF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1030 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_WS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1347 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_XK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1088 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_YE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      833 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_YT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2008 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_ZA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1370 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_ZM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3290 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/data/region_ZW.py
+-rw-r--r--   0 dmd        (501) staff       (20)    10966 2018-05-17 08:38:10.000000 phonenumbers-8.9.9/phonenumbers/geocoder.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/phonenumbers/geodata/
+-rw-r--r--   0 dmd        (501) staff       (20)     2255 2018-06-29 07:25:43.000000 phonenumbers-8.9.9/phonenumbers/geodata/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)   355683 2018-06-29 07:25:39.000000 phonenumbers-8.9.9/phonenumbers/geodata/data0.py
+-rw-r--r--   0 dmd        (501) staff       (20)   358303 2018-06-29 07:25:39.000000 phonenumbers-8.9.9/phonenumbers/geodata/data1.py
+-rw-r--r--   0 dmd        (501) staff       (20)   327894 2018-06-29 07:25:40.000000 phonenumbers-8.9.9/phonenumbers/geodata/data10.py
+-rw-r--r--   0 dmd        (501) staff       (20)   342087 2018-06-29 07:25:40.000000 phonenumbers-8.9.9/phonenumbers/geodata/data11.py
+-rw-r--r--   0 dmd        (501) staff       (20)   466008 2018-06-29 07:25:40.000000 phonenumbers-8.9.9/phonenumbers/geodata/data12.py
+-rw-r--r--   0 dmd        (501) staff       (20)   919549 2018-06-29 07:25:40.000000 phonenumbers-8.9.9/phonenumbers/geodata/data13.py
+-rw-r--r--   0 dmd        (501) staff       (20)   915475 2018-06-29 07:25:40.000000 phonenumbers-8.9.9/phonenumbers/geodata/data14.py
+-rw-r--r--   0 dmd        (501) staff       (20)   901730 2018-06-29 07:25:41.000000 phonenumbers-8.9.9/phonenumbers/geodata/data15.py
+-rw-r--r--   0 dmd        (501) staff       (20)   913040 2018-06-29 07:25:41.000000 phonenumbers-8.9.9/phonenumbers/geodata/data16.py
+-rw-r--r--   0 dmd        (501) staff       (20)   917750 2018-06-29 07:25:41.000000 phonenumbers-8.9.9/phonenumbers/geodata/data17.py
+-rw-r--r--   0 dmd        (501) staff       (20)   921018 2018-06-29 07:25:41.000000 phonenumbers-8.9.9/phonenumbers/geodata/data18.py
+-rw-r--r--   0 dmd        (501) staff       (20)   923238 2018-06-29 07:25:41.000000 phonenumbers-8.9.9/phonenumbers/geodata/data19.py
+-rw-r--r--   0 dmd        (501) staff       (20)   358619 2018-06-29 07:25:39.000000 phonenumbers-8.9.9/phonenumbers/geodata/data2.py
+-rw-r--r--   0 dmd        (501) staff       (20)   920700 2018-06-29 07:25:41.000000 phonenumbers-8.9.9/phonenumbers/geodata/data20.py
+-rw-r--r--   0 dmd        (501) staff       (20)   919835 2018-06-29 07:25:42.000000 phonenumbers-8.9.9/phonenumbers/geodata/data21.py
+-rw-r--r--   0 dmd        (501) staff       (20)   927988 2018-06-29 07:25:42.000000 phonenumbers-8.9.9/phonenumbers/geodata/data22.py
+-rw-r--r--   0 dmd        (501) staff       (20)   908636 2018-06-29 07:25:42.000000 phonenumbers-8.9.9/phonenumbers/geodata/data23.py
+-rw-r--r--   0 dmd        (501) staff       (20)   914964 2018-06-29 07:25:42.000000 phonenumbers-8.9.9/phonenumbers/geodata/data24.py
+-rw-r--r--   0 dmd        (501) staff       (20)   920951 2018-06-29 07:25:42.000000 phonenumbers-8.9.9/phonenumbers/geodata/data25.py
+-rw-r--r--   0 dmd        (501) staff       (20)   914124 2018-06-29 07:25:42.000000 phonenumbers-8.9.9/phonenumbers/geodata/data26.py
+-rw-r--r--   0 dmd        (501) staff       (20)   923203 2018-06-29 07:25:43.000000 phonenumbers-8.9.9/phonenumbers/geodata/data27.py
+-rw-r--r--   0 dmd        (501) staff       (20)   584516 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/geodata/data28.py
+-rw-r--r--   0 dmd        (501) staff       (20)   390404 2018-06-29 07:25:39.000000 phonenumbers-8.9.9/phonenumbers/geodata/data3.py
+-rw-r--r--   0 dmd        (501) staff       (20)   861636 2018-06-29 07:25:39.000000 phonenumbers-8.9.9/phonenumbers/geodata/data4.py
+-rw-r--r--   0 dmd        (501) staff       (20)   609339 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/geodata/data5.py
+-rw-r--r--   0 dmd        (501) staff       (20)   726827 2018-06-29 07:25:39.000000 phonenumbers-8.9.9/phonenumbers/geodata/data6.py
+-rw-r--r--   0 dmd        (501) staff       (20)   461462 2018-06-29 07:25:40.000000 phonenumbers-8.9.9/phonenumbers/geodata/data7.py
+-rw-r--r--   0 dmd        (501) staff       (20)   338194 2018-06-29 07:25:40.000000 phonenumbers-8.9.9/phonenumbers/geodata/data8.py
+-rw-r--r--   0 dmd        (501) staff       (20)   330259 2018-06-29 07:25:40.000000 phonenumbers-8.9.9/phonenumbers/geodata/data9.py
+-rw-r--r--   0 dmd        (501) staff       (20)   610934 2018-06-29 07:25:45.000000 phonenumbers-8.9.9/phonenumbers/geodata/locale.py
+-rw-r--r--   0 dmd        (501) staff       (20)    32671 2018-05-17 08:40:03.000000 phonenumbers-8.9.9/phonenumbers/phonemetadata.py
+-rw-r--r--   0 dmd        (501) staff       (20)    12452 2018-05-17 08:40:03.000000 phonenumbers-8.9.9/phonenumbers/phonenumber.py
+-rw-r--r--   0 dmd        (501) staff       (20)    38746 2018-05-17 08:40:03.000000 phonenumbers-8.9.9/phonenumbers/phonenumbermatcher.py
+-rw-r--r--   0 dmd        (501) staff       (20)   155085 2018-05-17 08:40:03.000000 phonenumbers-8.9.9/phonenumbers/phonenumberutil.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3650 2013-11-15 12:19:10.000000 phonenumbers-8.9.9/phonenumbers/prefix.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1428 2018-05-17 08:38:26.000000 phonenumbers-8.9.9/phonenumbers/re_util.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/phonenumbers/shortdata/
+-rw-r--r--   0 dmd        (501) staff       (20)     2180 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      558 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      696 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      807 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      791 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      773 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1137 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      822 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1004 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      676 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      737 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1360 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      788 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      578 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AX.py
+-rw-r--r--   0 dmd        (501) staff       (20)      826 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_AZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      786 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      565 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BB.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1089 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BD.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1212 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      717 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1146 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      966 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      822 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      541 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      777 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      684 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      788 2018-06-29 07:25:36.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BQ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1494 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      554 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      684 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      801 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      612 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      568 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_BZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1044 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      826 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      580 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      661 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1354 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      814 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1650 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      804 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      734 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      875 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      891 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      581 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CV.py
+-rw-r--r--   0 dmd        (501) staff       (20)      788 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CX.py
+-rw-r--r--   0 dmd        (501) staff       (20)      705 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      768 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_CZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      706 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_DE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_DJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      746 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_DK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_DM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_DO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      785 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_DZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      579 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_EC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2419 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_EE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      824 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_EG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      572 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_EH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      678 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_ER.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1620 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_ES.py
+-rw-r--r--   0 dmd        (501) staff       (20)      588 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_ET.py
+-rw-r--r--   0 dmd        (501) staff       (20)      707 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_FI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      749 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_FJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_FK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      576 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_FM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      591 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_FO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1551 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_FR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      588 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1338 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GB.py
+-rw-r--r--   0 dmd        (501) staff       (20)      773 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      844 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      636 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      856 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GH.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1286 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      566 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      676 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GP.py
+-rw-r--r--   0 dmd        (501) staff       (20)      719 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      829 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      860 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_GY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1155 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_HK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      793 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_HN.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1134 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_HR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      799 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_HT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      727 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_HU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      831 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_ID.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1249 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_IE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      848 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_IL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      720 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_IM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1625 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_IN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      860 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_IQ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1368 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_IR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1007 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_IS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1220 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_IT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      658 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_JE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      796 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_JM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      860 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_JO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      554 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_JP.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1594 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_KE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      796 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_KG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      810 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_KH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      725 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_KI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_KM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_KN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_KP.py
+-rw-r--r--   0 dmd        (501) staff       (20)      929 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_KR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      686 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_KW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_KY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      841 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_KZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_LA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      579 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_LB.py
+-rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_LC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      602 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_LI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      560 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_LK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      837 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_LR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_LS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      760 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_LT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      712 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_LU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1143 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_LV.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_LY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      572 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      579 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      786 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      697 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_ME.py
+-rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      564 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1470 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_ML.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MP.py
+-rw-r--r--   0 dmd        (501) staff       (20)      574 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MQ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      705 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      594 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      726 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MV.py
+-rw-r--r--   0 dmd        (501) staff       (20)      810 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      761 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MX.py
+-rw-r--r--   0 dmd        (501) staff       (20)      952 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      594 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_MZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      599 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_NA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      904 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_NC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      813 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_NE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      568 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_NF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      793 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_NG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      739 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_NI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1035 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_NL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      743 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_NO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_NP.py
+-rw-r--r--   0 dmd        (501) staff       (20)      566 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_NR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      676 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_NU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      901 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_NZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      552 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_OM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_PA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      568 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_PE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_PF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      741 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_PG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      565 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_PH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      599 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_PK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      773 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_PL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      678 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_PM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_PR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      675 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_PS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      699 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_PT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_PW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      565 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_PY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      589 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_QA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      574 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_RE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1043 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_RO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      602 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_RS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      595 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_RU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_RW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1045 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      650 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SB.py
+-rw-r--r--   0 dmd        (501) staff       (20)      638 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SD.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1316 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      748 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      582 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      711 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      747 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      808 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1279 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      561 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_ST.py
+-rw-r--r--   0 dmd        (501) staff       (20)      793 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SV.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SX.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_SZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_TC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_TD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      587 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_TG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1672 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_TH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_TJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      581 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_TL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_TM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_TN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      574 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_TO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1767 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_TR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      554 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_TT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_TV.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_TW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      808 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_TZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      956 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_UA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_UG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1618 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_US.py
+-rw-r--r--   0 dmd        (501) staff       (20)      707 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_UY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      833 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_UZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      558 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_VA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_VC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_VE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_VG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_VI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_VN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_VU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_WF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      710 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_WS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_XK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      558 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_YE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      567 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_YT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1188 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_ZA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      575 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_ZM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      984 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/shortdata/region_ZW.py
+-rw-r--r--   0 dmd        (501) staff       (20)    20748 2018-05-17 08:40:03.000000 phonenumbers-8.9.9/phonenumbers/shortnumberinfo.py
+-rw-r--r--   0 dmd        (501) staff       (20)     4947 2018-05-17 08:38:10.000000 phonenumbers-8.9.9/phonenumbers/timezone.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/phonenumbers/tzdata/
+-rw-r--r--   0 dmd        (501) staff       (20)      824 2018-06-29 07:25:44.000000 phonenumbers-8.9.9/phonenumbers/tzdata/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)   203444 2018-06-29 07:26:49.000000 phonenumbers-8.9.9/phonenumbers/tzdata/data0.py
+-rw-r--r--   0 dmd        (501) staff       (20)    18939 2013-11-15 12:19:10.000000 phonenumbers-8.9.9/phonenumbers/unicode_util.py
+-rw-r--r--   0 dmd        (501) staff       (20)     5865 2016-01-29 10:59:27.000000 phonenumbers-8.9.9/phonenumbers/util.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/phonenumbers.egg-info/
+-rw-r--r--   0 dmd        (501) staff       (20)        1 2018-06-29 07:35:40.000000 phonenumbers-8.9.9/phonenumbers.egg-info/dependency_links.txt
+-rw-r--r--   0 dmd        (501) staff       (20)      924 2018-06-29 07:35:40.000000 phonenumbers-8.9.9/phonenumbers.egg-info/PKG-INFO
+-rw-r--r--   0 dmd        (501) staff       (20)    21478 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/phonenumbers.egg-info/SOURCES.txt
+-rw-r--r--   0 dmd        (501) staff       (20)       13 2018-06-29 07:35:40.000000 phonenumbers-8.9.9/phonenumbers.egg-info/top_level.txt
+-rw-r--r--   0 dmd        (501) staff       (20)      924 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/PKG-INFO
+-rw-r--r--   0 dmd        (501) staff       (20)       67 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/setup.cfg
+-rwxr-xr-x   0 dmd        (501) staff       (20)     3319 2017-09-15 12:46:57.000000 phonenumbers-8.9.9/setup.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/tests/
+-rw-r--r--   0 dmd        (501) staff       (20)      585 2013-10-11 17:19:49.000000 phonenumbers-8.9.9/tests/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)    67545 2018-05-17 08:38:10.000000 phonenumbers-8.9.9/tests/asyoutypetest.py
+-rw-r--r--   0 dmd        (501) staff       (20)     5419 2013-11-15 12:19:10.000000 phonenumbers-8.9.9/tests/carriertest.py
+-rw-r--r--   0 dmd        (501) staff       (20)    18579 2018-05-17 08:40:03.000000 phonenumbers-8.9.9/tests/examplenumberstest.py
+-rw-r--r--   0 dmd        (501) staff       (20)    11403 2018-05-17 08:40:03.000000 phonenumbers-8.9.9/tests/geocodertest.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/tests/pb2/
+-rw-r--r--   0 dmd        (501) staff       (20)      127 2015-10-07 18:13:06.000000 phonenumbers-8.9.9/tests/pb2/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2564 2018-05-19 06:37:56.000000 phonenumbers-8.9.9/tests/pb2/converttest.py
+-rw-r--r--   0 dmd        (501) staff       (20)    49214 2018-05-17 08:40:03.000000 phonenumbers-8.9.9/tests/phonenumbermatchertest.py
+-rwxr-xr-x   0 dmd        (501) staff       (20)     7615 2018-05-17 08:38:10.000000 phonenumbers-8.9.9/tests/phonenumbertest.py
+-rwxr-xr-x   0 dmd        (501) staff       (20)   187153 2018-05-17 14:56:20.000000 phonenumbers-8.9.9/tests/phonenumberutiltest.py
+-rw-r--r--   0 dmd        (501) staff       (20)    19975 2018-05-17 08:40:03.000000 phonenumbers-8.9.9/tests/shortnumberinfotest.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/tests/testcarrierdata/
+-rw-r--r--   0 dmd        (501) staff       (20)      847 2018-06-29 07:25:43.000000 phonenumbers-8.9.9/tests/testcarrierdata/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1056 2018-06-29 07:25:43.000000 phonenumbers-8.9.9/tests/testcarrierdata/data0.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/tests/testdata/
+-rw-r--r--   0 dmd        (501) staff       (20)     2186 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)      520 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_800.py
+-rw-r--r--   0 dmd        (501) staff       (20)      527 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_882.py
+-rw-r--r--   0 dmd        (501) staff       (20)      533 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_979.py
+-rw-r--r--   0 dmd        (501) staff       (20)      436 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_AD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      440 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_AE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      731 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_AM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      746 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_AO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2450 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_AR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1247 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_AU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      420 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_BB.py
+-rw-r--r--   0 dmd        (501) staff       (20)      511 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_BR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1072 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_BS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      945 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_BY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_CA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_CC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1083 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_CN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_CX.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2079 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_DE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      671 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_FR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2140 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_GB.py
+-rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_GG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      502 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_HU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1308 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_IT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1990 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_JP.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3617 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_KR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2808 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_MX.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1503 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_NZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      909 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_PL.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1091 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_RE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      382 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_SE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1221 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_SG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      668 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_TA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1640 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_US.py
+-rw-r--r--   0 dmd        (501) staff       (20)      921 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_UZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      777 2018-06-29 07:25:37.000000 phonenumbers-8.9.9/tests/testdata/region_YT.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/tests/testgeodata/
+-rw-r--r--   0 dmd        (501) staff       (20)      847 2018-06-29 07:25:43.000000 phonenumbers-8.9.9/tests/testgeodata/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1881 2018-06-29 07:25:43.000000 phonenumbers-8.9.9/tests/testgeodata/data0.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2317 2017-07-24 12:06:48.000000 phonenumbers-8.9.9/tests/testmetadatatest.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:35:41.000000 phonenumbers-8.9.9/tests/testtzdata/
+-rw-r--r--   0 dmd        (501) staff       (20)      835 2018-06-29 07:25:44.000000 phonenumbers-8.9.9/tests/testtzdata/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1112 2018-06-29 07:25:44.000000 phonenumbers-8.9.9/tests/testtzdata/data0.py
+-rw-r--r--   0 dmd        (501) staff       (20)     5914 2013-11-15 12:19:10.000000 phonenumbers-8.9.9/tests/timezonetest.py
```

### Comparing `phonenumbers-8.9.8/phonenumbers/__init__.py` & `phonenumbers-8.9.9/phonenumbers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
                               is_carrier_specific_for_region,
                               is_sms_service_for_region)
 from .phonenumbermatcher import PhoneNumberMatch, PhoneNumberMatcher, Leniency
 
 
 # Version number is taken from the upstream libphonenumber version
 # together with an indication of the version of the Python-specific code.
-__version__ = "8.9.8"
+__version__ = "8.9.9"
 
 __all__ = ['PhoneNumber', 'CountryCodeSource', 'FrozenPhoneNumber',
            'REGION_CODE_FOR_NON_GEO_ENTITY', 'NumberFormat', 'PhoneNumberDesc', 'PhoneMetadata',
            'AsYouTypeFormatter',
            # items from phonenumberutil.py
            'COUNTRY_CODE_TO_REGION_CODE', 'SUPPORTED_REGIONS',
            'UNKNOWN_REGION', 'COUNTRY_CODES_FOR_NON_GEO_REGIONS',
```

### Comparing `phonenumbers-8.9.8/phonenumbers/asyoutypeformatter.py` & `phonenumbers-8.9.9/phonenumbers/asyoutypeformatter.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/carrier.py` & `phonenumbers-8.9.9/phonenumbers/carrier.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/carrierdata/__init__.py` & `phonenumbers-8.9.9/phonenumbers/carrierdata/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/carrierdata/data0.py` & `phonenumbers-8.9.9/phonenumbers/carrierdata/data0.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/carrierdata/data1.py` & `phonenumbers-8.9.9/phonenumbers/carrierdata/data1.py`

 * *Files 0% similar despite different names*

```diff
@@ -2733,15 +2733,14 @@
  '556699671':{'en': 'Vivo'},
  '556699678':{'en': 'Vivo'},
  '556699679':{'en': 'Vivo'},
  '6228599':{'en': 'Esia'},
  '6228591':{'en': 'Esia'},
  '861340':{'en': 'China Mobile', 'zh': u('\u4e2d\u56fd\u79fb\u52a8'), 'zh_Hant': u('\u4e2d\u570b\u79fb\u52d5')},
  '861341':{'en': 'China Mobile', 'zh': u('\u4e2d\u56fd\u79fb\u52a8'), 'zh_Hant': u('\u4e2d\u570b\u79fb\u52d5')},
- '861342':{'en': 'China Mobile', 'zh': u('\u4e2d\u56fd\u79fb\u52a8'), 'zh_Hant': u('\u4e2d\u570b\u79fb\u52d5')},
  '7983999':{'en': 'Beeline', 'ru': u('\u0411\u0438\u043b\u0430\u0439\u043d')},
  '559799957':{'en': 'Oi'},
  '559799953':{'en': 'Oi'},
  '559799959':{'en': 'Oi'},
  '559799958':{'en': 'Oi'},
  '5917373':{'en': 'Entel'},
  '5917372':{'en': 'Entel'},
@@ -6697,14 +6696,15 @@
  '558599974':{'en': 'TIM'},
  '558599975':{'en': 'TIM'},
  '558599972':{'en': 'TIM'},
  '558599973':{'en': 'TIM'},
  '558599971':{'en': 'TIM'},
  '62229613':{'en': 'Esia'},
  '58426':{'en': 'Movilnet'},
+ '58424':{'en': 'movistar'},
  '62751978':{'en': 'Esia'},
  '62421993':{'en': 'Esia'},
  '556298191':{'en': 'TIM'},
  '559399102':{'en': 'Vivo'},
  '79010135':{'en': 'Tele2', 'ru': 'Tele2'},
  '559899969':{'en': 'Oi'},
  '559399103':{'en': 'Vivo'},
```

### Comparing `phonenumbers-8.9.8/phonenumbers/carrierdata/data2.py` & `phonenumbers-8.9.9/phonenumbers/carrierdata/data2.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
  '97333':{'en': 'VIVA'},
  '97332':{'en': 'Batelco'},
  '97331':{'en': 'Royal Court'},
  '917604':{'en': 'Reliance Jio'},
  '97339':{'en': 'Batelco'},
  '97338':{'en': 'Batelco'},
  '92335':{'en': 'Ufone'},
- '99670':{'en': 'Nur Telecom'},
+ '9725501':{'en': 'Beezz'},
  '9187329':{'en': 'Telewings'},
  '9187328':{'en': 'Airtel'},
  '9177120':{'en': 'Aircel'},
  '9189638':{'en': 'Aircel'},
  '9177400':{'en': 'Reliance Jio'},
  '917238':{'en': 'Idea'},
  '9177409':{'en': 'Idea'},
@@ -173,14 +173,15 @@
  '919154':{'en': 'Telewings'},
  '919157':{'en': 'Telewings'},
  '919156':{'en': 'Telewings'},
  '919151':{'en': 'Tata Docomo'},
  '9185828':{'en': 'Airtel'},
  '9185829':{'en': 'Airtel'},
  '959349':{'en': 'MECTel'},
+ '996999':{'en': 'Sky mobile'},
  '9185820':{'en': 'Idea'},
  '9180796':{'en': 'BSNL MOBILE'},
  '96278':{'en': 'Umniah'},
  '9185318':{'en': 'Vodafone'},
  '9185319':{'en': 'Vodafone'},
  '92336':{'en': 'Ufone'},
  '919851':{'en': 'Aircel'},
@@ -411,15 +412,15 @@
  '9175459':{'en': 'Vodafone'},
  '9176118':{'en': 'Aircel'},
  '918999':{'en': 'Reliance Jio'},
  '9175450':{'en': 'Vodafone'},
  '9177192':{'en': 'Vodafone'},
  '918990':{'en': 'Reliance Jio'},
  '9176116':{'en': 'Aircel'},
- '919828':{'en': 'Vodafone'},
+ '861342':{'en': 'China Mobile', 'zh': u('\u4e2d\u56fd\u79fb\u52a8'), 'zh_Hant': u('\u4e2d\u570b\u79fb\u52d5')},
  '861343':{'en': 'China Mobile', 'zh': u('\u4e2d\u56fd\u79fb\u52a8'), 'zh_Hant': u('\u4e2d\u570b\u79fb\u52d5')},
  '861344':{'en': 'China Mobile', 'zh': u('\u4e2d\u56fd\u79fb\u52a8'), 'zh_Hant': u('\u4e2d\u570b\u79fb\u52d5')},
  '861345':{'en': 'China Mobile', 'zh': u('\u4e2d\u56fd\u79fb\u52a8'), 'zh_Hant': u('\u4e2d\u570b\u79fb\u52d5')},
  '861346':{'en': 'China Mobile', 'zh': u('\u4e2d\u56fd\u79fb\u52a8'), 'zh_Hant': u('\u4e2d\u570b\u79fb\u52d5')},
  '9173477':{'en': 'Idea'},
  '861348':{'en': 'China Mobile', 'zh': u('\u4e2d\u56fd\u79fb\u52a8'), 'zh_Hant': u('\u4e2d\u570b\u79fb\u52d5')},
  '9176114':{'en': 'Aircel'},
@@ -607,15 +608,15 @@
  '9191161':{'en': 'Airtel'},
  '9191163':{'en': 'Airtel'},
  '917247':{'en': 'Idea'},
  '9187772':{'en': 'Reliance Jio'},
  '9191168':{'en': 'Airtel'},
  '9191169':{'en': 'Airtel'},
  '9173670':{'en': 'Airtel'},
- '9173220':{'en': 'Idea'},
+ '9176300':{'en': 'Airtel'},
  '917742':{'en': 'Airtel'},
  '9173678':{'en': 'Airtel'},
  '9173679':{'en': 'Airtel'},
  '9177176':{'en': 'Reliance Jio'},
  '95979':{'en': 'Telenor'},
  '95978':{'en': 'Telenor'},
  '95977':{'en': 'Telenor'},
@@ -886,15 +887,15 @@
  '917623':{'en': 'Idea'},
  '917622':{'en': 'Idea'},
  '919591':{'en': 'Airtel'},
  '9179798':{'en': 'Reliance Jio'},
  '919226':{'en': 'Tata Docomo'},
  '919650':{'en': 'Airtel'},
  '919651':{'en': 'Airtel'},
- '9725501':{'en': 'Beezz'},
+ '919828':{'en': 'Vodafone'},
  '919166':{'en': 'Airtel'},
  '919779':{'en': 'Airtel'},
  '9183569':{'en': 'Reliance Jio'},
  '9183568':{'en': 'Reliance Jio'},
  '9173649':{'en': 'Airtel'},
  '9173648':{'en': 'Airtel'},
  '919792':{'en': 'Vodafone'},
@@ -1562,15 +1563,15 @@
  '9176099':{'en': 'Airtel'},
  '916005':{'en': 'Reliance Jio'},
  '916002':{'en': 'Reliance Jio'},
  '916003':{'en': 'Reliance Jio'},
  '916000':{'en': 'Reliance Jio'},
  '916001':{'en': 'Reliance Jio'},
  '9185198':{'en': 'Telewings'},
- '9176300':{'en': 'Airtel'},
+ '9173220':{'en': 'Idea'},
  '9471':{'en': 'Mobitel'},
  '9173229':{'en': 'Idea'},
  '9173228':{'en': 'Idea'},
  '918284':{'en': 'Airtel'},
  '9172868':{'en': 'Idea'},
  '9172869':{'en': 'Idea'},
  '918294':{'en': 'Airtel'},
@@ -2261,14 +2262,15 @@
  '8869673':{'en': 'FarEasTone'},
  '8869672':{'en': 'FarEasTone'},
  '95996':{'en': 'Ooredoo'},
  '959265':{'en': 'ZTE'},
  '919492':{'en': 'BSNL MOBILE'},
  '919543':{'en': 'Reliance Jio'},
  '9186930':{'en': 'Idea'},
+ '99670':{'en': 'Nur Telecom'},
  '919245':{'en': 'Tata Docomo'},
  '919244':{'en': 'Tata Docomo'},
  '919247':{'en': 'Tata Docomo'},
  '919246':{'en': 'Tata Docomo'},
  '919241':{'en': 'Tata Docomo'},
  '9186298':{'en': 'Airtel'},
  '917818':{'en': 'Reliance Jio'},
@@ -2308,14 +2310,15 @@
  '99365':{'en': 'TM-Cell'},
  '918448':{'en': 'Reliance Jio'},
  '918449':{'en': 'Idea'},
  '9173809':{'en': 'Airtel'},
  '9173808':{'en': 'Airtel'},
  '9174109':{'en': 'Vodafone'},
  '9174108':{'en': 'Vodafone'},
+ '996996':{'en': 'Sky mobile'},
  '9174103':{'en': 'Airtel'},
  '9174102':{'en': 'Airtel'},
  '9174101':{'en': 'Airtel'},
  '9174100':{'en': 'Airtel'},
  '9174107':{'en': 'Airtel'},
  '9174106':{'en': 'Airtel'},
  '9174105':{'en': 'Airtel'},
```

### Comparing `phonenumbers-8.9.8/phonenumbers/data/__init__.py` & `phonenumbers-8.9.9/phonenumbers/data/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/alt_format_372.py` & `phonenumbers-8.9.9/phonenumbers/data/alt_format_372.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/alt_format_381.py` & `phonenumbers-8.9.9/phonenumbers/data/alt_format_381.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/alt_format_385.py` & `phonenumbers-8.9.9/phonenumbers/data/alt_format_385.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/alt_format_43.py` & `phonenumbers-8.9.9/phonenumbers/data/alt_format_43.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/alt_format_44.py` & `phonenumbers-8.9.9/phonenumbers/data/alt_format_44.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/alt_format_49.py` & `phonenumbers-8.9.9/phonenumbers/data/alt_format_49.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/alt_format_61.py` & `phonenumbers-8.9.9/phonenumbers/data/alt_format_61.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/alt_format_62.py` & `phonenumbers-8.9.9/phonenumbers/data/alt_format_62.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/alt_format_7.py` & `phonenumbers-8.9.9/phonenumbers/data/alt_format_7.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/alt_format_91.py` & `phonenumbers-8.9.9/phonenumbers/data/alt_format_91.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_870.py` & `phonenumbers-8.9.9/phonenumbers/data/region_870.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_878.py` & `phonenumbers-8.9.9/phonenumbers/data/region_878.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_881.py` & `phonenumbers-8.9.9/phonenumbers/data/region_881.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_882.py` & `phonenumbers-8.9.9/phonenumbers/data/region_882.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_883.py` & `phonenumbers-8.9.9/phonenumbers/data/region_883.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_888.py` & `phonenumbers-8.9.9/phonenumbers/data/region_888.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_979.py` & `phonenumbers-8.9.9/phonenumbers/data/region_979.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AC.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AD.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AD.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AE.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AF.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AG.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AI.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AL.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AO.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AR.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AS.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AT.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AU.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AW.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AX.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AX.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_AZ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_AZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BA.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BB.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BB.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BD.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BD.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BE.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BF.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BG.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BH.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BI.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BJ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BJ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BL.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BN.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BO.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BQ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BQ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BR.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BS.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BT.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BW.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BY.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_BZ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_BZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CA.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CC.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CD.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CD.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CF.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CG.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CH.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CI.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CK.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CL.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CN.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CO.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CR.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CU.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CV.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CV.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CW.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CX.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CX.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CY.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_CZ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_CZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_DE.py` & `phonenumbers-8.9.9/phonenumbers/data/region_DE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_DJ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_DJ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_DK.py` & `phonenumbers-8.9.9/phonenumbers/data/region_DK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_DM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_DM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_DO.py` & `phonenumbers-8.9.9/phonenumbers/data/region_DO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_DZ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_DZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_EC.py` & `phonenumbers-8.9.9/phonenumbers/data/region_EC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_EE.py` & `phonenumbers-8.9.9/phonenumbers/data/region_EE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_EG.py` & `phonenumbers-8.9.9/phonenumbers/data/region_EG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_EH.py` & `phonenumbers-8.9.9/phonenumbers/data/region_EH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_ER.py` & `phonenumbers-8.9.9/phonenumbers/data/region_ER.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_ES.py` & `phonenumbers-8.9.9/phonenumbers/data/region_ES.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_ET.py` & `phonenumbers-8.9.9/phonenumbers/data/region_ET.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_FI.py` & `phonenumbers-8.9.9/phonenumbers/data/region_FI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_FJ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_FJ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_FK.py` & `phonenumbers-8.9.9/phonenumbers/data/region_FK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_FM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_FM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_FO.py` & `phonenumbers-8.9.9/phonenumbers/data/region_FO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_FR.py` & `phonenumbers-8.9.9/phonenumbers/data/region_FR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GA.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GB.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GB.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GD.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GD.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GE.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GF.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GG.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GH.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GI.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GL.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GN.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GP.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GP.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GQ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GQ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GR.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GT.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GU.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GW.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_GY.py` & `phonenumbers-8.9.9/phonenumbers/data/region_GY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_HK.py` & `phonenumbers-8.9.9/phonenumbers/data/region_HK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_HN.py` & `phonenumbers-8.9.9/phonenumbers/data/region_HN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_HR.py` & `phonenumbers-8.9.9/phonenumbers/data/region_HR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_HT.py` & `phonenumbers-8.9.9/phonenumbers/data/region_HT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_HU.py` & `phonenumbers-8.9.9/phonenumbers/data/region_HU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_ID.py` & `phonenumbers-8.9.9/phonenumbers/data/region_ID.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_IE.py` & `phonenumbers-8.9.9/phonenumbers/data/region_IE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_IL.py` & `phonenumbers-8.9.9/phonenumbers/data/region_IL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_IM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_IM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_IN.py` & `phonenumbers-8.9.9/phonenumbers/data/region_IN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_IO.py` & `phonenumbers-8.9.9/phonenumbers/data/region_IO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_IQ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_IQ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_IR.py` & `phonenumbers-8.9.9/phonenumbers/data/region_IR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_IS.py` & `phonenumbers-8.9.9/phonenumbers/data/region_IS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_IT.py` & `phonenumbers-8.9.9/phonenumbers/data/region_IT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_JE.py` & `phonenumbers-8.9.9/phonenumbers/data/region_JE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_JM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_JM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_JO.py` & `phonenumbers-8.9.9/phonenumbers/data/region_JO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_JP.py` & `phonenumbers-8.9.9/phonenumbers/data/region_JP.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_KE.py` & `phonenumbers-8.9.9/phonenumbers/data/region_KE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_KG.py` & `phonenumbers-8.9.9/phonenumbers/data/region_KG.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Auto-generated file, do not edit by hand. KG metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
 PHONE_METADATA_KG = PhoneMetadata(id='KG', country_code=996, international_prefix='00',
-    general_desc=PhoneNumberDesc(national_number_pattern='[235-8]\\d{8,9}', possible_length=(9, 10), possible_length_local_only=(5, 6)),
+    general_desc=PhoneNumberDesc(national_number_pattern='[235-9]\\d{8,9}', possible_length=(9, 10), possible_length_local_only=(5, 6)),
     fixed_line=PhoneNumberDesc(national_number_pattern='(?:3(?:1(?:[256]\\d|3[1-9]|47)|2(?:22|3[0-479]|6[0-7])|4(?:22|5[6-9]|6\\d)|5(?:22|3[4-7]|59|6\\d)|6(?:22|5[35-7]|6\\d)|7(?:22|3[468]|4[1-9]|59|[67]\\d)|9(?:22|4[1-8]|6\\d))|6(?:09|12|2[2-4])\\d)\\d{5}', example_number='312123456', possible_length=(9,), possible_length_local_only=(5, 6)),
-    mobile=PhoneNumberDesc(national_number_pattern='(?:2(?:0[0-35]|2\\d)|5[0-24-7]\\d|7(?:[07]\\d|55))\\d{6}', example_number='700123456', possible_length=(9,)),
+    mobile=PhoneNumberDesc(national_number_pattern='(?:2(?:0[0-35]|2\\d)|5[0-24-7]\\d|7(?:[07]\\d|55)|99[69])\\d{6}', example_number='700123456', possible_length=(9,)),
     toll_free=PhoneNumberDesc(national_number_pattern='800\\d{6,7}', example_number='800123456', possible_length=(9, 10)),
     national_prefix='0',
     national_prefix_for_parsing='0',
-    number_format=[NumberFormat(pattern='(\\d{3})(\\d{3})(\\d{3})', format='\\1 \\2 \\3', leading_digits_pattern=['[25-7]|31[25]'], national_prefix_formatting_rule='0\\1'),
+    number_format=[NumberFormat(pattern='(\\d{3})(\\d{3})(\\d{3})', format='\\1 \\2 \\3', leading_digits_pattern=['[25-79]|31[25]'], national_prefix_formatting_rule='0\\1'),
         NumberFormat(pattern='(\\d{4})(\\d{5})', format='\\1 \\2', leading_digits_pattern=['3(?:1[36]|[2-9])'], national_prefix_formatting_rule='0\\1'),
         NumberFormat(pattern='(\\d{3})(\\d{3})(\\d)(\\d{3})', format='\\1 \\2 \\3 \\4', leading_digits_pattern=['8'], national_prefix_formatting_rule='0\\1')])
```

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_KH.py` & `phonenumbers-8.9.9/phonenumbers/data/region_KH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_KI.py` & `phonenumbers-8.9.9/phonenumbers/data/region_KI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_KM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_KM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_KN.py` & `phonenumbers-8.9.9/phonenumbers/data/region_KN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_KP.py` & `phonenumbers-8.9.9/phonenumbers/data/region_KP.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_KR.py` & `phonenumbers-8.9.9/phonenumbers/data/region_KR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_KW.py` & `phonenumbers-8.9.9/phonenumbers/data/region_KW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_KY.py` & `phonenumbers-8.9.9/phonenumbers/data/region_KY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_KZ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_KZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_LA.py` & `phonenumbers-8.9.9/phonenumbers/data/region_LA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_LB.py` & `phonenumbers-8.9.9/phonenumbers/data/region_LB.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_LC.py` & `phonenumbers-8.9.9/phonenumbers/data/region_LC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_LI.py` & `phonenumbers-8.9.9/phonenumbers/data/region_LI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_LK.py` & `phonenumbers-8.9.9/phonenumbers/data/region_LK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_LR.py` & `phonenumbers-8.9.9/phonenumbers/data/region_LR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_LS.py` & `phonenumbers-8.9.9/phonenumbers/data/region_LS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_LT.py` & `phonenumbers-8.9.9/phonenumbers/data/region_LT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_LU.py` & `phonenumbers-8.9.9/phonenumbers/data/region_LU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_LV.py` & `phonenumbers-8.9.9/phonenumbers/data/region_LV.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_LY.py` & `phonenumbers-8.9.9/phonenumbers/data/region_LY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MA.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MC.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MD.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MD.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_ME.py` & `phonenumbers-8.9.9/phonenumbers/data/region_ME.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MF.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MG.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MH.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MK.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_ML.py` & `phonenumbers-8.9.9/phonenumbers/data/region_ML.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MN.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MO.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MP.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MP.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MQ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MQ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MR.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MS.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MT.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MU.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MV.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MV.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MW.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MX.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MX.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MY.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_MZ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_MZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_NA.py` & `phonenumbers-8.9.9/phonenumbers/data/region_NA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_NC.py` & `phonenumbers-8.9.9/phonenumbers/data/region_NC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_NE.py` & `phonenumbers-8.9.9/phonenumbers/data/region_NE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_NF.py` & `phonenumbers-8.9.9/phonenumbers/data/region_NF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_NG.py` & `phonenumbers-8.9.9/phonenumbers/data/region_NG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_NI.py` & `phonenumbers-8.9.9/phonenumbers/data/region_NI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_NL.py` & `phonenumbers-8.9.9/phonenumbers/data/region_NL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_NO.py` & `phonenumbers-8.9.9/phonenumbers/data/region_NO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_NP.py` & `phonenumbers-8.9.9/phonenumbers/data/region_NP.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_NR.py` & `phonenumbers-8.9.9/phonenumbers/data/region_NR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_NU.py` & `phonenumbers-8.9.9/phonenumbers/data/region_PW.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
-"""Auto-generated file, do not edit by hand. NU metadata"""
+"""Auto-generated file, do not edit by hand. PW metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_NU = PhoneMetadata(id='NU', country_code=683, international_prefix='00',
-    general_desc=PhoneNumberDesc(national_number_pattern='[1-5]\\d{3}', possible_length=(4,)),
-    fixed_line=PhoneNumberDesc(national_number_pattern='[34]\\d{3}', example_number='4002', possible_length=(4,)),
-    mobile=PhoneNumberDesc(national_number_pattern='[125]\\d{3}', example_number='1234', possible_length=(4,)))
+PHONE_METADATA_PW = PhoneMetadata(id='PW', country_code=680, international_prefix='01[12]',
+    general_desc=PhoneNumberDesc(national_number_pattern='[2-9]\\d{6}', possible_length=(7,)),
+    fixed_line=PhoneNumberDesc(national_number_pattern='(?:2(?:55|77)|345|488|5(?:35|44|87)|6(?:22|54|79)|7(?:33|47)|8(?:24|55|76)|900)\\d{4}', example_number='2771234', possible_length=(7,)),
+    mobile=PhoneNumberDesc(national_number_pattern='(?:6[234689]0|77\\d|88[0-4])\\d{4}', example_number='6201234', possible_length=(7,)),
+    number_format=[NumberFormat(pattern='(\\d{3})(\\d{4})', format='\\1 \\2')])
```

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_NZ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_NZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_OM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_OM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_PA.py` & `phonenumbers-8.9.9/phonenumbers/data/region_PA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_PE.py` & `phonenumbers-8.9.9/phonenumbers/data/region_PE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_PF.py` & `phonenumbers-8.9.9/phonenumbers/data/region_PF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_PG.py` & `phonenumbers-8.9.9/phonenumbers/data/region_PG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_PH.py` & `phonenumbers-8.9.9/phonenumbers/data/region_PH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_PK.py` & `phonenumbers-8.9.9/phonenumbers/data/region_PK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_PL.py` & `phonenumbers-8.9.9/phonenumbers/data/region_PL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_PM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_PM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_PR.py` & `phonenumbers-8.9.9/phonenumbers/data/region_PR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_PS.py` & `phonenumbers-8.9.9/phonenumbers/data/region_PS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_PT.py` & `phonenumbers-8.9.9/phonenumbers/data/region_PT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_PW.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_PA.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Auto-generated file, do not edit by hand. PW metadata"""
+"""Auto-generated file, do not edit by hand. PA metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_PW = PhoneMetadata(id='PW', country_code=680, international_prefix='01[12]',
-    general_desc=PhoneNumberDesc(national_number_pattern='[2-9]\\d{6}', possible_length=(7,)),
-    fixed_line=PhoneNumberDesc(national_number_pattern='(?:2(?:55|77)|345|488|5(?:35|44|87)|6(?:22|54|79)|7(?:33|47)|8(?:24|55|76)|900)\\d{4}', example_number='2771234', possible_length=(7,)),
-    mobile=PhoneNumberDesc(national_number_pattern='(?:6[234689]0|77\\d|88[0-4])\\d{4}', example_number='6201234', possible_length=(7,)),
-    number_format=[NumberFormat(pattern='(\\d{3})(\\d{4})', format='\\1 \\2')])
+PHONE_METADATA_PA = PhoneMetadata(id='PA', country_code=None, international_prefix=None,
+    general_desc=PhoneNumberDesc(national_number_pattern='[19]\\d{2}', possible_length=(3,)),
+    emergency=PhoneNumberDesc(national_number_pattern='911', example_number='911', possible_length=(3,)),
+    short_code=PhoneNumberDesc(national_number_pattern='10[2-4]|911', example_number='102', possible_length=(3,)),
+    short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_PY.py` & `phonenumbers-8.9.9/phonenumbers/data/region_PY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_QA.py` & `phonenumbers-8.9.9/phonenumbers/data/region_QA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_RE.py` & `phonenumbers-8.9.9/phonenumbers/data/region_RE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_RO.py` & `phonenumbers-8.9.9/phonenumbers/data/region_RO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_RS.py` & `phonenumbers-8.9.9/phonenumbers/data/region_RS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_RU.py` & `phonenumbers-8.9.9/phonenumbers/data/region_RU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_RW.py` & `phonenumbers-8.9.9/phonenumbers/data/region_RW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SA.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SB.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SB.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SC.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SD.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SD.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SE.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SE.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     premium_rate=PhoneNumberDesc(national_number_pattern='649\\d{6}|9(?:00|39|44)[1-8]\\d{3,6}', example_number='9001234567', possible_length=(7, 8, 9, 10)),
     shared_cost=PhoneNumberDesc(national_number_pattern='77(?:0\\d{3}(?:\\d{3})?|[1-7]\\d{6})', example_number='771234567', possible_length=(6, 9)),
     personal_number=PhoneNumberDesc(national_number_pattern='75[1-8]\\d{6}', example_number='751234567', possible_length=(9,)),
     pager=PhoneNumberDesc(national_number_pattern='74[02-9]\\d{6}', example_number='740123456', possible_length=(9,)),
     voicemail=PhoneNumberDesc(national_number_pattern='(?:25[245]|67[3-6])\\d{9}', example_number='254123456789', possible_length=(12,)),
     national_prefix='0',
     national_prefix_for_parsing='0',
-    number_format=[NumberFormat(pattern='(9[034]\\d)(\\d{4})', format='\\1-\\2', leading_digits_pattern=['9(?:00|39|44)'], national_prefix_formatting_rule='0\\1'),
+    number_format=[NumberFormat(pattern='([1-469]\\d)(\\d{3})(\\d{2})', format='\\1-\\2 \\3', leading_digits_pattern=['[12][136]|3[356]|4[0246]|6[03]|90[1-9]'], national_prefix_formatting_rule='0\\1'),
+        NumberFormat(pattern='(9[034]\\d)(\\d{4})', format='\\1-\\2', leading_digits_pattern=['9(?:00|39|44)'], national_prefix_formatting_rule='0\\1'),
         NumberFormat(pattern='(8)(\\d{2,3})(\\d{2,3})(\\d{2})', format='\\1-\\2 \\3 \\4', leading_digits_pattern=['8'], national_prefix_formatting_rule='0\\1'),
-        NumberFormat(pattern='([1-69]\\d)(\\d{2,3})(\\d{2})(\\d{2})', format='\\1-\\2 \\3 \\4', leading_digits_pattern=['1[013689]|2[0136]|3[1356]|4[0246]|54|6[03]|90[1-9]'], national_prefix_formatting_rule='0\\1'),
-        NumberFormat(pattern='([1-469]\\d)(\\d{3})(\\d{2})', format='\\1-\\2 \\3', leading_digits_pattern=['[12][136]|3[356]|4[0246]|6[03]|90[1-9]'], national_prefix_formatting_rule='0\\1'),
+        NumberFormat(pattern='([1-69]\\d)(\\d{2,3})(\\d{2})(\\d{2})', format='\\1-\\2 \\3 \\4', leading_digits_pattern=['1[013689]|2[0136]|3[1356]|4[0246]|54|6[03]|90'], national_prefix_formatting_rule='0\\1'),
         NumberFormat(pattern='(\\d{3})(\\d{2})(\\d{2})(\\d{2})', format='\\1-\\2 \\3 \\4', leading_digits_pattern=['1[2457]|2(?:[247-9]|5[0138])|3[0247-9]|4[1357-9]|5[0-35-9]|6(?:[124-689]|7[0-2])|9(?:[125-8]|3[0-5]|4[0-3])'], national_prefix_formatting_rule='0\\1'),
         NumberFormat(pattern='(\\d{3})(\\d{2,3})(\\d{2})', format='\\1-\\2 \\3', leading_digits_pattern=['1[2457]|2(?:[247-9]|5[0138])|3[0247-9]|4[1357-9]|5[0-35-9]|6(?:[124-689]|7[0-2])|9(?:[125-8]|3[0-5]|4[0-3])'], national_prefix_formatting_rule='0\\1'),
         NumberFormat(pattern='(7\\d)(\\d{3})(\\d{2})(\\d{2})', format='\\1-\\2 \\3 \\4', leading_digits_pattern=['7'], national_prefix_formatting_rule='0\\1'),
         NumberFormat(pattern='(77)(\\d{2})(\\d{2})', format='\\1-\\2\\3', leading_digits_pattern=['77'], national_prefix_formatting_rule='0\\1'),
         NumberFormat(pattern='(20)(\\d{2,3})(\\d{2})', format='\\1-\\2 \\3', leading_digits_pattern=['20'], national_prefix_formatting_rule='0\\1'),
         NumberFormat(pattern='(9[034]\\d)(\\d{2})(\\d{2})(\\d{3})', format='\\1-\\2 \\3 \\4', leading_digits_pattern=['9[034]'], national_prefix_formatting_rule='0\\1'),
         NumberFormat(pattern='(\\d{3})(\\d{2})(\\d{3})(\\d{2})(\\d{2})', format='\\1-\\2 \\3 \\4 \\5', leading_digits_pattern=['25[245]|67[3-6]'], national_prefix_formatting_rule='0\\1')],
-    intl_number_format=[NumberFormat(pattern='(9[034]\\d)(\\d{4})', format='\\1 \\2', leading_digits_pattern=['9(?:00|39|44)']),
+    intl_number_format=[NumberFormat(pattern='([1-469]\\d)(\\d{3})(\\d{2})', format='\\1 \\2 \\3', leading_digits_pattern=['[12][136]|3[356]|4[0246]|6[03]|90[1-9]']),
+        NumberFormat(pattern='(9[034]\\d)(\\d{4})', format='\\1 \\2', leading_digits_pattern=['9(?:00|39|44)']),
         NumberFormat(pattern='(8)(\\d{2,3})(\\d{2,3})(\\d{2})', format='\\1 \\2 \\3 \\4', leading_digits_pattern=['8']),
-        NumberFormat(pattern='([1-69]\\d)(\\d{2,3})(\\d{2})(\\d{2})', format='\\1 \\2 \\3 \\4', leading_digits_pattern=['1[013689]|2[0136]|3[1356]|4[0246]|54|6[03]|90[1-9]']),
-        NumberFormat(pattern='([1-469]\\d)(\\d{3})(\\d{2})', format='\\1 \\2 \\3', leading_digits_pattern=['[12][136]|3[356]|4[0246]|6[03]|90[1-9]']),
+        NumberFormat(pattern='([1-69]\\d)(\\d{2,3})(\\d{2})(\\d{2})', format='\\1 \\2 \\3 \\4', leading_digits_pattern=['1[013689]|2[0136]|3[1356]|4[0246]|54|6[03]|90']),
         NumberFormat(pattern='(\\d{3})(\\d{2})(\\d{2})(\\d{2})', format='\\1 \\2 \\3 \\4', leading_digits_pattern=['1[2457]|2(?:[247-9]|5[0138])|3[0247-9]|4[1357-9]|5[0-35-9]|6(?:[124-689]|7[0-2])|9(?:[125-8]|3[0-5]|4[0-3])']),
         NumberFormat(pattern='(\\d{3})(\\d{2,3})(\\d{2})', format='\\1 \\2 \\3', leading_digits_pattern=['1[2457]|2(?:[247-9]|5[0138])|3[0247-9]|4[1357-9]|5[0-35-9]|6(?:[124-689]|7[0-2])|9(?:[125-8]|3[0-5]|4[0-3])']),
         NumberFormat(pattern='(7\\d)(\\d{3})(\\d{2})(\\d{2})', format='\\1 \\2 \\3 \\4', leading_digits_pattern=['7']),
         NumberFormat(pattern='(77)(\\d{2})(\\d{2})', format='\\1 \\2 \\3', leading_digits_pattern=['77']),
         NumberFormat(pattern='(20)(\\d{2,3})(\\d{2})', format='\\1 \\2 \\3', leading_digits_pattern=['20']),
         NumberFormat(pattern='(9[034]\\d)(\\d{2})(\\d{2})(\\d{3})', format='\\1 \\2 \\3 \\4', leading_digits_pattern=['9[034]']),
         NumberFormat(pattern='(\\d{3})(\\d{2})(\\d{3})(\\d{2})(\\d{2})', format='\\1 \\2 \\3 \\4 \\5', leading_digits_pattern=['25[245]|67[3-6]'])],
```

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SG.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SH.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SI.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SJ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SJ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SK.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SL.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SN.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SO.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SR.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SS.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_ST.py` & `phonenumbers-8.9.9/phonenumbers/data/region_ST.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SV.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SV.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SX.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SX.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SY.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_SZ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_SZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_TC.py` & `phonenumbers-8.9.9/phonenumbers/data/region_TC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_TD.py` & `phonenumbers-8.9.9/phonenumbers/data/region_TD.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_TG.py` & `phonenumbers-8.9.9/phonenumbers/data/region_TG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_TH.py` & `phonenumbers-8.9.9/phonenumbers/data/region_TH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_TJ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_TJ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_TK.py` & `phonenumbers-8.9.9/phonenumbers/data/region_TK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_TL.py` & `phonenumbers-8.9.9/phonenumbers/data/region_TL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_TM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_TM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_TN.py` & `phonenumbers-8.9.9/phonenumbers/data/region_TN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_TO.py` & `phonenumbers-8.9.9/phonenumbers/data/region_TO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_TR.py` & `phonenumbers-8.9.9/phonenumbers/data/region_TR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_TT.py` & `phonenumbers-8.9.9/phonenumbers/data/region_TT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_TV.py` & `phonenumbers-8.9.9/phonenumbers/data/region_TV.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_TW.py` & `phonenumbers-8.9.9/phonenumbers/data/region_TW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_TZ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_TZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_UA.py` & `phonenumbers-8.9.9/phonenumbers/data/region_UA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_UG.py` & `phonenumbers-8.9.9/phonenumbers/data/region_UG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_US.py` & `phonenumbers-8.9.9/phonenumbers/data/region_US.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_UY.py` & `phonenumbers-8.9.9/phonenumbers/data/region_UY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_UZ.py` & `phonenumbers-8.9.9/phonenumbers/data/region_UZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_VA.py` & `phonenumbers-8.9.9/phonenumbers/data/region_VA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_VC.py` & `phonenumbers-8.9.9/phonenumbers/data/region_VC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_VE.py` & `phonenumbers-8.9.9/phonenumbers/data/region_VE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_VG.py` & `phonenumbers-8.9.9/phonenumbers/data/region_VG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_VI.py` & `phonenumbers-8.9.9/phonenumbers/data/region_VI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_VN.py` & `phonenumbers-8.9.9/phonenumbers/data/region_VN.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Auto-generated file, do not edit by hand. VN metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
 PHONE_METADATA_VN = PhoneMetadata(id='VN', country_code=84, international_prefix='00',
     general_desc=PhoneNumberDesc(national_number_pattern='1\\d{6,9}|2\\d{9}|6\\d{6,7}|7\\d{6}|8\\d{6,8}|9\\d{8}', possible_length=(7, 8, 9, 10)),
     fixed_line=PhoneNumberDesc(national_number_pattern='(?:2(?:0[3-9]|1[0-689]|2[0-25-9]|3[2-9]|4[2-8]|5[124-9]|6[0-39]|7[0-7]|8[2-7]|9[0-4679])\\d|866)\\d{6}', example_number='2101234567', possible_length=(9, 10)),
-    mobile=PhoneNumberDesc(national_number_pattern='(?:9\\d|1(?:2\\d|6[2-9]|8[68]|99))\\d{7}|8(?:6[689]|8\\d|9[89])\\d{6}', example_number='912345678', possible_length=(9, 10)),
+    mobile=PhoneNumberDesc(national_number_pattern='(?:9(?:[0-8]\\d|9[013-9])|1(?:2\\d|6[2-9]|8[68]|99)\\d|8(?:6[689]|8\\d|9[89]))\\d{6}', example_number='912345678', possible_length=(9, 10)),
     toll_free=PhoneNumberDesc(national_number_pattern='1800\\d{4,6}', example_number='1800123456', possible_length=(8, 9, 10)),
     premium_rate=PhoneNumberDesc(national_number_pattern='1900\\d{4,6}', example_number='1900123456', possible_length=(8, 9, 10)),
+    voip=PhoneNumberDesc(national_number_pattern='992\\d{6}', example_number='992012345', possible_length=(9,)),
     uan=PhoneNumberDesc(national_number_pattern='[17]99\\d{4}|69\\d{5,6}|80\\d{5}', example_number='1992000', possible_length=(7, 8)),
     no_international_dialling=PhoneNumberDesc(national_number_pattern='[17]99\\d{4}|69\\d{5,6}', example_number='1992000', possible_length=(7, 8)),
     national_prefix='0',
     national_prefix_for_parsing='0',
     number_format=[NumberFormat(pattern='([17]99)(\\d{4})', format='\\1 \\2', leading_digits_pattern=['[17]99'], national_prefix_formatting_rule='0\\1', national_prefix_optional_when_formatting=True),
         NumberFormat(pattern='(\\d{2})(\\d{4})(\\d{4})', format='\\1 \\2 \\3', leading_digits_pattern=['2[48]'], national_prefix_formatting_rule='0\\1', national_prefix_optional_when_formatting=True),
         NumberFormat(pattern='(80)(\\d{5})', format='\\1 \\2', leading_digits_pattern=['80'], national_prefix_formatting_rule='0\\1', national_prefix_optional_when_formatting=True),
```

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_VU.py` & `phonenumbers-8.9.9/phonenumbers/data/region_VU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_WF.py` & `phonenumbers-8.9.9/phonenumbers/data/region_WF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_WS.py` & `phonenumbers-8.9.9/phonenumbers/data/region_WS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_XK.py` & `phonenumbers-8.9.9/phonenumbers/data/region_XK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_YE.py` & `phonenumbers-8.9.9/phonenumbers/data/region_YE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_YT.py` & `phonenumbers-8.9.9/phonenumbers/data/region_YT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_ZA.py` & `phonenumbers-8.9.9/phonenumbers/data/region_ZA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_ZM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_ZM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/data/region_ZW.py` & `phonenumbers-8.9.9/phonenumbers/data/region_ZW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geocoder.py` & `phonenumbers-8.9.9/phonenumbers/geocoder.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/__init__.py` & `phonenumbers-8.9.9/phonenumbers/geodata/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data0.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data0.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data1.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data1.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data10.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data10.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data11.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data11.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data12.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data12.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data13.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data13.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data14.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data14.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data15.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data15.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data16.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data16.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data17.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data17.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data18.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data18.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data19.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data19.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data2.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data2.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data20.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data20.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data21.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data21.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data22.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data22.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data23.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data23.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data24.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data24.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data25.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data25.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data26.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data26.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data27.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data27.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data28.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data28.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,22 @@
  '90313':{'en': 'Ankara', 'tr': 'Ankara'},
  '90318':{'en': 'Kirikkale', 'tr': u('K\u0131r\u0131kkale')},
  '90319':{'en': 'Kirikkale', 'tr': u('K\u0131r\u0131kkale')},
  '918332':{'en': 'Gokak, Karnataka'},
  '918333':{'en': 'Hukkeri/Sankeshwar, Karnataka'},
  '880903256':{'en': 'Trisal, Mymensingh'},
  '9923322':{'en': 'Kulyab'},
+ '9963749':{'en': 'Kanysh-Kya (Chatkal), Jalal-Abat region'},
+ '9963748':{'en': 'Kok-Jangak/Suzak, Jalal-Abat region'},
+ '9963745':{'en': 'Tash-Kumyr, Jalal-Abat region'},
+ '9963744':{'en': 'Mailuu-Suu, Jalal-Abat region'},
+ '9963747':{'en': 'Toktogul, Jalal-Abat region'},
+ '9963746':{'en': 'Kara-Kul, Jalal-Abat region'},
+ '9963741':{'en': 'Ala-Buka, Jalal-Abat region'},
+ '9963742':{'en': 'Kerben, Jalal-Abat region'},
  '86189142':{'en': 'Wuxi, Jiangsu', 'zh': u('\u6c5f\u82cf\u7701\u65e0\u9521\u5e02')},
  '86189147':{'en': 'Nanjing, Jiangsu', 'zh': u('\u6c5f\u82cf\u7701\u5357\u4eac\u5e02')},
  '86189146':{'en': 'Yancheng, Jiangsu', 'zh': u('\u6c5f\u82cf\u7701\u76d0\u57ce\u5e02')},
  '917467':{'en': 'Bamanwas, Rajasthan'},
  '917466':{'en': 'Bonli, Rajasthan'},
  '917465':{'en': 'Sapotra, Rajasthan'},
  '917464':{'en': 'Karauli, Rajasthan'},
@@ -236,14 +244,18 @@
  '91479':{'en': 'Mavelikkara, Kerala'},
  '91476':{'en': 'Karunagapally, Kerala'},
  '91477':{'en': 'Alappuzha, Kerala'},
  '91474':{'en': 'Kollam, Kerala'},
  '91475':{'en': 'Punalur, Kerala'},
  '91470':{'en': 'Attingal, Kerala'},
  '91471':{'en': 'Thiruvananthapuram, Kerala'},
+ '9963536':{'en': 'Chaek/Minkush, Naryn region'},
+ '9963537':{'en': 'Baetov, Naryn region'},
+ '9963534':{'en': 'At-Bashy, Naryn region'},
+ '9963535':{'en': 'Kochkor, Naryn region'},
  '916132':{'en': 'Barh, Bihar'},
  '861890748':{'en': 'Changsha, Hunan', 'zh': u('\u6e56\u5357\u7701\u957f\u6c99\u5e02')},
  '861890749':{'en': 'Changsha, Hunan', 'zh': u('\u6e56\u5357\u7701\u957f\u6c99\u5e02')},
  '861890740':{'en': 'Yueyang, Hunan', 'zh': u('\u6e56\u5357\u7701\u5cb3\u9633\u5e02')},
  '861890741':{'en': 'Zhuzhou, Hunan', 'zh': u('\u6e56\u5357\u7701\u682a\u6d32\u5e02')},
  '861890742':{'en': 'Changde, Hunan', 'zh': u('\u6e56\u5357\u7701\u5e38\u5fb7\u5e02')},
  '861890743':{'en': 'Xiangxi, Hunan', 'zh': u('\u6e56\u5357\u7701\u6e58\u897f\u571f\u5bb6\u65cf\u82d7\u65cf\u81ea\u6cbb\u5dde')},
@@ -912,14 +924,15 @@
  '90447':{'en': 'Erzincan', 'tr': 'Erzincan'},
  '90442':{'en': 'Erzurum', 'tr': 'Erzurum'},
  '90443':{'en': 'Erzurum', 'tr': 'Erzurum'},
  '861893402':{'en': 'Zhanjiang, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u6e5b\u6c5f\u5e02')},
  '911491':{'en': 'Nasirabad, Rajasthan'},
  '861893400':{'en': 'Zhanjiang, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u6e5b\u6c5f\u5e02')},
  '88054248':{'en': 'Palashbari'},
+ '996312':{'en': 'Bishkek, Chuy region'},
  '86189424':{'en': 'Foshan, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u4f5b\u5c71\u5e02')},
  '861892368':{'en': 'Heyuan, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u6cb3\u6e90\u5e02')},
  '86189427':{'en': 'Panjin, Liaoning', 'zh': u('\u8fbd\u5b81\u7701\u76d8\u9526\u5e02')},
  '861892369':{'en': 'Heyuan, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u6cb3\u6e90\u5e02')},
  '861893235':{'en': 'Yangzhou, Jiangsu', 'zh': u('\u6c5f\u82cf\u7701\u626c\u5dde\u5e02')},
  '861893234':{'en': 'HuaiAn, Jiangsu', 'zh': u('\u6c5f\u82cf\u7701\u6dee\u5b89\u5e02')},
  '861893237':{'en': 'Yangzhou, Jiangsu', 'zh': u('\u6c5f\u82cf\u7701\u626c\u5dde\u5e02')},
@@ -982,15 +995,18 @@
  '88052169':{'en': 'Rangpur'},
  '918473':{'en': 'Yadgiri, Karnataka'},
  '95256':{'en': 'Amarapura'},
  '97615152':{'en': 'Halzan, Sukhbaatar'},
  '97615153':{'en': 'Erdenetsagaan, Sukhbaatar'},
  '97615151':{'en': 'Uulbayan, Sukhbaatar'},
  '918474':{'en': 'Chittapur, Karnataka'},
+ '9963457':{'en': 'Bakay-Ata, Talas region'},
+ '9963456':{'en': 'Kyzyl-Adyr, Talas region'},
  '99422428':{'en': 'Agstafa/Ganja/Yevlakh'},
+ '9963458':{'en': 'Kokoy, Talas region'},
  '88083278':{'en': 'Madabpur'},
  '91374':{'en': 'Tinsukhia, Assam'},
  '91376':{'en': 'Jorhat, Assam'},
  '91370':{'en': 'Kohima, Nagaland'},
  '91373':{'en': 'Dibrugarh, Assam'},
  '91372':{'en': 'Lungleh, Mizoram'},
  '861894588':{'en': 'Yichun, Heilongjiang', 'zh': u('\u9ed1\u9f99\u6c5f\u7701\u4f0a\u6625\u5e02')},
@@ -1577,14 +1593,15 @@
  '90213':{'en': 'Istanbul (Europe)', 'tr': 'Istanbul (Avrupa)'},
  '90212':{'en': 'Istanbul (Europe)', 'tr': 'Istanbul (Avrupa)'},
  '97615854':{'en': 'Chuluunkhoroot, Dornod'},
  '97615853':{'en': 'Choibalsan, Dornod'},
  '97615852':{'en': 'Tsagaan-Ovoo, Dornod'},
  '97615851':{'en': 'Khulunbuyir, Dornod'},
  '880903356':{'en': 'Phulpur, Mymensingh'},
+ '9963622':{'en': 'Batken, Naryn region'},
  '861890979':{'en': 'Haixi, Qinghai', 'zh': u('\u9752\u6d77\u7701\u6d77\u897f\u8499\u53e4\u65cf\u85cf\u65cf\u81ea\u6cbb\u5dde')},
  '861890978':{'en': 'Xining, Qinghai', 'zh': u('\u9752\u6d77\u7701\u897f\u5b81\u5e02')},
  '861890973':{'en': 'Huangnan, Qinghai', 'zh': u('\u9752\u6d77\u7701\u9ec4\u5357\u85cf\u65cf\u81ea\u6cbb\u5dde')},
  '861890972':{'en': 'Haidong, Qinghai', 'zh': u('\u9752\u6d77\u7701\u6d77\u4e1c\u5730\u533a')},
  '861890971':{'en': 'Xining, Qinghai', 'zh': u('\u9752\u6d77\u7701\u897f\u5b81\u5e02')},
  '861890970':{'en': 'Haibei, Qinghai', 'zh': u('\u9752\u6d77\u7701\u6d77\u5317\u85cf\u65cf\u81ea\u6cbb\u5dde')},
  '861890977':{'en': 'Haixi, Qinghai', 'zh': u('\u9752\u6d77\u7701\u6d77\u897f\u8499\u53e4\u65cf\u85cf\u65cf\u81ea\u6cbb\u5dde')},
@@ -3556,15 +3573,22 @@
  '861897054':{'en': 'Yichun, Jiangxi', 'zh': u('\u6c5f\u897f\u7701\u5b9c\u6625\u5e02')},
  '861897057':{'en': 'Yichun, Jiangxi', 'zh': u('\u6c5f\u897f\u7701\u5b9c\u6625\u5e02')},
  '861897056':{'en': 'Yichun, Jiangxi', 'zh': u('\u6c5f\u897f\u7701\u5b9c\u6625\u5e02')},
  '861897051':{'en': 'Yichun, Jiangxi', 'zh': u('\u6c5f\u897f\u7701\u5b9c\u6625\u5e02')},
  '861897050':{'en': 'Yichun, Jiangxi', 'zh': u('\u6c5f\u897f\u7701\u5b9c\u6625\u5e02')},
  '861897053':{'en': 'Yichun, Jiangxi', 'zh': u('\u6c5f\u897f\u7701\u5b9c\u6625\u5e02')},
  '861897052':{'en': 'Yichun, Jiangxi', 'zh': u('\u6c5f\u897f\u7701\u5b9c\u6625\u5e02')},
+ '9963137':{'en': 'Kayndy, Chuy region'},
  '916795':{'en': 'Udala, Odisha'},
+ '9963135':{'en': 'Kemin, Chuy region'},
+ '9963132':{'en': 'Kant, Chuy region'},
+ '9963133':{'en': 'Kara-Balta, Chuy region'},
+ '9963131':{'en': 'Belovodskoe, Chuy region'},
+ '9963138':{'en': 'Tokmok, Chuy region'},
+ '9963139':{'en': 'Lebedinovka, Chuy region'},
  '861899862':{'en': 'Yunfu, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u4e91\u6d6e\u5e02')},
  '861899863':{'en': 'Yangjiang, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u9633\u6c5f\u5e02')},
  '861899860':{'en': 'Qingyuan, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u6e05\u8fdc\u5e02')},
  '861899861':{'en': 'Qingyuan, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u6e05\u8fdc\u5e02')},
  '861899866':{'en': 'Shaoguan, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u97f6\u5173\u5e02')},
  '861899867':{'en': 'Zhanjiang, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u6e5b\u6c5f\u5e02')},
  '861899864':{'en': 'Yangjiang, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u9633\u6c5f\u5e02')},
@@ -3649,15 +3673,17 @@
  '97624347':{'en': 'Zereg, Khovd'},
  '861896699':{'en': 'Yulin, Shaanxi', 'zh': u('\u9655\u897f\u7701\u6986\u6797\u5e02')},
  '97624345':{'en': 'Durgun, Khovd'},
  '97624344':{'en': 'Darvi, Khovd'},
  '958523':{'en': 'Pyinoolwin'},
  '958522':{'en': 'Pyinoolwin'},
  '958521':{'en': 'Pyinoolwin'},
+ '9963734':{'en': 'Massy/Kochkor-Ata, Jalal-Abat region'},
  '97624343':{'en': 'Buyant, Khovd'},
+ '9963736':{'en': 'Bazarkorgon, Jalal-Abat region'},
  '958529':{'en': 'Padaythar Myothit'},
  '958528':{'en': 'Pyinoolwin'},
  '916565':{'en': 'Latehar, Bihar'},
  '91761':{'en': 'Jabalpur, Madhya Pradesh'},
  '97624341':{'en': 'Altai, Khovd'},
  '916564':{'en': 'Nagarutari, Bihar'},
  '916567':{'en': 'Barwadih, Bihar'},
@@ -3803,14 +3829,15 @@
  '918132':{'en': 'Kunigal, Karnataka'},
  '918133':{'en': 'Chikkanayakanahalli, Karnataka'},
  '918134':{'en': 'Tiptur, Karnataka'},
  '918135':{'en': 'Sira, Karnataka'},
  '918136':{'en': 'Pavagada, Karnataka'},
  '918137':{'en': 'Madugiri, Karnataka'},
  '86189896':{'en': 'Taizhou, Zhejiang', 'zh': u('\u6d59\u6c5f\u7701\u53f0\u5dde\u5e02')},
+ '9963722':{'en': 'Jalal-Abat'},
  '88055175':{'en': 'Domar, Nilphamari'},
  '861898038':{'en': 'Ziyang, Sichuan', 'zh': u('\u56db\u5ddd\u7701\u8d44\u9633\u5e02')},
  '861898039':{'en': 'Yibin, Sichuan', 'zh': u('\u56db\u5ddd\u7701\u5b9c\u5bbe\u5e02')},
  '861898036':{'en': 'Meishan, Sichuan', 'zh': u('\u56db\u5ddd\u7701\u7709\u5c71\u5e02')},
  '861898037':{'en': 'Meishan, Sichuan', 'zh': u('\u56db\u5ddd\u7701\u7709\u5c71\u5e02')},
  '861898034':{'en': 'Panzhihua, Sichuan', 'zh': u('\u56db\u5ddd\u7701\u6500\u679d\u82b1\u5e02')},
  '861898035':{'en': 'Panzhihua, Sichuan', 'zh': u('\u56db\u5ddd\u7701\u6500\u679d\u82b1\u5e02')},
@@ -4249,14 +4276,15 @@
  '86189561':{'en': 'Huaibei, Anhui', 'zh': u('\u5b89\u5fbd\u7701\u6dee\u5317\u5e02')},
  '86189560':{'en': 'Hefei, Anhui', 'zh': u('\u5b89\u5fbd\u7701\u5408\u80a5\u5e02')},
  '86189563':{'en': 'Xuancheng, Anhui', 'zh': u('\u5b89\u5fbd\u7701\u5ba3\u57ce\u5e02')},
  '86189562':{'en': 'Tongling, Anhui', 'zh': u('\u5b89\u5fbd\u7701\u94dc\u9675\u5e02')},
  '86189569':{'en': 'Anqing, Anhui', 'zh': u('\u5b89\u5fbd\u7701\u5b89\u5e86\u5e02')},
  '86189568':{'en': 'Bozhou, Anhui', 'zh': u('\u5b89\u5fbd\u7701\u4eb3\u5dde\u5e02')},
  '880852356':{'en': 'Bancharampur, Brahmanbaria'},
+ '9963134':{'en': 'Sokuluk, Chuy region'},
  '91878':{'en': 'Karimnagar, Andhra Pradesh'},
  '9762482':{'en': 'Altai city, Govi-Altai'},
  '917224':{'en': 'Daryapur, Maharashtra'},
  '88054189':{'en': 'Gaibandha'},
  '861892207':{'en': 'Zhanjiang, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u6e5b\u6c5f\u5e02')},
  '861892206':{'en': 'Zhanjiang, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u6e5b\u6c5f\u5e02')},
  '861892205':{'en': 'Jiangmen, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u6c5f\u95e8\u5e02')},
@@ -4669,14 +4697,15 @@
  '861892673':{'en': 'Maoming, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u8302\u540d\u5e02')},
  '861892670':{'en': 'Maoming, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u8302\u540d\u5e02')},
  '861892671':{'en': 'Maoming, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u8302\u540d\u5e02')},
  '861892676':{'en': 'Shenzhen, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u6df1\u5733\u5e02')},
  '861892677':{'en': 'Shenzhen, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u6df1\u5733\u5e02')},
  '861892674':{'en': 'Maoming, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u8302\u540d\u5e02')},
  '861892675':{'en': 'Shenzhen, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u6df1\u5733\u5e02')},
+ '9963738':{'en': 'Kazarman, Jalal-Abat region'},
  '861892678':{'en': 'Shenzhen, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u6df1\u5733\u5e02')},
  '861892679':{'en': 'Shenzhen, Guangdong', 'zh': u('\u5e7f\u4e1c\u7701\u6df1\u5733\u5e02')},
  '86438':{'en': 'Songyuan, Jilin', 'zh': u('\u5409\u6797\u7701\u677e\u539f\u5e02')},
  '86439':{'en': 'Baishan, Jilin', 'zh': u('\u5409\u6797\u7701\u767d\u5c71\u5e02')},
  '86436':{'en': 'Baicheng, Jilin', 'zh': u('\u5409\u6797\u7701\u767d\u57ce\u5e02')},
  '86437':{'en': 'Liaoyuan, Jilin', 'zh': u('\u5409\u6797\u7701\u8fbd\u6e90\u5e02')},
  '86434':{'en': 'Siping, Jilin', 'zh': u('\u5409\u6797\u7701\u56db\u5e73\u5e02')},
@@ -4982,14 +5011,18 @@
  '917605':{'en': 'Patera, Madhya Pradesh'},
  '917604':{'en': 'Hatta, Madhya Pradesh'},
  '88087238':{'en': 'Chatak'},
  '917608':{'en': 'Bijawar, Madhya Pradesh'},
  '915745':{'en': 'Jalesar, Uttar Pradesh'},
  '97624858':{'en': 'Erdene, Govi-Altai'},
  '97613862':{'en': 'Tsetserleg, Khuvsgul'},
+ '9963657':{'en': 'Kyzylkia, Naryn region'},
+ '9963656':{'en': 'Isfana, Naryn region'},
+ '9963655':{'en': 'Pulgon, Naryn region'},
+ '9963653':{'en': 'Sulukta, Naryn region'},
  '91421':{'en': 'Tirupur, Tamil Nadu'},
  '91423':{'en': 'Udhagamandalam, Tamil Nadu'},
  '91422':{'en': 'Coimbatore, Tamil Nadu'},
  '91424':{'en': 'Erode, Tamil Nadu'},
  '91427':{'en': 'Salem, Tamil Nadu'},
  '861895389':{'en': 'TaiAn, Shandong', 'zh': u('\u5c71\u4e1c\u7701\u6cf0\u5b89\u5e02')},
  '861895388':{'en': 'TaiAn, Shandong', 'zh': u('\u5c71\u4e1c\u7701\u6cf0\u5b89\u5e02')},
@@ -5203,35 +5236,39 @@
  '861897824':{'en': 'Laibin, Guangxi', 'zh': u('\u5e7f\u897f\u6765\u5bbe\u5e02')},
  '861897825':{'en': 'Laibin, Guangxi', 'zh': u('\u5e7f\u897f\u6765\u5bbe\u5e02')},
  '861897826':{'en': 'Laibin, Guangxi', 'zh': u('\u5e7f\u897f\u6765\u5bbe\u5e02')},
  '861897827':{'en': 'Hechi, Guangxi', 'zh': u('\u5e7f\u897f\u6cb3\u6c60\u5e02')},
  '861897828':{'en': 'Hechi, Guangxi', 'zh': u('\u5e7f\u897f\u6cb3\u6c60\u5e02')},
  '861897829':{'en': 'Hechi, Guangxi', 'zh': u('\u5e7f\u897f\u6cb3\u6c60\u5e02')},
  '9762342':{'en': 'Bulgan city, Bulgan'},
+ '9963231':{'en': 'Aravan, Osh region'},
  '86858':{'en': 'Liupanshui, Guizhou', 'zh': u('\u8d35\u5dde\u7701\u516d\u76d8\u6c34\u5e02')},
  '86859':{'en': 'Xingyi, Guizhou', 'zh': u('\u8d35\u5dde\u7701\u9ed4\u897f\u5357\u5e03\u4f9d\u65cf\u82d7\u65cf\u81ea\u6cbb\u5dde')},
+ '9963230':{'en': 'Eski-Nookat, Osh region'},
  '86854':{'en': 'Duyun, Guizhou', 'zh': u('\u8d35\u5dde\u7701\u9ed4\u5357\u5e03\u4f9d\u65cf\u82d7\u65cf\u81ea\u6cbb\u5dde')},
  '86855':{'en': 'Kaili, Guizhou', 'zh': u('\u8d35\u5dde\u7701\u9ed4\u4e1c\u5357\u82d7\u65cf\u4f97\u65cf\u81ea\u6cbb\u5dde')},
  '86856':{'en': 'Tongren, Guizhou', 'zh': u('\u8d35\u5dde\u7701\u94dc\u4ec1\u5730\u533a')},
  '86857':{'en': 'Bijie, Guizhou', 'zh': u('\u8d35\u5dde\u7701\u6bd5\u8282\u5730\u533a')},
  '86851':{'en': 'Guiyang/Zunyi/Anshun, Guizhou', 'zh': u('\u8d35\u5dde\u7701\u8d35\u9633\u5e02\u3001\u9075\u4e49\u5e02\u3001\u5b89\u987a\u5e02')},
  '86852':{'en': 'Zunyi, Guizhou', 'zh': u('\u8d35\u5dde\u7701\u9075\u4e49\u5e02')},
  '86853':{'en': 'Anshun, Guizhou', 'zh': u('\u8d35\u5dde\u7701\u5b89\u987a\u5e02')},
  '97613741':{'en': 'Orkhon, Darkhan-Uul'},
  '97613743':{'en': 'Sharingol, Darkhan-Uul'},
  '914898':{'en': 'Kiltan, Lakshadweep'},
  '918387':{'en': 'Honnavar, Karnataka'},
  '88042268':{'en': 'Keshobpur, Jessore'},
+ '9963239':{'en': 'Kara-Kulja, Osh region'},
  '97623243':{'en': 'Bayangol, Uvurkhangai'},
  '88072278':{'en': 'Paba'},
  '9491':{'en': 'Galle'},
  '9140':{'en': 'Hyderabad Local, Andhra Pradesh'},
  '9144':{'en': 'Chennai, Tamil Nadu'},
  '918388':{'en': 'Ankola, Karnataka'},
  '9724':{'en': 'Haifa and North Regions', 'iw': u('\u05d7\u05d9\u05e4\u05d4 \u05d5\u05d4\u05e6\u05e4\u05d5\u05df')},
+ '9963922':{'en': 'Karakol, Issyk-Ko region'},
  '9722':{'en': 'Jerusalem', 'iw': u('\u05d9\u05e8\u05d5\u05e9\u05dc\u05d9\u05dd')},
  '9723':{'en': 'Tel Aviv', 'iw': u('\u05ea\u05dc \u05d0\u05d1\u05d9\u05d1-\u05d9\u05e4\u05d5 \u05d5\u05d4\u05de\u05e8\u05db\u05d6')},
  '9728':{'en': 'Hashfela and South Regions', 'iw': u('\u05d4\u05e9\u05e4\u05dc\u05d4 \u05d5\u05d4\u05d3\u05e8\u05d5\u05dd')},
  '9729':{'en': 'Hasharon', 'iw': u('\u05d4\u05e9\u05e8\u05d5\u05df')},
  '86472':{'en': 'Baotou, Inner Mongolia', 'zh': u('\u5185\u8499\u53e4\u5305\u5934\u5e02')},
  '86473':{'en': 'Wuhai, Inner Mongolia', 'zh': u('\u5185\u8499\u53e4\u4e4c\u6d77\u5e02')},
  '86470':{'en': 'Hailaer, Inner Mongolia', 'zh': u('\u5185\u8499\u53e4\u547c\u4f26\u8d1d\u5c14\u5e02')},
@@ -5509,14 +5546,21 @@
  '861896642':{'en': 'Lishui, Zhejiang', 'zh': u('\u6d59\u6c5f\u7701\u4e3d\u6c34\u5e02')},
  '861896641':{'en': 'Quzhou, Zhejiang', 'zh': u('\u6d59\u6c5f\u7701\u8862\u5dde\u5e02')},
  '861896640':{'en': 'Quzhou, Zhejiang', 'zh': u('\u6d59\u6c5f\u7701\u8862\u5dde\u5e02')},
  '861896647':{'en': 'Huzhou, Zhejiang', 'zh': u('\u6d59\u6c5f\u7701\u6e56\u5dde\u5e02')},
  '861896646':{'en': 'Huzhou, Zhejiang', 'zh': u('\u6d59\u6c5f\u7701\u6e56\u5dde\u5e02')},
  '861896645':{'en': 'Zhoushan, Zhejiang', 'zh': u('\u6d59\u6c5f\u7701\u821f\u5c71\u5e02')},
  '861896644':{'en': 'Zhoushan, Zhejiang', 'zh': u('\u6d59\u6c5f\u7701\u821f\u5c71\u5e02')},
+ '9963948':{'en': 'Ak-Suu, Issyk-Ko region'},
+ '9963943':{'en': 'Cholpon-Ata, Issyk-Ko region'},
+ '9963942':{'en': 'Ananyevo, Issyk-Ko region'},
+ '9963947':{'en': 'Bokombaevo/Kadji-Say, Issyk-Ko region'},
+ '9963946':{'en': 'Kyzyl-Suu, Issyk-Ko region'},
+ '9963945':{'en': 'Tup, Issyk-Ko region'},
+ '9963944':{'en': 'Balykchy, Issyk-Ko region'},
  '8809175':{'en': 'Muktagacha, Mymensingh'},
  '861898902':{'en': 'Xigaze, Tibet', 'zh': u('\u897f\u85cf\u65e5\u5580\u5219\u5730\u533a')},
  '861898903':{'en': 'Shannan, Tibet', 'zh': u('\u897f\u85cf\u5c71\u5357\u5730\u533a')},
  '861898900':{'en': 'Lhasa, Tibet', 'zh': u('\u897f\u85cf\u62c9\u8428\u5e02')},
  '861898901':{'en': 'Lhasa, Tibet', 'zh': u('\u897f\u85cf\u62c9\u8428\u5e02')},
  '861898906':{'en': 'Nagqu, Tibet', 'zh': u('\u897f\u85cf\u90a3\u66f2\u5730\u533a')},
  '861898907':{'en': 'Ngari, Tibet', 'zh': u('\u897f\u85cf\u963f\u91cc\u5730\u533a')},
@@ -5748,14 +5792,15 @@
  '916722':{'en': 'Pardip, Odisha'},
  '916721':{'en': 'Narsinghpur, Odisha'},
  '916727':{'en': 'Kendrapara, Odisha'},
  '916726':{'en': 'Jajapur Road, Odisha'},
  '916725':{'en': 'Dhanmandal, Odisha'},
  '916724':{'en': 'Jagatsinghpur, Odisha'},
  '917258':{'en': 'Akot, Maharashtra'},
+ '9963422':{'en': 'Talas'},
  '917526':{'en': 'Ghatigaon, Madhya Pradesh'},
  '917527':{'en': 'Mehgaon, Madhya Pradesh'},
  '91612':{'en': 'Patna, Bihar'},
  '91341':{'en': 'Asansol, West Bengal'},
  '91342':{'en': 'Burdwan, West Bengal'},
  '91343':{'en': 'Durgapur, West Bengal'},
  '917525':{'en': 'Bhitarwar, Madhya Pradesh'},
@@ -6116,14 +6161,15 @@
  '861896932':{'en': 'Jiaxing, Zhejiang', 'zh': u('\u6d59\u6c5f\u7701\u5609\u5174\u5e02')},
  '861896935':{'en': 'Jinhua, Zhejiang', 'zh': u('\u6d59\u6c5f\u7701\u91d1\u534e\u5e02')},
  '861896934':{'en': 'Jiaxing, Zhejiang', 'zh': u('\u6d59\u6c5f\u7701\u5609\u5174\u5e02')},
  '861896937':{'en': 'Jinhua, Zhejiang', 'zh': u('\u6d59\u6c5f\u7701\u91d1\u534e\u5e02')},
  '861896936':{'en': 'Jinhua, Zhejiang', 'zh': u('\u6d59\u6c5f\u7701\u91d1\u534e\u5e02')},
  '861896939':{'en': 'Jinhua, Zhejiang', 'zh': u('\u6d59\u6c5f\u7701\u91d1\u534e\u5e02')},
  '861896938':{'en': 'Jinhua, Zhejiang', 'zh': u('\u6d59\u6c5f\u7701\u91d1\u534e\u5e02')},
+ '9963222':{'en': 'Osh'},
  '9762582':{'en': 'Choibalsan city, Dornod'},
  '912421':{'en': 'Jamkhed, Maharashtra'},
  '912422':{'en': 'Shri Rampur, Maharashtra'},
  '912423':{'en': 'Koparagon, Maharashtra'},
  '912424':{'en': 'Akole, Maharashtra'},
  '912425':{'en': 'Sangamner, Maharashtra'},
  '912426':{'en': 'Rahuri, Maharashtra'},
@@ -6369,14 +6415,15 @@
  '97615655':{'en': 'Norovlin, Khentii'},
  '97615654':{'en': 'Murun, Khentii'},
  '97615657':{'en': 'Tsenkhermandal, Khentii'},
  '97615656':{'en': 'Umnudelger, Khentii'},
  '97615651':{'en': 'Darkhan, Khentii'},
  '97615653':{'en': 'Jargaltkhaan, Khentii'},
  '97615652':{'en': 'Delgerkhaan, Khentii'},
+ '9963459':{'en': 'Pokrovka, Talas region'},
  '861897566':{'en': 'Changde, Hunan', 'zh': u('\u6e56\u5357\u7701\u5e38\u5fb7\u5e02')},
  '88065248':{'en': 'Zitka'},
  '88074169':{'en': 'Santahar, Nagoan'},
  '91651':{'en': 'Ranchi, Bihar'},
  '91657':{'en': 'Jamshedpur, Bihar'},
  '88074161':{'en': 'Nagoan'},
  '88074162':{'en': 'Nagoan'},
@@ -6584,14 +6631,18 @@
  '86354':{'en': 'Yuci, Shanxi', 'zh': u('\u5c71\u897f\u7701\u664b\u4e2d\u5e02')},
  '86353':{'en': 'Yangquan, Shanxi', 'zh': u('\u5c71\u897f\u7701\u9633\u6cc9\u5e02')},
  '86352':{'en': 'Datong, Shanxi', 'zh': u('\u5c71\u897f\u7701\u5927\u540c\u5e02')},
  '86351':{'en': 'Taiyuan, Shanxi', 'zh': u('\u5c71\u897f\u7701\u592a\u539f\u5e02')},
  '86350':{'en': 'Xinzhou, Shanxi', 'zh': u('\u5c71\u897f\u7701\u5ffb\u5dde\u5e02')},
  '861899589':{'en': 'Yichang, Hubei', 'zh': u('\u6e56\u5317\u7701\u5b9c\u660c\u5e02')},
  '861899588':{'en': 'Yichang, Hubei', 'zh': u('\u6e56\u5317\u7701\u5b9c\u660c\u5e02')},
+ '9963233':{'en': 'Uzgen, Osh region'},
+ '9963232':{'en': 'Kara-Suu, Osh region'},
+ '9963234':{'en': 'Gulcha, Osh region'},
+ '9963237':{'en': 'Daroot-Korgon, Osh region'},
  '861899581':{'en': 'Xianning, Hubei', 'zh': u('\u6e56\u5317\u7701\u54b8\u5b81\u5e02')},
  '861899580':{'en': 'Huangshi, Hubei', 'zh': u('\u6e56\u5317\u7701\u9ec4\u77f3\u5e02')},
  '861899583':{'en': 'Jingzhou, Hubei', 'zh': u('\u6e56\u5317\u7701\u8346\u5dde\u5e02')},
  '861899582':{'en': 'Xianning, Hubei', 'zh': u('\u6e56\u5317\u7701\u54b8\u5b81\u5e02')},
  '861899585':{'en': 'Jingzhou, Hubei', 'zh': u('\u6e56\u5317\u7701\u8346\u5dde\u5e02')},
  '861899584':{'en': 'Jingzhou, Hubei', 'zh': u('\u6e56\u5317\u7701\u8346\u5dde\u5e02')},
  '861899587':{'en': 'Yichang, Hubei', 'zh': u('\u6e56\u5317\u7701\u5b9c\u660c\u5e02')},
@@ -7116,14 +7167,15 @@
  '9923134':{'en': 'Rogun'},
  '912692':{'en': 'Anand, Gujarat'},
  '9923138':{'en': 'Nurek'},
  '9923139':{'en': 'Hissar'},
  '912875':{'en': 'Una/Diu, Gujarat'},
  '97624442':{'en': 'Bayanbulag, Bayankhongor'},
  '912690':{'en': 'Balasinor, Gujarat'},
+ '9963522':{'en': 'Naryn'},
  '912697':{'en': 'Retlad, Gujarat'},
  '912696':{'en': 'Borsad, Gujarat'},
  '97623654':{'en': 'Khuder, Selenge'},
  '97623655':{'en': 'Hushaat, Selenge'},
  '97623656':{'en': 'Tsagaannuur, Selenge'},
  '97623657':{'en': 'Shaamar, Selenge'},
  '97623651':{'en': 'Saikhan, Selenge'},
```

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data3.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data3.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data4.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data4.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data5.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data5.py`

 * *Files 0% similar despite different names*

```diff
@@ -5902,15 +5902,15 @@
  '437762':{'de': 'Raab', 'en': 'Raab'},
  '437765':{'de': 'Lambrechten', 'en': 'Lambrechten'},
  '437764':{'de': 'Riedau', 'en': 'Riedau'},
  '437767':{'de': 'Eggerding', 'en': 'Eggerding'},
  '437766':{'de': 'Andorf', 'en': 'Andorf'},
  '542928':{'en': 'Pedro Luro, Buenos Aires', 'es': 'Pedro Luro, Buenos Aires'},
  '542929':{'en': u('Guamin\u00ed, Buenos Aires'), 'es': u('Guamin\u00ed, Buenos Aires')},
- '5255':{'en': 'Mexico City, FD', 'es': u('Cuidad de M\u00e9xico, CDMX')},
+ '5255':{'en': 'Mexico City, FD', 'es': u('Ciudad de M\u00e9xico, CDMX')},
  '55112489':{'en': 'Guarulhos - SP', 'pt': 'Guarulhos - SP'},
  '497274':{'de': 'Germersheim', 'en': 'Germersheim'},
  '4938876':{'de': 'Roggendorf', 'en': 'Roggendorf'},
  '4938874':{'de': u('L\u00fctzow'), 'en': u('L\u00fctzow')},
  '4938875':{'de': 'Schlagsdorf bei Gadebusch', 'en': 'Schlagsdorf bei Gadebusch'},
  '4938872':{'de': 'Rehna', 'en': 'Rehna'},
  '4938873':{'de': 'Carlow', 'en': 'Carlow'},
```

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data6.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data6.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data7.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data7.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data8.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data8.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/data9.py` & `phonenumbers-8.9.9/phonenumbers/geodata/data9.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/geodata/locale.py` & `phonenumbers-8.9.9/phonenumbers/geodata/locale.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/phonemetadata.py` & `phonenumbers-8.9.9/phonenumbers/phonemetadata.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/phonenumber.py` & `phonenumbers-8.9.9/phonenumbers/phonenumber.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/phonenumbermatcher.py` & `phonenumbers-8.9.9/phonenumbers/phonenumbermatcher.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/phonenumberutil.py` & `phonenumbers-8.9.9/phonenumbers/phonenumberutil.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/prefix.py` & `phonenumbers-8.9.9/phonenumbers/prefix.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/re_util.py` & `phonenumbers-8.9.9/phonenumbers/re_util.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/__init__.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AC.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AD.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AD.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AE.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AF.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AG.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AI.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AL.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CH.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-"""Auto-generated file, do not edit by hand. AL metadata"""
+"""Auto-generated file, do not edit by hand. CH metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_AL = PhoneMetadata(id='AL', country_code=None, international_prefix=None,
-    general_desc=PhoneNumberDesc(national_number_pattern='[15]\\d{2,5}', possible_length=(3, 5, 6)),
-    toll_free=PhoneNumberDesc(national_number_pattern='1(?:3[15]|41|16\\d{3})', example_number='116000', possible_length=(3, 6)),
-    premium_rate=PhoneNumberDesc(national_number_pattern='5\\d{4}', example_number='50123', possible_length=(5,)),
-    emergency=PhoneNumberDesc(national_number_pattern='1(?:12|2[7-9])', example_number='129', possible_length=(3,)),
-    short_code=PhoneNumberDesc(national_number_pattern='1(?:1(?:\\d|6(?:000|1(?:06|11|23))|8\\d{2})|2[2-9]|[349]\\d|65\\d|89[12])|5\\d{4}', example_number='129', possible_length=(3, 5, 6)),
-    carrier_specific=PhoneNumberDesc(national_number_pattern='123', example_number='123', possible_length=(3,)),
-    sms_services=PhoneNumberDesc(national_number_pattern='131|5\\d{4}', example_number='51234', possible_length=(3, 5)),
+PHONE_METADATA_CH = PhoneMetadata(id='CH', country_code=None, international_prefix=None,
+    general_desc=PhoneNumberDesc(national_number_pattern='[1-9]\\d{2,5}', possible_length=(3, 4, 5, 6)),
+    toll_free=PhoneNumberDesc(national_number_pattern='1(?:16\\d{3}|47)|5200', example_number='116000', possible_length=(3, 4, 6)),
+    premium_rate=PhoneNumberDesc(national_number_pattern='1(?:145|8\\d{2})|543|83111', example_number='543', possible_length=(3, 4, 5)),
+    emergency=PhoneNumberDesc(national_number_pattern='1(?:1[278]|44)', example_number='112', possible_length=(3,)),
+    short_code=PhoneNumberDesc(national_number_pattern='1(?:0[78]\\d{2}|1(?:[278]|45|6(?:000|111))|4(?:[03457]|1[45])|6(?:00|[1-46])|8(?:02|1[189]|50|7|8[08]|99))|[2-9]\\d{2,4}', example_number='147', possible_length=(3, 4, 5, 6)),
+    standard_rate=PhoneNumberDesc(national_number_pattern='1(?:4(?:[035]|1\\d)|6\\d{1,2})', example_number='1600', possible_length=(3, 4)),
+    carrier_specific=PhoneNumberDesc(national_number_pattern='5(?:200|35)', example_number='535', possible_length=(3, 4)),
+    sms_services=PhoneNumberDesc(national_number_pattern='[2-9]\\d{2,4}', example_number='600', possible_length=(3, 4, 5)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AM.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AO.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AR.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AR.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,10 +2,10 @@
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
 PHONE_METADATA_AR = PhoneMetadata(id='AR', country_code=None, international_prefix=None,
     general_desc=PhoneNumberDesc(national_number_pattern='[01389]\\d{1,4}', possible_length=(2, 3, 4, 5)),
     toll_free=PhoneNumberDesc(national_number_pattern='[09]\\d{2}|1(?:[02-9]\\d?|1[0-24-9]?)', example_number='111', possible_length=(2, 3)),
     emergency=PhoneNumberDesc(national_number_pattern='10[017]|911', example_number='101', possible_length=(3,)),
     short_code=PhoneNumberDesc(national_number_pattern='000|1(?:0[0-35-7]|1[02-5]|2[15]|9)|3372|89338|911', example_number='121', possible_length=(2, 3, 4, 5)),
-    carrier_specific=PhoneNumberDesc(national_number_pattern='89338', example_number='89338', possible_length=(3, 5)),
+    carrier_specific=PhoneNumberDesc(national_number_pattern='89338', example_number='89338', possible_length=(5,)),
     sms_services=PhoneNumberDesc(national_number_pattern='3372|89338', example_number='3372', possible_length=(4, 5)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AS.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AT.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AU.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AW.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AX.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AX.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_AZ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BA.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BB.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BB.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BD.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BD.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BE.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BF.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BG.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BH.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BI.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BJ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BJ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BL.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BM.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BN.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BO.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BQ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BQ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BR.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BS.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BT.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BW.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BY.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_BZ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_BZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CA.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CC.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CD.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CD.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CF.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CG.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CH.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_IS.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-"""Auto-generated file, do not edit by hand. CH metadata"""
+"""Auto-generated file, do not edit by hand. IS metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_CH = PhoneMetadata(id='CH', country_code=None, international_prefix=None,
-    general_desc=PhoneNumberDesc(national_number_pattern='[1-9]\\d{2,5}', possible_length=(3, 4, 5, 6)),
-    toll_free=PhoneNumberDesc(national_number_pattern='1(?:16\\d{3}|47)|5200', example_number='116000', possible_length=(3, 4, 6)),
-    premium_rate=PhoneNumberDesc(national_number_pattern='1(?:145|8\\d{2})|543|83111', example_number='543', possible_length=(3, 4, 5)),
-    emergency=PhoneNumberDesc(national_number_pattern='1(?:1[278]|44)', example_number='112', possible_length=(3,)),
-    short_code=PhoneNumberDesc(national_number_pattern='1(?:0[78]\\d{2}|1(?:[278]|45|6(?:000|111))|4(?:[03457]|1[45])|6(?:00|[1-46])|8(?:02|1[189]|50|7|8[08]|99))|[2-9]\\d{2,4}', example_number='147', possible_length=(3, 4, 5, 6)),
-    standard_rate=PhoneNumberDesc(national_number_pattern='1(?:4(?:[035]|1\\d)|6\\d{1,2})', example_number='1600', possible_length=(3, 4)),
-    carrier_specific=PhoneNumberDesc(national_number_pattern='5(?:200|35)', example_number='535', possible_length=(3, 4)),
-    sms_services=PhoneNumberDesc(national_number_pattern='[2-9]\\d{2,4}', example_number='600', possible_length=(3, 4, 5)),
+PHONE_METADATA_IS = PhoneMetadata(id='IS', country_code=None, international_prefix=None,
+    general_desc=PhoneNumberDesc(national_number_pattern='1\\d{2,5}', possible_length=(3, 4, 6)),
+    toll_free=PhoneNumberDesc(national_number_pattern='1717', example_number='1717', possible_length=(4,)),
+    emergency=PhoneNumberDesc(national_number_pattern='112', example_number='112', possible_length=(3,)),
+    short_code=PhoneNumberDesc(national_number_pattern='1(?:1(?:[28]|6(?:1(?:23|16)))|4(?:00|1[145]|4[0146])|55|7(?:00|17|7[07-9])|8(?:[02]0|1[16-9]|88)|900)', example_number='112', possible_length=(3, 4, 6)),
+    carrier_specific=PhoneNumberDesc(national_number_pattern='14(?:00|41)', example_number='1441', possible_length=(4,)),
+    sms_services=PhoneNumberDesc(national_number_pattern='1(?:415|900)', example_number='1415', possible_length=(4,)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CI.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CK.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CL.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CM.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CN.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CO.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CR.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CU.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CV.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CV.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CW.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CX.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CX.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CY.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_CZ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_CZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_DE.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_DE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_DJ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_DJ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_DK.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_DK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_DM.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_DM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_DO.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_DO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_DZ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_DZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_EC.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_EC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_EE.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_EE.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Auto-generated file, do not edit by hand. EE metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
 PHONE_METADATA_EE = PhoneMetadata(id='EE', country_code=None, international_prefix=None,
     general_desc=PhoneNumberDesc(national_number_pattern='1\\d{2,5}', possible_length=(3, 4, 5, 6)),
     toll_free=PhoneNumberDesc(national_number_pattern='1(?:1(?:[02]|6(?:000|111))|2(?:0(?:16|5)|28|55[47])|3(?:014|24|3(?:21|5)|660)|492|5(?:1[03]|410|501|977)|6(?:112|333|644)|7(?:012|127|89)|8(?:10|8[57])|9(?:0(?:[134]|90)|14))', example_number='116000', possible_length=(3, 4, 5, 6)),
-    premium_rate=PhoneNumberDesc(national_number_pattern='1(?:18(?:[12458]|00)|2(?:0(?:[02-46-8]|1[0-36])|1(?:[0-4]|6[06])|2(?:[0-4]|5[25])|[367]|4(?:0[04]|[12]|4[24]|54)55[12457])|3(?:0(?:[02]|1[13578]|3[356])|1[1347]|2[02-5]|3(?:[01347]|2[023]|88)|4(?:[35]|4[34])|5(?:3[134]|5[035])|666)|4(?:2(?:00|4)|4(?:0[01358]|1[024]|50|7)|900)|5(?:0[0-35]|1(?:[1267]|5[0-7]|82)|2(?:[014-6]|22)|330|4(?:[35]|44)|5(?:00|[1-69])|9(?:[159]|[38]0|77))|6(?:1(?:00|1[19]|[356-9])|2(?:2[26]|[68])|3(?:22|36|6[36])|5|6(?:[0-359]|6[0-26])|7(?:00|55|7|8[89])|9(?:00|1|69))|7(?:0(?:[023]|1[0578])|1(?:00|2[034]|[4-9])|2(?:[07]|20|44)|7(?:[0-57]|9[79])|8(?:0[08]|2|8[0178])|9(?:00|97))|8(?:1[127]|8[1268]|9[269])|9(?:0(?:[02]|69|9[0269])|1[123689]|21))', example_number='1182', possible_length=(3, 4, 5)),
+    premium_rate=PhoneNumberDesc(national_number_pattern='1(?:18(?:[12458]|00)|2(?:0(?:[02-46-8]|1[0-36])|1(?:[0-4]|6[06])|2(?:[0-4]|5[25])|[367]|4(?:0[04]|[12]|4[24]|54)|55[12457])|3(?:0(?:[02]|1[13578]|3[356])|1[1347]|2[02-5]|3(?:[01347]|2[023]|88)|4(?:[35]|4[34])|5(?:3[134]|5[035])|666)|4(?:2(?:00|4)|4(?:0[01358]|1[024]|50|7)|900)|5(?:0[0-35]|1(?:[1267]|5[0-7]|82)|2(?:[014-6]|22)|330|4(?:[35]|44)|5(?:00|[1-69])|9(?:[159]|[38]0|77))|6(?:1(?:00|1[19]|[356-9])|2(?:2[26]|[68])|3(?:22|36|6[36])|5|6(?:[0-359]|6[0-26])|7(?:00|55|7|8[89])|9(?:00|1|69))|7(?:0(?:[023]|1[0578])|1(?:00|2[034]|[4-9])|2(?:[07]|20|44)|7(?:[0-57]|9[79])|8(?:0[08]|2|8[0178])|9(?:00|97))|8(?:1[127]|8[1268]|9[269])|9(?:0(?:[02]|69|9[0269])|1[123689]|21))', example_number='1182', possible_length=(3, 4, 5)),
     emergency=PhoneNumberDesc(national_number_pattern='11[02]', example_number='112', possible_length=(3,)),
     short_code=PhoneNumberDesc(national_number_pattern='1(?:1(?:[02-579]|6(?:000|111)|8(?:[09]\\d|[1-8]))|2(?:[0-245]\\d{1,2}|[36-9])|3(?:[0-6]\\d{1,2}|[7-9])|4(?:[1-489]\\d{1,2}|[05-7])|5(?:[0-59]\\d{1,2}|[6-8])|6(?:[05]|[1-46-9]\\d{1,2})|7(?:[0-27-9]\\d{1,2}|[3-6])|8(?:[02-7]|[189]\\d{1,2})|9(?:[0-2]\\d{1,2}|[3-9]))', example_number='115', possible_length=(3, 4, 5, 6)),
-    sms_services=PhoneNumberDesc(national_number_pattern='1(?:18[1258]2(?:0(?:1[036]|[46])|166|21|4(?:0[04]|1|5[47])|[67])|3(?:0(?:1[13-578]|2|3[56])|1[15]|2[045]|3(?:[13]|2[13])|43|5(?:00|3[34]|53))|44(?:0[0135]|14|50|7)|5(?:05|1(?:[12]|5[1246]|8[12])|2(?:[01]|22)|3(?:00|3[03])|4(?:15|5)|500|9(?:5|77|80))|6(?:1[35-8]|226|3(?:22|3[36]|66)|644|7(?:00|7|89)|9(?:00|69))|7(?:01[258]|1(?:00|[15])|2(?:44|7)|8(?:00|87|9))|8(?:1[128]|8[56]|9(?:[26]|77))|90(?:2|69|92))', example_number='13500', possible_length=(4, 5)),
+    sms_services=PhoneNumberDesc(national_number_pattern='1(?:18[1258]|2(?:0(?:1[036]|[46])|166|21|4(?:0[04]|1|5[47])|[67])|3(?:0(?:1[13-578]|2|3[56])|1[15]|2[045]|3(?:[13]|2[13])|43|5(?:00|3[34]|53))|44(?:0[0135]|14|50|7)|5(?:05|1(?:[12]|5[1246]|8[12])|2(?:[01]|22)|3(?:00|3[03])|4(?:15|5)|500|9(?:5|77|80))|6(?:1[35-8]|226|3(?:22|3[36]|66)|644|7(?:00|7|89)|9(?:00|69))|7(?:01[258]|1(?:00|[15])|2(?:44|7)|8(?:00|87|9))|8(?:1[128]|8[56]|9(?:[26]|77))|90(?:2|69|92))', example_number='13500', possible_length=(4, 5)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_EG.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_EG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_EH.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_EH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_ER.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_ER.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_ES.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_ES.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_ET.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_ET.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_FI.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_FI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_FJ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_FJ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_FK.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_FK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_FM.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_FM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_FO.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_FO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_FR.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_FR.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Auto-generated file, do not edit by hand. FR metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
 PHONE_METADATA_FR = PhoneMetadata(id='FR', country_code=None, international_prefix=None,
     general_desc=PhoneNumberDesc(national_number_pattern='1\\d{1,5}|[267]\\d{2,4}|3\\d{3,4}|[458]\\d{4}', possible_length=(2, 3, 4, 5, 6)),
     toll_free=PhoneNumberDesc(national_number_pattern='1(?:0(?:07|13)|1(?:[0459]|[68]\\d{3})|9[167])|224|3(?:[01]\\d{2}|3700)|740', example_number='3010', possible_length=(3, 4, 5, 6)),
-    premium_rate=PhoneNumberDesc(national_number_pattern='36665|[4-8]\\d{4}', example_number='42000', possible_length=(5, 6)),
+    premium_rate=PhoneNumberDesc(national_number_pattern='36665|[4-8]\\d{4}', example_number='42000', possible_length=(5,)),
     emergency=PhoneNumberDesc(national_number_pattern='1(?:[578]|12)', example_number='112', possible_length=(2, 3)),
     short_code=PhoneNumberDesc(national_number_pattern='1(?:0\\d{2}|1(?:[02459]|6(?:000|111)|8\\d{3})|9[167]|[578])|2(?:0(?:000|20)|24)|3\\d{3,4}|6(?:1[14]|34|\\d{4})|7(?:0[06]|22|40|\\d{4})|[458]\\d{4}', example_number='1010', possible_length=(2, 3, 4, 5, 6)),
     standard_rate=PhoneNumberDesc(national_number_pattern='10(?:14|2[23]|34|6[14]|99)|2020|3(?:646|9[07]0)|6(?:1[14]|34)|70[06]', example_number='1023', possible_length=(3, 4)),
     carrier_specific=PhoneNumberDesc(national_number_pattern='118777|2(?:0(?:000|20)|24)|6(?:1[14]|34)|7\\d{2}', example_number='118777', possible_length=(3, 4, 5, 6)),
     sms_services=PhoneNumberDesc(national_number_pattern='(?:114|[3-8]\\d{4})', example_number='33700', possible_length=(3, 5)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GA.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GB.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GB.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GD.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GD.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GE.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GF.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GG.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GH.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GI.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GL.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GM.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GN.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GP.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GP.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GR.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GT.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GU.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GW.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_GY.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_GY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_HK.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_HK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_HN.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_HN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_HR.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_HR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_HT.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_HT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_HU.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_HU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_ID.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_ID.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_IE.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_IE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_IL.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_IL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_IM.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_IM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_IN.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_IN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_IQ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_IQ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_IR.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_IR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_IS.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_LV.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-"""Auto-generated file, do not edit by hand. IS metadata"""
+"""Auto-generated file, do not edit by hand. LV metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_IS = PhoneMetadata(id='IS', country_code=None, international_prefix=None,
-    general_desc=PhoneNumberDesc(national_number_pattern='1\\d{2,5}', possible_length=(3, 4, 6)),
-    toll_free=PhoneNumberDesc(national_number_pattern='1717', example_number='1717', possible_length=(4,)),
-    emergency=PhoneNumberDesc(national_number_pattern='112', example_number='112', possible_length=(3,)),
-    short_code=PhoneNumberDesc(national_number_pattern='1(?:1(?:[28]|6(?:1(?:23|16)))|4(?:00|1[145]|4[0146])|55|7(?:00|17|7[07-9])|8(?:[02]0|1[16-9]|88)|900)', example_number='112', possible_length=(3, 4, 6)),
-    carrier_specific=PhoneNumberDesc(national_number_pattern='14(?:00|41)', example_number='1441', possible_length=(4,)),
-    sms_services=PhoneNumberDesc(national_number_pattern='1(?:415|900)', example_number='1415', possible_length=(4,)),
+PHONE_METADATA_LV = PhoneMetadata(id='LV', country_code=None, international_prefix=None,
+    general_desc=PhoneNumberDesc(national_number_pattern='0\\d|1\\d{2,6}|8\\d{3,4}', possible_length=(2, 3, 4, 5, 6)),
+    toll_free=PhoneNumberDesc(national_number_pattern='116\\d{3}', example_number='116000', possible_length=(6,)),
+    premium_rate=PhoneNumberDesc(national_number_pattern='1180|8(?:2\\d{3}|[89]\\d{2})', example_number='1180', possible_length=(4, 5)),
+    emergency=PhoneNumberDesc(national_number_pattern='0[123]|11[023]', example_number='112', possible_length=(2, 3)),
+    short_code=PhoneNumberDesc(national_number_pattern='0[1-4]|1(?:1(?:[02-4]|6(?:000|111)|8[0189])|55|655|77)|821[57]4', example_number='112', possible_length=(2, 3, 4, 5, 6)),
+    standard_rate=PhoneNumberDesc(national_number_pattern='1181', example_number='1181', possible_length=(4,)),
+    carrier_specific=PhoneNumberDesc(national_number_pattern='16\\d{2}', example_number='1655', possible_length=(4,)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_IT.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_IT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_JE.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_JE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_JM.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_JM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_JO.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_JO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_JP.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_JP.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_KE.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_KE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_KG.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_KG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_KH.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_KH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_KI.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_KI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_KM.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_KM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_KN.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_KN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_KP.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_KP.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_KR.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_KR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_KW.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_KW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_KY.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_KY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_KZ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_KZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_LA.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_LA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_LB.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_LB.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_LC.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_LC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_LI.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_LI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_LK.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_LK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_LR.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_LR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_LS.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_LS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_LT.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_LT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_LU.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_LU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_LV.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_ZA.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-"""Auto-generated file, do not edit by hand. LV metadata"""
+"""Auto-generated file, do not edit by hand. ZA metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_LV = PhoneMetadata(id='LV', country_code=None, international_prefix=None,
-    general_desc=PhoneNumberDesc(national_number_pattern='0\\d|1\\d{2,6}|8\\d{3,4}', possible_length=(2, 3, 4, 5, 6)),
-    toll_free=PhoneNumberDesc(national_number_pattern='116\\d{3}', example_number='116000', possible_length=(6,)),
-    premium_rate=PhoneNumberDesc(national_number_pattern='1180|8(?:2\\d{3}|[89]\\d{2})', example_number='1180', possible_length=(4, 5)),
-    emergency=PhoneNumberDesc(national_number_pattern='0[123]|11[023]', example_number='112', possible_length=(2, 3)),
-    short_code=PhoneNumberDesc(national_number_pattern='0[1-4]|1(?:1(?:[02-4]|6(?:000|111)|8[0189])|55|655|77)|821[57]4', example_number='112', possible_length=(2, 3, 4, 5, 6)),
-    standard_rate=PhoneNumberDesc(national_number_pattern='1181', example_number='1181', possible_length=(4,)),
-    carrier_specific=PhoneNumberDesc(national_number_pattern='16\\d{2}', example_number='1655', possible_length=(4,)),
+PHONE_METADATA_ZA = PhoneMetadata(id='ZA', country_code=None, international_prefix=None,
+    general_desc=PhoneNumberDesc(national_number_pattern='[134]\\d{2,4}', possible_length=(3, 4, 5)),
+    premium_rate=PhoneNumberDesc(national_number_pattern='41(?:348|851)', example_number='41851', possible_length=(5,)),
+    emergency=PhoneNumberDesc(national_number_pattern='1(?:0(?:1(?:11|77))|12)', example_number='10111', possible_length=(3, 5)),
+    short_code=PhoneNumberDesc(national_number_pattern='1(?:0(?:1(?:11|77)|20|7)|1[12]|77(?:3[237]|[45]7|6[279]|9[26]))|[34]\\d{4}', example_number='10111', possible_length=(3, 4, 5)),
+    standard_rate=PhoneNumberDesc(national_number_pattern='3(?:078[23]|7(?:064|567)|8126)|4(?:2699|3(?:699|94[16])|7751|8837)', example_number='47751', possible_length=(5,)),
+    carrier_specific=PhoneNumberDesc(national_number_pattern='111', example_number='111', possible_length=(3,)),
+    sms_services=PhoneNumberDesc(national_number_pattern='[34]\\d{4}', example_number='47751', possible_length=(5,)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_LY.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_LY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MA.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MC.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MD.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MD.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_ME.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_ME.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MF.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MG.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MH.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MK.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_ML.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_ML.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MM.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MN.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MO.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MP.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MP.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MQ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MQ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MR.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MS.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MT.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MU.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MV.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MV.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MW.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MX.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MX.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MY.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_MZ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_MZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_NA.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_NA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_NC.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_NC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_NE.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_NE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_NF.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_NF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_NG.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_NG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_NI.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_NI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_NL.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_NL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_NO.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_NO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_NP.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_NP.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_NR.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_NR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_NU.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SZ.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Auto-generated file, do not edit by hand. NU metadata"""
+"""Auto-generated file, do not edit by hand. SZ metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_NU = PhoneMetadata(id='NU', country_code=None, international_prefix=None,
+PHONE_METADATA_SZ = PhoneMetadata(id='SZ', country_code=None, international_prefix=None,
     general_desc=PhoneNumberDesc(national_number_pattern='9\\d{2}', possible_length=(3,)),
     emergency=PhoneNumberDesc(national_number_pattern='999', example_number='999', possible_length=(3,)),
     short_code=PhoneNumberDesc(national_number_pattern='999', example_number='999', possible_length=(3,)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_NZ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_NZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_OM.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_OM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_PA.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_PH.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Auto-generated file, do not edit by hand. PA metadata"""
+"""Auto-generated file, do not edit by hand. PH metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_PA = PhoneMetadata(id='PA', country_code=None, international_prefix=None,
+PHONE_METADATA_PH = PhoneMetadata(id='PH', country_code=None, international_prefix=None,
     general_desc=PhoneNumberDesc(national_number_pattern='[19]\\d{2}', possible_length=(3,)),
-    emergency=PhoneNumberDesc(national_number_pattern='911', example_number='911', possible_length=(3,)),
-    short_code=PhoneNumberDesc(national_number_pattern='10[2-4]|911', example_number='102', possible_length=(3,)),
+    emergency=PhoneNumberDesc(national_number_pattern='11[27]|911', example_number='117', possible_length=(3,)),
+    short_code=PhoneNumberDesc(national_number_pattern='11[27]|911', example_number='112', possible_length=(3,)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_PE.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_PE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_PF.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_PF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_PG.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_PG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_PH.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_VU.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Auto-generated file, do not edit by hand. PH metadata"""
+"""Auto-generated file, do not edit by hand. VU metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_PH = PhoneMetadata(id='PH', country_code=None, international_prefix=None,
-    general_desc=PhoneNumberDesc(national_number_pattern='[19]\\d{2}', possible_length=(3,)),
-    emergency=PhoneNumberDesc(national_number_pattern='11[27]|911', example_number='117', possible_length=(3,)),
-    short_code=PhoneNumberDesc(national_number_pattern='11[27]|911', example_number='112', possible_length=(3,)),
+PHONE_METADATA_VU = PhoneMetadata(id='VU', country_code=None, international_prefix=None,
+    general_desc=PhoneNumberDesc(national_number_pattern='1\\d{2}', possible_length=(3,)),
+    emergency=PhoneNumberDesc(national_number_pattern='112', example_number='112', possible_length=(3,)),
+    short_code=PhoneNumberDesc(national_number_pattern='112', example_number='112', possible_length=(3,)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_PK.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_PK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_PL.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_PL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_PM.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_PM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_PR.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_PR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_PS.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_PS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_PT.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_PT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_PW.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_PW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_PY.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_PY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_QA.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_QA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_RE.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_RE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_RO.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_RO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_RS.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_RS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_RU.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_RU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_RW.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_RW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SA.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SB.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SB.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SC.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SD.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SD.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SE.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SG.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SH.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SI.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SI.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SJ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SJ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SK.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SL.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SM.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SN.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SO.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SR.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_ST.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_ST.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SV.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SV.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SX.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SX.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SY.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_SY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_SZ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_UG.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Auto-generated file, do not edit by hand. SZ metadata"""
+"""Auto-generated file, do not edit by hand. UG metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_SZ = PhoneMetadata(id='SZ', country_code=None, international_prefix=None,
+PHONE_METADATA_UG = PhoneMetadata(id='UG', country_code=None, international_prefix=None,
     general_desc=PhoneNumberDesc(national_number_pattern='9\\d{2}', possible_length=(3,)),
     emergency=PhoneNumberDesc(national_number_pattern='999', example_number='999', possible_length=(3,)),
     short_code=PhoneNumberDesc(national_number_pattern='999', example_number='999', possible_length=(3,)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_TC.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_TC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_TD.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_TD.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_TG.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_TG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_TH.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_TH.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_TJ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_TJ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_TL.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_TL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_TM.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_TM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_TN.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_TN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_TO.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_TO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_TR.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_TR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_TT.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_TT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_TV.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_TV.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_TW.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_TW.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_TZ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_TZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_UA.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_UA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_UG.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_VI.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Auto-generated file, do not edit by hand. UG metadata"""
+"""Auto-generated file, do not edit by hand. VI metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_UG = PhoneMetadata(id='UG', country_code=None, international_prefix=None,
+PHONE_METADATA_VI = PhoneMetadata(id='VI', country_code=None, international_prefix=None,
     general_desc=PhoneNumberDesc(national_number_pattern='9\\d{2}', possible_length=(3,)),
-    emergency=PhoneNumberDesc(national_number_pattern='999', example_number='999', possible_length=(3,)),
-    short_code=PhoneNumberDesc(national_number_pattern='999', example_number='999', possible_length=(3,)),
+    emergency=PhoneNumberDesc(national_number_pattern='911', example_number='911', possible_length=(3,)),
+    short_code=PhoneNumberDesc(national_number_pattern='911', example_number='911', possible_length=(3,)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_US.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_US.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_UY.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_UY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_UZ.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_UZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_VA.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_VA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_VC.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_VC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_VE.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_VE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_VG.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_VG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_VI.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_YE.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Auto-generated file, do not edit by hand. VI metadata"""
+"""Auto-generated file, do not edit by hand. YE metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_VI = PhoneMetadata(id='VI', country_code=None, international_prefix=None,
-    general_desc=PhoneNumberDesc(national_number_pattern='9\\d{2}', possible_length=(3,)),
-    emergency=PhoneNumberDesc(national_number_pattern='911', example_number='911', possible_length=(3,)),
-    short_code=PhoneNumberDesc(national_number_pattern='911', example_number='911', possible_length=(3,)),
+PHONE_METADATA_YE = PhoneMetadata(id='YE', country_code=None, international_prefix=None,
+    general_desc=PhoneNumberDesc(national_number_pattern='1\\d{2}', possible_length=(3,)),
+    emergency=PhoneNumberDesc(national_number_pattern='19[1459]', example_number='191', possible_length=(3,)),
+    short_code=PhoneNumberDesc(national_number_pattern='19[1459]', example_number='191', possible_length=(3,)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_VN.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_VN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_VU.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_NU.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""Auto-generated file, do not edit by hand. VU metadata"""
+"""Auto-generated file, do not edit by hand. NU metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_VU = PhoneMetadata(id='VU', country_code=None, international_prefix=None,
-    general_desc=PhoneNumberDesc(national_number_pattern='1\\d{2}', possible_length=(3,)),
-    emergency=PhoneNumberDesc(national_number_pattern='112', example_number='112', possible_length=(3,)),
-    short_code=PhoneNumberDesc(national_number_pattern='112', example_number='112', possible_length=(3,)),
+PHONE_METADATA_NU = PhoneMetadata(id='NU', country_code=None, international_prefix=None,
+    general_desc=PhoneNumberDesc(national_number_pattern='[019]\\d{2}', possible_length=(3,)),
+    emergency=PhoneNumberDesc(national_number_pattern='999', example_number='999', possible_length=(3,)),
+    short_code=PhoneNumberDesc(national_number_pattern='01[05]|101|999', example_number='999', possible_length=(3,)),
+    carrier_specific=PhoneNumberDesc(national_number_pattern='010', example_number='010', possible_length=(3,)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_WF.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_WF.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_WS.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_WS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_XK.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_XK.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_YE.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_ZM.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Auto-generated file, do not edit by hand. YE metadata"""
+"""Auto-generated file, do not edit by hand. ZM metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_YE = PhoneMetadata(id='YE', country_code=None, international_prefix=None,
-    general_desc=PhoneNumberDesc(national_number_pattern='1\\d{2}', possible_length=(3,)),
-    emergency=PhoneNumberDesc(national_number_pattern='19[1459]', example_number='191', possible_length=(3,)),
-    short_code=PhoneNumberDesc(national_number_pattern='19[1459]', example_number='191', possible_length=(3,)),
+PHONE_METADATA_ZM = PhoneMetadata(id='ZM', country_code=None, international_prefix=None,
+    general_desc=PhoneNumberDesc(national_number_pattern='[19]\\d{2}', possible_length=(3,)),
+    emergency=PhoneNumberDesc(national_number_pattern='(?:112|99[139])', example_number='999', possible_length=(3,)),
+    short_code=PhoneNumberDesc(national_number_pattern='(?:112|99[139])', example_number='999', possible_length=(3,)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_YT.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_YT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_ZA.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_AL.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-"""Auto-generated file, do not edit by hand. ZA metadata"""
+"""Auto-generated file, do not edit by hand. AL metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_ZA = PhoneMetadata(id='ZA', country_code=None, international_prefix=None,
-    general_desc=PhoneNumberDesc(national_number_pattern='[134]\\d{2,4}', possible_length=(3, 4, 5)),
-    premium_rate=PhoneNumberDesc(national_number_pattern='41(?:348|851)', example_number='41851', possible_length=(5,)),
-    emergency=PhoneNumberDesc(national_number_pattern='1(?:0(?:1(?:11|77))|12)', example_number='10111', possible_length=(3, 5)),
-    short_code=PhoneNumberDesc(national_number_pattern='1(?:0(?:1(?:11|77)|20|7)|1[12]|77(?:3[237]|[45]7|6[279]|9[26]))|[34]\\d{4}', example_number='10111', possible_length=(3, 4, 5)),
-    standard_rate=PhoneNumberDesc(national_number_pattern='3(?:078[23]|7(?:064|567)|8126)|4(?:2699|3(?:699|94[16])|7751|8837)', example_number='47751', possible_length=(5,)),
-    carrier_specific=PhoneNumberDesc(national_number_pattern='111', example_number='111', possible_length=(3,)),
-    sms_services=PhoneNumberDesc(national_number_pattern='[34]\\d{4}', example_number='47751', possible_length=(5,)),
+PHONE_METADATA_AL = PhoneMetadata(id='AL', country_code=None, international_prefix=None,
+    general_desc=PhoneNumberDesc(national_number_pattern='[15]\\d{2,5}', possible_length=(3, 4, 5, 6)),
+    toll_free=PhoneNumberDesc(national_number_pattern='1(?:3[15]|41|16\\d{3})', example_number='116000', possible_length=(3, 6)),
+    premium_rate=PhoneNumberDesc(national_number_pattern='5\\d{4}', example_number='50123', possible_length=(5,)),
+    emergency=PhoneNumberDesc(national_number_pattern='1(?:12|2[7-9])', example_number='129', possible_length=(3,)),
+    short_code=PhoneNumberDesc(national_number_pattern='1(?:1(?:\\d|6(?:000|1(?:06|11|23))|8\\d{2})|2[2-9]|[349]\\d|65\\d|89[12])|5\\d{4}', example_number='129', possible_length=(3, 4, 5, 6)),
+    carrier_specific=PhoneNumberDesc(national_number_pattern='123', example_number='123', possible_length=(3,)),
+    sms_services=PhoneNumberDesc(national_number_pattern='131|5\\d{4}', example_number='51234', possible_length=(3, 5)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_ZM.py` & `phonenumbers-8.9.9/phonenumbers/data/region_NU.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Auto-generated file, do not edit by hand. ZM metadata"""
+"""Auto-generated file, do not edit by hand. NU metadata"""
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
-PHONE_METADATA_ZM = PhoneMetadata(id='ZM', country_code=None, international_prefix=None,
-    general_desc=PhoneNumberDesc(national_number_pattern='[19]\\d{2}', possible_length=(3,)),
-    emergency=PhoneNumberDesc(national_number_pattern='(?:112|99[139])', example_number='999', possible_length=(3,)),
-    short_code=PhoneNumberDesc(national_number_pattern='(?:112|99[139])', example_number='999', possible_length=(3,)),
-    short_data=True)
+PHONE_METADATA_NU = PhoneMetadata(id='NU', country_code=683, international_prefix='00',
+    general_desc=PhoneNumberDesc(national_number_pattern='[478]\\d{3,7}', possible_length=(4, 7)),
+    fixed_line=PhoneNumberDesc(national_number_pattern='[47]\\d{3}', example_number='7012', possible_length=(4,)),
+    mobile=PhoneNumberDesc(national_number_pattern='888[4-9]\\d{3}', example_number='8884012', possible_length=(7,)),
+    number_format=[NumberFormat(pattern='(\\d{3})(\\d{4})', format='\\1 \\2', leading_digits_pattern=['888'])])
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortdata/region_ZW.py` & `phonenumbers-8.9.9/phonenumbers/shortdata/region_ZW.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,10 +2,10 @@
 from ..phonemetadata import NumberFormat, PhoneNumberDesc, PhoneMetadata
 
 PHONE_METADATA_ZW = PhoneMetadata(id='ZW', country_code=None, international_prefix=None,
     general_desc=PhoneNumberDesc(national_number_pattern='[139]\\d{2,4}', possible_length=(3, 5)),
     toll_free=PhoneNumberDesc(national_number_pattern='9(?:5[023]|61)', example_number='961', possible_length=(3,)),
     premium_rate=PhoneNumberDesc(national_number_pattern='3\\d{4}', example_number='30123', possible_length=(5,)),
     emergency=PhoneNumberDesc(national_number_pattern='(?:11[24]|99[3-59])', example_number='999', possible_length=(3,)),
-    short_code=PhoneNumberDesc(national_number_pattern='11[2469]|9(?:5[023]|6[0-25]|9[3-59])', example_number='999', possible_length=(3, 5)),
+    short_code=PhoneNumberDesc(national_number_pattern='11[2469]|3\\d{4}|9(?:5[023]|6[0-25]|9[3-59])', example_number='999', possible_length=(3, 5)),
     carrier_specific=PhoneNumberDesc(national_number_pattern='(?:114|9(?:5[023]|6[0-25]))', example_number='114', possible_length=(3,)),
     short_data=True)
```

### Comparing `phonenumbers-8.9.8/phonenumbers/shortnumberinfo.py` & `phonenumbers-8.9.9/phonenumbers/shortnumberinfo.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/timezone.py` & `phonenumbers-8.9.9/phonenumbers/timezone.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/tzdata/__init__.py` & `phonenumbers-8.9.9/phonenumbers/tzdata/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/tzdata/data0.py` & `phonenumbers-8.9.9/phonenumbers/tzdata/data0.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,36 +32,34 @@
  '55813424':('America/Sao_Paulo',),
  '55813425':('America/Sao_Paulo',),
  '55813426':('America/Sao_Paulo',),
  '55813427':('America/Sao_Paulo',),
  '55813421':('America/Sao_Paulo',),
  '55813422':('America/Sao_Paulo',),
  '55813423':('America/Sao_Paulo',),
- '1684':('Pacific/Pago_Pago',),
  '1807737':('America/Winnipeg',),
  '961':('Asia/Beirut',),
  '962':('Asia/Amman',),
  '441779':('Europe/London',),
  '441778':('Europe/London',),
  '441777':('Europe/London',),
  '441776':('Europe/London',),
  '441775':('Europe/London',),
  '441773':('Europe/London',),
  '441772':('Europe/London',),
  '441771':('Europe/London',),
- '441770':('Europe/London',),
- '1250539':('America/Vancouver',),
- '1250537':('America/Vancouver',),
+ '55913617':('America/Sao_Paulo',),
+ '55813303':('America/Sao_Paulo',),
  '1775392':('America/Los_Angeles',),
  '1775391':('America/Los_Angeles',),
  '55913772':('America/Sao_Paulo',),
  '55913771':('America/Sao_Paulo',),
  '55913777':('America/Sao_Paulo',),
  '55913776':('America/Sao_Paulo',),
- '55913775':('America/Sao_Paulo',),
+ '55913803':('America/Sao_Paulo',),
  '55913774':('America/Sao_Paulo',),
  '55913809':('America/Sao_Paulo',),
  '52468':('America/Mexico_City',),
  '52469':('America/Mexico_City',),
  '52461':('America/Mexico_City',),
  '52462':('America/Mexico_City',),
  '52463':('America/Mexico_City',),
@@ -82,35 +80,29 @@
  '1308635':('America/Denver',),
  '441366':('Europe/London',),
  '441367':('Europe/London',),
  '1308630':('America/Denver',),
  '441361':('Europe/London',),
  '1308632':('America/Denver',),
  '1308633':('America/Denver',),
- '1906586':('America/New_York',),
- '1812466':('America/New_York',),
  '1812464':('America/Chicago',),
- '1812462':('America/New_York',),
- '1906273':('America/New_York',),
  '9765050':('Asia/Ulaanbaatar',),
  '1605348':('America/Denver',),
- '62368':('Asia/Makassar',),
  '55939965':('America/Sao_Paulo',),
  '1605341':('America/Denver',),
  '1605342':('America/Denver',),
  '1605343':('America/Denver',),
  '1605345':('America/Chicago',),
  '1605347':('America/Denver',),
- '1418476':('America/Toronto',),
  '1541868':('America/Los_Angeles',),
  '62816':('Asia/Jakarta',),
  '62552':('Asia/Makassar',),
- '62361':('Asia/Makassar',),
+ '62817':('Asia/Jakarta',),
  '1541863':('America/Los_Angeles',),
- '62362':('Asia/Makassar',),
+ '62814':('Asia/Jakarta',),
  '1541867':('America/Los_Angeles',),
  '441942':('Europe/London',),
  '441943':('Europe/London',),
  '441944':('Europe/London',),
  '441945':('Europe/London',),
  '441946':('Europe/London',),
  '441947':('Europe/London',),
@@ -118,39 +110,25 @@
  '441949':('Europe/London',),
  '62813':('Asia/Jakarta',),
  '62885':('Asia/Jakarta',),
  '62884':('Asia/Jakarta',),
  '62887':('Asia/Jakarta', 'Asia/Makassar'),
  '62886':('Asia/Jakarta',),
  '62881':('Asia/Jakarta',),
- '62366':('Asia/Makassar',),
+ '62810':('Asia/Jakarta',),
  '62883':('Asia/Jakarta',),
  '62882':('Asia/Jakarta',),
  '91':('Asia/Calcutta',),
  '90':('Europe/Istanbul',),
  '93':('Asia/Kabul',),
  '92':('Asia/Karachi',),
  '62889':('Asia/Jakarta',),
  '62888':('Asia/Jakarta',),
  '1423365':('America/New_York',),
- '55813226':('America/Sao_Paulo',),
- '1418548':('America/Toronto',),
- '1418549':('America/Toronto',),
- '1418542':('America/Toronto',),
- '1418543':('America/Toronto',),
- '1418547':('America/Toronto',),
- '1418544':('America/Toronto',),
- '1418545':('America/Toronto',),
- '1250881':('America/Vancouver',),
- '1250882':('America/Vancouver',),
- '1250885':('America/Vancouver',),
- '1250884':('America/Vancouver',),
- '1250886':('America/Vancouver',),
- '1250889':('America/Vancouver',),
- '1250888':('America/Vancouver',),
+ '1867536':('America/Vancouver',),
  '1208446':('America/Los_Angeles',),
  '1208440':('America/Denver',),
  '1208442':('America/Denver',),
  '1208443':('America/Los_Angeles',),
  '1208448':('America/Los_Angeles',),
  '644':('Pacific/Auckland',),
  '1541488':('America/Los_Angeles',),
@@ -159,114 +137,88 @@
  '1541481':('America/Los_Angeles',),
  '1541484':('America/Los_Angeles',),
  '1541485':('America/Los_Angeles',),
  '1219756':('America/Chicago',),
  '1208535':('America/Denver',),
  '1219558':('America/Chicago',),
  '1225':('America/Chicago',),
- '1785341':('America/Chicago',),
  '1224':('America/Chicago',),
- '1785346':('America/Chicago',),
  '1701437':('America/Chicago',),
- '55933534':('America/Sao_Paulo',),
- '1906875':('America/Chicago',),
+ '1220':('America/New_York',),
  '1850863':('America/Chicago',),
  '1850862':('America/Chicago',),
  '1850689':('America/Chicago',),
  '1850864':('America/Chicago',),
+ '1850867':('America/Chicago',),
  '1850866':('America/Chicago',),
  '1850685':('America/Chicago',),
  '1850684':('America/Chicago',),
  '1850687':('America/Chicago',),
- '1850681':('America/New_York',),
  '1850683':('America/Chicago',),
  '1850682':('America/Chicago',),
  '1228':('America/Chicago',),
- '62457':('Asia/Makassar',),
- '1812247':('America/New_York',),
- '1308995':('America/Chicago',),
- '1785969':('America/Chicago',),
- '55913617':('America/Sao_Paulo',),
- '441880':('Europe/London',),
- '1812254':('America/New_York',),
+ '441770':('Europe/London',),
  '1270495':('America/Chicago',),
- '1812256':('America/New_York',),
- '1812257':('America/New_York',),
  '4721':('Europe/Oslo',),
  '4723':('Europe/Oslo',),
  '4722':('Europe/Oslo',),
- '1250709':('America/Vancouver',),
- '1250707':('America/Vancouver',),
- '1250702':('America/Vancouver',),
- '1250703':('America/Vancouver',),
- '1250701':('America/Vancouver',),
  '1775250':('America/Los_Angeles',),
  '3906698':('Europe/Vatican',),
- '1906643':('America/New_York',),
  '521988':('America/Mexico_City',),
- '1906647':('America/New_York',),
  '521985':('America/Mexico_City',),
  '521984':('America/New_York',),
  '521987':('America/New_York',),
  '521986':('America/Mexico_City',),
  '521981':('America/Mexico_City',),
  '521983':('America/New_York',),
  '521982':('America/Mexico_City',),
  '1605598':('America/Chicago',),
  '1605594':('America/Chicago',),
  '1605593':('America/Denver',),
- '1620783':('America/Chicago',),
  '390985':('Europe/Rome',),
  '390984':('Europe/Rome',),
  '390983':('Europe/Rome',),
  '390982':('Europe/Rome',),
  '390981':('Europe/Rome',),
- '1574855':('America/New_York',),
  '390187':('Europe/Rome',),
  '390185':('Europe/Rome',),
  '390184':('Europe/Rome',),
  '390183':('Europe/Rome',),
  '390182':('Europe/Rome',),
- '1308468':('America/Chicago',),
  '1270251':('America/Chicago',),
  '1775829':('America/Los_Angeles',),
  '1775828':('America/Los_Angeles',),
  '1775825':('America/Los_Angeles',),
  '1775824':('America/Los_Angeles',),
  '1775827':('America/Los_Angeles',),
  '1270259':('America/Chicago',),
  '86421':('Asia/Shanghai',),
  '1775823':('America/Los_Angeles',),
- '55913803':('America/Sao_Paulo',),
+ '55913775':('America/Sao_Paulo',),
  '55913802':('America/Sao_Paulo',),
  '1769':('America/Chicago',),
  '1762':('America/New_York',),
  '1763':('America/Chicago',),
  '1760':('America/Los_Angeles',),
- '1418915':('America/Toronto',),
  '1767':('America/Dominica',),
  '1765':('America/New_York',),
  '55949966':('America/Sao_Paulo',),
  '1208875':('America/Los_Angeles',),
- '1418687':('America/Toronto',),
- '1418686':('America/Toronto',),
- '1208871':('America/Denver',),
+ '690':('Pacific/Fakaofo',),
+ '691':('Pacific/Kosrae', 'Pacific/Ponape', 'Pacific/Truk'),
+ '1418937':('America/Halifax',),
  '1208870':('America/Denver',),
- '1418683':('America/Toronto',),
- '1418682':('America/Toronto',),
- '1418689':('America/Toronto',),
- '1418688':('America/Toronto',),
- '1423821':('America/New_York',),
+ '1540':('America/New_York',),
+ '1208879':('America/Denver',),
+ '1208878':('America/Denver',),
+ '1548':('America/Toronto',),
  '1541298':('America/Los_Angeles',),
  '1541296':('America/Los_Angeles',),
- '1208398':('America/Denver',),
  '1541292':('America/Los_Angeles',),
- '62635':('Asia/Jakarta',),
  '62632':('Asia/Jakarta',),
- '62633':('Asia/Jakarta',),
  '1850473':('America/Chicago',),
  '1850470':('America/Chicago',),
  '1850471':('America/Chicago',),
  '1850476':('America/Chicago',),
  '1850477':('America/Chicago',),
  '1850474':('America/Chicago',),
  '1850475':('America/Chicago',),
@@ -275,34 +227,22 @@
  '1208305':('America/Los_Angeles',),
  '1208304':('America/Los_Angeles',),
  '1208302':('America/Denver',),
  '1208308':('America/Denver',),
  '52646':('America/Tijuana',),
  '52647':('America/Mazatlan',),
  '52648':('America/Mazatlan',),
- '521622':('America/Mazatlan',),
  '52649':('America/Mazatlan', 'America/Mexico_City'),
- '1785286':('America/Chicago',),
- '1785284':('America/Chicago',),
- '521623':('America/Mazatlan',),
- '1785282':('America/Chicago',),
+ '62639':('Asia/Jakarta',),
  '62515':('Asia/Jakarta',),
  '62513':('Asia/Jakarta',),
  '62512':('Asia/Makassar',),
- '34928':('Atlantic/Canary',),
- '1250551':('America/Vancouver',),
- '1250550':('America/Vancouver',),
- '55913638':('America/Sao_Paulo',),
- '1250554':('America/Vancouver',),
  '55913636':('America/Sao_Paulo',),
  '55913637':('America/Sao_Paulo',),
- '1250559':('America/Vancouver',),
- '1250558':('America/Vancouver',),
  '55913633':('America/Sao_Paulo',),
- '1620473':('America/Chicago',),
  '39015':('Europe/Rome',),
  '39010':('Europe/Rome',),
  '39011':('Europe/Rome',),
  '39019':('Europe/Rome',),
  '1775623':('America/Los_Angeles',),
  '1775622':('America/Los_Angeles',),
  '1775626':('America/Los_Angeles',),
@@ -315,52 +255,46 @@
  '250':('Africa/Kigali',),
  '251':('Africa/Addis_Ababa',),
  '256':('Africa/Kampala',),
  '257':('Africa/Bujumbura',),
  '254':('Africa/Nairobi',),
  '255':('Africa/Dar_es_Salaam',),
  '441360':('Europe/London',),
+ '1270535':('America/Chicago',),
  '1270534':('America/Chicago',),
  '441362':('Europe/London',),
  '441363':('Europe/London',),
  '1270538':('America/Chicago',),
- '1906253':('America/New_York',),
- '868068':('Asia/Shanghai',),
- '1208610':('America/Los_Angeles',),
- '1812443':('America/New_York',),
- '1812442':('America/New_York',),
- '1812446':('America/New_York',),
- '1812448':('America/New_York',),
+ '1208962':('America/Los_Angeles',),
  '1541842':('America/Los_Angeles',),
  '1541840':('America/Los_Angeles',),
  '1541846':('America/Los_Angeles',),
  '1541844':('America/Los_Angeles',),
  '1423697':('America/New_York',),
  '390864':('Europe/Rome',),
  '390865':('Europe/Rome',),
  '390861':('Europe/Rome',),
  '390862':('Europe/Rome',),
  '390863':('Europe/Rome',),
  '441928':('Europe/London',),
  '441929':('Europe/London',),
- '1606487':('America/New_York',),
  '441922':('Europe/London',),
  '441923':('Europe/London',),
  '441920':('Europe/London',),
  '441926':('Europe/London',),
  '441924':('Europe/London',),
  '441925':('Europe/London',),
  '1423434':('America/New_York',),
  '1423343':('America/New_York',),
  '1423346':('America/New_York',),
  '1423431':('America/New_York',),
  '1423344':('America/New_York',),
  '1423345':('America/New_York',),
  '1423349':('America/New_York',),
- '1423439':('America/New_York',),
+ '1907852':('America/Juneau',),
  '1605362':('America/Chicago',),
  '1605363':('America/Chicago',),
  '1605360':('America/Chicago',),
  '1605361':('America/Chicago',),
  '1605366':('America/Chicago',),
  '1605367':('America/Chicago',),
  '55814121':('America/Sao_Paulo',),
@@ -368,23 +302,19 @@
  '55814123':('America/Sao_Paulo',),
  '1208682':('America/Los_Angeles',),
  '1208683':('America/Los_Angeles',),
  '1208681':('America/Denver',),
  '1208686':('America/Los_Angeles',),
  '1208687':('America/Los_Angeles',),
  '1208684':('America/Denver',),
- '1606666':('America/New_York',),
- '1606663':('America/New_York',),
  '29991':('America/Godthab',),
- '1785776':('America/Chicago',),
  '29996':('America/Godthab',),
  '29997':('America/Thule',),
  '1812867':('America/Chicago',),
- '1541347':('America/Los_Angeles',),
- '1812865':('America/New_York',),
+ '29994':('America/Godthab',),
  '29995':('America/Godthab',),
  '1208468':('America/Denver',),
  '1208466':('America/Denver',),
  '1208467':('America/Denver',),
  '1208465':('America/Denver',),
  '1208462':('America/Denver',),
  '1208463':('America/Denver',),
@@ -397,110 +327,92 @@
  '441544':('Europe/London',),
  '441545':('Europe/London',),
  '441546':('Europe/London',),
  '441547':('Europe/London',),
  '441540':('Europe/London',),
  '441542':('Europe/London',),
  '441543':('Europe/London',),
- '1785368':('America/Chicago',),
  '1701452':('America/Chicago',),
  '1701456':('America/Denver',),
- '1785363':('America/Chicago',),
  '1701454':('America/Chicago',),
- '390445':('Europe/Rome',),
- '1785550':('America/Chicago',),
  '52836':('America/Mexico_City',),
  '52835':('America/Mexico_City',),
  '52834':('America/Mexico_City',),
  '52833':('America/Mexico_City',),
  '52832':('America/Mexico_City',),
  '52831':('America/Mexico_City',),
  '1270707':('America/Chicago',),
+ '1208573':('America/Denver',),
  '1219473':('America/Chicago',),
- '1785945':('America/Chicago',),
- '1323':('America/Los_Angeles',),
+ '1219472':('America/Chicago',),
  '1320':('America/Chicago',),
  '1709637':('America/St_Johns',),
- '1812277':('America/New_York',),
  '1709635':('America/St_Johns',),
  '1709634':('America/St_Johns',),
- '1812273':('America/New_York',),
  '1219477':('America/Chicago',),
  '1709639':('America/St_Johns',),
- '1812279':('America/New_York',),
+ '1219476':('America/Chicago',),
  '1208389':('America/Denver',),
  '1219474':('America/Chicago',),
- '1701361':('America/Chicago',),
  '1907283':('America/Juneau',),
- '1250768':('America/Vancouver',),
- '1250769':('America/Vancouver',),
- '1418328':('America/Toronto',),
  '52349':('America/Mexico_City',),
  '52348':('America/Mexico_City',),
  '52345':('America/Mexico_City',),
  '52344':('America/Mexico_City',),
- '1250762':('America/Vancouver',),
- '1250763':('America/Vancouver',),
- '1250764':('America/Vancouver',),
- '1250765':('America/Vancouver',),
- '1250766':('America/Vancouver',),
- '1418325':('America/Toronto',),
+ '52347':('America/Mexico_City',),
+ '52346':('America/Mexico_City',),
+ '52341':('America/Mexico_City',),
+ '52343':('America/Mexico_City',),
+ '52342':('America/Mexico_City',),
  '1208381':('America/Denver',),
- '55913321':('America/Sao_Paulo',),
- '55913322':('America/Sao_Paulo',),
+ '1701355':('America/Chicago',),
+ '1208577':('America/Denver',),
+ '1701356':('America/Chicago',),
  '55813363':('America/Sao_Paulo',),
  '55813362':('America/Sao_Paulo',),
  '55813361':('America/Sao_Paulo',),
  '55813366':('America/Sao_Paulo',),
  '52698':('America/Mazatlan',),
  '1701352':('America/Chicago',),
  '52697':('America/Mazatlan',),
- '141865':('America/Toronto',),
+ '52696':('America/Mazatlan',),
  '52695':('America/Mazatlan',),
  '52694':('America/Mazatlan',),
- '55813678':('America/Sao_Paulo',),
- '1785562':('America/Chicago',),
+ '521474':('America/Mexico_City',),
  '390474':('Europe/Rome',),
  '390473':('Europe/Rome',),
  '390472':('Europe/Rome',),
  '390471':('Europe/Rome',),
  '98':('Asia/Tehran',),
  '6238':('Asia/Makassar',),
  '6231':('Asia/Jakarta',),
  '62880':('Asia/Jakarta',),
  '7817':('Europe/Moscow',),
- '1418274':('America/Toronto',),
- '1606877':('America/New_York',),
- '1418276':('America/Toronto',),
- '1606874':('America/New_York',),
  '95':('Asia/Rangoon',),
- '1606878':('America/New_York',),
  '94':('Asia/Colombo',),
- '1250635':('America/Vancouver',),
+ '1701':('America/Denver', 'America/North_Dakota/Center'),
  '1702':('America/Los_Angeles',),
  '1703':('America/New_York',),
  '1704':('America/New_York',),
  '1705':('America/Toronto',),
  '1706':('America/New_York',),
  '1707':('America/Los_Angeles',),
  '1708':('America/Chicago',),
- '1709466':('America/St_Johns',),
+ '1709':('America/Puerto_Rico', 'America/St_Johns'),
  '1541729':('America/Los_Angeles',),
  '1541728':('America/Los_Angeles',),
  '1541726':('America/Los_Angeles',),
- '1606297':('America/New_York',),
- '1606298':('America/New_York',),
- '521648':('America/Mazatlan',),
- '1208898':('America/Denver',),
+ '1208899':('America/Denver',),
+ '521649':('America/Mazatlan',),
  '521646':('America/Tijuana',),
- '1418914':('America/Toronto',),
+ '521647':('America/Mazatlan', 'America/Tijuana'),
  '1208895':('America/Denver',),
  '521645':('America/Mazatlan',),
  '521642':('America/Mazatlan',),
- '1418662':('America/Toronto',),
+ '521643':('America/Mazatlan',),
  '1208891':('America/Denver',),
  '1208890':('America/Denver',),
  '34983':('Europe/Madrid',),
  '34982':('Europe/Madrid',),
  '34981':('Europe/Madrid',),
  '34980':('Europe/Madrid',),
  '34987':('Europe/Madrid',),
@@ -508,16 +420,14 @@
  '34985':('Europe/Madrid',),
  '34984':('Europe/Madrid',),
  '34988':('Europe/Madrid',),
  '5671':('America/Santiago',),
  '5672':('America/Santiago',),
  '5673':('America/Santiago',),
  '5675':('America/Santiago',),
- '55813416':('America/Sao_Paulo',),
- '1701400':('America/Chicago',),
  '521391':('America/Mexico_City',),
  '521392':('America/Mexico_City',),
  '521393':('America/Mexico_City',),
  '521394':('America/Mexico_City',),
  '521395':('America/Mexico_City',),
  '1850499':('America/Chicago',),
  '1850494':('America/Chicago',),
@@ -543,85 +453,73 @@
  '441487':('Europe/London',),
  '441733':('Europe/London',),
  '441732':('Europe/London',),
  '441730':('Europe/London',),
  '441737':('Europe/London',),
  '441736':('Europe/London',),
  '441738':('Europe/London',),
- '55913656':('America/Sao_Paulo',),
- '1250579':('America/Vancouver',),
- '1250578':('America/Vancouver',),
- '1250575':('America/Vancouver',),
- '1250574':('America/Vancouver',),
+ '55813281':('America/Sao_Paulo',),
  '55913658':('America/Sao_Paulo',),
- '1250573':('America/Vancouver',),
  '39039':('Europe/Rome',),
  '39035':('Europe/Rome',),
  '39030':('Europe/Rome',),
  '39031':('Europe/Rome',),
  '1907495':('America/Juneau',),
  '1775359':('America/Los_Angeles',),
- '1907490':('America/Juneau',),
+ '1775358':('America/Los_Angeles',),
  '1775356':('America/Los_Angeles',),
  '1775355':('America/Los_Angeles',),
  '1775354':('America/Los_Angeles',),
  '1775353':('America/Los_Angeles',),
  '1775352':('America/Los_Angeles',),
  '1775351':('America/Los_Angeles',),
  '238':('Atlantic/Cape_Verde',),
  '239':('Africa/Sao_Tome',),
  '55913739':('America/Sao_Paulo',),
  '55913738':('America/Sao_Paulo',),
  '234':('Africa/Lagos',),
  '235':('Africa/Ndjamena',),
  '236':('Africa/Bangui',),
- '237':('Africa/Douala',),
+ '55913734':('America/Sao_Paulo',),
  '230':('Indian/Mauritius',),
  '231':('Atlantic/Reykjavik',),
  '232':('Africa/Freetown',),
  '233':('Africa/Accra',),
  '62430':('Asia/Makassar',),
  '62431':('Asia/Makassar',),
- '1867536':('America/Vancouver',),
  '62924':('Asia/Jayapura',),
- '1785754':('America/Chicago',),
  '1907723':('America/Juneau',),
- '1308675':('America/Chicago',),
  '1907727':('America/Juneau',),
  '1907729':('America/Juneau',),
  '55813821':('America/Sao_Paulo',),
- '55813822':('America/Sao_Paulo',),
  '55813823':('America/Sao_Paulo',),
  '62923':('Asia/Jayapura',),
- '1574287':('America/New_York',),
- '1418788':('America/Toronto',),
  '62436':('Asia/Makassar',),
  '62921':('Asia/Jayapura',),
+ '1541653':('America/Los_Angeles',),
  '1812428':('America/Chicago',),
  '1812423':('America/Chicago',),
  '1812422':('America/Chicago',),
  '1812421':('America/Chicago',),
- '1812427':('America/New_York',),
  '1812426':('America/Chicago',),
  '1812425':('America/Chicago',),
  '1812424':('America/Chicago',),
- '1606464':('America/New_York',),
  '1757':('America/New_York',),
  '62338':('Asia/Jakarta',),
  '62333':('Asia/Jakarta',),
  '62332':('Asia/Jakarta',),
  '62331':('Asia/Jakarta',),
  '1907874':('America/Juneau',),
  '62335':('Asia/Jakarta',),
  '62334':('Asia/Jakarta',),
  '1754':('America/New_York',),
  '1605388':('America/Denver',),
  '55814108':('America/Sao_Paulo',),
  '55814109':('America/Sao_Paulo',),
- '1605384':('America/Chicago',),
+ '55814106':('America/Sao_Paulo',),
  '55814107':('America/Sao_Paulo',),
  '55814104':('America/Sao_Paulo',),
  '1605387':('America/Chicago',),
  '55814102':('America/Sao_Paulo',),
  '1605381':('America/Denver',),
  '55814100':('America/Sao_Paulo',),
  '55814101':('America/Sao_Paulo',),
@@ -632,174 +530,149 @@
  '1208660':('America/Los_Angeles',),
  '1208661':('America/Los_Angeles',),
  '441904':('Europe/London',),
  '441905':('Europe/London',),
  '441900':('Europe/London',),
  '441902':('Europe/London',),
  '441903':('Europe/London',),
- '1812847':('America/New_York',),
  '441908':('Europe/London',),
  '441909':('Europe/London',),
  '1812842':('America/Chicago',),
  '1208409':('America/Denver',),
  '1208401':('America/Denver',),
  '1208402':('America/Denver',),
  '1208403':('America/Denver',),
- '55939997':('America/Sao_Paulo',),
  '1208407':('America/Denver',),
  '1775982':('America/Los_Angeles',),
- '1270352':('America/New_York',),
- '1270351':('America/New_York',),
+ '1270354':('America/Chicago',),
+ '55943222':('America/Sao_Paulo',),
  '1605837':('America/Denver',),
  '1605835':('America/Chicago',),
- '1270358':('America/New_York',),
  '1701477':('America/Chicago',),
  '1701476':('America/Chicago',),
  '1701471':('America/Chicago',),
  '1701478':('America/Chicago',),
  '1850393':('America/Chicago',),
- '1850391':('America/New_York',),
+ '7498':('Europe/Moscow',),
  '7499':('Europe/Moscow',),
  '1850396':('America/Chicago',),
  '7492':('Europe/Moscow',),
  '7493':('Europe/Moscow',),
  '1850398':('America/Chicago',),
  '7496':('Europe/Moscow',),
  '7494':('Europe/Moscow',),
  '7495':('Europe/Moscow',),
  '1541554':('America/Los_Angeles',),
  '1541556':('America/Los_Angeles',),
  '1270725':('America/Chicago',),
  '1541550':('America/Los_Angeles',),
  '1541552':('America/Los_Angeles',),
  '1541553':('America/Los_Angeles',),
- '1418492':('America/Toronto',),
- '1250295':('America/Vancouver',),
  '4761':('Europe/Oslo',),
- '1850536':('America/New_York',),
  '1850535':('America/Chicago',),
  '4762':('Europe/Oslo',),
  '4764':('Europe/Oslo',),
  '4767':('Europe/Oslo',),
  '4766':('Europe/Oslo',),
  '4769':('Europe/Oslo',),
- '1850539':('America/New_York',),
- '55933735':('America/Sao_Paulo',),
  '1907269':('America/Juneau',),
  '1907264':('America/Juneau',),
  '1907260':('America/Juneau',),
  '1907262':('America/Juneau',),
  '685':('Pacific/Apia',),
  '55933793':('America/Sao_Paulo',),
  '687':('Pacific/Noumea',),
- '686':('Pacific/Enderbury', 'Pacific/Kiritimati', 'Pacific/Tarawa'),
+ '1570':('America/New_York',),
  '521695':('America/Mazatlan',),
  '521694':('America/Mazatlan',),
  '55813341':('America/Sao_Paulo',),
- '55813343':('America/Sao_Paulo',),
+ '55813611':('America/Sao_Paulo',),
  '55813342':('America/Sao_Paulo',),
  '55813345':('America/Sao_Paulo',),
- '1575':('America/Denver',),
- '521696':('America/Mazatlan',),
+ '55813344':('America/Sao_Paulo',),
+ '1208847':('America/Denver',),
  '55933538':('America/Sao_Paulo',),
  '55933533':('America/Sao_Paulo',),
  '55933532':('America/Sao_Paulo',),
  '55933531':('America/Sao_Paulo',),
  '55933537':('America/Sao_Paulo',),
  '55933536':('America/Sao_Paulo',),
- '521474':('America/Mexico_City',),
- '1250743':('America/Vancouver',),
- '1250740':('America/Vancouver',),
- '1250741':('America/Vancouver',),
- '1250746':('America/Vancouver',),
- '1250747':('America/Vancouver',),
- '1250744':('America/Vancouver',),
- '1250748':('America/Vancouver',),
- '1250749':('America/Vancouver',),
- '52481':('America/Mexico_City',),
+ '55933534':('America/Sao_Paulo',),
  '390784':('Europe/Rome',),
  '97622':('Asia/Ulaanbaatar',),
  '9765515':('Asia/Ulaanbaatar',),
- '1785543':('America/Chicago',),
- '1785542':('America/Chicago',),
+ '97625':('Asia/Ulaanbaatar',),
  '441229':('Europe/London',),
  '441228':('Europe/London',),
  '441225':('Europe/London',),
  '441224':('Europe/London',),
  '441227':('Europe/London',),
  '441226':('Europe/London',),
  '441223':('Europe/London',),
- '1906353':('America/New_York',),
  '1605448':('America/Chicago',),
- '1308425':('America/Chicago',),
- '55813651':('America/Sao_Paulo',),
  '1308423':('America/Denver',),
  '86464':('Asia/Shanghai',),
  '86467':('Asia/Shanghai',),
  '86469':('Asia/Shanghai',),
  '86468':('Asia/Shanghai',),
  '1270298':('America/Chicago',),
- '1812988':('America/New_York',),
- '52995':('America/Mexico_City',),
  '672':('Pacific/Norfolk',),
  '1812985':('America/Chicago',),
- '1418704':('America/Toronto',),
  '62746':('Asia/Jakarta',),
  '1726':('America/Chicago',),
  '1727':('America/New_York',),
  '1724':('America/New_York',),
+ '1725':('America/Los_Angeles',),
  '62744':('Asia/Jakarta',),
  '1720':('America/Denver',),
  '1721':('America/Lower_Princes',),
  '62745':('Asia/Jakarta',),
  '62742':('Asia/Jakarta',),
+ '52993':('America/Mexico_City',),
  '62743':('Asia/Jakarta',),
  '1541708':('America/Los_Angeles',),
+ '1906875':('America/Chicago',),
  '62741':('Asia/Jakarta',),
  '1541704':('America/Los_Angeles',),
  '1541706':('America/Los_Angeles',),
  '521668':('America/Mazatlan',),
  '521669':('America/Mazatlan',),
- '1620431':('America/Chicago',),
- '1418641':('America/Toronto',),
  '521661':('America/Tijuana',),
- '521662':('America/Mazatlan',),
+ '1580':('America/Chicago',),
  '1581':('America/Toronto',),
  '1586':('America/New_York',),
- '1587':('America/Edmonton',),
- '1418647':('America/Toronto',),
+ '521665':('America/Tijuana',),
  '521667':('America/Mazatlan',),
  '1701288':('America/Chicago',),
  '62748':('Asia/Jakarta',),
+ '1605275':('America/Chicago',),
  '1701282':('America/Chicago',),
  '1850865':('America/Chicago',),
  '1701280':('America/Chicago',),
  '1701281':('America/Chicago',),
  '1701284':('America/Chicago',),
  '1850708':('America/Chicago',),
- '62865':('Asia/Jakarta',),
  '5658':('America/Santiago',),
  '5657':('America/Santiago',),
  '5655':('America/Santiago',),
  '5652':('America/Santiago',),
  '5653':('America/Santiago',),
  '5651':('America/Santiago',),
- '34855':('Europe/Madrid',),
  '55913018':('America/Sao_Paulo',),
+ '441259':('Europe/London',),
  '86147':('Asia/Shanghai',),
  '55813118':('America/Sao_Paulo',),
- '34853':('Europe/Madrid',),
- '1308745':('America/Chicago',),
  '1208343':('America/Denver',),
  '1208342':('America/Denver',),
- '1208340':('America/Denver',),
+ '55813117':('America/Sao_Paulo',),
  '55813110':('America/Sao_Paulo',),
- '1208346':('America/Denver',),
+ '55813111':('America/Sao_Paulo',),
  '1208345':('America/Denver',),
  '1208344':('America/Denver',),
+ '441257':('Europe/London',),
  '1701866':('America/Chicago',),
  '5594992':('America/Sao_Paulo',),
  '1219659':('America/Chicago',),
  '5594991':('America/Sao_Paulo',),
  '39059':('Europe/Rome',),
  '39050':('Europe/Rome',),
  '39051':('Europe/Rome',),
@@ -810,44 +683,39 @@
  '211':('Africa/Nairobi',),
  '218':('Europe/Bucharest',),
  '1775376':('America/Los_Angeles',),
  '55913711':('America/Sao_Paulo',),
  '55913712':('America/Sao_Paulo',),
  '86813':('Asia/Shanghai',),
  '1270575':('America/Chicago',),
- '86816':('Asia/Shanghai',),
  '1907743':('America/Juneau',),
  '1907742':('America/Juneau',),
- '86817':('Asia/Shanghai',),
  '1907747':('America/Juneau',),
  '1907746':('America/Juneau',),
  '1907745':('America/Juneau',),
- '1906296':('America/New_York',),
  '86818':('Asia/Shanghai',),
- '1906293':('America/New_York',),
  '521868':('America/Mexico_City',),
  '521869':('America/Mexico_City',),
  '521866':('America/Mexico_City',),
  '521867':('America/Mexico_City',),
  '521864':('America/Mexico_City',),
  '521862':('America/Mexico_City',),
  '521861':('America/Mexico_City',),
  '1812401':('America/Chicago',),
  '1812402':('America/Chicago',),
  '55813437':('America/Sao_Paulo',),
- '55813436':('America/Sao_Paulo',),
- '55813517':('America/Sao_Paulo',),
+ '1907333':('America/Juneau',),
  '55813433':('America/Sao_Paulo',),
- '1574400':('America/New_York',),
+ '55913011':('America/Sao_Paulo',),
  '55813432':('America/Sao_Paulo',),
  '1541887':('America/Los_Angeles',),
  '1541884':('America/Los_Angeles',),
  '1541885':('America/Los_Angeles',),
- '1423658':('America/Chicago',),
- '1541883':('America/Los_Angeles',),
+ '1541882':('America/Los_Angeles',),
+ '55813431':('America/Sao_Paulo',),
  '1541881':('America/Denver',),
  '1423652':('America/New_York',),
  '1541889':('America/Denver',),
  '62823':('Asia/Jakarta',),
  '62351':('Asia/Jakarta',),
  '62353':('Asia/Jakarta',),
  '62352':('Asia/Jakarta',),
@@ -859,159 +727,130 @@
  '1423478':('America/New_York',),
  '1423479':('America/New_York',),
  '1423472':('America/New_York',),
  '1423473':('America/New_York',),
  '1423475':('America/New_York',),
  '1423476':('America/New_York',),
  '1423477':('America/New_York',),
- '1785483':('America/Chicago',),
- '1785484':('America/Chicago',),
- '1785486':('America/Chicago',),
- '55813431':('America/Sao_Paulo',),
- '1250828':('America/Vancouver',),
- '1250826':('America/Vancouver',),
- '1785738':('America/Chicago',),
  '55813087':('America/Sao_Paulo',),
  '1605859':('America/Denver',),
  '505':('America/Chicago',),
  '1605852':('America/Chicago',),
  '1605853':('America/Chicago',),
  '1605854':('America/Chicago',),
  '1605856':('America/Chicago',),
  '1208642':('America/Denver',),
  '500':('Atlantic/Stanley',),
  '1208640':('America/Los_Angeles',),
- '1541632':('America/Los_Angeles',),
+ '501':('America/Belize',),
  '55913085':('America/Sao_Paulo',),
  '55913084':('America/Sao_Paulo',),
  '55913087':('America/Sao_Paulo',),
  '55913086':('America/Sao_Paulo',),
  '55913081':('America/Sao_Paulo',),
- '1701499':('America/Chicago',),
+ '55913083':('America/Sao_Paulo',),
  '55913082':('America/Sao_Paulo',),
  '55913089':('America/Sao_Paulo',),
  '1701492':('America/Chicago',),
+ '1541515':('America/Los_Angeles',),
  '1541393':('America/Los_Angeles',),
  '1541390':('America/Los_Angeles',),
  '1541396':('America/Los_Angeles',),
+ '1216':('America/New_York',),
  '1208422':('America/Denver',),
  '1208423':('America/Denver',),
  '1208420':('America/Denver',),
- '1208426':('America/Denver',),
- '1208424':('America/Denver',),
- '1208425':('America/Denver',),
+ '1443':('America/New_York',),
+ '1442':('America/Los_Angeles',),
+ '1441':('Atlantic/Bermuda',),
+ '1440':('America/New_York',),
  '1208429':('America/Denver',),
+ '1219728':('America/Chicago',),
  '1270745':('America/Chicago',),
  '1270746':('America/Chicago',),
  '1541579':('America/Los_Angeles',),
  '1541576':('America/Los_Angeles',),
  '1541574':('America/Los_Angeles',),
  '1541575':('America/Los_Angeles',),
  '1541572':('America/Los_Angeles',),
  '1541573':('America/Los_Angeles',),
  '4724':('Europe/Oslo',),
  '55913606':('America/Sao_Paulo',),
- '1850510':('America/New_York',),
- '1812238':('America/New_York',),
- '1850514':('America/New_York',),
+ '55913605':('America/Sao_Paulo',),
  '590590':('America/Guadeloupe',),
  '1850516':('America/Chicago',),
- '1812232':('America/New_York',),
- '1812231':('America/New_York',),
- '1812237':('America/New_York',),
- '1812234':('America/New_York',),
- '1812235':('America/New_York',),
+ '1709673':('America/St_Johns',),
+ '86724':('Asia/Shanghai',),
  '1907246':('America/Juneau',),
  '1907247':('America/Juneau',),
  '1907244':('America/Juneau',),
  '1907245':('America/Juneau',),
  '1907243':('America/Juneau',),
  '1907248':('America/Juneau',),
- '1867587':('America/Edmonton',),
- '441676':('Europe/London',),
- '441677':('Europe/London',),
+ '55813639':('America/Sao_Paulo',),
+ '55813638':('America/Sao_Paulo',),
  '441674':('Europe/London',),
  '441675':('Europe/London',),
  '441672':('Europe/London',),
  '441673':('Europe/London',),
  '441670':('Europe/London',),
  '441671':('Europe/London',),
  '55813631':('America/Sao_Paulo',),
  '55813633':('America/Sao_Paulo',),
  '55813635':('America/Sao_Paulo',),
  '55813634':('America/Sao_Paulo',),
- '441678':('Europe/London',),
+ '55813637':('America/Sao_Paulo',),
  '55813636':('America/Sao_Paulo',),
  '55813327':('America/Sao_Paulo',),
  '55813326':('America/Sao_Paulo',),
  '55813325':('America/Sao_Paulo',),
  '55813323':('America/Sao_Paulo',),
  '55813322':('America/Sao_Paulo',),
- '55813321':('America/Sao_Paulo',),
  '55813320':('America/Sao_Paulo',),
  '55813328':('America/Sao_Paulo',),
  '55933512':('America/Sao_Paulo',),
  '55933515':('America/Sao_Paulo',),
  '55933514':('America/Sao_Paulo',),
  '55933517':('America/Sao_Paulo',),
  '55933518':('America/Sao_Paulo',),
- '1418523':('America/Toronto',),
  '86825':('Asia/Shanghai',),
  '86827':('Asia/Shanghai',),
  '86826':('Asia/Shanghai',),
  '1605284':('America/Chicago',),
  '390439':('Europe/Rome',),
  '390438':('Europe/Rome',),
  '390433':('Europe/Rome',),
  '390432':('Europe/Rome',),
  '390431':('Europe/Rome',),
- '421':('Europe/Bratislava',),
  '390921':('Europe/Rome',),
  '390436':('Europe/Rome',),
- '390435':('Europe/Rome',),
+ '390923':('Europe/Rome',),
  '390434':('Europe/Rome',),
  '441207':('Europe/London',),
  '441206':('Europe/London',),
  '441205':('Europe/London',),
  '441204':('Europe/London',),
  '441202':('Europe/London',),
  '441200':('Europe/London',),
  '441209':('Europe/London',),
  '441208':('Europe/London',),
  '6273':('Asia/Jakarta',),
  '6276':('Asia/Jakarta',),
- '1906370':('America/New_York',),
  '55943435':('America/Sao_Paulo',),
  '55943434':('America/Sao_Paulo',),
  '55943431':('America/Sao_Paulo',),
  '55943433':('America/Sao_Paulo',),
  '55943432':('America/Sao_Paulo',),
- '62252':('Asia/Jakarta',),
- '125038':('America/Vancouver',),
  '855':('Asia/Phnom_Penh',),
- '613':('Australia/Sydney',),
- '850':('Asia/Pyongyang',),
+ '856':('Asia/Vientiane',),
+ '850':('Asia/Seoul',),
  '852':('Asia/Hong_Kong',),
- '62253':('Asia/Jakarta',),
+ '853':('Asia/Shanghai',),
  '1775384':('America/Los_Angeles',),
- '1574217':('America/New_York',),
- '1418728':('America/Toronto',),
- '1418724':('America/Toronto',),
- '1418725':('America/Toronto',),
- '1418722':('America/Toronto',),
- '1418723':('America/Toronto',),
- '1418721':('America/Toronto',),
- '1418623':('America/Toronto',),
- '1418622':('America/Toronto',),
- '1418627':('America/Toronto',),
- '1418626':('America/Toronto',),
- '1418625':('America/Toronto',),
- '1418624':('America/Toronto',),
- '1418629':('America/Toronto',),
- '1418628':('America/Toronto',),
+ '1219392':('America/Chicago',),
  '1541761':('America/Los_Angeles',),
  '1541760':('America/Los_Angeles',),
  '1541767':('America/Los_Angeles',),
  '1541766':('America/Los_Angeles',),
  '1541765':('America/Los_Angeles',),
  '1541764':('America/Los_Angeles',),
  '1541768':('America/Los_Angeles',),
@@ -1024,50 +863,37 @@
  '1303':('America/Denver',),
  '1807223':('America/Winnipeg',),
  '1309':('America/Chicago',),
  '1867633':('America/Vancouver',),
  '55813132':('America/Sao_Paulo',),
  '55813130':('America/Sao_Paulo',),
  '55813131':('America/Sao_Paulo',),
- '441449':('Europe/London',),
+ '55813136':('America/Sao_Paulo',),
  '55813137':('America/Sao_Paulo',),
  '55813134':('America/Sao_Paulo',),
  '441445':('Europe/London',),
  '441444':('Europe/London',),
- '1423735':('America/New_York',),
+ '55813138':('America/Sao_Paulo',),
  '441446':('Europe/London',),
  '441440':('Europe/London',),
  '441443':('Europe/London',),
  '441442':('Europe/London',),
- '1785228':('America/Chicago',),
- '1785229':('America/Chicago',),
- '1785227':('America/Chicago',),
- '1785221':('America/Chicago',),
- '1785222':('America/Chicago',),
- '1785223':('America/Chicago',),
- '1850727':('America/New_York',),
  '1850722':('America/Chicago',),
  '1850723':('America/Chicago',),
  '1850729':('America/Chicago',),
  '1850593':('America/Chicago',),
  '55913692':('America/Sao_Paulo',),
  '55913694':('America/Sao_Paulo',),
  '39070':('Europe/Rome',),
  '39071':('Europe/Rome',),
  '39075':('Europe/Rome',),
  '39079':('Europe/Rome',),
  '55813797':('America/Sao_Paulo',),
  '1270554':('America/Chicago',),
- '5585':('America/Sao_Paulo',),
- '1250462':('America/Vancouver',),
- '55813862':('America/Sao_Paulo',),
- '55813863':('America/Sao_Paulo',),
- '55813869':('America/Sao_Paulo',),
- '1250469':('America/Vancouver',),
- '1250468':('America/Vancouver',),
+ '1208602':('America/Denver',),
  '521841':('America/Mexico_City',),
  '521842':('America/Mexico_City',),
  '521844':('America/Mexico_City',),
  '521845':('America/Mexico_City',),
  '521846':('America/Mexico_City',),
  '55912121':('America/Sao_Paulo',),
  '55912123':('America/Sao_Paulo',),
@@ -1077,65 +903,56 @@
  '521593':('America/Mexico_City',),
  '521591':('America/Mexico_City',),
  '521596':('America/Mexico_City',),
  '521597':('America/Mexico_City',),
  '521594':('America/Mexico_City',),
  '521595':('America/Mexico_City',),
  '521599':('America/Mexico_City',),
- '593':('America/Guayaquil', 'Pacific/Galapagos'),
- '595':('America/Asuncion',),
+ '1541354':('America/Los_Angeles',),
+ '1541352':('America/Los_Angeles',),
  '1208991':('America/Denver',),
  '977':('Asia/Katmandu',),
  '976':('Asia/Choibalsan', 'Asia/Hovd', 'Asia/Ulaanbaatar'),
  '975':('Asia/Thimphu',),
  '974':('Asia/Qatar',),
  '973':('Asia/Bahrain',),
- '597':('America/Paramaribo',),
+ '1541350':('America/Los_Angeles',),
  '1605610':('America/Chicago',),
  '970':('Europe/Bucharest',),
  '1907766':('America/Juneau',),
- '598':('America/Montevideo',),
- '1620626':('America/Chicago',),
  '1423453':('America/New_York',),
- '1620624':('America/Chicago',),
- '1620625':('America/Chicago',),
+ '1423907':('America/New_York',),
  '55813753':('America/Sao_Paulo',),
  '1907835':('America/Juneau',),
  '62376':('Asia/Makassar',),
  '62374':('Asia/Makassar',),
  '62373':('Asia/Makassar',),
- '1907830':('America/Juneau',),
+ '62372':('Asia/Makassar',),
  '62371':('Asia/Makassar',),
  '62370':('Asia/Makassar',),
- '55813751':('America/Sao_Paulo',),
- '55813757':('America/Sao_Paulo',),
+ '55813023':('America/Sao_Paulo',),
+ '55813025':('America/Sao_Paulo',),
  '1541688':('America/Los_Angeles',),
- '55813755':('America/Sao_Paulo',),
+ '55813026':('America/Sao_Paulo',),
+ '441598':('Europe/London',),
  '55813028':('America/Sao_Paulo',),
- '55813758':('America/Sao_Paulo',),
+ '441595':('Europe/London',),
  '55813759':('America/Sao_Paulo',),
- '55913075':('America/Sao_Paulo',),
- '1250809':('America/Vancouver',),
+ '441592':('Europe/London',),
  '390771':('Europe/Rome',),
  '390773':('Europe/Rome',),
  '390774':('Europe/Rome',),
  '390775':('Europe/Rome',),
  '390776':('Europe/Rome',),
- '1250801':('America/Vancouver',),
- '1250803':('America/Vancouver',),
- '1250804':('America/Vancouver',),
- '1250807':('America/Vancouver',),
- '1606423':('America/New_York',),
  '1701652':('America/Chicago',),
  '1775945':('America/Los_Angeles',),
  '1605874':('America/Chicago',),
  '55943779':('America/Sao_Paulo',),
  '1605878':('America/Chicago',),
  '86580':('Asia/Shanghai',),
- '266':('Africa/Maseru',),
  '1681':('America/New_York',),
  '1680':('America/New_York',),
  '1208622':('America/Denver',),
  '1682':('America/Chicago',),
  '1208996':('America/Denver',),
  '1208625':('America/Los_Angeles',),
  '1208994':('America/Denver',),
@@ -1145,162 +962,132 @@
  '55812011':('America/Sao_Paulo',),
  '86631':('Asia/Shanghai',),
  '86632':('Asia/Shanghai',),
  '86633':('Asia/Shanghai',),
  '86634':('Asia/Shanghai',),
  '86635':('Asia/Shanghai',),
  '1541372':('America/Denver',),
- '1785505':('America/Chicago',),
- '55943382':('America/Sao_Paulo',),
  '1469':('America/Chicago',),
  '1463':('America/New_York',),
- '1270769':('America/New_York',),
+ '1541752':('America/Los_Angeles',),
  '1270762':('America/Chicago',),
- '1270763':('America/New_York',),
  '1541512':('America/Los_Angeles',),
  '1270761':('America/Chicago',),
- '1270766':('America/New_York',),
+ '1541514':('America/Los_Angeles',),
  '1270767':('America/Chicago',),
- '1270765':('America/New_York',),
+ '1541517':('America/Los_Angeles',),
  '5591':('America/Manaus',),
  '5593':('America/Manaus',),
  '5592':('America/Manaus',),
  '5595':('America/Manaus',),
  '5594':('America/Manaus',),
  '5597':('America/Manaus',),
  '5596':('America/Sao_Paulo',),
  '5599':('America/Sao_Paulo',),
  '5598':('America/Sao_Paulo',),
  '1709651':('America/St_Johns',),
- '55913031':('America/Sao_Paulo',),
  '1850572':('America/Chicago',),
- '1850570':('America/New_York',),
- '1850577':('America/New_York',),
- '1850576':('America/New_York',),
- '1850575':('America/New_York',),
- '1850574':('America/New_York',),
- '1775677':('America/Los_Angeles',),
+ '1907222':('America/Juneau',),
  '1907223':('America/Juneau',),
  '1907224':('America/Juneau',),
  '1907225':('America/Juneau',),
  '1907227':('America/Juneau',),
  '1907228':('America/Juneau',),
  '1907229':('America/Juneau',),
  '1208397':('America/Denver',),
  '1208390':('America/Denver',),
  '1330':('America/New_York',),
- '62273':('Asia/Jakarta',),
  '441650':('Europe/London',),
  '441651':('Europe/London',),
  '441652':('Europe/London',),
  '441653':('Europe/London',),
  '441654':('Europe/London',),
  '441655':('Europe/London',),
  '441656':('Europe/London',),
  '55813658':('America/Sao_Paulo',),
  '55813305':('America/Sao_Paulo',),
- '441659':('Europe/London',),
+ '55813656':('America/Sao_Paulo',),
  '55813655':('America/Sao_Paulo',),
  '55813654':('America/Sao_Paulo',),
- '55813301':('America/Sao_Paulo',),
+ '55813653':('America/Sao_Paulo',),
  '55813652':('America/Sao_Paulo',),
- '55813303':('America/Sao_Paulo',),
+ '55813651':('America/Sao_Paulo',),
  '55813302':('America/Sao_Paulo',),
  '8699':('Asia/Shanghai',),
- '1250256':('America/Vancouver',),
  '55933574':('America/Sao_Paulo',),
- '1812537':('America/New_York',),
  '1250787':('America/Edmonton',),
  '1250784':('America/Edmonton',),
  '1250785':('America/Edmonton',),
  '1250782':('America/Edmonton',),
  '1250788':('America/Edmonton',),
  '52983':('America/New_York',),
  '52982':('America/Mexico_City',),
  '52981':('America/Mexico_City',),
  '52987':('America/New_York',),
  '52986':('America/Mexico_City',),
  '52329':('America/Mexico_City',),
- '52328':('America/Mexico_City',),
+ '52984':('America/New_York',),
  '52327':('America/Mazatlan',),
  '52326':('America/Mexico_City',),
  '52325':('America/Mazatlan',),
  '52324':('America/Mazatlan',),
  '52323':('America/Mazatlan',),
  '52322':('America/Mexico_City',),
  '52321':('America/Mexico_City',),
  '1775432':('America/Los_Angeles',),
  '1605262':('America/Chicago',),
+ '1605261':('America/Chicago',),
  '1605260':('America/Chicago',),
  '441261':('Europe/London',),
  '441260':('Europe/London',),
  '441263':('Europe/London',),
  '441262':('Europe/London',),
  '441264':('Europe/London',),
  '441267':('Europe/London',),
  '441269':('Europe/London',),
  '441268':('Europe/London',),
- '1308754':('America/Chicago',),
  '55913521':('America/Sao_Paulo',),
  '1423357':('America/New_York',),
- '55913528':('America/Sao_Paulo',),
  '52181':('America/Mexico_City',),
- '1423893':('America/New_York',),
- '1423725':('America/New_York',),
- '1418296':('America/Toronto',),
  '1867920':('America/Edmonton',),
- '1418295':('America/Toronto',),
  '97621':('Asia/Ulaanbaatar',),
  '1812618':('America/Chicago',),
- '97623':('Asia/Ulaanbaatar',),
  '441885':('Europe/London',),
  '441884':('Europe/London',),
  '441887':('Europe/London',),
  '441886':('Europe/London',),
- '1812948':('America/New_York',),
- '1812949':('America/New_York',),
+ '441880':('Europe/London',),
  '441883':('Europe/London',),
  '441882':('Europe/London',),
- '1812944':('America/New_York',),
- '1812945':('America/New_York',),
+ '3485':('Europe/Madrid',),
  '441889':('Europe/London',),
- '1812941':('America/New_York',),
- '1574239':('America/New_York',),
- '1574231':('America/New_York',),
- '1574233':('America/New_York',),
- '1574232':('America/New_York',),
- '1574235':('America/New_York',),
- '1574234':('America/New_York',),
- '1574237':('America/New_York',),
- '1418748':('America/Toronto',),
- '1541301':('America/Los_Angeles',),
+ '441888':('Europe/London',),
+ '1850226':('America/Chicago',),
  '62636':('Asia/Jakarta',),
  '62634':('Asia/Jakarta',),
- '1850556':('America/New_York',),
+ '62635':('Asia/Jakarta',),
  '521628':('America/Mazatlan',),
- '521629':('America/Mazatlan', 'America/Mexico_City'),
+ '62633':('Asia/Jakarta',),
  '62631':('Asia/Jakarta',),
  '521624':('America/Mazatlan',),
  '521625':('America/Mazatlan',),
  '521626':('America/Hermosillo', 'America/Tijuana'),
  '521627':('America/Mazatlan',),
  '521621':('America/Mazatlan',),
- '1418603':('America/Toronto',),
- '1418602':('America/Toronto',),
- '1785675':('America/Chicago',),
- '1785672':('America/Chicago',),
+ '521622':('America/Mazatlan',),
+ '521623':('America/Mazatlan',),
+ '34928':('Atlantic/Canary',),
  '34925':('Europe/Madrid',),
  '34924':('Europe/Madrid',),
  '34927':('Europe/Madrid',),
  '34926':('Europe/Madrid',),
  '34921':('Europe/Madrid',),
  '34920':('Europe/Madrid',),
  '34923':('Europe/Madrid',),
  '34922':('Atlantic/Canary',),
- '1606387':('America/Chicago',),
  '1541749':('America/Los_Angeles',),
  '1541745':('America/Los_Angeles',),
  '1541744':('America/Los_Angeles',),
  '1541747':('America/Los_Angeles',),
  '1541746':('America/Los_Angeles',),
  '1541741':('America/Los_Angeles',),
  '1541740':('America/Los_Angeles',),
@@ -1314,151 +1101,129 @@
  '441461':('Europe/London',),
  '441460':('Europe/London',),
  '1208385':('America/Denver',),
  '1208384':('America/Denver',),
  '1208383':('America/Denver',),
  '1208382':('America/Denver',),
  '441469':('Europe/London',),
- '1701355':('America/Chicago',),
- '1701356':('America/Chicago',),
+ '55913321':('America/Sao_Paulo',),
+ '55913322':('America/Sao_Paulo',),
  '55913323':('America/Sao_Paulo',),
  '8687':('Asia/Shanghai',),
  '1701824':('America/Denver',),
  '55943018':('America/Sao_Paulo',),
  '55943013':('America/Sao_Paulo',),
  '55943012':('America/Sao_Paulo',),
  '55943016':('America/Sao_Paulo',),
  '1709468':('America/St_Johns',),
- '1850745':('America/New_York',),
  '1850747':('America/Chicago',),
+ '1850748':('America/Chicago',),
  '1850968':('America/Chicago',),
  '1850969':('America/Chicago',),
  '441790':('Europe/London',),
  '441793':('Europe/London',),
  '441792':('Europe/London',),
  '441795':('Europe/London',),
  '441794':('Europe/London',),
  '441797':('Europe/London',),
  '441796':('Europe/London',),
  '441799':('Europe/London',),
- '441798':('Europe/London',),
+ '1219696':('America/Chicago',),
  '1219690':('America/Chicago',),
- '351266':('Europe/Lisbon',),
+ '1907209':('America/Juneau',),
  '39099':('Europe/Rome',),
  '39095':('Europe/Rome',),
  '39090':('Europe/Rome',),
  '39091':('Europe/Rome',),
  '86429':('Asia/Shanghai',),
- '181233':('America/New_York',),
- '55813616':('America/Sao_Paulo',),
  '86427':('Asia/Shanghai',),
  '1775826':('America/Los_Angeles',),
- '1812379':('America/New_York',),
- '1812378':('America/New_York',),
- '1812376':('America/New_York',),
- '1812375':('America/New_York',),
- '1812373':('America/New_York',),
- '1812372':('America/New_York',),
+ '20':('Africa/Cairo',),
  '521823':('America/Mexico_City',),
  '521821':('America/Mexico_City',),
  '521826':('America/Mexico_City',),
  '521824':('America/Mexico_City',),
  '521825':('America/Mexico_City',),
- '1250448':('America/Vancouver',),
  '521828':('America/Mexico_City',),
  '62916':('Asia/Jayapura',),
  '62914':('Asia/Jayapura',),
- '1785766':('America/Chicago',),
  '1775338':('America/Los_Angeles',),
  '1775334':('America/Los_Angeles',),
  '1775337':('America/Los_Angeles',),
  '1775336':('America/Los_Angeles',),
  '1775331':('America/Los_Angeles',),
  '1775333':('America/Los_Angeles',),
  '1775332':('America/Los_Angeles',),
  '1423610':('America/New_York',),
- '1906786':('America/New_York',),
  '1423613':('America/New_York',),
  '1423614':('America/New_York',),
- '1906789':('America/New_York',),
  '1605673':('America/Denver',),
  '1605677':('America/Chicago',),
  '55813518':('America/Sao_Paulo',),
  '55813519':('America/Sao_Paulo',),
  '1907789':('America/Juneau',),
- '55813510':('America/Sao_Paulo',),
  '1907786':('America/Juneau',),
  '55813512':('America/Sao_Paulo',),
  '1907783':('America/Juneau',),
- '55813516':('America/Sao_Paulo',),
  '1907780':('America/Juneau',),
  '62829':('Asia/Jakarta', 'Asia/Makassar'),
  '62828':('Asia/Jakarta',),
  '1423928':('America/New_York',),
  '1423929':('America/New_York',),
  '1423926':('America/New_York',),
  '62822':('Asia/Jakarta',),
  '62821':('Asia/Jakarta',),
  '62820':('Asia/Jakarta',),
  '62827':('Asia/Jakarta',),
  '62826':('Asia/Jakarta',),
  '62825':('Asia/Jakarta',),
  '1423921':('America/New_York',),
- '1785448':('America/Chicago',),
  '390578':('Europe/Rome',),
  '390577':('Europe/Rome',),
  '390574':('Europe/Rome',),
  '390575':('Europe/Rome',),
  '390572':('Europe/Rome',),
  '390573':('Europe/Rome',),
  '390571':('Europe/Rome',),
  '1219996':('America/Chicago',),
- '1250863':('America/Vancouver',),
- '1250862':('America/Vancouver',),
- '1250861':('America/Vancouver',),
- '1250860':('America/Vancouver',),
- '1250864':('America/Vancouver',),
- '1250869':('America/Vancouver',),
- '1250868':('America/Vancouver',),
- '1606408':('America/New_York',),
- '1219696':('America/Chicago',),
  '1270335':('America/Chicago',),
  '1270846':('America/Chicago',),
  '44191':('Europe/London',),
  '55813676':('America/Sao_Paulo',),
  '1270843':('America/Chicago',),
  '1270842':('America/Chicago',),
  '1270333':('America/Chicago',),
  '44198':('Europe/London',),
  '1270338':('America/Chicago',),
  '1605892':('America/Denver',),
  '1208608':('America/Denver',),
- '1208602':('America/Denver',),
+ '1669':('America/Los_Angeles',),
+ '1667':('America/New_York',),
  '1664':('America/Montserrat',),
  '1662':('America/Chicago',),
  '1661':('America/Los_Angeles',),
  '1660':('America/Chicago',),
  '591':('America/La_Paz',),
- '1541357':('America/Los_Angeles',),
- '1541354':('America/Los_Angeles',),
+ '590':('America/Guadeloupe', 'America/Halifax', 'America/Marigot'),
+ '593':('America/Guayaquil', 'Pacific/Galapagos'),
  '592':('America/Guyana',),
- '1541352':('America/Los_Angeles',),
+ '595':('America/Asuncion',),
  '594':('America/Cayenne',),
- '1541350':('America/Los_Angeles',),
+ '597':('America/Paramaribo',),
  '596':('America/Martinique',),
  '599':('America/Curacao', 'America/Kralendijk'),
- '55813679':('America/Sao_Paulo',),
+ '598':('America/Montevideo',),
  '1208388':('America/Denver',),
  '1541359':('America/Los_Angeles',),
  '1850883':('America/Chicago',),
  '1541689':('America/Los_Angeles',),
+ '1775232':('America/Los_Angeles',),
  '1541682':('America/Los_Angeles',),
  '1541683':('America/Los_Angeles',),
  '1541684':('America/Los_Angeles',),
- '1541685':('America/Los_Angeles',),
  '1541686':('America/Los_Angeles',),
  '1541687':('America/Los_Angeles',),
  '1409':('America/Chicago',),
  '1408':('America/Los_Angeles',),
  '1403':('America/Edmonton',),
  '1402':('America/Chicago',),
  '1401':('America/New_York',),
@@ -1466,147 +1231,119 @@
  '1406':('America/Denver',),
  '1405':('America/Chicago',),
  '1404':('America/New_York',),
  '692':('Pacific/Majuro',),
  '1541531':('America/Los_Angeles',),
  '1541536':('America/Los_Angeles',),
  '1541535':('America/Los_Angeles',),
- '690':('Pacific/Fakaofo',),
- '691':('Pacific/Kosrae', 'Pacific/Ponape', 'Pacific/Truk'),
- '1418937':('America/Halifax',),
+ '1208871':('America/Denver',),
  '521916':('America/Mexico_City',),
- '1540':('America/New_York',),
  '521445':('America/Mexico_City',),
  '521914':('America/Mexico_City',),
+ '1930':('America/New_York',),
  '521913':('America/Mexico_City',),
  '1850227':('America/Chicago',),
- '1850226':('America/Chicago',),
+ '521831':('America/Mexico_City',),
  '1850225':('America/Chicago',),
- '1850224':('America/New_York',),
- '1850223':('America/New_York',),
- '1850222':('America/New_York',),
  '1850221':('America/Chicago',),
- '1208879':('America/Denver',),
+ '1934':('America/New_York',),
  '1850229':('America/Chicago',),
- '1850228':('America/New_York',),
  '521832':('America/Mexico_City',),
  '1208765':('America/Los_Angeles',),
  '351265':('Europe/Lisbon',),
- '1907209':('America/Juneau',),
+ '351266':('Europe/Lisbon',),
  '351261':('Europe/Lisbon',),
  '351263':('Europe/Lisbon',),
  '351262':('Europe/Lisbon',),
  '351269':('Europe/Lisbon',),
  '351268':('Europe/Lisbon',),
+ '521919':('America/Mexico_City',),
  '5581303':('America/Sao_Paulo',),
  '55813675':('America/Sao_Paulo',),
  '441638':('Europe/London',),
  '441639':('Europe/London',),
  '55813671':('America/Sao_Paulo',),
  '55813673':('America/Sao_Paulo',),
  '441633':('Europe/London',),
  '441630':('Europe/London',),
  '441631':('Europe/London',),
- '441636':('Europe/London',),
- '441637':('Europe/London',),
+ '55813679':('America/Sao_Paulo',),
+ '55813678':('America/Sao_Paulo',),
  '441634':('Europe/London',),
  '441635':('Europe/London',),
+ '1208766':('America/Denver',),
  '55693527':('America/Sao_Paulo',),
+ '1219427':('America/Chicago',),
  '1775450':('America/Los_Angeles',),
  '1775453':('America/Los_Angeles',),
  '1605791':('America/Denver',),
  '1605796':('America/Chicago',),
  '441249':('Europe/London',),
  '441248':('Europe/London',),
  '441243':('Europe/London',),
  '441242':('Europe/London',),
  '441241':('Europe/London',),
  '1308772':('America/Denver',),
  '441246':('Europe/London',),
  '441245':('Europe/London',),
  '441244':('Europe/London',),
- '1906337':('America/New_York',),
  '55933559':('America/Sao_Paulo',),
  '55933558':('America/Sao_Paulo',),
  '55933557':('America/Sao_Paulo',),
  '55933552':('America/Sao_Paulo',),
  '55939841':('America/Sao_Paulo',),
  '55939840':('America/Sao_Paulo',),
  '390961':('Europe/Rome',),
  '390963':('Europe/Rome',),
  '390962':('Europe/Rome',),
  '390965':('Europe/Rome',),
  '390964':('Europe/Rome',),
  '390967':('Europe/Rome',),
  '390966':('Europe/Rome',),
- '1812636':('America/New_York',),
  '390968':('Europe/Rome',),
- '1812634':('America/New_York',),
- '1574252':('America/New_York',),
- '1574257':('America/New_York',),
- '1574256':('America/New_York',),
- '1574255':('America/New_York',),
- '1574254':('America/New_York',),
- '1574259':('America/New_York',),
- '1574258':('America/New_York',),
- '1418763':('America/Toronto',),
- '1418766':('America/Toronto',),
+ '1423553':('America/New_York',),
  '1423559':('America/New_York',),
  '62773':('Asia/Jakarta',),
  '1605425':('America/Chicago',),
  '1605426':('America/Chicago',),
  '1605428':('America/Chicago',),
- '1606218':('America/New_York',),
- '1620327':('America/Chicago',),
- '1620326':('America/Chicago',),
- '1620325':('America/Chicago',),
- '1620456':('America/Chicago',),
  '62779':('Asia/Jakarta',),
  '390385':('Europe/Rome',),
  '390384':('Europe/Rome',),
  '390386':('Europe/Rome',),
  '390381':('Europe/Rome',),
  '390383':('Europe/Rome',),
  '390382':('Europe/Rome',),
- '1785658':('America/Chicago',),
- '1812967':('America/New_York',),
  '1812962':('America/Chicago',),
  '1812963':('America/Chicago',),
- '1812961':('America/New_York',),
  '1701595':('America/Chicago',),
  '55919850':('America/Sao_Paulo',),
  '55919851':('America/Sao_Paulo',),
  '55919852':('America/Sao_Paulo',),
  '55919853':('America/Sao_Paulo',),
  '55919854':('America/Sao_Paulo',),
- '55813736':('America/Sao_Paulo',),
+ '55919855':('America/Sao_Paulo',),
  '55919856':('America/Sao_Paulo',),
- '1850696':('America/Chicago',),
+ '55943382':('America/Sao_Paulo',),
  '55943386':('America/Sao_Paulo',),
  '55943385':('America/Sao_Paulo',),
  '55813737':('America/Sao_Paulo',),
  '441400':('Europe/London',),
- '1418889':('America/Toronto',),
- '1418888':('America/Toronto',),
+ '441403':('Europe/London',),
  '441405':('Europe/London',),
  '441404':('Europe/London',),
  '441407':('Europe/London',),
  '441406':('Europe/London',),
- '1340':('America/St_Thomas',),
+ '441409':('Europe/London',),
  '1219326':('America/Chicago',),
  '1219325':('America/Chicago',),
- '1219324':('America/Chicago',),
- '1418887':('America/Toronto',),
- '1219322':('America/Chicago',),
- '1418885':('America/Toronto',),
- '1418884':('America/Toronto',),
- '55913544':('America/Sao_Paulo',),
- '1785263':('America/Chicago',),
- '1785266':('America/Chicago',),
- '1785267':('America/Chicago',),
+ '1343':('America/Toronto',),
+ '1345':('America/Cayman',),
+ '1346':('America/Chicago',),
+ '1347':('America/New_York',),
  '55813738':('America/Sao_Paulo',),
  '1701373':('America/Chicago',),
  '1701371':('America/Chicago',),
  '7711':('Asia/Aqtobe',),
  '7710':('Asia/Almaty',),
  '7713':('Asia/Aqtobe',),
  '7712':('Asia/Aqtobe',),
@@ -1615,84 +1352,61 @@
  '7717':('Asia/Almaty',),
  '7716':('Asia/Almaty',),
  '1906932':('America/Chicago',),
  '1850769':('America/Chicago',),
  '55813739':('America/Sao_Paulo',),
  '1850763':('America/Chicago',),
  '1850944':('America/Chicago',),
- '1850766':('America/New_York',),
- '1850765':('America/New_York',),
- '1785883':('America/Chicago',),
- '1785889':('America/Chicago',),
- '1812358':('America/New_York',),
- '1812353':('America/New_York',),
- '1812352':('America/New_York',),
- '1812355':('America/New_York',),
- '1812354':('America/New_York',),
+ '1850941':('America/Chicago',),
+ '1270598':('America/Chicago',),
  '1270597':('America/Chicago',),
  '52281':('America/Mexico_City',),
  '52282':('America/Mexico_City',),
  '52283':('America/Mexico_City',),
  '52284':('America/Mexico_City',),
  '52285':('America/Mexico_City',),
  '52287':('America/Mexico_City',),
- '1250423':('America/Edmonton',),
+ '52288':('America/Mexico_City',),
  '1250427':('America/Edmonton',),
  '1250426':('America/Edmonton',),
  '1250425':('America/Edmonton',),
  '55813155':('America/Sao_Paulo',),
- '55949881':('America/Sao_Paulo',),
  '1807482':('America/Winnipeg',),
- '1812883':('America/New_York',),
+ '7388':('Asia/Krasnoyarsk',),
  '1423638':('America/New_York',),
  '1423639':('America/New_York',),
- '1308224':('America/Chicago',),
+ '1423631':('America/New_York',),
  '1423636':('America/New_York',),
  '1423634':('America/New_York',),
  '55813538':('America/Sao_Paulo',),
  '55813536':('America/Sao_Paulo',),
  '55813537':('America/Sao_Paulo',),
  '55813534':('America/Sao_Paulo',),
  '55813535':('America/Sao_Paulo',),
  '55813533':('America/Sao_Paulo',),
- '1423949':('America/Chicago',),
- '1620669':('America/Chicago',),
- '1785462':('America/Chicago',),
- '1785460':('America/Chicago',),
- '1620846':('America/Chicago',),
- '1620663':('America/Chicago',),
- '1423942':('America/Chicago',),
- '1620845':('America/Chicago',),
- '1620842':('America/Chicago',),
- '1620664':('America/Chicago',),
- '1620665':('America/Chicago',),
- '1620672':('America/Chicago',),
  '55913481':('America/Sao_Paulo',),
  '55913483':('America/Sao_Paulo',),
  '55913482':('America/Sao_Paulo',),
  '55913485':('America/Sao_Paulo',),
  '55913484':('America/Sao_Paulo',),
  '390734':('Europe/Rome',),
  '390735':('Europe/Rome',),
  '390736':('Europe/Rome',),
  '390737':('Europe/Rome',),
  '390731':('Europe/Rome',),
  '390732':('Europe/Rome',),
  '390733':('Europe/Rome',),
- '1785798':('America/Chicago',),
- '1250847':('America/Vancouver',),
- '1250842':('America/Vancouver',),
- '390566':('Europe/Rome',),
  '1308546':('America/Denver',),
  '1423496':('America/New_York',),
  '1423495':('America/New_York',),
  '1423493':('America/New_York',),
  '1423490':('America/New_York',),
+ '55813736':('America/Sao_Paulo',),
+ '1423498':('America/New_York',),
  '1423499':('America/New_York',),
- '1270862':('America/New_York',),
  '1270864':('America/Chicago',),
  '1270866':('America/Chicago',),
  '86546':('Asia/Shanghai',),
  '1709834':('America/St_Johns',),
  '86543':('Asia/Shanghai',),
  '1709832':('America/St_Johns',),
  '1647':('America/Toronto',),
@@ -1700,182 +1414,155 @@
  '1641':('America/Chicago',),
  '1649':('America/Grand_Turk',),
  '1541330':('America/Los_Angeles',),
  '1541332':('America/Los_Angeles',),
  '1541336':('America/Los_Angeles',),
  '1541337':('America/Los_Angeles',),
  '1541338':('America/Los_Angeles',),
- '521783':('America/Mexico_City',),
+ '62265':('Asia/Jakarta',),
  '521782':('America/Mexico_City',),
  '521781':('America/Mexico_City',),
  '62266':('Asia/Jakarta',),
  '1425':('America/Los_Angeles',),
  '521786':('America/Mexico_City',),
- '521785':('America/Mexico_City',),
+ '62263':('Asia/Jakarta',),
  '521784':('America/Mexico_City',),
  '1208489':('America/Denver',),
  '521789':('America/Mexico_City',),
  '1208360':('America/Denver',),
  '62268':('Asia/Jakarta',),
  '55919999':('America/Sao_Paulo',),
- '1205':('America/Chicago',),
+ '55919998':('America/Sao_Paulo',),
  '55919991':('America/Sao_Paulo',),
  '55919990':('America/Sao_Paulo',),
  '55919993':('America/Sao_Paulo',),
  '55919992':('America/Sao_Paulo',),
- '1208514':('America/Denver',),
+ '55919994':('America/Sao_Paulo',),
  '55919997':('America/Sao_Paulo',),
  '55919996':('America/Sao_Paulo',),
  '1208515':('America/Denver',),
- '1812637':('America/New_York',),
  '55913243':('America/Sao_Paulo',),
- '55913242':('America/Sao_Paulo',),
- '55913241':('America/Sao_Paulo',),
- '1418412':('America/Toronto',),
+ '1701250':('America/Chicago',),
+ '1701253':('America/Chicago',),
+ '1219864':('America/Chicago',),
  '55913247':('America/Sao_Paulo',),
- '55913246':('America/Sao_Paulo',),
- '1850201':('America/New_York',),
+ '1701254':('America/Chicago',),
  '1850200':('America/Chicago',),
  '1850206':('America/Chicago',),
  '1850208':('America/Chicago',),
- '55913244':('America/Sao_Paulo',),
+ '1701256':('America/Chicago',),
  '1709695':('America/St_Johns',),
  '1208226':('America/Denver',),
  '1208227':('America/Denver',),
  '1208221':('America/Denver',),
+ '1208228':('America/Denver',),
  '1701787':('America/Chicago',),
  '1701786':('America/Chicago',),
  '351249':('Europe/Lisbon',),
  '1701780':('America/Chicago',),
  '351245':('Europe/Lisbon',),
- '351244':('Europe/Lisbon',),
+ '599318':('America/Kralendijk',),
  '351243':('Europe/Lisbon',),
  '351242':('Europe/Lisbon',),
  '351241':('Europe/Lisbon',),
  '1701788':('America/Chicago',),
- '1250212':('America/Vancouver',),
- '1250213':('America/Vancouver',),
- '1250215':('America/Vancouver',),
- '1250216':('America/Vancouver',),
- '1250217':('America/Vancouver',),
- '1250218':('America/Vancouver',),
  '357':('Asia/Nicosia',),
  '356':('Europe/Malta',),
  '355':('Europe/Tirane',),
  '354':('Atlantic/Reykjavik',),
  '353':('Europe/Dublin',),
  '352':('Europe/Luxembourg',),
  '351':('Atlantic/Azores', 'Europe/Lisbon'),
  '350':('Europe/Gibraltar',),
- '1423553':('America/New_York',),
  '359':('Europe/Sofia',),
  '358':('Europe/Helsinki', 'Europe/Mariehamn'),
  '1270678':('America/Chicago',),
  '8675':('Asia/Shanghai',),
  '1907622':('America/Juneau',),
  '1775473':('America/Los_Angeles',),
  '1775470':('America/Los_Angeles',),
- '1418332':('America/Toronto',),
  '52495':('America/Mexico_City',),
- '52494':('America/Mexico_City',),
+ '55913751':('America/Sao_Paulo',),
  '52496':('America/Mexico_City',),
  '1423790':('America/New_York',),
  '52493':('America/Mexico_City',),
  '52492':('America/Mexico_City',),
  '52499':('America/Mexico_City',),
  '52498':('America/Mexico_City',),
  '55913752':('America/Sao_Paulo',),
  '55913755':('America/Sao_Paulo',),
  '55913754':('America/Sao_Paulo',),
  '1605223':('America/Denver',),
- '1812659':('America/New_York',),
  '1605221':('America/Chicago',),
  '1605226':('America/Chicago',),
  '1605225':('America/Chicago',),
  '1605224':('America/Chicago',),
  '390942':('Europe/Rome',),
  '390941':('Europe/Rome',),
  '55913756':('America/Sao_Paulo',),
- '1812654':('America/New_York',),
- '1574277':('America/New_York',),
- '1574271':('America/New_York',),
- '1574273':('America/New_York',),
- '1574272':('America/New_York',),
  '52723':('America/Mexico_City',),
  '52722':('America/Mexico_City',),
  '52721':('America/Mexico_City',),
  '52727':('America/Mexico_City',),
  '52726':('America/Mexico_City',),
  '52725':('America/Mexico_City',),
  '52724':('America/Mexico_City',),
  '62984':('Asia/Jayapura',),
  '1423578':('America/New_York',),
- '62986':('Asia/Jayapura',),
+ '52729':('America/Mexico_City',),
  '52728':('America/Mexico_City',),
- '1418780':('America/Toronto',),
- '1418781':('America/Toronto',),
- '1418782':('America/Toronto',),
+ '62452':('Asia/Makassar',),
+ '62453':('Asia/Makassar',),
  '62451':('Asia/Makassar',),
  '55913072':('America/Sao_Paulo',),
  '55814042':('America/Sao_Paulo',),
- '55913073':('America/Sao_Paulo',),
  '86391':('Asia/Shanghai',),
- '1606237':('America/New_York',),
- '1620308':('America/Chicago',),
  '1208623':('America/Los_Angeles',),
- '1785632':('America/Chicago',),
- '1208624':('America/Denver',),
  '691320':('Pacific/Ponape',),
  '55919876':('America/Sao_Paulo',),
- '1701575':('America/Denver',),
+ '55919877':('America/Sao_Paulo',),
  '55919874':('America/Sao_Paulo',),
- '1701577':('America/Chicago',),
+ '55919875':('America/Sao_Paulo',),
  '55919872':('America/Sao_Paulo',),
  '55919873':('America/Sao_Paulo',),
- '1701572':('America/Chicago',),
+ '55919870':('America/Sao_Paulo',),
  '55919871':('America/Sao_Paulo',),
  '55813493':('America/Sao_Paulo',),
  '441429':('Europe/London',),
  '441428':('Europe/London',),
  '441423':('Europe/London',),
  '441422':('Europe/London',),
  '55913366':('America/Sao_Paulo',),
  '441420':('Europe/London',),
  '441427':('Europe/London',),
  '441425':('Europe/London',),
  '441424':('Europe/London',),
- '1785242':('America/Chicago',),
- '1785243':('America/Chicago',),
- '1785246':('America/Chicago',),
- '1850926':('America/New_York',),
  '1541476':('America/Los_Angeles',),
  '1541475':('America/Los_Angeles',),
  '1541474':('America/Los_Angeles',),
  '1541473':('America/Denver',),
  '1541472':('America/Los_Angeles',),
  '1541471':('America/Los_Angeles',),
  '1541479':('America/Los_Angeles',),
- '441408':('Europe/London',),
+ '1364':('America/New_York',),
+ '1365':('America/Toronto',),
  '1360':('America/Los_Angeles',),
  '1361':('America/Chicago',),
  '1709576':('America/St_Johns',),
  '1709579':('America/St_Johns',),
  '521221':('America/Mexico_City',),
  '521222':('America/Mexico_City',),
  '521223':('America/Mexico_City',),
  '521224':('America/Mexico_City',),
  '521225':('America/Mexico_City',),
  '521226':('America/Mexico_City',),
  '521227':('America/Mexico_City',),
  '521228':('America/Mexico_City',),
  '521229':('America/Mexico_City',),
  '1812485':('America/Chicago',),
- '1812486':('America/New_York',),
- '1812481':('America/New_York',),
- '1812482':('America/New_York',),
  '1208944':('America/Denver',),
  '55813731':('America/Sao_Paulo',),
  '55813732':('America/Sao_Paulo',),
  '55813733':('America/Sao_Paulo',),
  '55813734':('America/Sao_Paulo',),
  '55813735':('America/Sao_Paulo',),
  '298':('Atlantic/Faeroe',),
@@ -1887,126 +1574,113 @@
  '55813083':('America/Sao_Paulo',),
  '290':('Atlantic/St_Helena',),
  '291':('Africa/Asmera',),
  '691924':('Pacific/Ponape',),
  '691926':('Pacific/Ponape',),
  '691921':('Pacific/Ponape',),
  '691920':('Pacific/Ponape',),
- '55813887':('America/Sao_Paulo',),
  '55813551':('America/Sao_Paulo',),
  '55813552':('America/Sao_Paulo',),
  '55813553':('America/Sao_Paulo',),
  '55813559':('America/Sao_Paulo',),
  '390532':('Europe/Rome',),
  '390533':('Europe/Rome',),
- '1785404':('America/Chicago',),
+ '390536':('Europe/Rome',),
  '390534':('Europe/Rome',),
  '390535':('Europe/Rome',),
- '1785408':('America/Chicago',),
- '1620825':('America/Chicago',),
+ '55813747':('America/Sao_Paulo',),
  '7867':('Europe/Moscow',),
  '7866':('Europe/Moscow',),
  '7865':('Europe/Moscow',),
  '7863':('Europe/Moscow',),
  '7862':('Europe/Moscow',),
  '7861':('Europe/Moscow',),
  '55813741':('America/Sao_Paulo',),
  '7869':('Europe/Moscow',),
- '1208878':('America/Denver',),
  '1219956':('America/Chicago',),
- '55813742':('America/Sao_Paulo',),
+ '1250341':('America/Edmonton',),
  '1775737':('America/Los_Angeles',),
  '1775738':('America/Los_Angeles',),
  '62869':('Asia/Jakarta',),
- '1906475':('America/New_York',),
+ '62868':('Asia/Jakarta', 'Asia/Makassar'),
  '62867':('Asia/Jakarta',),
  '62866':('Asia/Jakarta',),
  '1423968':('America/New_York',),
  '62864':('Asia/Jakarta',),
  '62863':('Asia/Jakarta',),
  '62862':('Asia/Jakarta',),
  '62861':('Asia/Jakarta',),
  '62860':('Asia/Jakarta',),
  '86564':('Asia/Shanghai',),
  '86566':('Asia/Shanghai',),
  '86561':('Asia/Shanghai',),
  '86562':('Asia/Shanghai',),
- '86563':('Asia/Shanghai',),
+ '55819830':('America/Sao_Paulo',),
  '521797':('America/Mexico_City',),
  '1623':('America/Phoenix',),
  '521427':('America/Mexico_City',),
  '521424':('America/Mexico_City',),
- '521425':('America/Mexico_City',),
+ '1620':('America/Chicago',),
  '1208934':('America/Denver',),
  '1208935':('America/Los_Angeles',),
  '1208936':('America/Denver',),
  '521421':('America/Mexico_City',),
  '1208938':('America/Denver',),
  '1208939':('America/Denver',),
  '1629':('America/Chicago',),
- '1628':('America/Los_Angeles',),
- '1574594':('America/New_York',),
  '521428':('America/Mexico_City',),
  '521429':('America/Mexico_City',),
  '1541914':('America/Los_Angeles',),
  '1541915':('America/Los_Angeles',),
  '1541917':('America/Los_Angeles',),
  '1541912':('America/Los_Angeles',),
  '1541913':('America/Los_Angeles',),
  '86692':('Asia/Shanghai',),
  '1541318':('America/Los_Angeles',),
  '86691':('Asia/Shanghai',),
  '1541312':('America/Los_Angeles',),
  '554':('America/Sao_Paulo',),
- '557':('America/Sao_Paulo',),
+ '1541646':('America/Los_Angeles',),
  '1541647':('America/Los_Angeles',),
  '1541316':('America/Los_Angeles',),
  '1541317':('America/Los_Angeles',),
  '553':('America/Sao_Paulo',),
  '552':('America/Sao_Paulo',),
- '55819835':('America/Sao_Paulo',),
  '1907983':('America/Juneau',),
  '1423217':('America/New_York',),
  '521769':('America/Mexico_City',),
  '521768':('America/Mexico_City',),
  '521765':('America/Mexico_City',),
  '521764':('America/Mexico_City',),
  '521767':('America/Mexico_City',),
  '521766':('America/Mexico_City',),
  '1423218':('America/New_York',),
  '521763':('America/Mexico_City',),
  '521762':('America/Mexico_City',),
- '55819834':('America/Sao_Paulo',),
  '1423698':('America/New_York',),
  '1709364':('America/St_Johns',),
- '1418435':('America/Toronto',),
- '55819837':('America/Sao_Paulo',),
- '1418439':('America/Toronto',),
+ '9762362':('Asia/Choibalsan', 'Asia/Ulaanbaatar'),
+ '1423794':('America/New_York',),
  '1850269':('America/Chicago',),
  '1850263':('America/Chicago',),
  '1850261':('America/Chicago',),
  '1850592':('America/Chicago',),
  '1850267':('America/Chicago',),
- '441403':('Europe/London',),
  '1850265':('America/Chicago',),
  '1850596':('America/Chicago',),
  '1219791':('America/Chicago',),
  '1208201':('America/Denver',),
- '441409':('Europe/London',),
- '1418882':('America/Toronto',),
- '1418881':('America/Toronto',),
- '1345':('America/Cayman',),
- '1346':('America/Chicago',),
- '1347':('America/New_York',),
+ '1340':('America/St_Thomas',),
+ '441408':('Europe/London',),
+ '1219324':('America/Chicago',),
+ '1219322':('America/Chicago',),
  '55913117':('America/Sao_Paulo',),
  '55913116':('America/Sao_Paulo',),
  '55913115':('America/Sao_Paulo',),
- '1785989':('America/Chicago',),
  '55913110':('America/Sao_Paulo',),
- '1785985':('America/Chicago',),
  '55913119':('America/Sao_Paulo',),
  '55913118':('America/Sao_Paulo',),
  '378':('Europe/San_Marino',),
  '371':('Europe/Bucharest',),
  '370':('Europe/Bucharest',),
  '373':('Europe/Bucharest',),
  '372':('Europe/Bucharest',),
@@ -2014,82 +1688,68 @@
  '374':('Asia/Yerevan',),
  '377':('Europe/Monaco',),
  '376':('Europe/Andorra',),
  '52924':('America/Mexico_City',),
  '52921':('America/Mexico_City',),
  '52923':('America/Mexico_City',),
  '52922':('America/Mexico_City',),
- '1308865':('America/Chicago',),
+ '55933735':('America/Sao_Paulo',),
  '55933737':('America/Sao_Paulo',),
  '55933736':('America/Sao_Paulo',),
  '1270659':('America/Chicago',),
  '1270653':('America/Chicago',),
  '1270651':('America/Chicago',),
  '55933598':('America/Sao_Paulo',),
  '55933593':('America/Sao_Paulo',),
  '55933597':('America/Sao_Paulo',),
  '55933596':('America/Sao_Paulo',),
- '1418407':('America/Toronto',),
  '7718':('Asia/Almaty',),
  '1423778':('America/New_York',),
- '1418235':('America/Toronto',),
  '1423775':('America/New_York',),
  '1423772':('America/New_York',),
- '1418233':('America/Toronto',),
- '1907852':('America/Juneau',),
- '1250650':('America/Vancouver',),
+ '1423439':('America/New_York',),
+ '52415':('America/Mexico_City',),
  '1605209':('America/Denver',),
  '1605759':('America/Chicago',),
- '52414':('America/Mexico_City',),
  '1605755':('America/Denver',),
  '1605201':('America/Chicago',),
- '52417':('America/Mexico_City',),
  '62474':('Asia/Makassar',),
  '62471':('Asia/Makassar',),
  '62473':('Asia/Makassar',),
- '1250655':('America/Vancouver',),
  '52749':('America/Mexico_City',),
  '52748':('America/Mexico_City',),
- '1250656':('America/Vancouver',),
  '52741':('America/Mexico_City',),
  '52743':('America/Mexico_City',),
  '52742':('America/Mexico_City',),
  '52745':('America/Mexico_City',),
  '52744':('America/Mexico_City',),
  '52747':('America/Mexico_City',),
  '52746':('America/Mexico_City',),
- '1850942':('America/New_York',),
  '55814062':('America/Sao_Paulo',),
- '1850941':('America/Chicago',),
  '1850235':('America/Chicago',),
  '34949':('Europe/Madrid',),
  '34948':('Europe/Madrid',),
  '34947':('Europe/Madrid',),
  '34946':('Europe/Madrid',),
  '34945':('Europe/Madrid',),
- '1620492':('America/Chicago',),
+ '34944':('Europe/Madrid',),
  '34943':('Europe/Madrid',),
  '34942':('Europe/Madrid',),
- '1620365':('America/Chicago',),
- '1620364':('America/Chicago',),
- '1850233':('America/Chicago',),
+ '34941':('Europe/Madrid',),
+ '1850547':('America/Chicago',),
  '441395':('Europe/London',),
  '441394':('Europe/London',),
  '441397':('Europe/London',),
- '441393':('Europe/London',),
  '441392':('Europe/London',),
- '1812923':('America/New_York',),
- '1812926':('America/New_York',),
  '441398':('Europe/London',),
  '1812925':('America/Chicago',),
+ '55939991':('America/Sao_Paulo',),
  '55939990':('America/Sao_Paulo',),
  '1605977':('America/Chicago',),
  '55939995':('America/Sao_Paulo',),
- '1606256':('America/New_York',),
- '1606258':('America/New_York',),
  '55913342':('America/Sao_Paulo',),
  '55913343':('America/Sao_Paulo',),
  '1701883':('America/Chicago',),
  '55913346':('America/Sao_Paulo',),
  '55913347':('America/Sao_Paulo',),
  '55913344':('America/Sao_Paulo',),
  '55913345':('America/Sao_Paulo',),
@@ -2097,174 +1757,144 @@
  '8625':('Asia/Shanghai',),
  '55913348':('America/Sao_Paulo',),
  '55913349':('America/Sao_Paulo',),
  '8620':('Asia/Shanghai',),
  '8621':('Asia/Shanghai',),
  '8622':('Asia/Shanghai',),
  '8623':('Asia/Shanghai',),
- '55913753':('America/Sao_Paulo',),
  '86739':('Asia/Shanghai',),
  '86738':('Asia/Shanghai',),
- '1606668':('America/New_York',),
  '86731':('Asia/Shanghai',),
  '86730':('Asia/Shanghai',),
  '86735':('Asia/Shanghai',),
  '86734':('Asia/Shanghai',),
  '86737':('Asia/Shanghai',),
  '86736':('Asia/Shanghai',),
  '1541451':('America/Los_Angeles',),
  '1541450':('America/Los_Angeles',),
- '86914':('Asia/Shanghai',),
  '1541459':('America/Los_Angeles',),
  '1219362':('America/Chicago',),
- '1418594':('America/Toronto',),
- '1418849':('America/Toronto',),
- '1418848':('America/Toronto',),
- '1418847':('America/Toronto',),
- '1418598':('America/Toronto',),
+ '1219365':('America/Chicago',),
+ '1385':('America/Denver',),
  '1386':('America/New_York',),
- '1418844':('America/Toronto',),
- '1418843':('America/Toronto',),
- '1418842':('America/Toronto',),
- '1418841':('America/Toronto',),
- '1418840':('America/Toronto',),
+ '1380':('America/New_York',),
  '1850674':('America/Chicago',),
  '1850675':('America/Chicago',),
  '1850677':('America/Chicago',),
- '1850670':('America/New_York',),
- '1850671':('America/New_York',),
  '1709944':('America/Halifax',),
- '1812314':('America/New_York',),
  '1850678':('America/Chicago',),
  '86434':('Asia/Shanghai',),
  '86435':('Asia/Shanghai',),
  '521248':('America/Mexico_City',),
  '521249':('America/Mexico_City',),
  '521243':('America/Mexico_City',),
  '521241':('America/Mexico_City',),
  '521246':('America/Mexico_City',),
  '521247':('America/Mexico_City',),
  '521244':('America/Mexico_City',),
  '521245':('America/Mexico_City',),
- '62817':('Asia/Jakarta',),
- '86724':('Asia/Shanghai',),
- '62814':('Asia/Jakarta',),
  '1907452':('America/Juneau',),
  '1907451':('America/Juneau',),
  '1907457':('America/Juneau',),
  '1907456':('America/Juneau',),
  '1907455':('America/Juneau',),
  '1907459':('America/Juneau',),
  '1907458':('America/Juneau',),
- '1250395':('America/Vancouver',),
- '1250391':('America/Vancouver',),
- '1250390':('America/Vancouver',),
- '1250392':('America/Vancouver',),
+ '55813712':('America/Sao_Paulo',),
  '62815':('Asia/Jakarta',),
- '1250398':('America/Vancouver',),
  '55813719':('America/Sao_Paulo',),
  '62812':('Asia/Jakarta',),
  '55813576':('America/Sao_Paulo',),
  '55813577':('America/Sao_Paulo',),
  '52244':('America/Mexico_City',),
  '52245':('America/Mexico_City',),
  '52246':('America/Mexico_City',),
  '52247':('America/Mexico_City',),
  '52241':('America/Mexico_City',),
  '52243':('America/Mexico_City',),
  '52248':('America/Mexico_City',),
  '52249':('America/Mexico_City',),
- '1812866':('America/New_York',),
- '1785421':('America/Chicago',),
- '1785425':('America/Chicago',),
  '1219977':('America/Chicago',),
  '1219972':('America/Chicago',),
  '1775284':('America/Los_Angeles',),
- '62810':('Asia/Jakarta',),
+ '1775287':('America/Los_Angeles',),
  '1775289':('America/Los_Angeles',),
  '7844':('Europe/Moscow',),
  '7847':('Europe/Moscow',),
  '7846':('Europe/Samara',),
  '7841':('Europe/Moscow',),
  '7840':('Europe/Bucharest', 'Europe/Moscow'),
  '7843':('Europe/Moscow',),
  '7842':('Europe/Samara',),
- '1418380':('America/Toronto',),
- '1418386':('America/Toronto',),
  '1775753':('America/Los_Angeles',),
  '1775752':('America/Los_Angeles',),
  '1775751':('America/Los_Angeles',),
  '1775750':('America/Los_Angeles',),
  '1814':('America/New_York',),
  '1815':('America/Chicago',),
  '1816':('America/Chicago',),
  '1817':('America/Chicago',),
  '1810':('America/New_York',),
+ '1812':('America/New_York',),
  '1813':('America/New_York',),
  '1818':('America/Los_Angeles',),
  '1819':('America/Toronto',),
  '1423989':('America/New_York',),
- '1620805':('America/Chicago',),
- '1250858':('America/Vancouver',),
- '1906495':('America/New_York',),
- '1906493':('America/New_York',),
  '1270393':('America/Chicago',),
  '1270824':('America/Chicago',),
  '1270827':('America/Chicago',),
  '1270826':('America/Chicago',),
  '1270821':('America/Chicago',),
  '1270395':('America/Chicago',),
- '1270598':('America/Chicago',),
  '44131':('Europe/London',),
- '1270828':('America/New_York',),
+ '44130':('Europe/London',),
  '1609':('America/New_York',),
  '1608':('America/Chicago',),
  '1208918':('America/Denver',),
  '1979':('America/Chicago',),
  '1978':('America/New_York',),
  '1601':('America/Chicago',),
  '1603':('America/New_York',),
  '1602':('America/Denver',),
  '1973':('America/New_York',),
- '1604':('America/Vancouver',),
+ '1208917':('America/Denver',),
  '1607':('America/New_York',),
  '1970':('America/Denver',),
  '1541938':('America/Los_Angeles',),
  '1541937':('America/Los_Angeles',),
  '1541935':('America/Los_Angeles',),
+ '441624':('Europe/Isle_of_Man',),
  '521747':('America/Mexico_City',),
  '521746':('America/Mexico_City',),
  '521745':('America/Mexico_City',),
  '521744':('America/Mexico_City',),
+ '521743':('America/Mexico_City',),
  '521742':('America/Mexico_City',),
  '1867393':('America/Vancouver',),
  '521749':('America/Mexico_City',),
  '521748':('America/Mexico_City',),
  '1423238':('America/New_York',),
  '1423239':('America/New_York',),
+ '1423236':('America/New_York',),
  '1423234':('America/New_York',),
  '1423235':('America/New_York',),
  '1423232':('America/New_York',),
  '1423230':('America/New_York',),
  '34888':('Europe/Madrid',),
  '34882':('Europe/Madrid',),
  '34883':('Europe/Madrid',),
  '34880':('Europe/Madrid',),
  '34881':('Europe/Madrid',),
  '34886':('Europe/Madrid',),
  '34887':('Europe/Madrid',),
  '34884':('Europe/Madrid',),
  '34885':('Europe/Madrid',),
- '1418692':('America/Toronto',),
- '1418693':('America/Toronto',),
- '1208860':('America/Denver',),
- '1418459':('America/Toronto',),
  '521453':('America/Mexico_City',),
  '521452':('America/Mexico_City',),
- '521451':('America/Mexico_City',),
+ '52637':('America/Mazatlan',),
  '1541667':('America/Los_Angeles',),
  '1541664':('America/Los_Angeles',),
  '1541665':('America/Los_Angeles',),
  '1541663':('America/Los_Angeles',),
  '1541660':('America/Los_Angeles',),
  '521457':('America/Mexico_City',),
  '52633':('America/Mazatlan',),
@@ -2275,25 +1905,24 @@
  '1208262':('America/Los_Angeles',),
  '1208263':('America/Los_Angeles',),
  '1208265':('America/Los_Angeles',),
  '1208267':('America/Los_Angeles',),
  '55913287':('America/Sao_Paulo',),
  '55913286':('America/Sao_Paulo',),
  '55913285':('America/Sao_Paulo',),
- '1905':('America/Toronto',),
+ '55913284':('America/Sao_Paulo',),
  '55913283':('America/Sao_Paulo',),
  '55913282':('America/Sao_Paulo',),
  '55913281':('America/Sao_Paulo',),
  '52639':('America/Mazatlan',),
  '55913289':('America/Sao_Paulo',),
- '52638':('America/Mazatlan',),
- '52288':('America/Mexico_City',),
+ '1903':('America/Chicago',),
+ '1250423':('America/Edmonton',),
  '1541592':('America/Los_Angeles',),
  '1541593':('America/Los_Angeles',),
- '62958':('Asia/Jakarta',),
  '1541598':('America/Los_Angeles',),
  '55913131':('America/Sao_Paulo',),
  '1850244':('America/Chicago',),
  '1850240':('America/Chicago',),
  '1850243':('America/Chicago',),
  '1972':('America/Chicago',),
  '1850249':('America/Chicago',),
@@ -2301,20 +1930,14 @@
  '62852':('Asia/Jakarta',),
  '1270639':('America/Chicago',),
  '1308882':('America/Denver',),
  '86888':('Asia/Shanghai',),
  '86887':('Asia/Shanghai',),
  '86886':('Asia/Shanghai',),
  '86883':('Asia/Shanghai',),
- '1250614':('America/Vancouver',),
- '1250615':('America/Vancouver',),
- '1250612':('America/Vancouver',),
- '1250618':('America/Vancouver',),
- '1250619':('America/Vancouver',),
- '1785364':('America/Chicago',),
  '1423753':('America/New_York',),
  '1423752':('America/New_York',),
  '1423757':('America/New_York',),
  '1423756':('America/New_York',),
  '1605778':('America/Chicago',),
  '1605773':('America/Chicago',),
  '1605772':('America/Chicago',),
@@ -2329,375 +1952,315 @@
  '5281':('America/Mexico_City',),
  '62418':('Asia/Makassar',),
  '62419':('Asia/Makassar',),
  '1423538':('America/New_York',),
  '52769':('America/Mexico_City',),
  '52768':('America/Mexico_City',),
  '9765088':('Asia/Ulaanbaatar',),
- '55943326':('America/Sao_Paulo',),
- '521649':('America/Mazatlan',),
  '1605487':('America/Chicago',),
  '1605484':('America/Denver',),
  '55814007':('America/Sao_Paulo',),
  '55814004':('America/Sao_Paulo',),
  '55814003':('America/Sao_Paulo',),
  '55814002':('America/Sao_Paulo',),
  '55814001':('America/Sao_Paulo',),
  '55814009':('America/Sao_Paulo',),
- '1620345':('America/Chicago',),
- '1620347':('America/Chicago',),
- '1620341':('America/Chicago',),
- '1620340':('America/Chicago',),
- '1620343':('America/Chicago',),
- '1620342':('America/Chicago',),
- '1250949':('America/Vancouver',),
- '521647':('America/Mazatlan', 'America/Tijuana'),
- '1250941':('America/Vancouver',),
  '7302':('Asia/Yakutsk',),
  '7301':('Asia/Irkutsk',),
  '441809':('Europe/London',),
- '1574946':('America/New_York',),
- '521644':('America/Mazatlan',),
+ '441808':('Europe/London',),
  '441805':('Europe/London',),
  '441807':('Europe/London',),
  '441806':('Europe/London',),
  '441803':('Europe/London',),
  '1701530':('America/Chicago',),
- '1423631':('America/New_York',),
- '521643':('America/Mazatlan',),
+ '1701532':('America/Chicago',),
+ '1605951':('America/Chicago',),
+ '1308352':('America/Denver',),
+ '1701854':('America/Chicago',),
  '1541432':('America/Los_Angeles',),
  '1541431':('America/Los_Angeles',),
+ '1541430':('America/Los_Angeles',),
+ '1541436':('America/Los_Angeles',),
  '1541434':('America/Los_Angeles',),
- '1418868':('America/Toronto',),
  '1219345':('America/Chicago',),
- '1418860':('America/Toronto',),
- '1418863':('America/Toronto',),
- '1418862':('America/Toronto',),
- '1418867':('America/Toronto',),
  '1850659':('America/Chicago',),
- '1850656':('America/New_York',),
  '1850654':('America/Chicago',),
  '1709533':('America/St_Johns',),
  '1709535':('America/St_Johns',),
  '1850650':('America/Chicago',),
  '1850651':('America/Chicago',),
- '1701854':('America/Chicago',),
+ '55813416':('America/Sao_Paulo',),
  '1907479':('America/Juneau',),
  '55813413':('America/Sao_Paulo',),
  '1907474':('America/Juneau',),
  '55813771':('America/Sao_Paulo',),
- '1785392':('America/Chicago',),
- '1250378':('America/Vancouver',),
- '1250377':('America/Vancouver',),
- '1250376':('America/Vancouver',),
- '1250374':('America/Vancouver',),
- '1250372':('America/Vancouver',),
- '1250371':('America/Vancouver',),
- '1250370':('America/Vancouver',),
  '55813419':('America/Sao_Paulo',),
  '6896':('Pacific/Tahiti',),
+ '1219398':('America/Chicago',),
  '441495':('Europe/London',),
  '52222':('America/Mexico_City',),
  '52223':('America/Mexico_City',),
  '52221':('America/Mexico_City',),
  '52226':('America/Mexico_City',),
  '52227':('America/Mexico_City',),
  '52224':('America/Mexico_City',),
  '52225':('America/Mexico_City',),
  '52228':('America/Mexico_City',),
  '52229':('America/Mexico_City',),
+ '1430':('America/Chicago',),
  '55914042':('America/Sao_Paulo',),
  '7821':('Europe/Moscow',),
  '7820':('Europe/Moscow',),
  '55913423':('America/Sao_Paulo',),
  '55913425':('America/Sao_Paulo',),
- '55913424':('America/Sao_Paulo',),
  '55913429':('America/Sao_Paulo',),
  '52599':('America/Mexico_City',),
- '1219397':('America/Chicago',),
  '52591':('America/Mexico_City',),
  '52592':('America/Mexico_City',),
  '52593':('America/Mexico_City',),
  '52594':('America/Mexico_City',),
  '52595':('America/Mexico_City',),
  '52596':('America/Mexico_City',),
  '52597':('America/Mexico_City',),
  '1775777':('America/Los_Angeles',),
  '1775771':('America/Los_Angeles',),
  '1775770':('America/Los_Angeles',),
  '1775772':('America/Los_Angeles',),
- '1775778':('America/Los_Angeles',),
+ '1605543':('America/Chicago',),
  '1832':('America/Chicago',),
  '1830':('America/Chicago',),
  '1831':('America/Los_Angeles',),
  '1838':('America/New_York',),
- '1812735':('America/New_York',),
- '1812734':('America/New_York',),
- '1812738':('America/New_York',),
+ '1423202':('America/New_York',),
  '44118':('Europe/London',),
  '44113':('Europe/London',),
  '86523':('Asia/Shanghai',),
  '44117':('Europe/London',),
  '44116':('Europe/London',),
  '44115':('Europe/London',),
  '44114':('Europe/London',),
  '1954':('America/New_York',),
  '1956':('America/Chicago',),
  '1951':('America/Los_Angeles',),
  '1952':('America/Chicago',),
- '1574551':('America/New_York',),
+ '1959':('America/New_York',),
  '521468':('America/Mexico_City',),
  '521469':('America/Mexico_City',),
  '521462':('America/Mexico_City',),
  '521463':('America/Mexico_City',),
+ '1219393':('America/Chicago',),
  '521461':('America/Mexico_City',),
  '521466':('America/Mexico_City',),
  '521467':('America/Mexico_City',),
  '521464':('America/Mexico_City',),
  '521465':('America/Mexico_City',),
- '1812275':('America/New_York',),
  '1541951':('America/Los_Angeles',),
  '1541953':('America/Los_Angeles',),
  '1541954':('America/Los_Angeles',),
  '1541955':('America/Los_Angeles',),
  '1541956':('America/Los_Angeles',),
  '1541957':('America/Los_Angeles',),
- '618':('Australia/Adelaide', 'Australia/Perth'),
- '1606598':('America/New_York',),
- '1606599':('America/New_York',),
+ '1208569':('America/Denver',),
+ '521721':('America/Mexico_City',),
+ '62754':('Asia/Jakarta',),
  '521723':('America/Mexico_City',),
  '1480':('America/Denver',),
  '521725':('America/Mexico_City',),
  '521724':('America/Mexico_City',),
  '521727':('America/Mexico_City',),
  '1484':('America/New_York',),
  '521728':('America/Mexico_City',),
  '1574772':('America/Chicago',),
- '1606593':('America/New_York',),
  '62759':('Asia/Jakarta',),
  '62758':('Asia/Jakarta',),
  '1423253':('America/New_York',),
  '1423254':('America/New_York',),
  '1423257':('America/New_York',),
- '1812278':('America/New_York',),
- '1208562':('America/Denver',),
- '1606735':('America/New_York',),
- '1606738':('America/New_York',),
- '1606739':('America/New_York',),
+ '1270':('America/New_York',),
+ '613':('Australia/Sydney',),
+ '1219707':('America/Chicago',),
  '1208798':('America/Los_Angeles',),
  '1208799':('America/Los_Angeles',),
  '1208297':('America/Denver',),
  '1208791':('America/Los_Angeles',),
  '1208794':('America/Denver',),
- '1418475':('America/Toronto',),
  '390131':('Europe/Rome',),
  '1541601':('America/Los_Angeles',),
  '1541602':('America/Los_Angeles',),
+ '1541604':('America/Los_Angeles',),
  '1541606':('America/Los_Angeles',),
  '1541607':('America/Los_Angeles',),
  '1541608':('America/Los_Angeles',),
- '55913272':('America/Sao_Paulo',),
  '1208242':('America/Denver',),
  '1226':('America/Toronto',),
  '1208536':('America/Denver',),
  '1208241':('America/Denver',),
  '1223':('America/New_York',),
  '1208245':('America/Los_Angeles',),
+ '1208249':('America/Denver',),
  '1208538':('America/Denver',),
+ '1208539':('America/Denver',),
  '1229':('America/New_York',),
  '1219759':('America/Chicago',),
  '1701277':('America/Chicago',),
  '1701271':('America/Chicago',),
  '1219285':('America/Chicago',),
+ '1219286':('America/Chicago',),
  '5581989':('America/Sao_Paulo',),
  '5581988':('America/Sao_Paulo',),
  '5581987':('America/Sao_Paulo',),
  '5581986':('America/Sao_Paulo',),
  '5581985':('America/Sao_Paulo',),
  '5581984':('America/Sao_Paulo',),
  '5581982':('America/Sao_Paulo',),
  '5581981':('America/Sao_Paulo',),
- '1250845':('America/Vancouver',),
- '55913279':('America/Sao_Paulo',),
+ '1701241':('America/Chicago',),
+ '521785':('America/Mexico_City',),
  '1423547':('America/New_York',),
  '1423543':('America/New_York',),
  '52961':('America/Mexico_City',),
  '52963':('America/Mexico_City',),
  '52962':('America/Mexico_City',),
  '52965':('America/Mexico_City',),
  '52964':('America/Mexico_City',),
  '52967':('America/Mexico_City',),
  '52966':('America/Mexico_City',),
  '52969':('America/Mexico_City',),
  '52968':('America/Mexico_City',),
+ '1270618':('America/Chicago',),
  '62443':('Asia/Makassar',),
- '52347':('America/Mexico_City',),
- '1250585':('America/Vancouver',),
- '1250586':('America/Vancouver',),
- '52346':('America/Mexico_City',),
- '52341':('America/Mexico_City',),
- '1250588':('America/Vancouver',),
- '1250589':('America/Vancouver',),
- '52343':('America/Mexico_City',),
- '1250767':('America/Vancouver',),
  '5937':('America/Guayaquil',),
  '5936':('America/Guayaquil',),
  '5935':('America/Guayaquil',),
  '5934':('America/Guayaquil',),
  '5933':('America/Guayaquil',),
  '5932':('America/Guayaquil',),
  '1423733':('America/New_York',),
  '1423884':('America/New_York',),
- '1418272':('America/Toronto',),
  '1423886':('America/New_York',),
- '1423881':('America/Chicago',),
- '1418275':('America/Toronto',),
- '1250638':('America/Vancouver',),
+ '1423735':('America/New_York',),
  '3496':('Europe/Madrid',),
  '3495':('Europe/Madrid',),
- '1250632':('America/Vancouver',),
  '3493':('Europe/Madrid',),
  '3491':('Europe/Madrid',),
- '55913724':('America/Sao_Paulo',),
+ '227':('Africa/Niamey',),
  '55913725':('America/Sao_Paulo',),
  '55913726':('America/Sao_Paulo',),
  '55913727':('America/Sao_Paulo',),
  '1605717':('America/Denver',),
  '1605716':('America/Denver',),
  '1605719':('America/Denver',),
  '1605718':('America/Denver',),
  '55913721':('America/Sao_Paulo',),
  '55913184':('America/Sao_Paulo',),
  '1907646':('America/Juneau',),
  '55913722':('America/Sao_Paulo',),
  '1907644':('America/Juneau',),
  '55913723':('America/Sao_Paulo',),
  '62438':('Asia/Makassar',),
- '441680':('Europe/London',),
  '52789':('America/Mexico_City',),
  '62929':('Asia/Jayapura',),
  '52785':('America/Mexico_City',),
  '52784':('America/Mexico_City',),
  '62432':('Asia/Makassar',),
  '52786':('America/Mexico_City',),
  '52781':('America/Mexico_City',),
  '62435':('Asia/Makassar',),
  '52783':('America/Mexico_City',),
  '52782':('America/Mexico_City',),
  '55913182':('America/Sao_Paulo',),
  '55814020':('America/Sao_Paulo',),
- '1250964':('America/Vancouver',),
- '1250962':('America/Vancouver',),
- '1250963':('America/Vancouver',),
- '1250960':('America/Vancouver',),
- '1250961':('America/Vancouver',),
  '441827':('Europe/London',),
  '86393':('Asia/Shanghai',),
  '441825':('Europe/London',),
  '441824':('Europe/London',),
  '441823':('Europe/London',),
  '441822':('Europe/London',),
  '441821':('Europe/London',),
  '7365':('Europe/Moscow',),
  '441829':('Europe/London',),
  '441828':('Europe/London',),
- '1574968':('America/New_York',),
- '1574967':('America/New_York',),
  '86395':('Asia/Shanghai',),
  '55943301':('America/Sao_Paulo',),
- '55943305':('America/Sao_Paulo',),
  '55943309':('America/Sao_Paulo',),
- '1606929':('America/New_York',),
- '1606928':('America/New_York',),
  '1308254':('America/Denver',),
+ '441522':('Europe/London',),
  '1541414':('America/Los_Angeles',),
  '1541416':('America/Los_Angeles',),
  '1541410':('America/Los_Angeles',),
  '1541412':('America/Los_Angeles',),
  '1541419':('America/Los_Angeles',),
- '52696':('America/Mazatlan',),
+ '1208954':('America/Denver',),
  '1208955':('America/Denver',),
- '1418802':('America/Toronto',),
- '1418800':('America/Toronto',),
- '1418809':('America/Toronto',),
+ '1867587':('America/Edmonton',),
  '1850638':('America/Chicago',),
  '1850639':('America/Chicago',),
  '1850637':('America/Chicago',),
  '521288':('America/Mexico_City',),
  '521287':('America/Mexico_City',),
  '521284':('America/Mexico_City',),
  '521285':('America/Mexico_City',),
  '521282':('America/Mexico_City',),
  '521283':('America/Mexico_City',),
  '521281':('America/Mexico_City',),
- '868078':('Asia/Shanghai',),
- '1308928':('America/Chicago',),
+ '1575':('America/Denver',),
  '55813020':('America/Sao_Paulo',),
  '55813021':('America/Sao_Paulo',),
- '55813023':('America/Sao_Paulo',),
- '55813025':('America/Sao_Paulo',),
+ '55813751':('America/Sao_Paulo',),
+ '55813757':('America/Sao_Paulo',),
  '441599':('Europe/London',),
- '441598':('Europe/London',),
+ '55813755':('America/Sao_Paulo',),
  '441597':('Europe/London',),
- '441595':('Europe/London',),
- '441594':('Europe/London',),
+ '55813758':('America/Sao_Paulo',),
+ '55913073':('America/Sao_Paulo',),
  '441593':('Europe/London',),
- '441592':('Europe/London',),
+ '55913075':('America/Sao_Paulo',),
  '441591':('Europe/London',),
  '441590':('Europe/London',),
- '1250353':('America/Vancouver',),
- '1250352':('America/Vancouver',),
- '1250354':('America/Vancouver',),
- '1250357':('America/Vancouver',),
- '1250356':('America/Vancouver',),
  '52200':('America/Mexico_City', 'America/Tijuana'),
  '52201':('America/Mexico_City', 'America/New_York'),
  '1775577':('America/Los_Angeles',),
  '1775575':('America/Los_Angeles',),
- '55813004':('America/Sao_Paulo',),
  '1219938':('America/Chicago',),
  '1219939':('America/Chicago',),
  '1219932':('America/Chicago',),
  '1219933':('America/Chicago',),
  '1219931':('America/Chicago',),
  '1219937':('America/Chicago',),
  '1219934':('America/Chicago',),
- '1250336':('America/Vancouver',),
- '1250335':('America/Vancouver',),
- '55817904':('America/Sao_Paulo',),
  '55817908':('America/Sao_Paulo',),
  '1605528':('America/Chicago',),
  '1858':('America/Los_Angeles',),
  '1859':('America/New_York',),
- '1418392':('America/Toronto',),
- '1418397':('America/Toronto',),
+ '1850':('America/New_York',),
+ '1854':('America/New_York',),
  '1856':('America/New_York',),
  '1857':('America/New_York',),
- '62715':('Asia/Jakarta',),
- '62265':('Asia/Jakarta',),
+ '521783':('America/Mexico_City',),
  '62264':('Asia/Jakarta',),
  '62267':('Asia/Jakarta',),
  '521444':('America/Mexico_City',),
  '521917':('America/Mexico_City',),
  '1931':('America/Chicago',),
  '521447':('America/Mexico_City',),
  '1937':('America/New_York',),
  '1936':('America/Chicago',),
  '521442':('America/Mexico_City',),
  '521443':('America/Mexico_City',),
- '1208484':('America/Denver',),
+ '62261':('Asia/Jakarta',),
  '1939':('America/Puerto_Rico',),
+ '1938':('America/Chicago',),
  '521448':('America/Mexico_City',),
  '521449':('America/Mexico_City',),
  '521918':('America/Mexico_City',),
- '521919':('America/Mexico_City',),
+ '62260':('Asia/Jakarta',),
  '1541973':('America/Los_Angeles',),
  '1541977':('America/Los_Angeles',),
  '62262':('Asia/Jakarta',),
- '1574753':('America/New_York',),
  '1423272':('America/New_York',),
  '62772':('Asia/Jakarta',),
  '62771':('Asia/Jakarta',),
  '62770':('Asia/Jakarta',),
  '62777':('Asia/Jakarta',),
  '62776':('Asia/Jakarta',),
  '1907929':('America/Juneau',),
@@ -2709,95 +2272,79 @@
  '34846':('Europe/Madrid',),
  '34847':('Europe/Madrid',),
  '34845':('Europe/Madrid',),
  '34843':('Europe/Madrid',),
  '34841':('Europe/Madrid',),
  '44172':('Europe/London',),
  '995':('Asia/Tbilisi',),
- '55919994':('America/Sao_Paulo',),
  '1541622':('America/Los_Angeles',),
  '1541621':('America/Los_Angeles',),
  '1219733':('America/Chicago',),
  '1209':('America/Los_Angeles',),
+ '1208':('America/Boise', 'America/Los_Angeles'),
  '1219736':('America/Chicago',),
  '1219738':('America/Chicago',),
  '1204':('America/Winnipeg',),
- '1207':('America/New_York',),
+ '1208514':('America/Denver',),
  '1206':('America/Los_Angeles',),
  '1201':('America/New_York',),
  '1203':('America/New_York',),
  '1202':('America/New_York',),
  '1701251':('America/Chicago',),
- '1701250':('America/Chicago',),
- '1701253':('America/Chicago',),
+ '55913242':('America/Sao_Paulo',),
+ '55913241':('America/Sao_Paulo',),
  '1701252':('America/Chicago',),
  '1701255':('America/Chicago',),
- '1701254':('America/Chicago',),
+ '55913246':('America/Sao_Paulo',),
  '55913245':('America/Sao_Paulo',),
- '1701256':('America/Chicago',),
+ '55913244':('America/Sao_Paulo',),
  '1701258':('America/Chicago',),
  '55913249':('America/Sao_Paulo',),
  '55913248':('America/Sao_Paulo',),
  '1351':('America/New_York',),
+ '55813139':('America/Sao_Paulo',),
  '441698':('Europe/London',),
  '441694':('Europe/London',),
  '441695':('Europe/London',),
  '441697':('Europe/London',),
  '441690':('Europe/London',),
  '441691':('Europe/London',),
  '441692':('Europe/London',),
- '1850286':('America/Chicago',),
- '1208896':('America/Denver',),
- '992':('Asia/Dushanbe',),
- '1574387':('America/New_York',),
- '441932':('Europe/London',),
- '441935':('Europe/London',),
- '1812526':('America/New_York',),
- '1812524':('America/New_York',),
- '1812522':('America/New_York',),
- '1812523':('America/New_York',),
- '1907345':('America/Juneau',),
- '55813079':('America/Sao_Paulo',),
- '55813481':('America/Sao_Paulo',),
- '55813486':('America/Sao_Paulo',),
- '1250658':('America/Vancouver',),
- '62719':('Asia/Jakarta',),
+ '1907346':('America/Juneau',),
+ '1907344':('America/Juneau',),
+ '1907343':('America/Juneau',),
  '52419':('America/Mexico_City',),
  '52418':('America/Mexico_City',),
  '1423869':('America/New_York',),
  '1423867':('America/New_York',),
- '1418253':('America/Toronto',),
- '1250652':('America/Vancouver',),
+ '52414':('America/Mexico_City',),
+ '52417':('America/Mexico_City',),
  '52411':('America/Mexico_City',),
  '1423710':('America/New_York',),
  '52413':('America/Mexico_City',),
  '52412':('America/Mexico_City',),
  '62718':('Asia/Jakarta',),
  '1605734':('America/Chicago',),
- '55813656':('America/Sao_Paulo',),
  '55813253':('America/Sao_Paulo',),
  '55813252':('America/Sao_Paulo',),
  '55813251':('America/Sao_Paulo',),
  '55813257':('America/Sao_Paulo',),
  '55813256':('America/Sao_Paulo',),
  '55813255':('America/Sao_Paulo',),
  '55813254':('America/Sao_Paulo',),
- '1423595':('America/New_York',),
  '390324':('Europe/Rome',),
  '390323':('Europe/Rome',),
  '390322':('Europe/Rome',),
  '390321':('Europe/Rome',),
- '1620382':('America/Chicago',),
  '1620384':('America/Denver',),
  '7346':('Asia/Yekaterinburg',),
  '7347':('Asia/Yekaterinburg',),
  '7345':('Asia/Yekaterinburg',),
  '7342':('Asia/Yekaterinburg',),
  '7343':('Asia/Yekaterinburg',),
- '55813073':('America/Sao_Paulo',),
  '7341':('Europe/Samara',),
  '7349':('Asia/Yekaterinburg',),
  '441841':('Europe/London',),
  '441840':('Europe/London',),
  '441843':('Europe/London',),
  '441842':('Europe/London',),
  '441845':('Europe/London',),
@@ -2808,183 +2355,155 @@
  '62902':('Asia/Jayapura',),
  '55943328':('America/Sao_Paulo',),
  '55943321':('America/Sao_Paulo',),
  '55943323':('America/Sao_Paulo',),
  '55943322':('America/Sao_Paulo',),
  '55943324':('America/Sao_Paulo',),
  '55943327':('America/Sao_Paulo',),
- '55814137':('America/Sao_Paulo',),
+ '55943326':('America/Sao_Paulo',),
  '1270965':('America/Chicago',),
  '1605990':('America/Chicago',),
  '1605995':('America/Chicago',),
  '1605997':('America/Chicago',),
  '1605996':('America/Chicago',),
- '1308352':('America/Denver',),
- '1308233':('America/Chicago',),
- '1308234':('America/Chicago',),
+ '55814137':('America/Sao_Paulo',),
  '1308235':('America/Denver',),
- '1308236':('America/Chicago',),
- '1308237':('America/Chicago',),
  '1812897':('America/Chicago',),
  '1709282':('America/Halifax',),
- '1606365':('America/New_York',),
- '1606364':('America/New_York',),
- '1418829':('America/Toronto',),
- '1418828':('America/Toronto',),
- '1418538':('America/Toronto',),
- '1418824':('America/Toronto',),
- '1418827':('America/Toronto',),
- '1418534':('America/Toronto',),
- '1418822':('America/Toronto',),
+ '55913765':('America/Sao_Paulo',),
+ '521937':('America/Mexico_City',),
+ '62715':('Asia/Jakarta',),
+ '1701390':('America/Chicago',),
  '1701391':('America/Chicago',),
  '8647':('Asia/Shanghai',),
  '8641':('Asia/Shanghai',),
- '599318':('America/Kralendijk',),
- '62714':('Asia/Jakarta',),
- '1785826':('America/Chicago',),
- '1785827':('America/Chicago',),
- '1250331':('America/Vancouver',),
- '1785825':('America/Chicago',),
- '1250337':('America/Vancouver',),
- '1785823':('America/Chicago',),
- '1785820':('America/Chicago',),
- '1250334':('America/Vancouver',),
- '1250339':('America/Vancouver',),
- '1250338':('America/Vancouver',),
- '1785828':('America/Chicago',),
- '62336':('Asia/Jakarta',),
- '1423907':('America/New_York',),
+ '351244':('Europe/Lisbon',),
+ '1850341':('America/Chicago',),
+ '55813004':('America/Sao_Paulo',),
+ '55813003':('America/Sao_Paulo',),
+ '55813000':('America/Sao_Paulo',),
+ '1208352':('America/Denver',),
  '1250489':('America/Edmonton',),
- '1250488':('America/Vancouver',),
- '1250487':('America/Vancouver',),
- '1250486':('America/Vancouver',),
- '1250480':('America/Vancouver',),
- '1250483':('America/Vancouver',),
  '1270797':('America/Chicago',),
  '1270796':('America/Chicago',),
  '1270793':('America/Chicago',),
+ '1270792':('America/Chicago',),
  '7':('Asia/Almaty', 'Asia/Anadyr', 'Asia/Aqtobe', 'Asia/Irkutsk', 'Asia/Kamchatka', 'Asia/Krasnoyarsk', 'Asia/Magadan', 'Asia/Novosibirsk', 'Asia/Omsk', 'Asia/Sakhalin', 'Asia/Vladivostok', 'Asia/Yakutsk', 'Asia/Yekaterinburg', 'Europe/Bucharest', 'Europe/Moscow', 'Europe/Samara'),
  '1270798':('America/Chicago',),
  '1907567':('America/Juneau',),
+ '1709466':('America/St_Johns',),
  '1907563':('America/Juneau',),
  '1907562':('America/Juneau',),
  '1907561':('America/Juneau',),
  '1907569':('America/Juneau',),
  '55913469':('America/Sao_Paulo',),
  '55913468':('America/Sao_Paulo',),
  '55913467':('America/Sao_Paulo',),
  '55913466':('America/Sao_Paulo',),
  '55913464':('America/Sao_Paulo',),
  '55913462':('America/Sao_Paulo',),
  '55913461':('America/Sao_Paulo',),
- '1270586':('America/Chicago',),
- '1270422':('America/New_York',),
  '86908':('Asia/Shanghai',),
  '86909':('Asia/Shanghai',),
  '86906':('Asia/Shanghai',),
  '86902':('Asia/Shanghai',),
  '86903':('Asia/Shanghai',),
  '86901':('Asia/Shanghai',),
  '1876':('America/Jamaica',),
  '1872':('America/Chicago',),
+ '1873':('America/Toronto',),
  '1870':('America/Chicago',),
+ '1878':('America/New_York',),
  '52626':('America/Hermosillo',),
- '52627':('America/Mazatlan',),
- '52624':('America/Mazatlan',),
+ '1918':('America/Chicago',),
+ '521932':('America/Mexico_City',),
  '52625':('America/Mazatlan',),
- '521934':('America/Mexico_City',),
+ '52622':('America/Mazatlan',),
  '52623':('America/Mazatlan',),
  '521936':('America/Mexico_City',),
  '52621':('America/Mazatlan',),
  '521938':('America/Mexico_City',),
  '1910':('America/New_York',),
  '1913':('America/Chicago',),
  '1912':('America/New_York',),
  '1915':('America/Denver',),
  '1914':('America/New_York',),
  '52628':('America/Mazatlan',),
- '52629':('America/Mazatlan',),
+ '1916':('America/Los_Angeles',),
  '1541998':('America/Los_Angeles',),
- '1541999':('America/Los_Angeles',),
+ '1250347':('America/Edmonton',),
  '1541994':('America/Los_Angeles',),
  '1541995':('America/Los_Angeles',),
  '1541996':('America/Los_Angeles',),
  '1541997':('America/Los_Angeles',),
  '1541990':('America/Los_Angeles',),
  '1541993':('America/Los_Angeles',),
  '880':('Asia/Dhaka',),
  '886':('Asia/Taipei',),
- '1606889':('America/New_York',),
- '1606886':('America/New_York',),
- '1620244':('America/Chicago',),
+ '1867334':('America/Vancouver',),
+ '34864':('Europe/Madrid',),
  '34865':('Europe/Madrid',),
- '34867':('Europe/Madrid',),
  '34860':('Europe/Madrid',),
- '1620241':('America/Chicago',),
  '34863':('Europe/Madrid',),
  '62711':('Asia/Jakarta',),
  '1423296':('America/New_York',),
  '62712':('Asia/Jakarta',),
  '34868':('Europe/Madrid',),
- '1620249':('America/Chicago',),
+ '62714':('Asia/Jakarta',),
  '62717':('Asia/Jakarta',),
  '62716':('Asia/Jakarta',),
- '1785597':('America/Chicago',),
- '1785594':('America/Chicago',),
  '1270881':('America/Chicago',),
  '1270887':('America/Chicago',),
  '1270886':('America/Chicago',),
  '1270885':('America/Chicago',),
  '44156':('Europe/London',),
  '1270889':('America/Chicago',),
  '44151':('Europe/London',),
  '1208755':('America/Los_Angeles',),
  '1208756':('America/Denver',),
  '1919':('America/New_York',),
- '1208899':('America/Denver',),
- '1918':('America/Chicago',),
+ '521648':('America/Mazatlan',),
+ '52627':('America/Mazatlan',),
  '390172':('Europe/Rome',),
  '390173':('Europe/Rome',),
- '1418668':('America/Toronto',),
- '521932':('America/Mexico_City',),
+ '1208898':('America/Denver',),
+ '52624':('America/Mazatlan',),
  '390174':('Europe/Rome',),
  '390175':('Europe/Rome',),
- '1418667':('America/Toronto',),
  '521933':('America/Mexico_City',),
- '1418666':('America/Toronto',),
- '52622':('America/Mazatlan',),
- '1418665':('America/Toronto',),
+ '1208896':('America/Denver',),
+ '521934':('America/Mexico_City',),
+ '521644':('America/Mazatlan',),
  '1208578':('America/Denver',),
  '55913268':('America/Sao_Paulo',),
  '1269':('America/New_York',),
  '1268':('America/Antigua',),
  '1208570':('America/Denver',),
- '1418663':('America/Toronto',),
+ '1208571':('America/Denver',),
  '55913263':('America/Sao_Paulo',),
- '521937':('America/Mexico_City',),
+ '55913262':('America/Sao_Paulo',),
  '1267':('America/New_York',),
  '55913264':('America/Sao_Paulo',),
- '1219242':('America/Chicago',),
- '1264':('America/Anguilla',),
+ '55913267':('America/Sao_Paulo',),
+ '55913266':('America/Sao_Paulo',),
  '1701239':('America/Chicago',),
  '1701238':('America/Chicago',),
- '1418661':('America/Toronto',),
  '1701232':('America/Chicago',),
  '1701231':('America/Chicago',),
  '521641':('America/Mazatlan',),
  '1701237':('America/Chicago',),
  '1701724':('America/Chicago',),
  '1701235':('America/Chicago',),
  '1701234':('America/Chicago',),
  '62428':('Asia/Makassar',),
  '1917':('America/New_York',),
- '1916':('America/Los_Angeles',),
+ '52629':('America/Mazatlan',),
  '55913199':('America/Sao_Paulo',),
- '1250434':('America/Vancouver',),
  '55913194':('America/Sao_Paulo',),
+ '1541999':('America/Los_Angeles',),
  '62426':('Asia/Makassar',),
  '1208286':('America/Denver',),
  '1208287':('America/Denver',),
  '1208284':('America/Denver',),
  '1208282':('America/Denver',),
  '1208283':('America/Denver',),
  '1208288':('America/Denver',),
@@ -2995,274 +2514,222 @@
  '521324':('America/Mazatlan',),
  '521327':('America/Mazatlan',),
  '521321':('America/Mexico_City',),
  '521323':('America/Mazatlan',),
  '521322':('America/Mexico_City',),
  '521329':('America/Mexico_City',),
  '521328':('America/Mexico_City',),
- '1812542':('America/New_York',),
  '1709722':('America/St_Johns',),
- '1850402':('America/New_York',),
- '1812546':('America/New_York',),
  '1812547':('America/Chicago',),
  '1709729':('America/St_Johns',),
  '55813499':('America/Sao_Paulo',),
  '55813498':('America/Sao_Paulo',),
  '55813495':('America/Sao_Paulo',),
  '55813494':('America/Sao_Paulo',),
  '55813497':('America/Sao_Paulo',),
  '1907357':('America/Juneau',),
- '1907350':('America/Juneau',),
+ '55813491':('America/Sao_Paulo',),
  '1907351':('America/Juneau',),
  '1907352':('America/Juneau',),
  '55813492':('America/Sao_Paulo',),
  '52438':('America/Mexico_City',),
  '52433':('America/Mexico_City',),
  '52432':('America/Mexico_City',),
  '1423843':('America/New_York',),
  '1423842':('America/New_York',),
  '52437':('America/Mexico_City',),
- '52436':('America/Mexico_City',),
+ '1423844':('America/New_York',),
  '52435':('America/Mexico_City',),
  '52434':('America/Mexico_City',),
- '1418678':('America/Toronto',),
  '1907683':('America/Juneau',),
  '1907688':('America/Juneau',),
  '55813271':('America/Sao_Paulo',),
  '55813273':('America/Sao_Paulo',),
  '55813272':('America/Sao_Paulo',),
  '55813274':('America/Sao_Paulo',),
- '86456':('Asia/Shanghai',),
+ '1605988':('America/Chicago',),
  '1807934':('America/Winnipeg',),
- '34864':('Europe/Madrid',),
+ '62719':('Asia/Jakarta',),
  '1219879':('America/Chicago',),
- '1620245':('America/Chicago',),
+ '1219878':('America/Chicago',),
  '1219874':('America/Chicago',),
  '1219873':('America/Chicago',),
  '1219872':('America/Chicago',),
- '1250672':('America/Vancouver',),
  '97611':('Asia/Ulaanbaatar',),
- '55913854':('America/Sao_Paulo',),
+ '97612':('Asia/Ulaanbaatar',),
  '97613':('Asia/Ulaanbaatar',),
  '97614':('Asia/Hovd',),
  '97615':('Asia/Ulaanbaatar',),
- '1250674':('America/Vancouver',),
- '1250675':('America/Vancouver',),
- '1250679':('America/Vancouver',),
- '55913859':('America/Sao_Paulo',),
  '390341':('Europe/Rome',),
  '390343':('Europe/Rome',),
  '390342':('Europe/Rome',),
  '390345':('Europe/Rome',),
  '390344':('Europe/Rome',),
  '390346':('Europe/Rome',),
- '1250923':('America/Vancouver',),
- '1250920':('America/Vancouver',),
  '62713':('Asia/Jakarta',),
- '5582':('America/Sao_Paulo',),
  '441869':('Europe/London',),
  '441863':('Europe/London',),
  '441862':('Europe/London',),
  '441866':('Europe/London',),
  '441865':('Europe/London',),
  '441864':('Europe/London',),
- '1906227':('America/New_York',),
- '1906226':('America/New_York',),
- '1906225':('America/New_York',),
+ '62962':('Asia/Jayapura',),
+ '62963':('Asia/Jakarta',),
  '62966':('Asia/Jayapura',),
  '62967':('Asia/Jayapura',),
- '1906553':('America/New_York',),
+ '1423595':('America/New_York',),
  '62969':('Asia/Jayapura',),
- '1906228':('America/New_York',),
  '1605312':('America/Chicago',),
- '1605310':('America/Chicago',),
+ '55943348':('America/Sao_Paulo',),
  '55943347':('America/Sao_Paulo',),
  '55943346':('America/Sao_Paulo',),
  '55943345':('America/Sao_Paulo',),
  '55943344':('America/Sao_Paulo',),
  '55943342':('America/Sao_Paulo',),
  '55943341':('America/Sao_Paulo',),
  '1541836':('America/Los_Angeles',),
  '1541830':('America/Los_Angeles',),
  '1541839':('America/Los_Angeles',),
- '868081':('Asia/Shanghai',),
- '1574656':('America/New_York',),
  '1850982':('America/Chicago',),
  '1850983':('America/Chicago',),
  '1850981':('America/Chicago',),
- '1574658':('America/New_York',),
  '1423337':('America/New_York',),
  '1423336':('America/New_York',),
  '1423334':('America/New_York',),
  '1423332':('America/New_York',),
- '1219427':('America/Chicago',),
+ '1423339':('America/New_York',),
  '1423338':('America/New_York',),
- '1606340':('America/New_York',),
- '1606346':('America/New_York',),
- '1606349':('America/New_York',),
- '1606348':('America/New_York',),
- '1418673':('America/Toronto',),
  '52828':('America/Mexico_City',),
  '52829':('America/Mexico_City',),
  '1850368':('America/Chicago',),
  '1850362':('America/Chicago',),
  '1850361':('America/Chicago',),
  '62778':('Asia/Jakarta',),
  '52826':('America/Mexico_City',),
  '441488':('Europe/London',),
- '1308962':('America/Chicago',),
  '130824':('America/Denver',),
  '55813064':('America/Sao_Paulo',),
  '55813066':('America/Sao_Paulo',),
  '55813061':('America/Sao_Paulo',),
  '55813062':('America/Sao_Paulo',),
- '1785840':('America/Chicago',),
- '1785841':('America/Chicago',),
- '1785842':('America/Chicago',),
- '1785843':('America/Chicago',),
- '1250319':('America/Vancouver',),
- '1250318':('America/Vancouver',),
+ '55913031':('America/Sao_Paulo',),
  '55913032':('America/Sao_Paulo',),
  '55913033':('America/Sao_Paulo',),
- '1250314':('America/Vancouver',),
- '1250317':('America/Vancouver',),
  '55913038':('America/Sao_Paulo',),
  '55913039':('America/Sao_Paulo',),
  '7427':('Asia/Anadyr',),
  '7426':('Asia/Vladivostok',),
  '7424':('Asia/Magadan',),
  '7423':('Asia/Vladivostok',),
  '7421':('Asia/Vladivostok',),
  '55813688':('America/Sao_Paulo',),
  '55813689':('America/Sao_Paulo',),
  '1907543':('America/Juneau',),
- '1775200':('America/Los_Angeles',),
+ '55813681':('America/Sao_Paulo',),
  '55813682':('America/Sao_Paulo',),
  '55813683':('America/Sao_Paulo',),
  '55813684':('America/Sao_Paulo',),
  '55813685':('America/Sao_Paulo',),
  '55813686':('America/Sao_Paulo',),
  '55813687':('America/Sao_Paulo',),
  '55913445':('America/Sao_Paulo',),
  '55913444':('America/Sao_Paulo',),
- '1775232':('America/Los_Angeles',),
+ '55913447':('America/Sao_Paulo',),
  '55913446':('America/Sao_Paulo',),
  '55913441':('America/Sao_Paulo',),
  '55913443':('America/Sao_Paulo',),
  '55913442':('America/Sao_Paulo',),
  '55913449':('America/Sao_Paulo',),
  '55913448':('America/Sao_Paulo',),
- '1423794':('America/New_York',),
- '62526':('Asia/Jakarta', 'Asia/Makassar'),
- '1812288':('America/New_York',),
- '1812283':('America/New_York',),
- '1812282':('America/New_York',),
+ '52494':('America/Mexico_City',),
+ '62526':('Asia/Makassar',),
+ '1270443':('America/Chicago',),
+ '1270442':('America/Chicago',),
  '1270441':('America/Chicago',),
- '1812280':('America/New_York',),
- '1812285':('America/New_York',),
- '1812284':('America/New_York',),
+ '1270444':('America/Chicago',),
  '390171':('Europe/Rome',),
- '1308583':('America/Chicago',),
  '62527':('Asia/Makassar',),
- '1418356':('America/Toronto',),
- '1418353':('America/Toronto',),
  '1812753':('America/Chicago',),
- '1812752':('America/New_York',),
- '1620886':('America/Chicago',),
  '1423798':('America/New_York',),
- '1574825':('America/New_York',),
- '1574537':('America/New_York',),
- '1574534':('America/New_York',),
- '1574535':('America/New_York',),
  '521488':('America/Mexico_City',),
  '521489':('America/Mexico_City',),
  '521958':('America/Mexico_City',),
  '62553':('Asia/Makassar',),
  '521481':('America/Mexico_City',),
  '521482':('America/Mexico_City',),
  '521951':('America/Mexico_City',),
  '521485':('America/Mexico_City',),
  '521954':('America/Mexico_City',),
  '521487':('America/Mexico_City',),
  '55913269':('America/Sao_Paulo',),
  '1907966':('America/Juneau',),
- '52777':('America/Mexico_City',),
  '390481':('Europe/Rome',),
  '55913261':('America/Sao_Paulo',),
- '1208571':('America/Denver',),
- '1208573':('America/Denver',),
+ '1262':('America/Chicago',),
+ '1260':('America/New_York',),
  '55913265':('America/Sao_Paulo',),
- '55913267':('America/Sao_Paulo',),
- '62639':('Asia/Jakarta',),
- '1208577':('America/Denver',),
+ '1219242':('America/Chicago',),
+ '1264':('America/Anguilla',),
  '1605229':('America/Chicago',),
- '1606573':('America/New_York',),
  '1701742':('America/Chicago',),
  '351289':('Europe/Lisbon',),
  '1701746':('America/Chicago',),
  '1701212':('America/Chicago',),
- '351283':('Europe/Lisbon',),
+ '55913207':('America/Sao_Paulo',),
  '351282':('Europe/Lisbon',),
- '351281':('Europe/Lisbon',),
+ '55913205':('America/Sao_Paulo',),
  '1701748':('America/Chicago',),
- '351286':('Europe/Lisbon',),
+ '55913202':('America/Sao_Paulo',),
  '351285':('Europe/Lisbon',),
  '351284':('Europe/Lisbon',),
  '1270202':('America/Chicago',),
  '1775856':('America/Los_Angeles',),
  '1775857':('America/Los_Angeles',),
  '1775850':('America/Los_Angeles',),
  '1775851':('America/Los_Angeles',),
  '1775852':('America/Los_Angeles',),
  '1775853':('America/Los_Angeles',),
  '1208777':('America/Los_Angeles',),
- '1606756':('America/New_York',),
+ '1208772':('America/Los_Angeles',),
  '1208773':('America/Los_Angeles',),
- '1606754':('America/New_York',),
- '1606759':('America/New_York',),
  '55812101':('America/Sao_Paulo',),
  '55812102':('America/Sao_Paulo',),
  '55812103':('America/Sao_Paulo',),
  '55812104':('America/Sao_Paulo',),
  '1423570':('America/New_York',),
  '1423573':('America/New_York',),
  '1208552':('America/Denver',),
- '1418524':('America/Toronto',),
+ '1240':('America/New_York',),
  '643':('Pacific/Auckland',),
  '1534':('America/Chicago',),
- '1208556':('America/Los_Angeles',),
+ '1418986':('America/Halifax',),
  '1219263':('America/Chicago',),
- '647':('Pacific/Auckland',),
- '1530':('America/Los_Angeles',),
- '649':('Pacific/Auckland',),
+ '1531':('America/Chicago',),
+ '1246':('America/Barbados',),
+ '1249':('America/Toronto',),
  '1248':('America/New_York',),
  '1208558':('America/Denver',),
  '1208559':('America/Denver',),
- '1418789':('America/Toronto',),
- '1418831':('America/Toronto',),
+ '1539':('America/Chicago',),
  '62458':('Asia/Jakarta', 'Asia/Makassar'),
  '1850797':('America/Chicago',),
  '1850796':('America/Chicago',),
- '1418522':('America/Toronto',),
  '1850791':('America/Chicago',),
- '1541229':('America/Los_Angeles',),
+ '62457':('Asia/Makassar',),
  '1541226':('America/Los_Angeles',),
  '1541225':('America/Los_Angeles',),
  '1541222':('America/Los_Angeles',),
  '1541223':('America/Los_Angeles',),
  '1541221':('America/Los_Angeles',),
- '62452':('Asia/Makassar',),
- '1775358':('America/Los_Angeles',),
- '62453':('Asia/Makassar',),
+ '62980':('Asia/Jayapura',),
+ '1907490':('America/Juneau',),
+ '62981':('Asia/Jayapura',),
  '62983':('Asia/Jayapura',),
- '1850421':('America/New_York',),
  '1850420':('America/Chicago',),
  '1850423':('America/Chicago',),
- '1850422':('America/New_York',),
- '1850425':('America/New_York',),
  '1850424':('America/Chicago',),
  '1850429':('America/Chicago',),
  '1709747':('America/St_Johns',),
  '1709745':('America/St_Johns',),
  '1907376':('America/Juneau',),
  '1907374':('America/Juneau',),
  '1907375':('America/Juneau',),
@@ -3273,50 +2740,46 @@
  '1907378':('America/Juneau',),
  '55813473':('America/Sao_Paulo',),
  '55813472':('America/Sao_Paulo',),
  '55813471':('America/Sao_Paulo',),
  '55813477':('America/Sao_Paulo',),
  '55813476':('America/Sao_Paulo',),
  '55813475':('America/Sao_Paulo',),
- '1308532':('America/Chicago',),
- '52415':('America/Mexico_City',),
+ '55813474':('America/Sao_Paulo',),
+ '55813479':('America/Sao_Paulo',),
  '55813478':('America/Sao_Paulo',),
- '1308537':('America/Chicago',),
- '1308535':('America/Chicago',),
- '1308534':('America/Chicago',),
  '62434':('Asia/Makassar',),
  '441746':('Europe/London',),
  '441747':('Europe/London',),
  '441744':('Europe/London',),
  '441745':('Europe/London',),
  '441743':('Europe/London',),
  '441740':('Europe/London',),
  '55913733':('America/Sao_Paulo',),
  '441748':('Europe/London',),
  '441749':('Europe/London',),
  '55813217':('America/Sao_Paulo',),
  '55813216':('America/Sao_Paulo',),
  '55813214':('America/Sao_Paulo',),
  '55813213':('America/Sao_Paulo',),
- '55813212':('America/Sao_Paulo',),
+ '55913731':('America/Sao_Paulo',),
  '55913783':('America/Sao_Paulo',),
  '1219853':('America/Chicago',),
- '1219852':('America/Chicago',),
+ '55913781':('America/Sao_Paulo',),
  '55913784':('America/Sao_Paulo',),
  '52451':('America/Mexico_City',),
  '1423822':('America/New_York',),
  '52453':('America/Mexico_City',),
  '52452':('America/Mexico_City',),
  '52455':('America/Mexico_City',),
- '1250699':('America/Vancouver',),
+ '1423826':('America/New_York',),
  '1423825':('America/New_York',),
  '52456':('America/Mexico_City',),
  '52459':('America/Mexico_City',),
  '52458':('America/Mexico_City',),
- '1250692':('America/Vancouver',),
  '390369':('Europe/Rome',),
  '390363':('Europe/Rome',),
  '390362':('Europe/Rome',),
  '390365':('Europe/Rome',),
  '390364':('Europe/Rome',),
  '441337':('Europe/London',),
  '441335':('Europe/London',),
@@ -3329,134 +2792,111 @@
  '7381':('Asia/Omsk',),
  '441339':('Europe/London',),
  '7385':('Asia/Krasnoyarsk',),
  '9765006':('Asia/Ulaanbaatar',),
  '9765002':('Asia/Ulaanbaatar',),
  '9765000':('Asia/Ulaanbaatar',),
  '9765001':('Asia/Ulaanbaatar',),
- '62755':('Asia/Jakarta',),
  '55943365':('America/Sao_Paulo',),
  '55943364':('America/Sao_Paulo',),
  '55943366':('America/Sao_Paulo',),
- '55943369':('America/Sao_Paulo',),
  '1270928':('America/Chicago',),
  '1270929':('America/Chicago',),
- '1308398':('America/Chicago',),
  '1308394':('America/Denver',),
  '1270924':('America/Chicago',),
  '1270926':('America/Chicago',),
  '1270927':('America/Chicago',),
  '1867872':('America/Edmonton',),
  '1867873':('America/Edmonton',),
  '1867874':('America/Edmonton',),
  '1541812':('America/Los_Angeles',),
  '1541815':('America/Los_Angeles',),
  '62757':('Asia/Jakarta',),
+ '1541816':('America/Los_Angeles',),
  '1270879':('America/Chicago',),
- '1574675':('America/New_York',),
- '1574674':('America/New_York',),
- '1250442':('America/Vancouver',),
- '1620697':('America/Chicago',),
- '1620694':('America/Chicago',),
+ '62756':('Asia/Jakarta',),
  '1423317':('America/New_York',),
  '1423318':('America/New_York',),
  '62751':('Asia/Jakarta',),
- '1262':('America/Chicago',),
- '55933522':('America/Sao_Paulo',),
  '1630':('America/Chicago',),
  '1208922':('America/Denver',),
  '1208921':('America/Denver',),
- '1606329':('America/New_York',),
  '1985':('America/Chicago',),
- '1606327':('America/New_York',),
- '1606326':('America/New_York',),
- '1606325':('America/New_York',),
- '1606324':('America/New_York',),
+ '1775778':('America/Los_Angeles',),
  '1636':('America/Chicago',),
- '1260':('America/New_York',),
- '1850309':('America/New_York',),
  '1850301':('America/Chicago',),
  '62752':('Asia/Jakarta',),
  '1850306':('America/Chicago',),
  '1867695':('America/Edmonton',),
  '1989':('America/New_York',),
  '1701683':('America/Chicago',),
  '1541902':('America/Los_Angeles',),
  '1807468':('America/Winnipeg',),
  '1807467':('America/Winnipeg',),
  '55813040':('America/Sao_Paulo',),
- '55813041':('America/Sao_Paulo',),
+ '55913019':('America/Sao_Paulo',),
  '441539':('Europe/London',),
  '441538':('Europe/London',),
  '55813045':('America/Sao_Paulo',),
  '441535':('Europe/London',),
  '441534':('Europe/Jersey',),
  '55813048':('America/Sao_Paulo',),
- '441536':('Europe/London',),
+ '55813049':('America/Sao_Paulo',),
  '441531':('Europe/London',),
- '441530':('Europe/London',),
+ '55913017':('America/Sao_Paulo',),
  '55913014':('America/Sao_Paulo',),
  '55913015':('America/Sao_Paulo',),
- '1906847':('America/New_York',),
- '1785862':('America/Chicago',),
- '1785863':('America/Chicago',),
- '1785864':('America/Chicago',),
- '1785865':('America/Chicago',),
  '7401':('Europe/Bucharest',),
  '55819710':('America/Sao_Paulo',),
  '55819711':('America/Sao_Paulo',),
  '55819712':('America/Sao_Paulo',),
- '55813010':('America/Sao_Paulo',),
  '52846':('America/Mexico_City',),
  '52844':('America/Mexico_City',),
  '52845':('America/Mexico_City',),
  '52842':('America/Mexico_City',),
  '52841':('America/Mexico_City',),
- '1308946':('America/Chicago',),
- '1541306':('America/Los_Angeles',),
+ '1541654':('America/Los_Angeles',),
  '1907523':('America/Juneau',),
  '1907522':('America/Juneau',),
- '1785856':('America/Chicago',),
- '1270465':('America/New_York',),
  '86943':('Asia/Shanghai',),
  '86941':('Asia/Shanghai',),
  '1270462':('America/Chicago',),
- '1270469':('America/New_York',),
- '55919875':('America/Sao_Paulo',),
- '55913011':('America/Sao_Paulo',),
+ '1701575':('America/Denver',),
+ '1701577':('America/Chicago',),
  '1775267':('America/Los_Angeles',),
- '55919870':('America/Sao_Paulo',),
+ '1701572':('America/Chicago',),
  '1775265':('America/Los_Angeles',),
  '62531':('Asia/Jakarta',),
  '62532':('Asia/Jakarta',),
- '62535':('Asia/Jakarta', 'Asia/Makassar'),
+ '62535':('Asia/Jakarta',),
  '521971':('America/Mexico_City',),
  '521972':('America/Mexico_City',),
  '62536':('Asia/Jakarta',),
  '62539':('Asia/Jakarta', 'Asia/Makassar'),
  '62538':('Asia/Jakarta',),
  '52668':('America/Mazatlan',),
  '52669':('America/Mazatlan',),
  '52662':('America/Mazatlan',),
  '52661':('America/Tijuana',),
  '52667':('America/Mazatlan',),
  '52664':('America/Tijuana',),
  '52665':('America/Tijuana',),
- '62271':('Asia/Jakarta',),
+ '521779':('America/Mexico_City',),
  '1867993':('America/Vancouver',),
- '52454':('America/Mexico_City',),
  '34828':('Atlantic/Canary',),
+ '34820':('Europe/Madrid',),
  '34821':('Europe/Madrid',),
  '34822':('Atlantic/Canary',),
  '34823':('Europe/Madrid',),
  '34824':('Europe/Madrid',),
  '34825':('Europe/Madrid',),
  '34826':('Europe/Madrid',),
+ '34827':('Atlantic/Canary',),
  '1775482':('America/Los_Angeles',),
- '1574807':('America/New_York',),
+ '1671':('Pacific/Guam',),
  '55912992':('America/Sao_Paulo',),
  '55913225':('America/Sao_Paulo',),
  '55913224':('America/Sao_Paulo',),
  '55913227':('America/Sao_Paulo',),
  '55913226':('America/Sao_Paulo',),
  '55913221':('America/Sao_Paulo',),
  '55913223':('America/Sao_Paulo',),
@@ -3465,14 +2905,15 @@
  '1709726':('America/St_Johns',),
  '55913229':('America/Sao_Paulo',),
  '55913228':('America/Sao_Paulo',),
  '1775870':('America/Los_Angeles',),
  '55913181':('America/Sao_Paulo',),
  '1270265':('America/Chicago',),
  '1208713':('America/Denver',),
+ '1208716':('America/Denver',),
  '55812128':('America/Sao_Paulo',),
  '55812129':('America/Sao_Paulo',),
  '55812126':('America/Sao_Paulo',),
  '55812127':('America/Sao_Paulo',),
  '55812125':('America/Sao_Paulo',),
  '55812122':('America/Sao_Paulo',),
  '55812123':('America/Sao_Paulo',),
@@ -3485,80 +2926,68 @@
  '1515':('America/Chicago',),
  '1514':('America/Toronto',),
  '1517':('America/New_York',),
  '1516':('America/New_York',),
  '1510':('America/Los_Angeles',),
  '1513':('America/New_York',),
  '1512':('America/Chicago',),
- '1270699':('America/New_York',),
- '1270692':('America/New_York',),
  '1541241':('America/Los_Angeles',),
  '1541242':('America/Los_Angeles',),
  '1270691':('America/Chicago',),
  '1541244':('America/Los_Angeles',),
  '1541245':('America/Los_Angeles',),
  '1541246':('America/Los_Angeles',),
  '1541247':('America/Los_Angeles',),
- '55913817':('America/Sao_Paulo',),
- '1850443':('America/New_York',),
- '1850445':('America/New_York',),
  '1850444':('America/Chicago',),
  '55813459':('America/Sao_Paulo',),
  '55813458':('America/Sao_Paulo',),
  '1907317':('America/Juneau',),
  '55813451':('America/Sao_Paulo',),
- '55813491':('America/Sao_Paulo',),
+ '1907350':('America/Juneau',),
  '55813453':('America/Sao_Paulo',),
  '55813452':('America/Sao_Paulo',),
  '55813455':('America/Sao_Paulo',),
  '55813454':('America/Sao_Paulo',),
  '55813457':('America/Sao_Paulo',),
  '55813456':('America/Sao_Paulo',),
  '55813184':('America/Sao_Paulo',),
  '55813183':('America/Sao_Paulo',),
  '55813182':('America/Sao_Paulo',),
  '55813181':('America/Sao_Paulo',),
- '1418423':('America/Toronto',),
- '1418427':('America/Toronto',),
- '1418426':('America/Toronto',),
  '441760':('Europe/London',),
  '441761':('Europe/London',),
  '441763':('Europe/London',),
  '441764':('Europe/London',),
  '441765':('Europe/London',),
  '441766':('Europe/London',),
  '441767':('Europe/London',),
  '441768':('Europe/London',),
  '441769':('Europe/London',),
  '55813236':('America/Sao_Paulo',),
  '55813231':('America/Sao_Paulo',),
  '55813233':('America/Sao_Paulo',),
  '55813232':('America/Sao_Paulo',),
- '1250508':('America/Vancouver',),
- '1250505':('America/Vancouver',),
- '1250507':('America/Vancouver',),
  '52431':('America/Mexico_City',),
- '1250503':('America/Vancouver',),
- '1423844':('America/New_York',),
+ '52436':('America/Mexico_City',),
  '263':('Africa/Harare',),
  '262':('Indian/Mayotte', 'Indian/Reunion'),
  '261':('Indian/Antananarivo',),
  '260':('Africa/Lusaka',),
  '267':('Africa/Gaborone',),
- '1423847':('America/New_York',),
+ '266':('Africa/Maseru',),
  '265':('Africa/Blantyre',),
  '264':('Africa/Windhoek',),
  '1775674':('America/Los_Angeles',),
  '269':('Indian/Comoro',),
  '268':('Africa/Mbabane',),
  '1775673':('America/Los_Angeles',),
  '55913812':('America/Sao_Paulo',),
  '55913811':('America/Sao_Paulo',),
  '55913764':('America/Sao_Paulo',),
- '55913765':('America/Sao_Paulo',),
+ '55913817':('America/Sao_Paulo',),
  '55913767':('America/Sao_Paulo',),
  '52478':('America/Mexico_City',),
  '52477':('America/Mexico_City',),
  '52476':('America/Mexico_City',),
  '52475':('America/Mexico_City',),
  '52474':('America/Mexico_City',),
  '52473':('America/Mexico_City',),
@@ -3582,16 +3011,16 @@
  '1270904':('America/Chicago',),
  '1605353':('America/Chicago',),
  '1605352':('America/Chicago',),
  '1605351':('America/Chicago',),
  '1605357':('America/Chicago',),
  '1605356':('America/Chicago',),
  '1605355':('America/Denver',),
- '55814106':('America/Sao_Paulo',),
- '390588':('Europe/Rome',),
+ '1605384':('America/Chicago',),
+ '441668':('Europe/London',),
  '55814105':('America/Sao_Paulo',),
  '390836':('Europe/Rome',),
  '390835':('Europe/Rome',),
  '1541878':('America/Los_Angeles',),
  '390833':('Europe/Rome',),
  '390832':('Europe/Rome',),
  '390831':('Europe/Rome',),
@@ -3599,92 +3028,71 @@
  '441974':('Europe/London',),
  '441977':('Europe/London',),
  '441971':('Europe/London',),
  '441970':('Europe/London',),
  '441972':('Europe/London',),
  '441978':('Europe/London',),
  '1423378':('America/New_York',),
+ '1208484':('America/Denver',),
  '1907883':('America/Juneau',),
  '1701797':('America/Chicago',),
- '1385':('America/Denver',),
- '1418554':('America/Toronto',),
- '1620549':('America/Chicago',),
- '1785743':('America/Chicago',),
- '1785742':('America/Chicago',),
- '1620543':('America/Chicago',),
- '1785749':('America/Chicago',),
- '1620544':('America/Chicago',),
+ '1205':('America/Chicago',),
  '1208457':('America/Los_Angeles',),
  '1208455':('America/Denver',),
  '1208454':('America/Denver',),
  '1208453':('America/Denver',),
  '1208452':('America/Denver',),
  '1208459':('America/Denver',),
+ '1207':('America/New_York',),
  '1541499':('America/Los_Angeles',),
  '1709227':('America/St_Johns',),
  '1709229':('America/St_Johns',),
+ '1541497':('America/Los_Angeles',),
  '1541496':('America/Los_Angeles',),
  '1541490':('America/Los_Angeles',),
  '1219548':('America/Chicago',),
- '1785336':('America/Chicago',),
- '52297':('America/Mexico_City',),
- '1785332':('America/Chicago',),
- '1785331':('America/Chicago',),
+ '1701952':('America/Chicago',),
+ '1701400':('America/Chicago',),
+ '1323':('America/Los_Angeles',),
  '62463':('Asia/Makassar',),
  '1906863':('America/Chicago',),
  '1906864':('America/Chicago',),
  '5255':('America/Mexico_City',),
- '1850322':('America/New_York',),
- '1850320':('America/New_York',),
+ '1850855':('America/Chicago',),
  '1850857':('America/Chicago',),
  '1850327':('America/Chicago',),
  '1850324':('America/Chicago',),
- '1850325':('America/New_York',),
- '1850329':('America/New_York',),
  '1709596':('America/St_Johns',),
  '55819732':('America/Sao_Paulo',),
  '55819733':('America/Sao_Paulo',),
  '55819730':('America/Sao_Paulo',),
  '55819731':('America/Sao_Paulo',),
  '52864':('America/Mexico_City',),
  '52866':('America/Mexico_City',),
  '52867':('America/Mexico_City',),
  '1321':('America/New_York',),
  '52861':('America/Mexico_City',),
  '52862':('America/Mexico_City',),
  '52868':('America/Mexico_City',),
  '52869':('America/Mexico_City',),
- '1812849':('America/New_York',),
  '4732':('Europe/Oslo',),
  '4733':('Europe/Oslo',),
  '4731':('Europe/Oslo',),
  '4737':('Europe/Oslo',),
  '4735':('Europe/Oslo',),
  '1270487':('America/Chicago',),
- '1812246':('America/New_York',),
  '4738':('Europe/Oslo',),
- '1219878':('America/Chicago',),
  '1270483':('America/Chicago',),
- '1812242':('America/New_York',),
- '1250710':('America/Vancouver',),
- '1250712':('America/Vancouver',),
- '1250715':('America/Vancouver',),
- '1250714':('America/Vancouver',),
- '1250717':('America/Vancouver',),
- '1250716':('America/Vancouver',),
  '1250719':('America/Edmonton',),
- '1250718':('America/Vancouver',),
  '1325':('America/Chicago',),
  '52392':('America/Mexico_City',),
  '52393':('America/Mexico_City',),
  '52391':('America/Mexico_City',),
  '52394':('America/Mexico_City',),
  '52395':('America/Mexico_City',),
- '1812794':('America/New_York',),
- '55943314':('America/Sao_Paulo',),
  '1775246':('America/Los_Angeles',),
  '1775240':('America/Los_Angeles',),
  '52641':('America/Mazatlan',),
  '52642':('America/Mazatlan',),
  '52643':('America/Mazatlan',),
  '52644':('America/Mazatlan',),
  '52133':('America/Mexico_City',),
@@ -3694,77 +3102,59 @@
  '521997':('America/Mexico_City',),
  '521994':('America/Mexico_City',),
  '521995':('America/Mexico_City',),
  '521992':('America/Mexico_City',),
  '521993':('America/Mexico_City',),
  '62511':('Asia/Makassar',),
  '521991':('America/Mexico_City',),
- '1620223':('America/Chicago',),
- '1620221':('America/Chicago',),
- '1620227':('America/Chicago',),
- '1620225':('America/Chicago',),
- '1620229':('America/Chicago',),
- '1250929':('America/Vancouver',),
- '1785539':('America/Chicago',),
  '390444':('Europe/Rome',),
- '1785537':('America/Chicago',),
+ '390445':('Europe/Rome',),
  '390442':('Europe/Rome',),
- '1785532':('America/Chicago',),
- '1574862':('America/New_York',),
- '1574523':('America/New_York',),
- '521659':('America/Mazatlan',),
- '521658':('America/Tijuana',),
- '1308455':('America/Chicago',),
- '55943222':('America/Sao_Paulo',),
- '1308452':('America/Chicago',),
- '1418903':('America/Toronto',),
+ '1208888':('America/Denver',),
  '521656':('America/Hermosillo',),
  '62568':('Asia/Jakarta',),
- '1418907':('America/Toronto',),
+ '1208880':('America/Denver',),
  '1270247':('America/Chicago',),
  '1270240':('America/Chicago',),
  '1270242':('America/Chicago',),
- '521652':('America/Mazatlan',),
+ '1208883':('America/Los_Angeles',),
  '62564':('Asia/Jakarta',),
- '1606796':('America/New_York',),
  '521924':('America/Mexico_City',),
- '1574282':('America/New_York',),
- '1574283':('America/New_York',),
  '62562':('Asia/Jakarta',),
- '1574288':('America/New_York',),
- '1574289':('America/New_York',),
  '62563':('Asia/Jakarta',),
  '1758':('America/St_Lucia',),
  '1208732':('America/Denver',),
  '1208733':('America/Denver',),
  '1208731':('America/Denver',),
  '1208736':('America/Denver',),
  '1208737':('America/Denver',),
  '1208734':('America/Denver',),
  '1208735':('America/Denver',),
  '1208596':('America/Los_Angeles',),
  '1284':('America/Tortola',),
  '1208595':('America/Denver',),
  '1281':('America/Chicago',),
+ '1283':('America/New_York',),
  '1289':('America/Toronto',),
- '1418948':('America/Toronto',),
  '521698':('America/Mazatlan',),
+ '1579':('America/Toronto',),
  '689':('Pacific/Gambier', 'Pacific/Marquesas', 'Pacific/Tahiti'),
  '688':('Pacific/Funafuti',),
  '1573':('America/Chicago',),
  '1208841':('America/Denver',),
  '1571':('America/New_York',),
- '1570':('America/New_York',),
+ '1208843':('America/Los_Angeles',),
  '1219226':('America/Chicago',),
  '1219227':('America/Chicago',),
  '1208846':('America/Denver',),
- '1208847':('America/Denver',),
+ '1574':('America/New_York',),
  '1541261':('America/Los_Angeles',),
  '1541266':('America/Los_Angeles',),
  '1541267':('America/Los_Angeles',),
+ '1541264':('America/Los_Angeles',),
  '1541265':('America/Los_Angeles',),
  '1541269':('America/Los_Angeles',),
  '521343':('America/Mexico_City',),
  '521342':('America/Mexico_City',),
  '521341':('America/Mexico_City',),
  '521347':('America/Mexico_City',),
  '521346':('America/Mexico_City',),
@@ -3781,128 +3171,97 @@
  '5999':('America/Curacao',),
  '5663':('America/Santiago',),
  '1907338':('America/Juneau',),
  '1907339':('America/Juneau',),
  '55813439':('America/Sao_Paulo',),
  '55813438':('America/Sao_Paulo',),
  '1907332':('America/Juneau',),
- '1907333':('America/Juneau',),
+ '55813436':('America/Sao_Paulo',),
  '55813435':('America/Sao_Paulo',),
  '55813434':('America/Sao_Paulo',),
  '1907336':('America/Juneau',),
  '1907337':('America/Juneau',),
  '1907334':('America/Juneau',),
  '1907335':('America/Juneau',),
  '521441':('America/Mexico_City',),
- '1785295':('America/Chicago',),
- '1785296':('America/Chicago',),
  '5667':('America/Santiago',),
  '5665':('America/Santiago',),
  '1807727':('America/Winnipeg',),
  '441708':('Europe/London',),
  '441709':('Europe/London',),
  '441702':('Europe/London',),
  '441700':('Europe/London',),
- '55943348':('America/Sao_Paulo',),
+ '1605310':('America/Chicago',),
  '441706':('Europe/London',),
  '441707':('Europe/London',),
  '441704':('Europe/London',),
- '1208585':('America/Denver',),
  '1775657':('America/Los_Angeles',),
- '55813316':('America/Sao_Paulo',),
  '55813088':('America/Sao_Paulo',),
  '55813089':('America/Sao_Paulo',),
- '7498':('Europe/Moscow',),
- '1574784':('America/New_York',),
  '245':('Atlantic/Reykjavik',),
  '244':('Africa/Luanda',),
  '247':('Atlantic/St_Helena',),
  '246':('Indian/Chagos',),
  '241':('Africa/Libreville',),
  '240':('Africa/Malabo',),
  '243':('Africa/Kinshasa', 'Africa/Lubumbashi'),
  '242':('Africa/Brazzaville',),
  '249':('Africa/Khartoum',),
  '248':('Indian/Mahe',),
  '55913746':('America/Sao_Paulo',),
- '55813317':('America/Sao_Paulo',),
  '55913744':('America/Sao_Paulo',),
  '55913741':('America/Sao_Paulo',),
- '55913262':('America/Sao_Paulo',),
- '1620272':('America/Chicago',),
  '55813080':('America/Sao_Paulo',),
  '55813081':('America/Sao_Paulo',),
  '7491':('Europe/Moscow',),
+ '62702':('Asia/Jakarta',),
  '441379':('Europe/London',),
  '441373':('Europe/London',),
  '441372':('Europe/London',),
  '441371':('Europe/London',),
  '441377':('Europe/London',),
  '441376':('Europe/London',),
  '441375':('Europe/London',),
- '1906249':('America/New_York',),
- '1906248':('America/New_York',),
  '1812474':('America/Chicago',),
  '1812475':('America/Chicago',),
  '1812476':('America/Chicago',),
  '1812477':('America/Chicago',),
  '1812471':('America/Chicago',),
  '1812473':('America/Chicago',),
- '1812478':('America/New_York',),
  '1812479':('America/Chicago',),
- '1574453':('America/New_York',),
- '1574457':('America/New_York',),
  '1541855':('America/Los_Angeles',),
  '1541857':('America/Los_Angeles',),
  '1541850':('America/Los_Angeles',),
- '55913266':('America/Sao_Paulo',),
  '1541858':('America/Los_Angeles',),
- '1574631':('America/New_York',),
  '441959':('Europe/London',),
  '441957':('Europe/London',),
  '441955':('Europe/London',),
  '441954':('Europe/London',),
  '441953':('Europe/London',),
  '441952':('Europe/London',),
  '441951':('Europe/London',),
  '441950':('Europe/London',),
  '1423425':('America/New_York',),
  '1423424':('America/New_York',),
  '1423422':('America/New_York',),
  '1423421':('America/New_York',),
  '55942103':('America/Sao_Paulo',),
  '55942101':('America/Sao_Paulo',),
- '62567':('Asia/Jakarta',),
  '1605374':('America/Denver',),
  '1605376':('America/Chicago',),
  '1605371':('America/Chicago',),
  '1605370':('America/Chicago',),
  '1605373':('America/Chicago',),
  '1208695':('America/Denver',),
  '1208697':('America/Denver',),
- '1606672':('America/New_York',),
  '1208691':('America/Los_Angeles',),
- '1606674':('America/New_York',),
- '1606677':('America/New_York',),
- '1606676':('America/New_York',),
- '1606679':('America/New_York',),
- '1606678':('America/New_York',),
  '1208699':('America/Los_Angeles',),
- '1620564':('America/Chicago',),
- '1620563':('America/Chicago',),
  '62565':('Asia/Jakarta',),
  '1270726':('America/Chicago',),
- '1785762':('America/Chicago',),
- '1785765':('America/Chicago',),
- '1250898':('America/Vancouver',),
- '1250899':('America/Vancouver',),
- '1250896':('America/Vancouver',),
- '1250897':('America/Vancouver',),
  '55812626':('America/Sao_Paulo',),
- '1250893':('America/Vancouver',),
  '1208473':('America/Denver',),
  '1208472':('America/Denver',),
  '1208475':('America/Denver',),
  '1208476':('America/Los_Angeles',),
  '1208478':('America/Denver',),
  '1208334':('America/Denver',),
  '1208761':('America/Denver',),
@@ -3918,91 +3277,67 @@
  '441573':('Europe/London',),
  '441572':('Europe/London',),
  '441575':('Europe/London',),
  '441577':('Europe/London',),
  '441576':('Europe/London',),
  '441579':('Europe/London',),
  '441578':('Europe/London',),
- '1785350':('America/Chicago',),
- '1785354':('America/Chicago',),
  '1701428':('America/Chicago',),
- '1785357':('America/Chicago',),
  '1701426':('America/Chicago',),
- '1208766':('America/Denver',),
+ '1701425':('America/Chicago',),
  '1850699':('America/Chicago',),
- '1850878':('America/New_York',),
- '1850692':('America/New_York',),
- '1850877':('America/New_York',),
  '1850874':('America/Chicago',),
- '1850875':('America/New_York',),
- '1850872':('America/Chicago',),
- '1850697':('America/New_York',),
+ '1850696':('America/Chicago',),
  '1850871':('America/Chicago',),
- '1606785':('America/New_York',),
- '390536':('Europe/Rome',),
- '9762362':('Asia/Choibalsan', 'Asia/Ulaanbaatar'),
- '1785979':('America/Chicago',),
  '380':('Europe/Bucharest',),
  '381':('Europe/Belgrade',),
  '382':('Europe/Podgorica',),
  '383':('Europe/Belgrade',),
  '385':('Europe/Zagreb',),
  '386':('Europe/Ljubljana',),
  '387':('Europe/Sarajevo',),
  '389':('Europe/Skopje',),
- '1812268':('America/New_York',),
  '4751':('Europe/Oslo',),
  '4752':('Europe/Oslo',),
  '4753':('Europe/Oslo',),
- '1812265':('America/New_York',),
  '4755':('Europe/Oslo',),
  '4756':('Europe/Oslo',),
  '4757':('Europe/Oslo',),
  '1907299':('America/Juneau',),
  '52483':('America/Mexico_City',),
- '1418338':('America/Toronto',),
  '86436':('Asia/Shanghai',),
- '1418335':('America/Toronto',),
- '1418337':('America/Toronto',),
- '1250770':('America/Vancouver',),
  '1250774':('America/Edmonton',),
- '1423339':('America/New_York',),
  '86437':('Asia/Shanghai',),
  '55813378':('America/Sao_Paulo',),
  '55813379':('America/Sao_Paulo',),
- '1418221':('America/Toronto',),
  '55813371':('America/Sao_Paulo',),
  '55813372':('America/Sao_Paulo',),
  '55813375':('America/Sao_Paulo',),
  '55813376':('America/Sao_Paulo',),
  '55813377':('America/Sao_Paulo',),
  '1850537':('America/Chicago',),
  '1605589':('America/Chicago',),
  '1605582':('America/Chicago',),
  '4763':('Europe/Oslo',),
  '1605584':('America/Denver',),
- '1620792':('America/Chicago',),
- '1620793':('America/Chicago',),
- '1620795':('America/Chicago',),
- '1812218':('America/New_York',),
  '390461':('Europe/Rome',),
  '390462':('Europe/Rome',),
  '390463':('Europe/Rome',),
  '390464':('Europe/Rome',),
  '390465':('Europe/Rome',),
  '6222':('Asia/Jakarta',),
- '1574848':('America/New_York',),
  '6221':('Asia/Jakarta',),
  '6224':('Asia/Jakarta',),
  '675':('Pacific/Port_Moresby',),
- '1574842':('America/New_York',),
  '6228':('Asia/Jakarta',),
  '676':('Pacific/Tongatapu',),
  '351292':('Atlantic/Azores',),
  '86431':('Asia/Shanghai',),
+ '673':('Asia/Brunei',),
+ '1308':('America/Chicago',),
  '86438':('Asia/Shanghai',),
  '86439':('Asia/Shanghai',),
  '1775832':('America/Los_Angeles',),
  '1775833':('America/Los_Angeles',),
  '1775830':('America/Los_Angeles',),
  '1775831':('America/Los_Angeles',),
  '86432':('Asia/Shanghai',),
@@ -4011,39 +3346,34 @@
  '1775':('America/Boise', 'America/Los_Angeles'),
  '1774':('America/New_York',),
  '1770':('America/New_York',),
  '1773':('America/Chicago',),
  '1772':('America/New_York',),
  '1779':('America/Chicago',),
  '1778':('America/Vancouver',),
- '86483':('Asia/Shanghai',),
  '1551':('America/New_York',),
  '1208863':('America/Denver',),
- '1418690':('America/Toronto',),
+ '1208860':('America/Denver',),
  '1208861':('America/Denver',),
- '1418696':('America/Toronto',),
+ '1208866':('America/Denver',),
  '1208867':('America/Denver',),
- '1418694':('America/Toronto',),
- '1418695':('America/Toronto',),
  '1559':('America/Los_Angeles',),
- '1418929':('America/Toronto',),
- '1418698':('America/Toronto',),
  '1208869':('America/Denver',),
  '1541289':('America/Los_Angeles',),
  '1541284':('America/Los_Angeles',),
  '1541286':('America/Los_Angeles',),
  '1541280':('America/Los_Angeles',),
  '1541282':('America/Los_Angeles',),
  '52734':('America/Mexico_City',),
  '62462':('Asia/Makassar',),
  '62461':('Asia/Makassar',),
  '1867777':('America/Edmonton',),
  '62465':('Asia/Makassar',),
  '62464':('Asia/Makassar',),
- '1850488':('America/New_York',),
+ '1423855':('America/New_York',),
  '1850484':('America/Chicago',),
  '1850482':('America/Chicago',),
  '1850481':('America/Chicago',),
  '1208315':('America/Denver',),
  '1208317':('America/Denver',),
  '1208313':('America/Denver',),
  '1208319':('America/Denver',),
@@ -4060,162 +3390,130 @@
  '441491':('Europe/London',),
  '441496':('Europe/London',),
  '441497':('Europe/London',),
  '441494':('Europe/London',),
  '1701858':('America/Chicago',),
  '1541342':('America/Los_Angeles',),
  '55913621':('America/Sao_Paulo',),
- '1250542':('America/Vancouver',),
- '1250544':('America/Vancouver',),
- '1250545':('America/Vancouver',),
- '1250546':('America/Vancouver',),
- '1250547':('America/Vancouver',),
- '1250549':('America/Vancouver',),
  '1775635':('America/Los_Angeles',),
  '1775636':('America/Los_Angeles',),
- '62868':('Asia/Jakarta', 'Asia/Makassar'),
  '55913728':('America/Sao_Paulo',),
  '55913729':('America/Sao_Paulo',),
  '229':('Africa/Porto-Novo',),
  '228':('Africa/Lome',),
- '227':('Africa/Niamey',),
+ '55913724':('America/Sao_Paulo',),
  '226':('Africa/Ouagadougou',),
  '225':('Africa/Abidjan',),
  '224':('Africa/Conakry',),
  '223':('Africa/Bamako',),
  '222':('Africa/Nouakchott',),
  '221':('Africa/Dakar',),
  '220':('Africa/Banjul',),
- '55813744':('America/Sao_Paulo',),
  '1270524':('America/Chicago',),
  '86392':('Asia/Shanghai',),
  '1270526':('America/Chicago',),
  '1270527':('America/Chicago',),
  '86396':('Asia/Shanghai',),
  '1270522':('America/Chicago',),
  '86394':('Asia/Shanghai',),
  '86398':('Asia/Shanghai',),
  '1270528':('America/Chicago',),
  '1907714':('America/Juneau',),
- '55813747':('America/Sao_Paulo',),
  '1308665':('America/Denver',),
- '55813613':('America/Sao_Paulo',),
- '868070':('Asia/Shanghai',),
- '55813611':('America/Sao_Paulo',),
- '1208580':('America/Denver',),
- '55813610':('America/Sao_Paulo',),
+ '86563':('Asia/Shanghai',),
+ '55813343':('America/Sao_Paulo',),
  '1812450':('America/Chicago',),
- '55813344':('America/Sao_Paulo',),
+ '55813616':('America/Sao_Paulo',),
  '390873':('Europe/Rome',),
  '390872':('Europe/Rome',),
  '390871':('Europe/Rome',),
  '390875':('Europe/Rome',),
  '390874':('Europe/Rome',),
  '441939':('Europe/London',),
  '441938':('Europe/London',),
- '1574389':('America/New_York',),
- '1606478':('America/New_York',),
  '441931':('Europe/London',),
- '1606476':('America/New_York',),
  '441933':('Europe/London',),
- '1606474':('America/New_York',),
- '1606473':('America/New_York',),
+ '441932':('Europe/London',),
+ '441935':('Europe/London',),
  '441934':('Europe/London',),
  '441937':('Europe/London',),
- '86156':('Asia/Shanghai',),
+ '1423402':('America/New_York',),
  '1907841':('America/Juneau',),
  '1907842':('America/Juneau',),
  '1254':('America/Chicago',),
  '1208546':('America/Denver',),
  '1605399':('America/Denver',),
  '1605397':('America/Chicago',),
- '1252':('America/New_York',),
+ '1520':('America/Denver',),
  '55814131':('America/Sao_Paulo',),
  '1605394':('America/Denver',),
  '1605393':('America/Denver',),
  '1605391':('America/Denver',),
  '1605390':('America/Denver',),
  '521426':('America/Mexico_City',),
+ '1250':('America/Vancouver',),
  '1208678':('America/Denver',),
  '1208677':('America/Denver',),
  '1208676':('America/Los_Angeles',),
  '1251':('America/Chicago',),
  '1208672':('America/Denver',),
- '55813000':('America/Sao_Paulo',),
+ '521425':('America/Mexico_City',),
  '521422':('America/Mexico_City',),
- '1620585':('America/Chicago',),
- '1620584':('America/Chicago',),
- '1620583':('America/Chicago',),
- '1620582':('America/Chicago',),
  '1626':('America/Los_Angeles',),
  '1812874':('America/Chicago',),
- '1812875':('America/New_York',),
- '1812876':('America/New_York',),
- '1812877':('America/New_York',),
+ '237':('Africa/Douala',),
  '1208419':('America/Denver',),
  '1208412':('America/Denver',),
  '1208414':('America/Denver',),
  '1701628':('America/Chicago',),
  '1701627':('America/Chicago',),
  '1701623':('America/Denver',),
  '1605823':('America/Denver',),
- '441382':('Europe/London',),
  '1709884':('America/St_Johns',),
  '441559':('Europe/London',),
  '441558':('Europe/London',),
  '441553':('Europe/London',),
  '441550':('Europe/London',),
  '441557':('Europe/London',),
  '441556':('Europe/London',),
  '441555':('Europe/London',),
  '441554':('Europe/London',),
  '1701448':('America/Chicago',),
- '1785378':('America/Chicago',),
- '1785379':('America/Chicago',),
  '1701444':('America/Chicago',),
  '1906828':('America/Chicago',),
  '1701446':('America/Chicago',),
  '86663':('Asia/Shanghai',),
  '86662':('Asia/Shanghai',),
  '86660':('Asia/Shanghai',),
  '86668':('Asia/Shanghai',),
  '1850819':('America/Chicago',),
- '441388':('Europe/London',),
- '441389':('Europe/London',),
  '1850814':('America/Chicago',),
  '1541547':('America/Los_Angeles',),
  '1541546':('America/Los_Angeles',),
  '1541543':('America/Los_Angeles',),
  '52821':('America/Mexico_City',),
  '52823':('America/Mexico_City',),
  '52824':('America/Mexico_City',),
  '52825':('America/Mexico_City',),
  '1541549':('America/Los_Angeles',),
  '1541548':('America/Los_Angeles',),
- '1270735':('America/New_York',),
- '1270737':('America/New_York',),
- '1418486':('America/Toronto',),
- '1418484':('America/Toronto',),
- '1418480':('America/Toronto',),
- '1250283':('America/Vancouver',),
+ '1208562':('America/Denver',),
+ '555':('America/Sao_Paulo',),
+ '557':('America/Sao_Paulo',),
  '551':('America/Sao_Paulo',),
- '1250287':('America/Vancouver',),
- '1250286':('America/Vancouver',),
- '1250285':('America/Vancouver',),
  '4776':('Europe/Oslo',),
  '4777':('Europe/Oslo',),
  '4774':('Europe/Oslo',),
  '4775':('Europe/Oslo',),
  '4772':('Europe/Oslo',),
  '4773':('Europe/Oslo',),
  '4770':('Europe/Oslo',),
  '4771':('Europe/Oslo',),
  '4778':('Europe/Oslo',),
  '4779':('Arctic/Longyearbyen',),
- '55819000':('America/Sao_Paulo',),
  '1907279':('America/Juneau',),
  '1907278':('America/Juneau',),
  '1907277':('America/Juneau',),
  '1907276':('America/Juneau',),
  '1907274':('America/Juneau',),
  '1907272':('America/Juneau',),
  '1907271':('America/Juneau',),
@@ -4233,145 +3531,114 @@
  '55813607':('America/Sao_Paulo',),
  '55813355':('America/Sao_Paulo',),
  '55813352':('America/Sao_Paulo',),
  '55813351':('America/Sao_Paulo',),
  '55933528':('America/Sao_Paulo',),
  '55933529':('America/Sao_Paulo',),
  '55933521':('America/Sao_Paulo',),
- '1906632':('America/New_York',),
+ '55933522':('America/Sao_Paulo',),
  '55933523':('America/Sao_Paulo',),
  '55933524':('America/Sao_Paulo',),
- '1906635':('America/New_York',),
  '55933526':('America/Sao_Paulo',),
  '55933527':('America/Sao_Paulo',),
- '1250755':('America/Vancouver',),
- '1250754':('America/Vancouver',),
- '1250756':('America/Vancouver',),
- '1250751':('America/Vancouver',),
- '1250753':('America/Vancouver',),
- '1250752':('America/Vancouver',),
- '1250758':('America/Vancouver',),
  '521761':('America/Mexico_City',),
  '441239':('Europe/London',),
  '441236':('Europe/London',),
  '441237':('Europe/London',),
  '441234':('Europe/London',),
  '441235':('Europe/London',),
  '441233':('Europe/London',),
  '52686':('America/Tijuana',),
  '52687':('America/Mazatlan',),
- '1785783':('America/Chicago',),
+ '1541520':('America/Los_Angeles',),
  '55932122':('America/Sao_Paulo',),
- '1606862':('America/New_York',),
- '1606864':('America/New_York',),
  '1867979':('America/Toronto',),
  '5591323':('America/Sao_Paulo',),
  '5591321':('America/Sao_Paulo',),
  '5591325':('America/Sao_Paulo',),
  '1709368':('America/St_Johns',),
- '62962':('Asia/Jayapura',),
  '1270282':('America/Chicago',),
  '1713':('America/Chicago',),
  '1712':('America/Chicago',),
  '1717':('America/New_York',),
  '1716':('America/New_York',),
  '1715':('America/Chicago',),
  '1714':('America/Los_Angeles',),
  '1719':('America/Denver',),
  '1718':('America/New_York',),
  '1541738':('America/Los_Angeles',),
  '1541734':('America/Los_Angeles',),
  '1541736':('America/Los_Angeles',),
  '1541737':('America/Los_Angeles',),
  '1541732':('America/Los_Angeles',),
- '62756':('Asia/Jakarta',),
- '1606285':('America/New_York',),
- '1606286':('America/New_York',),
- '1606287':('America/New_York',),
- '1208888':('America/Denver',),
- '1418679':('America/Toronto',),
+ '521659':('America/Mazatlan',),
+ '521658':('America/Tijuana',),
  '1208884':('America/Denver',),
  '1208885':('America/Los_Angeles',),
  '1208886':('America/Denver',),
  '1208887':('America/Denver',),
- '1208880':('America/Denver',),
+ '521651':('America/Mazatlan',),
  '1208881':('America/Denver',),
- '1418672':('America/Toronto',),
- '1208883':('America/Los_Angeles',),
+ '1208882':('America/Los_Angeles',),
+ '521652':('America/Mazatlan',),
  '1701298':('America/Chicago',),
  '1701297':('America/Chicago',),
  '1701290':('America/Denver',),
  '1701293':('America/Chicago',),
  '1850712':('America/Chicago',),
  '1709437':('America/St_Johns',),
  '521387':('America/Mexico_City',),
  '521386':('America/Mexico_City',),
  '521385':('America/Mexico_City',),
  '521384':('America/Mexico_City',),
  '521383':('America/Mexico_City',),
- '521382':('America/Mexico_City',),
  '521381':('America/Mexico_City',),
  '5664':('America/Santiago',),
  '521389':('America/Mazatlan',),
  '521388':('America/Mexico_City',),
  '55949930':('America/Sao_Paulo',),
  '1850914':('America/Chicago',),
  '262269':('Indian/Mayotte',),
  '1208338':('America/Denver',),
- '55813469':('America/Sao_Paulo',),
+ '1208339':('America/Denver',),
  '1208336':('America/Denver',),
  '1208337':('America/Denver',),
  '262262':('Indian/Reunion',),
  '1208333':('America/Denver',),
  '1208331':('America/Denver',),
  '1701873':('America/Chicago',),
  '1701872':('America/Denver',),
  '55913397':('America/Sao_Paulo',),
  '1850912':('America/Chicago',),
  '3906':('Europe/Rome',),
  '3902':('Europe/Rome',),
  '5594981':('America/Sao_Paulo',),
- '55913646':('America/Sao_Paulo',),
- '1250569':('America/Vancouver',),
- '1250562':('America/Vancouver',),
- '1250563':('America/Vancouver',),
- '1250561':('America/Vancouver',),
- '1250566':('America/Vancouver',),
- '1250567':('America/Vancouver',),
- '1250564':('America/Vancouver',),
- '1250565':('America/Vancouver',),
  '39049':('Europe/Rome',),
- '55813681':('America/Sao_Paulo',),
+ '1775200':('America/Los_Angeles',),
  '39041':('Europe/Rome',),
  '39040':('Europe/Rome',),
  '39045':('Europe/Rome',),
  '1907486':('America/Juneau',),
  '1907487':('America/Juneau',),
  '1775348':('America/Los_Angeles',),
  '1775345':('America/Los_Angeles',),
  '1907488':('America/Juneau',),
- '55913447':('America/Sao_Paulo',),
  '55933064':('America/Sao_Paulo',),
  '55933067':('America/Sao_Paulo',),
  '55933063':('America/Sao_Paulo',),
  '55933062':('America/Sao_Paulo',),
- '55813831':('America/Sao_Paulo',),
  '1907733':('America/Juneau',),
- '55813835':('America/Sao_Paulo',),
  '521892':('America/Mexico_City',),
  '521891':('America/Mexico_City',),
  '521897':('America/Mexico_City',),
  '521894':('America/Mexico_City',),
  '521899':('America/Mexico_City',),
- '1812438':('America/New_York',),
- '1812432':('America/New_York',),
  '1812435':('America/Chicago',),
  '1812437':('America/Chicago',),
  '1850595':('America/Chicago',),
- '1850597':('America/New_York',),
  '1423648':('America/New_York',),
  '1423643':('America/New_York',),
  '1541899':('America/Los_Angeles',),
  '1541891':('America/Los_Angeles',),
  '1541890':('America/Los_Angeles',),
  '1541892':('America/Los_Angeles',),
  '1541895':('America/Los_Angeles',),
@@ -4382,113 +3649,97 @@
  '62324':('Asia/Jakarta',),
  '62325':('Asia/Jakarta',),
  '62326':('Asia/Jakarta',),
  '62327':('Asia/Jakarta',),
  '62321':('Asia/Jakarta',),
  '62322':('Asia/Jakarta',),
  '62323':('Asia/Jakarta',),
- '1606451':('America/New_York',),
  '62328':('Asia/Jakarta',),
  '1907868':('America/Juneau',),
- '1606456':('America/New_York',),
  '1423468':('America/New_York',),
  '1423391':('America/New_York',),
  '1423392':('America/New_York',),
  '1423467':('America/New_York',),
  '1423396':('America/New_York',),
  '55814112':('America/Sao_Paulo',),
  '55814115':('America/Sao_Paulo',),
  '55814116':('America/Sao_Paulo',),
  '1208659':('America/Los_Angeles',),
  '1208658':('America/Denver',),
  '1208651':('America/Los_Angeles',),
+ '27':('Africa/Johannesburg',),
  '1208652':('America/Denver',),
  '1208656':('America/Denver',),
- '1270443':('America/Chicago',),
- '1785727':('America/Chicago',),
- '1785726':('America/Chicago',),
- '1270442':('America/Chicago',),
  '1812858':('America/Chicago',),
  '1812853':('America/Chicago',),
- '1270444':('America/Chicago',),
- '1812855':('America/New_York',),
  '1701609':('America/Chicago',),
  '55919964':('America/Sao_Paulo',),
  '55919960':('America/Sao_Paulo',),
  '55919961':('America/Sao_Paulo',),
  '55919962':('America/Sao_Paulo',),
  '55919963':('America/Sao_Paulo',),
  '253':('Africa/Djibouti',),
  '1270343':('America/Chicago',),
  '1605842':('America/Chicago',),
  '55914040':('America/Sao_Paulo',),
  '1775972':('America/Los_Angeles',),
  '1605845':('America/Chicago',),
- '1606631':('America/New_York',),
- '1606633':('America/New_York',),
- '1606639':('America/New_York',),
- '1606638':('America/New_York',),
  '1701462':('America/Chicago',),
  '1701463':('America/Chicago',),
  '1541385':('America/Los_Angeles',),
  '1541384':('America/Los_Angeles',),
  '1541387':('America/Los_Angeles',),
  '1541386':('America/Los_Angeles',),
  '7481':('Europe/Moscow',),
  '1541383':('America/Los_Angeles',),
  '1541382':('America/Los_Angeles',),
  '1541389':('America/Los_Angeles',),
  '1541388':('America/Los_Angeles',),
  '1850380':('America/Chicago',),
  '1850833':('America/Chicago',),
  '1850830':('America/Chicago',),
- '1850383':('America/New_York',),
  '1850384':('America/Chicago',),
- '1850385':('America/New_York',),
- '1850386':('America/New_York',),
+ '1850837':('America/Chicago',),
  '1850387':('America/Chicago',),
- '1850838':('America/New_York',),
  '1208437':('America/Los_Angeles',),
  '1208436':('America/Denver',),
  '1208431':('America/Denver',),
  '1208433':('America/Denver',),
  '1458':('America/Los_Angeles',),
  '1208438':('America/Denver',),
+ '686':('Pacific/Enderbury', 'Pacific/Kiritimati', 'Pacific/Tarawa'),
  '1270753':('America/Chicago',),
  '1541563':('America/Los_Angeles',),
  '1270756':('America/Chicago',),
- '1270755':('America/Chicago',),
+ '1541567':('America/Los_Angeles',),
  '1270754':('America/Chicago',),
  '1270759':('America/Chicago',),
  '681':('Pacific/Wallis',),
  '680':('Pacific/Palau',),
- '1850524':('America/New_York',),
+ '1850525':('America/Chicago',),
  '1850526':('America/Chicago',),
  '1850527':('America/Chicago',),
  '1850522':('America/Chicago',),
- '1850523':('America/New_York',),
  '683':('Pacific/Niue',),
  '1850529':('America/Chicago',),
- '1812222':('America/New_York',),
  '1907258':('America/Juneau',),
- '1850664':('America/Chicago',),
  '682':('Pacific/Rarotonga',),
  '1907250':('America/Juneau',),
  '1907252':('America/Juneau',),
  '55819790':('America/Sao_Paulo',),
  '55819791':('America/Sao_Paulo',),
  '1907257':('America/Juneau',),
  '1423857':('America/New_York',),
  '1423854':('America/New_York',),
  '55813334':('America/Sao_Paulo',),
- '1423803':('America/New_York',),
+ '55813627':('America/Sao_Paulo',),
  '55813624':('America/Sao_Paulo',),
- '52427':('America/Mexico_City',),
+ '55813625':('America/Sao_Paulo',),
  '55813622':('America/Sao_Paulo',),
- '55813333':('America/Sao_Paulo',),
+ '55813621':('America/Sao_Paulo',),
  '55813338':('America/Sao_Paulo',),
  '55813339':('America/Sao_Paulo',),
  '55813628':('America/Sao_Paulo',),
  '55813629':('America/Sao_Paulo',),
  '86858':('Asia/Shanghai',),
  '86859':('Asia/Shanghai',),
  '86854':('Asia/Shanghai',),
@@ -4505,124 +3756,104 @@
  '52372':('America/Mexico_City',),
  '52373':('America/Mexico_City',),
  '52378':('America/Mexico_City',),
  '390428':('Europe/Rome',),
  '390429':('Europe/Rome',),
  '390424':('Europe/Rome',),
  '390425':('Europe/Rome',),
- '390426':('Europe/Rome',),
+ '390934':('Europe/Rome',),
  '390427':('Europe/Rome',),
  '390932':('Europe/Rome',),
  '390421':('Europe/Rome',),
- '1785554':('America/Chicago',),
+ '390422':('Europe/Rome',),
  '390423':('Europe/Rome',),
  '6265':('Asia/Jakarta',),
  '6262':('Asia/Jakarta',),
  '55813647':('America/Sao_Paulo',),
  '6261':('Asia/Jakarta',),
- '1308784':('America/Chicago',),
- '1308785':('America/Chicago',),
- '1906346':('America/New_York',),
- '1906341':('America/New_York',),
- '1574533':('America/New_York',),
+ '52155':('America/Mexico_City',),
  '55943422':('America/Sao_Paulo',),
- '1418649':('America/Toronto',),
+ '1605455':('America/Denver',),
  '55943421':('America/Sao_Paulo',),
  '55943426':('America/Sao_Paulo',),
  '55943427':('America/Sao_Paulo',),
  '55943424':('America/Sao_Paulo',),
- '1418648':('America/Toronto',),
  '55943428':('America/Sao_Paulo',),
- '1308432':('America/Denver',),
- '55819831':('America/Sao_Paulo',),
+ '55932101':('America/Sao_Paulo',),
+ '521237':('America/Mexico_City',),
  '1308436':('America/Denver',),
  '55939813':('America/Sao_Paulo',),
  '55939810':('America/Sao_Paulo',),
- '55819830':('America/Sao_Paulo',),
+ '55939811':('America/Sao_Paulo',),
  '55819833':('America/Sao_Paulo',),
- '55813641':('America/Sao_Paulo',),
- '1606849':('America/New_York',),
- '1606843':('America/New_York',),
- '1606845':('America/New_York',),
+ '55819835':('America/Sao_Paulo',),
+ '55819834':('America/Sao_Paulo',),
  '9765525':('Asia/Ulaanbaatar',),
  '9765526':('Asia/Ulaanbaatar',),
- '1620285':('America/Chicago',),
- '1418643':('America/Toronto',),
+ '521231':('America/Mexico_City',),
+ '521662':('America/Mazatlan',),
  '521664':('America/Tijuana',),
- '521665':('America/Tijuana',),
+ '1587':('America/Edmonton',),
  '1775971':('America/Los_Angeles',),
  '521953':('America/Mexico_City',),
  '1585':('America/New_York',),
  '62551':('Asia/Makassar',),
- '1418730':('America/Toronto',),
  '521483':('America/Mexico_City',),
- '1418736':('America/Toronto',),
- '1418739':('America/Toronto',),
+ '1731':('America/Chicago',),
  '1732':('America/New_York',),
  '1734':('America/New_York',),
+ '1737':('|America/Chicago',),
  '62556':('Asia/Makassar',),
  '521486':('America/Mexico_City',),
  '62554':('Asia/Makassar',),
  '521677':('America/Mexico_City',),
  '521676':('America/Mexico_City',),
  '521675':('America/Mexico_City',),
  '521674':('America/Mexico_City',),
  '521673':('America/Mazatlan',),
  '521672':('America/Mazatlan',),
  '521671':('America/Mexico_City',),
- '1620421':('America/Chicago',),
- '1620423':('America/Chicago',),
- '1620429':('America/Chicago',),
  '1850733':('America/Chicago',),
  '5641':('America/Santiago',),
  '5643':('America/Santiago',),
  '5642':('America/Santiago',),
  '5645':('America/Santiago',),
- '55813474':('America/Sao_Paulo',),
- '1423587':('America/New_York',),
- '1418883':('America/Toronto',),
+ '62958':('Asia/Jakarta',),
  '1208359':('America/Denver',),
  '441458':('Europe/London',),
  '55813108':('America/Sao_Paulo',),
  '441456':('Europe/London',),
- '1208351':('America/Denver',),
+ '441457':('Europe/London',),
  '441454':('Europe/London',),
  '1208353':('America/Denver',),
- '441452':('Europe/London',),
+ '1208354':('America/Denver',),
  '441453':('Europe/London',),
  '441450':('Europe/London',),
- '441451':('Europe/London',),
+ '1208357':('America/Denver',),
  '7485':('Europe/Moscow',),
- '1785239':('America/Chicago',),
- '1785238':('America/Chicago',),
- '1785235':('America/Chicago',),
- '1785234':('America/Chicago',),
- '1785233':('America/Chicago',),
- '1785232':('America/Chicago',),
+ '7484':('Europe/Moscow',),
+ '7487':('Europe/Moscow',),
  '7486':('Europe/Moscow',),
  '1709454':('America/St_Johns',),
  '1709458':('America/St_Johns',),
  '7483':('Europe/Moscow',),
  '7482':('Europe/Moscow',),
  '55913665':('America/Sao_Paulo',),
- '55913667':('America/Sao_Paulo',),
  '55913661':('America/Sao_Paulo',),
  '55913662':('America/Sao_Paulo',),
  '55813723':('America/Sao_Paulo',),
  '55813722':('America/Sao_Paulo',),
  '55813721':('America/Sao_Paulo',),
  '55813727':('America/Sao_Paulo',),
  '55813726':('America/Sao_Paulo',),
  '1850832':('America/Chicago',),
  '55813725':('America/Sao_Paulo',),
- '55813724':('America/Sao_Paulo',),
- '1850837':('America/Chicago',),
+ '55813096':('America/Sao_Paulo',),
  '1850835':('America/Chicago',),
  '1270563':('America/Chicago',),
- '55939923':('America/Sao_Paulo',),
  '521878':('America/Mexico_City',),
  '521877':('America/Mexico_City', 'America/Tijuana'),
  '521871':('America/Mexico_City',),
  '521873':('America/Mexico_City',),
  '521872':('America/Mexico_City',),
  '1775360':('America/Los_Angeles',),
  '1450':('America/Toronto',),
@@ -4641,113 +3872,92 @@
  '4420':('Europe/London',),
  '4424':('Europe/London',),
  '62342':('Asia/Jakarta',),
  '62343':('Asia/Jakarta',),
  '1423915':('America/New_York',),
  '62341':('Asia/Jakarta',),
  '1423913':('America/New_York',),
+ '1423443':('America/New_York',),
  '1423442':('America/New_York',),
- '97612':('Asia/Ulaanbaatar',),
- '1620635':('America/Chicago',),
  '1270988':('America/Chicago',),
- '1270982':('America/New_York',),
  '390744':('Europe/Rome',),
  '390746':('Europe/Rome',),
- '1250838':('America/Vancouver',),
  '390743':('Europe/Rome',),
  '390742':('Europe/Rome',),
- '1250836':('America/Vancouver',),
- '1250837':('America/Vancouver',),
- '1250830':('America/Vancouver',),
- '1250832':('America/Vancouver',),
- '1250833':('America/Vancouver',),
- '1606433':('America/New_York',),
- '1606432':('America/New_York',),
- '1606437':('America/New_York',),
- '1606436':('America/New_York',),
- '1606435':('America/New_York',),
- '1606439':('America/New_York',),
  '1541564':('America/Los_Angeles',),
  '1701662':('America/Chicago',),
  '1701663':('America/Chicago',),
  '1701664':('America/Chicago',),
- '1541567':('America/Los_Angeles',),
+ '1270755':('America/Chicago',),
  '1701667':('America/Chicago',),
  '1541566':('America/Los_Angeles',),
  '55813114':('America/Sao_Paulo',),
  '1605867':('America/Denver',),
- '55813115':('America/Sao_Paulo',),
  '86599':('Asia/Shanghai',),
  '86598':('Asia/Shanghai',),
- '55813117':('America/Sao_Paulo',),
- '1270369':('America/New_York',),
+ '1208340':('America/Denver',),
  '86591':('Asia/Shanghai',),
  '86593':('Asia/Shanghai',),
  '1270365':('America/Chicago',),
  '1270362':('America/Chicago',),
  '86594':('Asia/Shanghai',),
- '1270360':('America/New_York',),
- '55813111':('America/Sao_Paulo',),
+ '86597':('Asia/Shanghai',),
+ '1208346':('America/Denver',),
  '1208631':('America/Denver',),
  '1208637':('America/Denver',),
  '1208983':('America/Los_Angeles',),
  '1208634':('America/Denver',),
- '1208639':('America/Denver',),
+ '1606387':('America/Chicago',),
  '1208989':('America/Denver',),
  '55813542':('America/Sao_Paulo',),
  '1701483':('America/Denver',),
  '1541367':('America/Los_Angeles',),
- '1208962':('America/Los_Angeles',),
  '1473':('America/Grenada',),
  '1470':('America/New_York',),
+ '1475':('America/New_York',),
  '1478':('America/New_York',),
  '1479':('America/Chicago',),
  '1541508':('America/Los_Angeles',),
+ '1423803':('America/New_York',),
  '1541500':('America/Los_Angeles',),
  '1541506':('America/Los_Angeles',),
- '1541505':('America/Los_Angeles',),
+ '1270773':('America/Chicago',),
  '1541504':('America/Los_Angeles',),
  '5586':('America/Sao_Paulo',),
  '5587':('America/Sao_Paulo',),
  '5584':('America/Sao_Paulo',),
- '27':('Africa/Johannesburg',),
- '20':('Africa/Cairo',),
+ '5585':('America/Sao_Paulo',),
+ '5582':('America/Sao_Paulo',),
  '5583':('America/Sao_Paulo',),
  '5581':('America/Noronha',),
  '5588':('America/Sao_Paulo',),
  '5589':('America/Sao_Paulo',),
- '1850508':('America/New_York',),
- '1850509':('America/New_York',),
  '1850505':('America/Chicago',),
  '1850502':('America/Chicago',),
+ '1850501':('America/Chicago',),
  '1907232':('America/Juneau',),
  '1541228':('America/Los_Angeles',),
  '1907230':('America/Juneau',),
  '1907235':('America/Juneau',),
  '441665':('Europe/London',),
  '441664':('Europe/London',),
- '441667':('Europe/London',),
- '441666':('Europe/London',),
- '441661':('Europe/London',),
+ '55813318':('America/Sao_Paulo',),
+ '55813319':('America/Sao_Paulo',),
+ '55813648':('America/Sao_Paulo',),
  '55813649':('America/Sao_Paulo',),
  '441663':('Europe/London',),
- '55813312':('America/Sao_Paulo',),
+ '55813644':('America/Sao_Paulo',),
  '55813645':('America/Sao_Paulo',),
  '55813646':('America/Sao_Paulo',),
- '1907586':('America/Juneau',),
+ '55813311':('America/Sao_Paulo',),
  '441669':('Europe/London',),
- '1907580':('America/Juneau',),
- '55813314':('America/Sao_Paulo',),
+ '55813317':('America/Sao_Paulo',),
+ '55813642':('America/Sao_Paulo',),
  '55813643':('America/Sao_Paulo',),
- '1250248':('America/Vancouver',),
- '1250247':('America/Vancouver',),
- '1250246':('America/Vancouver',),
- '1250245':('America/Vancouver',),
  '1250242':('America/Edmonton',),
- '1250240':('America/Vancouver',),
  '55933563':('America/Sao_Paulo',),
  '521423':('America/Mexico_City',),
  '52312':('America/Mexico_City',),
  '52313':('America/Mexico_City',),
  '52311':('America/Mazatlan',),
  '52316':('America/Mexico_City',),
  '52317':('America/Mexico_City',),
@@ -4764,47 +3974,37 @@
  '441274':('Europe/London',),
  '441275':('Europe/London',),
  '441278':('Europe/London',),
  '441279':('Europe/London',),
  '1775425':('America/Los_Angeles',),
  '1775424':('America/Los_Angeles',),
  '6289':('Asia/Jakarta',),
- '55913515':('America/Sao_Paulo',),
- '55913207':('America/Sao_Paulo',),
- '55817811':('America/Sao_Paulo',),
- '55913205':('America/Sao_Paulo',),
+ '351283':('Europe/Lisbon',),
+ '351281':('Europe/Lisbon',),
  '55913204':('America/Sao_Paulo',),
  '1605472':('America/Chicago',),
- '55913202':('America/Sao_Paulo',),
+ '351286':('Europe/Lisbon',),
  '55913201':('America/Sao_Paulo',),
- '1418285':('America/Toronto',),
- '1418287':('America/Toronto',),
- '1418286':('America/Toronto',),
- '1418289':('America/Toronto',),
  '1605753':('America/Chicago',),
  '441896':('Europe/London',),
  '86459':('Asia/Shanghai',),
  '441895':('Europe/London',),
  '441892':('Europe/London',),
  '441890':('Europe/London',),
  '86451':('Asia/Shanghai',),
  '86452':('Asia/Shanghai',),
  '86453':('Asia/Shanghai',),
  '86454':('Asia/Shanghai',),
- '1812952':('America/New_York',),
- '1812951':('America/New_York',),
+ '86455':('Asia/Shanghai',),
+ '86456':('Asia/Shanghai',),
  '441899':('Europe/London',),
- '1574204':('America/New_York',),
- '1574206':('America/New_York',),
- '1418759':('America/Toronto',),
  '62481':('Asia/Makassar',),
- '1418752':('America/Toronto',),
- '1418750':('America/Toronto',),
+ '62482':('Asia/Makassar',),
  '62485':('Asia/Makassar',),
- '1418756':('America/Toronto',),
+ '62484':('Asia/Makassar',),
  '521613':('America/Mazatlan',),
  '521612':('America/Mazatlan',),
  '521615':('America/Mazatlan',),
  '521614':('America/Mazatlan',),
  '521616':('America/Tijuana',),
  '521618':('America/Mexico_City',),
  '1219836':('America/Chicago',),
@@ -4813,40 +4013,36 @@
  '1541771':('America/Los_Angeles',),
  '1541772':('America/Los_Angeles',),
  '1541773':('America/Los_Angeles',),
  '1541774':('America/Los_Angeles',),
  '1541776':('America/Los_Angeles',),
  '1541778':('America/Los_Angeles',),
  '1541779':('America/Los_Angeles',),
- '55913623':('America/Sao_Paulo',),
  '1317':('America/New_York',),
  '1316':('America/Chicago',),
  '1315':('America/New_York',),
  '1314':('America/Chicago',),
  '1313':('America/New_York',),
  '1312':('America/Chicago',),
  '1208375':('America/Denver',),
  '1208378':('America/Denver',),
  '1319':('America/Chicago',),
  '1318':('America/Chicago',),
  '1701347':('America/Chicago',),
- '1701837':('America/Chicago',),
+ '55813127':('America/Sao_Paulo',),
  '55813126':('America/Sao_Paulo',),
  '1701343':('America/Chicago',),
  '1701833':('America/Chicago',),
- '1701839':('America/Chicago',),
- '1701838':('America/Chicago',),
+ '55813129':('America/Sao_Paulo',),
+ '55813128':('America/Sao_Paulo',),
  '1701349':('America/Chicago',),
- '1785218':('America/Chicago',),
- '1423743':('America/New_York',),
- '1785215':('America/Chicago',),
  '7728':('Asia/Almaty',),
  '7729':('Asia/Aqtobe',),
  '1850974':('America/Chicago',),
- '1850973':('America/New_York',),
+ '1850972':('America/Chicago',),
  '7721':('Asia/Almaty',),
  '7722':('Asia/Almaty',),
  '7723':('Asia/Almaty',),
  '7724':('Asia/Almaty',),
  '7725':('Asia/Almaty',),
  '7726':('Asia/Almaty',),
  '7727':('Asia/Almaty',),
@@ -4857,270 +4053,225 @@
  '441786':('Europe/London',),
  '441787':('Europe/London',),
  '441784':('Europe/London',),
  '441785':('Europe/London',),
  '441788':('Europe/London',),
  '441789':('Europe/London',),
  '86592':('Asia/Shanghai',),
+ '1219838':('America/Chicago',),
  '39089':('Europe/Rome',),
  '39085':('Europe/Rome',),
  '39081':('Europe/Rome',),
  '39080':('Europe/Rome',),
  '86595':('Asia/Shanghai',),
- '62870':('Asia/Jakarta',),
- '62871':('Asia/Jakarta',),
- '62872':('Asia/Jakarta',),
  '1270542':('America/Chicago',),
- '62873':('Asia/Jakarta',),
  '1812386':('America/Chicago',),
  '1270547':('America/Chicago',),
- '1812384':('America/New_York',),
  '1812385':('America/Chicago',),
  '86335':('Asia/Shanghai',),
- '62874':('Asia/Jakarta',),
- '62875':('Asia/Jakarta',),
- '1250474':('America/Vancouver',),
- '1250475':('America/Vancouver',),
- '1250477':('America/Vancouver',),
- '1250470':('America/Vancouver',),
- '1250472':('America/Vancouver',),
- '1250478':('America/Vancouver',),
- '1250479':('America/Vancouver',),
+ '55813877':('America/Sao_Paulo',),
  '55813879':('America/Sao_Paulo',),
  '55813878':('America/Sao_Paulo',),
  '55813626':('America/Sao_Paulo',),
- '55813627':('America/Sao_Paulo',),
- '55813625':('America/Sao_Paulo',),
  '1423602':('America/New_York',),
- '55813621':('America/Sao_Paulo',),
+ '55813333':('America/Sao_Paulo',),
  '964':('Asia/Baghdad',),
  '965':('Asia/Kuwait',),
  '966':('Asia/Riyadh',),
  '967':('Asia/Aden',),
  '960':('Indian/Maldives',),
  '1605666':('America/Denver',),
  '1605665':('America/Chicago',),
  '963':('Asia/Damascus',),
  '1605669':('America/Chicago',),
  '1605668':('America/Chicago',),
  '968':('Asia/Muscat',),
  '1907772':('America/Juneau',),
  '1907770':('America/Juneau',),
  '1907776':('America/Juneau',),
- '1620653':('America/Chicago',),
- '1620873':('America/Chicago',),
- '1620872':('America/Chicago',),
+ '62368':('Asia/Makassar',),
+ '1423933':('America/New_York',),
  '62818':('Asia/Jakarta', 'Asia/Makassar'),
  '62819':('Asia/Jakarta', 'Asia/Makassar'),
  '1907822':('America/Juneau',),
- '1906428':('America/New_York',),
- '1620659':('America/Chicago',),
+ '62361':('Asia/Makassar',),
+ '62362':('Asia/Makassar',),
  '62363':('Asia/Makassar',),
  '1907826':('America/Juneau',),
  '62365':('Asia/Makassar',),
- '1620879':('America/Chicago',),
+ '62366':('Asia/Makassar',),
  '62811':('Asia/Jakarta', 'Asia/Makassar'),
  '390583':('Europe/Rome',),
  '390587':('Europe/Rome',),
  '390586':('Europe/Rome',),
  '390585':('Europe/Rome',),
  '390584':('Europe/Rome',),
- '1785456':('America/Chicago',),
- '1785454':('America/Chicago',),
- '1785452':('America/Chicago',),
- '34944':('Europe/Madrid',),
- '1240':('America/New_York',),
+ '390588':('Europe/Rome',),
  '1219989':('America/Chicago',),
  '1242':('America/Nassau',),
- '34941':('Europe/Madrid',),
  '1219983':('America/Chicago',),
- '1418986':('America/Halifax',),
+ '1208556':('America/Los_Angeles',),
  '1219980':('America/Chicago',),
  '1219987':('America/Chicago',),
  '1208557':('America/Denver',),
- '1250814':('America/Vancouver',),
  '86857':('Asia/Shanghai',),
- '1250812':('America/Vancouver',),
- '1246':('America/Barbados',),
- '521635':('America/Mazatlan',),
- '1250818':('America/Vancouver',),
- '1250819':('America/Vancouver',),
+ '1208398':('America/Denver',),
+ '647':('Pacific/Auckland',),
+ '1530':('America/Los_Angeles',),
+ '649':('Pacific/Auckland',),
  '390769':('Europe/Rome',),
  '390766':('Europe/Rome',),
  '390765':('Europe/Rome',),
  '390763':('Europe/Rome',),
  '390761':('Europe/Rome',),
  '521433':('America/Mexico_City',),
- '1619':('America/Los_Angeles',),
+ '521432':('America/Mexico_City',),
  '1617':('America/New_York',),
  '1615':('America/Chicago',),
  '1701642':('America/Chicago',),
+ '1612':('America/Chicago',),
  '521438':('America/Mexico_City',),
  '1605886':('America/Chicago',),
  '1605882':('America/Chicago',),
  '1605881':('America/Chicago',),
  '1678':('America/New_York',),
  '1208964':('America/Los_Angeles',),
  '1670':('Pacific/Saipan',),
- '1671':('Pacific/Guam',),
- '1906884':('America/New_York',),
+ '1208610':('America/Los_Angeles',),
  '55673480':('America/Sao_Paulo',),
  '1541349':('America/Los_Angeles',),
  '29998':('America/Godthab',),
  '29999':('America/Scoresbysund',),
  '29992':('America/Godthab',),
  '1541343':('America/Los_Angeles',),
  '1541690':('America/Los_Angeles',),
  '1541345':('America/Los_Angeles',),
  '1541344':('America/Los_Angeles',),
- '29994':('America/Godthab',),
+ '1541347':('America/Los_Angeles',),
  '1541346':('America/Los_Angeles',),
+ '1418':('America/Toronto',),
  '1419':('America/New_York',),
  '1410':('America/New_York',),
  '1412':('America/New_York',),
  '1413':('America/New_York',),
  '1414':('America/Chicago',),
  '1415':('America/Los_Angeles',),
  '1416':('America/Toronto',),
  '1417':('America/Chicago',),
  '1541525':('America/Los_Angeles',),
  '1541526':('America/Los_Angeles',),
  '1541521':('America/Los_Angeles',),
- '1541520':('America/Los_Angeles',),
+ '441528':('Europe/London',),
  '1541523':('America/Los_Angeles',),
  '55813078':('America/Sao_Paulo',),
- '55813077':('America/Sao_Paulo',),
- '55813076':('America/Sao_Paulo',),
- '55813075':('America/Sao_Paulo',),
- '55813074':('America/Sao_Paulo',),
+ '441526':('Europe/London',),
+ '441527':('Europe/London',),
+ '441524':('Europe/London',),
+ '441525':('Europe/London',),
  '5568':('America/Rio_Branco',),
  '5569':('America/Manaus',),
  '5564':('America/Sao_Paulo',),
  '5565':('America/Manaus',),
  '5566':('America/Manaus',),
  '5567':('America/Manaus',),
  '5561':('America/Sao_Paulo',),
  '5562':('America/Sao_Paulo',),
  '5563':('America/Sao_Paulo',),
- '55813071':('America/Sao_Paulo',),
+ '441520':('Europe/London',),
  '646':('Pacific/Auckland',),
  '1709643':('America/St_Johns',),
- '1701968':('America/Chicago',),
- '1850561':('America/New_York',),
- '1850562':('America/New_York',),
- '1850566':('America/New_York',),
- '1850567':('America/New_York',),
  '351276':('Europe/Lisbon',),
  '351277':('Europe/Lisbon',),
  '351274':('Europe/Lisbon',),
  '351275':('Europe/Lisbon',),
  '351272':('Europe/Lisbon',),
  '351273':('Europe/Lisbon',),
  '351271':('Europe/Lisbon',),
  '351278':('Europe/Lisbon',),
  '1907212':('America/Juneau',),
- '1250300':('America/Vancouver',),
- '555':('America/Sao_Paulo',),
- '1250304':('America/Vancouver',),
- '55913028':('America/Sao_Paulo',),
  '55813662':('America/Sao_Paulo',),
  '55813661':('America/Sao_Paulo',),
- '62261':('Asia/Jakarta',),
  '441647':('Europe/London',),
  '441646':('Europe/London',),
  '441644':('Europe/London',),
  '441643':('Europe/London',),
  '441642':('Europe/London',),
  '441641':('Europe/London',),
  '1250261':('America/Edmonton',),
- '1250260':('America/Vancouver',),
  '1250263':('America/Edmonton',),
  '1250262':('America/Edmonton',),
- '1250265':('America/Vancouver',),
- '390934':('Europe/Rome',),
- '521758':('America/Mexico_City',),
+ '390426':('Europe/Rome',),
  '390935':('Europe/Rome',),
- '62260':('Asia/Jakarta',),
  '390933':('Europe/Rome',),
- '390422':('Europe/Rome',),
  '390931':('Europe/Rome',),
- '62263':('Asia/Jakarta',),
- '7395':('Asia/Irkutsk',),
  '52998':('America/New_York',),
  '52999':('America/Mexico_City',),
  '52994':('America/Mexico_City',),
- '1541882':('America/Los_Angeles',),
+ '52995':('America/Mexico_City',),
  '52996':('America/Mexico_City',),
  '52997':('America/Mexico_City',),
  '52991':('America/Mexico_City',),
  '52992':('America/Mexico_City',),
- '52993':('America/Mexico_City',),
+ '1541883':('America/Los_Angeles',),
  '1605279':('America/Denver',),
  '1775445':('America/Los_Angeles',),
  '1605274':('America/Chicago',),
- '1605275':('America/Chicago',),
+ '55939997':('America/Sao_Paulo',),
  '1605271':('America/Chicago',),
  '62251':('Asia/Jakarta',),
  '441258':('Europe/London',),
- '441259':('Europe/London',),
+ '62252':('Asia/Jakarta',),
  '441254':('Europe/London',),
  '441255':('Europe/London',),
  '441256':('Europe/London',),
- '441257':('Europe/London',),
+ '521757':('America/Mexico_City',),
  '441250':('Europe/London',),
  '441252':('Europe/London',),
  '441253':('Europe/London',),
- '1812597':('America/New_York',),
  '86812':('Asia/Shanghai',),
  '55933549':('America/Sao_Paulo',),
  '1541888':('America/Los_Angeles',),
- '1812591':('America/New_York',),
- '1812590':('America/New_York',),
+ '86816':('Asia/Shanghai',),
+ '86817':('Asia/Shanghai',),
  '55933542':('America/Sao_Paulo',),
  '55933543':('America/Sao_Paulo',),
  '55933541':('America/Sao_Paulo',),
  '55933547':('America/Sao_Paulo',),
  '55933544':('America/Sao_Paulo',),
  '1605415':('America/Denver',),
  '390972':('Europe/Rome',),
  '390973':('Europe/Rome',),
- '1812623':('America/New_York',),
  '390971':('Europe/Rome',),
  '390976':('Europe/Rome',),
  '390974':('Europe/Rome',),
  '390975':('Europe/Rome',),
- '1574223':('America/New_York',),
- '1418775':('America/Toronto',),
- '1418774':('America/Toronto',),
  '8628':('Asia/Shanghai',),
  '8629':('Asia/Shanghai',),
  '1908':('America/New_York',),
- '52155':('America/Mexico_City',),
  '1909':('America/Los_Angeles',),
  '8627':('Asia/Shanghai',),
  '521639':('America/Mazatlan',),
  '521638':('America/Mazatlan',),
  '521633':('America/Mazatlan',),
  '521632':('America/Mazatlan',),
  '521631':('America/Mazatlan',),
  '521637':('America/Mazatlan',),
- '521636':('America/Mazatlan', 'America/Mexico_City'),
- '1418614':('America/Toronto',),
+ '521636':('America/Hermosillo', 'America/Mazatlan'),
+ '521635':('America/Mazatlan',),
  '521634':('America/Mazatlan',),
- '1785665':('America/Chicago',),
- '1620465':('America/Chicago',),
- '1605455':('America/Denver',),
  '1701584':('America/Denver',),
  '1904':('America/New_York',),
  '55949995':('America/Sao_Paulo',),
  '55943392':('America/Sao_Paulo',),
  '55949997':('America/Sao_Paulo',),
  '55949990':('America/Sao_Paulo',),
+ '55949991':('America/Sao_Paulo',),
+ '55949992':('America/Sao_Paulo',),
  '1541758':('America/Los_Angeles',),
- '1541752':('America/Los_Angeles',),
+ '1905':('America/Toronto',),
  '1541753':('America/Los_Angeles',),
  '1541751':('America/Los_Angeles',),
  '1541756':('America/Los_Angeles',),
  '1541757':('America/Los_Angeles',),
  '1541754':('America/Los_Angeles',),
  '1219462':('America/Chicago',),
  '1219464':('America/Chicago',),
@@ -5128,48 +4279,38 @@
  '1334':('America/Chicago',),
  '1337':('America/Chicago',),
  '1336':('America/New_York',),
  '1331':('America/Chicago',),
  '1208391':('America/Denver',),
  '1208392':('America/Denver',),
  '1332':('America/New_York',),
- '1785273':('America/Chicago',),
- '1785272':('America/Chicago',),
- '1785271':('America/Chicago',),
+ '1701361':('America/Chicago',),
  '1701365':('America/Chicago',),
  '1701364':('America/Chicago',),
  '1701367':('America/Chicago',),
- '55813479':('America/Sao_Paulo',),
  '8693':('Asia/Shanghai',),
- '1850907':('America/New_York',),
- '55932101':('America/Sao_Paulo',),
+ '1308432':('America/Denver',),
  '39':('Europe/Rome', 'Europe/Vatican'),
  '33':('Europe/Paris',),
  '32':('Europe/Brussels',),
  '31':('Europe/Amsterdam',),
  '30':('Europe/Athens',),
  '36':('Europe/Budapest',),
  '34':('Atlantic/Canary', 'Europe/Madrid'),
  '1850951':('America/Chicago',),
- '1850547':('America/Chicago',),
  '55939812':('America/Sao_Paulo',),
- '55939811':('America/Sao_Paulo',),
  '1785890':('America/Denver',),
  '1785899':('America/Denver',),
- '1812364':('America/New_York',),
- '1812365':('America/New_York',),
- '1812367':('America/New_York',),
- '521831':('America/Mexico_City',),
+ '52297':('America/Mexico_City',),
  '52296':('America/Mexico_City',),
  '521833':('America/Mexico_City',),
  '52294':('America/Mexico_City',),
+ '521835':('America/Mexico_City',),
  '521834':('America/Mexico_City',),
  '521836':('America/Mexico_City',),
- '1250457':('America/Vancouver',),
- '1250453':('America/Vancouver',),
  '1775328':('America/Los_Angeles',),
  '1775329':('America/Los_Angeles',),
  '1775322':('America/Los_Angeles',),
  '1775323':('America/Los_Angeles',),
  '1775327':('America/Los_Angeles',),
  '1775324':('America/Los_Angeles',),
  '1423629':('America/New_York',),
@@ -5181,51 +4322,43 @@
  '1605649':('America/Chicago',),
  '1605644':('America/Denver',),
  '1605647':('America/Chicago',),
  '1605641':('America/Denver',),
  '1605642':('America/Denver',),
  '55813501':('America/Sao_Paulo',),
  '1907790':('America/Juneau',),
- '1620855':('America/Chicago',),
- '1620856':('America/Chicago',),
- '1620675':('America/Chicago',),
  '1423952':('America/New_York',),
  '1423485':('America/New_York',),
  '1423487':('America/New_York',),
  '1423954':('America/New_York',),
- '1785478':('America/Chicago',),
  '390565':('Europe/Rome',),
  '390564':('Europe/Rome',),
- '1785472':('America/Chicago',),
- '1785475':('America/Chicago',),
+ '390566':('Europe/Rome',),
  '1775588':('America/Los_Angeles',),
  '1775586':('America/Los_Angeles',),
  '55913494':('America/Sao_Paulo',),
- '1250870':('America/Vancouver',),
- '1250871':('America/Vancouver',),
- '1250877':('America/Vancouver',),
- '1250878':('America/Vancouver',),
+ '55813212':('America/Sao_Paulo',),
  '9761362':('Asia/Choibalsan', 'Asia/Ulaanbaatar'),
  '62834':('Asia/Jakarta', 'Asia/Makassar'),
  '62835':('Asia/Jakarta',),
  '62836':('Asia/Jakarta',),
  '62837':('Asia/Jakarta',),
  '62830':('Asia/Jakarta',),
  '62831':('Asia/Jakarta', 'Asia/Makassar'),
  '62832':('Asia/Jakarta',),
- '62833':('Asia/Jakarta',),
+ '62833':('Asia/Jakarta', 'Asia/Makassar'),
  '62838':('Asia/Jakarta',),
- '62839':('Asia/Jakarta',),
- '55913605':('America/Sao_Paulo',),
+ '62839':('Asia/Jakarta', 'Asia/Makassar'),
+ '55919987':('America/Sao_Paulo',),
  '55919984':('America/Sao_Paulo',),
  '55919982':('America/Sao_Paulo',),
  '55919983':('America/Sao_Paulo',),
  '55919980':('America/Sao_Paulo',),
  '55919981':('America/Sao_Paulo',),
- '1785735':('America/Chicago',),
+ '55919988':('America/Sao_Paulo',),
  '1270852':('America/Chicago',),
  '44187':('Europe/London',),
  '1208949':('America/Denver',),
  '1208941':('America/Denver',),
  '1650':('America/Los_Angeles',),
  '1651':('America/Chicago',),
  '1657':('America/Los_Angeles',),
@@ -5233,36 +4366,35 @@
  '1208946':('America/Los_Angeles',),
  '1541323':('America/Los_Angeles',),
  '1541322':('America/Los_Angeles',),
  '1541327':('America/Los_Angeles',),
  '1541326':('America/Los_Angeles',),
  '1541324':('America/Los_Angeles',),
  '1850890':('America/Chicago',),
- '1850891':('America/New_York',),
  '1850892':('America/Chicago',),
- '1850893':('America/New_York',),
- '1850894':('America/New_York',),
  '1850897':('America/Chicago',),
- '1418845':('America/Toronto',),
+ '1850898':('America/Chicago',),
+ '1219369':('America/Chicago',),
+ '1437':('America/Winnipeg',),
  '1434':('America/New_York',),
  '1435':('America/Denver',),
  '1432':('America/Chicago',),
  '521791':('America/Mexico_City',),
  '1208495':('America/Denver',),
+ '1431':('America/Winnipeg',),
  '1438':('America/Toronto',),
- '1731':('America/Chicago',),
  '5233':('America/Mexico_City',),
  '1867456':('America/Vancouver',),
  '1850234':('America/Chicago',),
  '1850543':('America/Chicago',),
  '1850236':('America/Chicago',),
  '1850230':('America/Chicago',),
  '1850231':('America/Chicago',),
  '1850232':('America/Chicago',),
- '1850545':('America/New_York',),
+ '1850233':('America/Chicago',),
  '1850238':('America/Chicago',),
  '1208237':('America/Denver',),
  '1208236':('America/Denver',),
  '1208234':('America/Denver',),
  '1208233':('America/Denver',),
  '1208232':('America/Denver',),
  '1208239':('America/Denver',),
@@ -5272,128 +4404,103 @@
  '351253':('Europe/Lisbon',),
  '351254':('Europe/Lisbon',),
  '351255':('Europe/Lisbon',),
  '351256':('Europe/Lisbon',),
  '86349':('Asia/Shanghai',),
  '351258':('Europe/Lisbon',),
  '351259':('Europe/Lisbon',),
- '1606475':('America/New_York',),
- '55913781':('America/Sao_Paulo',),
- '1308832':('America/Chicago',),
+ '1219852':('America/Chicago',),
  '441629':('Europe/London',),
  '441628':('Europe/London',),
  '441621':('Europe/London',),
  '441620':('Europe/London',),
  '441623':('Europe/London',),
  '441622':('Europe/London',),
  '441625':('Europe/London',),
- '441624':('Europe/Isle_of_Man',),
+ '1423821':('America/New_York',),
  '441626':('Europe/London',),
- '1423826':('America/New_York',),
+ '52454':('America/Mexico_City',),
  '52457':('America/Mexico_City',),
+ '1541357':('America/Los_Angeles',),
  '1270667':('America/Chicago',),
  '1270665':('America/Chicago',),
+ '390925':('Europe/Rome',),
  '1308762':('America/Denver',),
  '1907631':('America/Juneau',),
  '62545':('Asia/Makassar',),
- '1605782':('America/Chicago',),
  '1775461':('America/Los_Angeles',),
  '1775463':('America/Los_Angeles',),
  '1605787':('America/Denver',),
  '55913556':('America/Sao_Paulo',),
  '390924':('Europe/Rome',),
  '62541':('Asia/Makassar',),
- '1850587':('America/Chicago',),
- '7388':('Asia/Krasnoyarsk',),
+ '441798':('Europe/London',),
+ '55813469':('America/Sao_Paulo',),
  '976158':('Asia/Choibalsan',),
  '1605256':('America/Chicago',),
  '1812649':('America/Chicago',),
- '1812645':('America/New_York',),
- '1574243':('America/New_York',),
- '1574246':('America/New_York',),
- '1574247':('America/New_York',),
+ '1605255':('America/Denver',),
  '52716':('America/Mexico_City',),
  '52717':('America/Mexico_City',),
  '52714':('America/Mexico_City',),
  '52715':('America/Mexico_City',),
  '52712':('America/Mexico_City',),
  '52713':('America/Mexico_City',),
  '1423542':('America/New_York',),
  '52711':('America/Mexico_City',),
  '52718':('America/Mexico_City',),
  '52719':('America/Mexico_City',),
  '1605432':('America/Chicago',),
  '1605430':('America/Denver',),
  '1605431':('America/Denver',),
  '7384':('Asia/Krasnoyarsk',),
- '1620442':('America/Chicago',),
- '1620336':('America/Chicago',),
- '1620441':('America/Chicago',),
- '1620331':('America/Chicago',),
- '1620332':('America/Chicago',),
- '1250999':('America/Vancouver',),
- '1250992':('America/Vancouver',),
- '1250991':('America/Vancouver',),
- '1250997':('America/Vancouver',),
- '1250996':('America/Vancouver',),
- '1812917':('America/New_York',),
  '1701567':('America/Denver',),
  '1701566':('America/Chicago',),
  '1605925':('America/Chicago',),
- '55913083':('America/Sao_Paulo',),
+ '1701499':('America/Chicago',),
  '1605923':('America/Denver',),
  '691330':('Pacific/Truk',),
  '1605928':('America/Chicago',),
  '1605929':('America/Chicago',),
- '1418898':('America/Toronto',),
- '1418899':('America/Toronto',),
  '55913311':('America/Sao_Paulo',),
  '1352':('America/New_York',),
  '1219440':('America/Chicago',),
- '1418893':('America/Toronto',),
  '55913088':('America/Sao_Paulo',),
- '1785258':('America/Chicago',),
- '1785256':('America/Chicago',),
  '1701306':('America/Chicago',),
  '86766':('Asia/Shanghai',),
  '86762':('Asia/Shanghai',),
  '86763':('Asia/Shanghai',),
  '86760':('Asia/Shanghai',),
  '86768':('Asia/Shanghai',),
  '86769':('Asia/Shanghai',),
  '1850939':('America/Chicago',),
- '1850933':('America/New_York',),
  '1850932':('America/Chicago',),
  '1850937':('America/Chicago',),
  '1850936':('America/Chicago',),
  '1850934':('America/Chicago',),
  '1807274':('America/Winnipeg',),
- '55813712':('America/Sao_Paulo',),
  '643305':('Pacific/Chatham',),
- '55813711':('America/Sao_Paulo',),
  '1208255':('America/Los_Angeles',),
- '1812346':('America/New_York',),
- '1812347':('America/New_York',),
- '1812345':('America/New_York',),
- '1812342':('America/New_York',),
- '1812343':('America/New_York',),
- '1812349':('America/New_York',),
+ '1270586':('America/Chicago',),
+ '55913753':('America/Sao_Paulo',),
  '52279':('America/Mexico_City',),
  '52278':('America/Mexico_City',),
  '52275':('America/Mexico_City',),
  '52274':('America/Mexico_City',),
  '52276':('America/Mexico_City',),
  '52271':('America/Mexico_City',),
  '52273':('America/Mexico_City',),
  '52272':('America/Mexico_City',),
  '55925009':('America/Sao_Paulo',),
- '1443':('America/New_York',),
- '1441':('Atlantic/Bermuda',),
+ '1445':('America/New_York',),
+ '1208426':('America/Denver',),
+ '1208251':('America/Denver',),
+ '1208424':('America/Denver',),
  '55813972':('America/Sao_Paulo',),
- '1440':('America/New_York',),
+ '1208425':('America/Denver',),
  '691933':('Pacific/Truk',),
  '1208250':('America/Denver',),
  '55813521':('America/Sao_Paulo',),
  '55813523':('America/Sao_Paulo',),
  '55813522':('America/Sao_Paulo',),
  '55813525':('America/Sao_Paulo',),
  '55813524':('America/Sao_Paulo',),
@@ -5417,96 +4524,84 @@
  '1219947':('America/Chicago',),
  '1219945':('America/Chicago',),
  '1219944':('America/Chicago',),
  '1219942':('America/Chicago',),
  '1219940':('America/Chicago',),
  '390722':('Europe/Rome',),
  '390721':('Europe/Rome',),
- '1250859':('America/Vancouver',),
- '1250851':('America/Vancouver',),
- '1250857':('America/Vancouver',),
+ '1907581':('Pacific/Honolulu',),
+ '1907580':('America/Juneau',),
  '441993':('Europe/London',),
  '441992':('Europe/London',),
  '441997':('Europe/London',),
- '1308536':('America/Chicago',),
  '441995':('Europe/London',),
  '441994':('Europe/London',),
  '1423975':('America/New_York',),
  '62853':('Asia/Jakarta', 'Asia/Makassar'),
  '62850':('Asia/Jakarta',),
  '62851':('Asia/Jakarta',),
  '62856':('Asia/Jakarta',),
  '62857':('Asia/Jakarta',),
  '62854':('Asia/Jakarta',),
  '62855':('Asia/Jakarta',),
  '62858':('Asia/Jakarta',),
  '62859':('Asia/Jakarta',),
  '1423979':('America/New_York',),
- '1219365':('America/Chicago',),
- '1219398':('America/Chicago',),
- '1208350':('America/Denver',),
- '441457':('Europe/London',),
- '1270877':('America/New_York',),
- '1208352':('America/Denver',),
+ '55813109':('America/Sao_Paulo',),
+ '55813107':('America/Sao_Paulo',),
+ '1219397':('America/Chicago',),
+ '55813105':('America/Sao_Paulo',),
  '1986':('America/Boise', 'America/Los_Angeles'),
  '1631':('America/New_York',),
  '1984':('America/New_York',),
  '1219395':('America/Chicago',),
  '1208926':('America/Los_Angeles',),
  '1980':('America/New_York',),
- '1574583':('America/New_York',),
- '1219392':('America/Chicago',),
+ '1639':('America/Winnipeg',),
  '1208928':('America/Denver',),
- '1574586':('America/New_York',),
- '1219393':('America/Chicago',),
+ '55813102':('America/Sao_Paulo',),
  '1208356':('America/Denver',),
- '1208357':('America/Denver',),
+ '441451':('Europe/London',),
  '569':('America/Santiago',),
  '1541659':('America/Los_Angeles',),
  '562':('America/Santiago',),
- '1541654':('America/Los_Angeles',),
- '1541653':('America/Los_Angeles',),
+ '1541306':('America/Los_Angeles',),
+ '1541301':('America/Los_Angeles',),
  '1541302':('America/Los_Angeles',),
- '1574722':('America/New_York',),
- '1580':('America/Chicago',),
  '62276':('Asia/Jakarta',),
  '62274':('Asia/Jakarta',),
  '62275':('Asia/Jakarta',),
  '62272':('Asia/Jakarta',),
- '1423202':('America/New_York',),
+ '62273':('Asia/Jakarta',),
  '521778':('America/Mexico_City',),
- '521779':('America/Mexico_City',),
+ '62271':('Asia/Jakarta',),
  '521776':('America/Mexico_City',),
  '521777':('America/Mexico_City',),
  '521774':('America/Mexico_City',),
  '521775':('America/Mexico_City',),
  '521772':('America/Mexico_City',),
  '521773':('America/Mexico_City',),
  '1423209':('America/New_York',),
  '521771':('America/Mexico_City',),
- '1219369':('America/Chicago',),
  '48':('Europe/Warsaw',),
  '49':('Europe/Berlin',),
  '46':('Europe/Stockholm',),
  '47':('Arctic/Longyearbyen', 'Europe/Oslo'),
  '44':('Europe/Guernsey', 'Europe/Isle_of_Man', 'Europe/Jersey', 'Europe/London'),
  '45':('Europe/Copenhagen',),
  '43':('Europe/Vienna',),
  '40':('Europe/Bucharest',),
  '41':('Europe/Zurich',),
  '1850218':('America/Chicago',),
- '1850219':('America/New_York',),
- '1850216':('America/New_York',),
  '1850217':('America/Chicago',),
  '1850215':('America/Chicago',),
- '1850212':('America/New_York',),
  '1850213':('America/Chicago',),
- '1850210':('America/New_York',),
  '1219785':('America/Chicago',),
  '1219787':('America/Chicago',),
+ '1208215':('America/Los_Angeles',),
  '1701795':('America/Chicago',),
  '351238':('Europe/Lisbon',),
  '351239':('Europe/Lisbon',),
  '1701793':('America/Chicago',),
  '351232':('Europe/Lisbon',),
  '351233':('Europe/Lisbon',),
  '351231':('Europe/Lisbon',),
@@ -5518,47 +4613,34 @@
  '441603':('Europe/London',),
  '1775537':('America/Los_Angeles',),
  '441600':('Europe/London',),
  '441606':('Europe/London',),
  '441604':('Europe/London',),
  '441609':('Europe/London',),
  '441608':('Europe/London',),
- '1250226':('America/Vancouver',),
- '1250220':('America/Vancouver',),
+ '1709687':('America/St_Johns',),
  '1709685':('America/St_Johns',),
- '55153245':('America/Manaus',),
+ '1709682':('America/St_Johns',),
  '1270640':('America/Chicago',),
  '1270646':('America/Chicago',),
- '1709673':('America/St_Johns',),
  '1701757':('America/Chicago',),
  '55933582':('America/Sao_Paulo',),
  '55933589':('America/Sao_Paulo',),
  '52486':('America/Mexico_City',),
  '52487':('America/Mexico_City',),
  '52485':('America/Mexico_City',),
  '52482':('America/Mexico_City',),
  '1423787':('America/New_York',),
  '1423784':('America/New_York',),
- '1418228':('America/Toronto',),
- '1418227':('America/Toronto',),
- '1418226':('America/Toronto',),
- '1418222':('America/Toronto',),
+ '52481':('America/Mexico_City',),
+ '1423788':('America/New_York',),
  '52488':('America/Mexico_City',),
  '52489':('America/Mexico_City',),
- '1812665':('America/New_York',),
- '1812663':('America/New_York',),
- '1812662':('America/New_York',),
  '1605232':('America/Chicago',),
  '1605234':('America/Chicago',),
- '1574268':('America/New_York',),
- '1574269':('America/New_York',),
- '1574262':('America/New_York',),
- '1574266':('America/New_York',),
- '1574267':('America/New_York',),
- '1574264':('America/New_York',),
  '52738':('America/Mexico_City',),
  '52739':('America/Mexico_City',),
  '1423569':('America/New_York',),
  '1423566':('America/New_York',),
  '52735':('America/Mexico_City',),
  '52736':('America/Mexico_City',),
  '52737':('America/Mexico_City',),
@@ -5577,186 +4659,168 @@
  '34971':('Europe/Madrid',),
  '34976':('Europe/Madrid',),
  '34977':('Europe/Madrid',),
  '34974':('Europe/Madrid',),
  '34975':('Europe/Madrid',),
  '34978':('Europe/Madrid',),
  '34979':('Europe/Madrid',),
- '1785628':('America/Chicago',),
- '1785621':('America/Chicago',),
- '1785623':('America/Chicago',),
- '1785625':('America/Chicago',),
- '1785626':('America/Chicago',),
  '441386':('Europe/London',),
  '441387':('Europe/London',),
  '441384':('Europe/London',),
- '1812939':('America/New_York',),
+ '441382':('Europe/London',),
  '441383':('Europe/London',),
  '441380':('Europe/London',),
  '441381':('Europe/London',),
- '1812934':('America/New_York',),
  '1812937':('America/Chicago',),
- '1812936':('America/New_York',),
- '1812933':('America/New_York',),
- '1812932':('America/New_York',),
+ '441388':('Europe/London',),
+ '441389':('Europe/London',),
  '1701549':('America/Chicago',),
  '691350':('Pacific/Truk',),
  '1701540':('America/Chicago',),
  '52751':('America/Mexico_City',),
  '55914103':('America/Sao_Paulo',),
  '55914104':('America/Sao_Paulo',),
  '55914107':('America/Sao_Paulo',),
  '8683':('Asia/Shanghai',),
  '52755':('America/Mexico_City',),
  '1701893':('America/Chicago',),
  '1701324':('America/Chicago',),
  '1701323':('America/Chicago',),
  '1701328':('America/Chicago',),
+ '1208350':('America/Denver',),
  '1308284':('America/Denver',),
  '1850916':('America/Chicago',),
  '1850913':('America/Chicago',),
  '1308282':('America/Denver',),
  '86744':('Asia/Shanghai',),
  '86745':('Asia/Shanghai',),
  '86746':('Asia/Shanghai',),
  '86743':('Asia/Shanghai',),
+ '1208351':('America/Denver',),
  '1541464':('America/Los_Angeles',),
  '1541465':('America/Los_Angeles',),
  '1541466':('America/Los_Angeles',),
  '1541461':('America/Los_Angeles',),
  '1541463':('America/Los_Angeles',),
  '1541469':('America/Los_Angeles',),
- '55813639':('America/Sao_Paulo',),
- '55813638':('America/Sao_Paulo',),
- '1208354':('America/Denver',),
- '1812320':('America/New_York',),
- '1812322':('America/New_York',),
- '1812323':('America/New_York',),
- '1850663':('America/New_York',),
- '1812325':('America/New_York',),
- '1812327':('America/New_York',),
- '1850668':('America/New_York',),
+ '441676':('Europe/London',),
+ '441677':('Europe/London',),
+ '1850664':('America/Chicago',),
  '55819839':('America/Sao_Paulo',),
  '521238':('America/Mexico_City',),
- '521237':('America/Mexico_City',),
+ '55819831':('America/Sao_Paulo',),
  '521236':('America/Mexico_City',),
  '521235':('America/Mexico_City',),
  '55819832':('America/Sao_Paulo',),
  '521233':('America/Mexico_City',),
  '521232':('America/Mexico_City',),
- '521231':('America/Mexico_City',),
+ '55819837':('America/Sao_Paulo',),
  '55819836':('America/Sao_Paulo',),
  '1270825':('America/Chicago',),
- '55813637':('America/Sao_Paulo',),
+ '441678':('Europe/London',),
  '1812490':('America/Chicago',),
  '1812491':('America/Chicago',),
- '994':('Asia/Baku',),
  '1907424':('America/Juneau',),
  '55813091':('America/Sao_Paulo',),
  '55813090':('America/Sao_Paulo',),
  '55813093':('America/Sao_Paulo',),
  '55813092':('America/Sao_Paulo',),
  '55813095':('America/Sao_Paulo',),
  '55813094':('America/Sao_Paulo',),
  '55813097':('America/Sao_Paulo',),
- '55813096':('America/Sao_Paulo',),
+ '55813724':('America/Sao_Paulo',),
  '55813099':('America/Sao_Paulo',),
  '55813729':('America/Sao_Paulo',),
  '55813728':('America/Sao_Paulo',),
  '1219261':('America/Chicago',),
- '44130':('Europe/London',),
- '1208772':('America/Los_Angeles',),
- '1250412':('America/Vancouver',),
  '55813545':('America/Sao_Paulo',),
  '55813544':('America/Sao_Paulo',),
  '55813543':('America/Sao_Paulo',),
  '1250417':('America/Edmonton',),
  '55813541':('America/Sao_Paulo',),
  '55813548':('America/Sao_Paulo',),
  '390521':('Europe/Rome',),
  '390523':('Europe/Rome',),
  '390522':('Europe/Rome',),
  '390525':('Europe/Rome',),
  '390524':('Europe/Rome',),
  '62824':('Asia/Jakarta', 'Asia/Makassar'),
- '1785434':('America/Chicago',),
- '1785437':('America/Chicago',),
  '7851':('Europe/Samara',),
  '7855':('Europe/Moscow',),
  '1208830':('America/Denver',),
  '1219963':('America/Chicago',),
  '1219962':('America/Chicago',),
- '1620375':('America/Chicago',),
- '1250951':('America/Vancouver',),
  '1208835':('America/Los_Angeles',),
  '1605574':('America/Denver',),
  '1208837':('America/Denver',),
  '1605578':('America/Denver',),
  '1775726':('America/Los_Angeles',),
  '1775727':('America/Los_Angeles',),
  '1775722':('America/Los_Angeles',),
  '1775720':('America/Los_Angeles',),
  '1775721':('America/Los_Angeles',),
  '62878':('Asia/Jakarta',),
  '62879':('Asia/Jakarta',),
- '1906487':('America/New_York',),
- '1906486':('America/New_York',),
- '1906485':('America/New_York',),
- '1906484':('America/New_York',),
- '1906483':('America/New_York',),
- '1906482':('America/New_York',),
+ '521967':('America/Mexico_City',),
+ '62870':('Asia/Jakarta',),
+ '62871':('Asia/Jakarta',),
+ '62872':('Asia/Jakarta',),
+ '62873':('Asia/Jakarta',),
+ '62874':('Asia/Jakarta',),
+ '62875':('Asia/Jakarta',),
  '62876':('Asia/Jakarta', 'Asia/Makassar'),
  '62877':('Asia/Jakarta',),
  '55553682':('America/Manaus',),
- '1208917':('America/Denver',),
+ '1605':('America/Denver', 'America/North_Dakota/Center'),
+ '1604':('America/Vancouver',),
  '1971':('America/Los_Angeles',),
+ '1606':('America/New_York',),
  '521435':('America/Mexico_City',),
  '521434':('America/Mexico_City',),
  '521437':('America/Mexico_City',),
  '521436':('America/Mexico_City',),
  '521431':('America/Mexico_City',),
  '1208908':('America/Denver',),
  '1618':('America/Chicago',),
- '521432':('America/Mexico_City',),
+ '1619':('America/Los_Angeles',),
  '1616':('America/New_York',),
  '1208904':('America/Denver',),
  '1614':('America/New_York',),
  '1208906':('America/Denver',),
- '1612':('America/Chicago',),
+ '1208901':('America/Denver',),
  '1613':('America/Toronto',),
  '1610':('America/New_York',),
  '1541923':('America/Los_Angeles',),
  '1541922':('America/Los_Angeles',),
  '1541924':('America/Los_Angeles',),
  '1541926':('America/Los_Angeles',),
  '1541929':('America/Los_Angeles',),
  '1541928':('America/Los_Angeles',),
  '1541679':('America/Los_Angeles',),
  '1541678':('America/Los_Angeles',),
  '1541673':('America/Los_Angeles',),
  '1541672':('America/Los_Angeles',),
  '1541677':('America/Los_Angeles',),
  '1541676':('America/Los_Angeles',),
- '1620767':('America/Chicago',),
+ '521758':('America/Mexico_City',),
  '521759':('America/Mexico_City',),
  '1423224':('America/New_York',),
  '62254':('Asia/Jakarta',),
  '521751':('America/Mexico_City',),
  '521753':('America/Mexico_City',),
  '521754':('America/Mexico_City',),
  '521755':('America/Mexico_City',),
  '521756':('America/Mexico_City',),
- '521757':('America/Mexico_City',),
- '55913019':('America/Sao_Paulo',),
+ '62253':('Asia/Jakarta',),
+ '55813041':('America/Sao_Paulo',),
  '55813046':('America/Sao_Paulo',),
  '55913013':('America/Sao_Paulo',),
- '1418449':('America/Toronto',),
- '55813049':('America/Sao_Paulo',),
- '55913017':('America/Sao_Paulo',),
- '1541255':('America/Los_Angeles',),
+ '441536':('Europe/London',),
+ '441530':('Europe/London',),
+ '1270683':('America/Chicago',),
  '1850279':('America/Chicago',),
  '1850271':('America/Chicago',),
  '1850276':('America/Chicago',),
  '1208278':('America/Denver',),
  '1219769':('America/Chicago',),
  '1219766':('America/Chicago',),
  '1219764':('America/Chicago',),
@@ -5764,52 +4828,43 @@
  '1219762':('America/Chicago',),
  '55913295':('America/Sao_Paulo',),
  '55913297':('America/Sao_Paulo',),
  '55913292':('America/Sao_Paulo',),
  '55913298':('America/Sao_Paulo',),
  '55913299':('America/Sao_Paulo',),
  '1541582':('America/Los_Angeles',),
- '55913734':('America/Sao_Paulo',),
+ '1541580':('America/Los_Angeles',),
  '521741':('America/Mexico_City',),
- '1785312':('America/Chicago',),
  '55913120':('America/Sao_Paulo',),
  '55913121':('America/Sao_Paulo',),
- '55919998':('America/Sao_Paulo',),
  '1850586':('America/Chicago',),
- '390925':('Europe/Rome',),
- '1850584':('America/New_York',),
+ '1850587':('America/Chicago',),
  '1850585':('America/Chicago',),
- '1850580':('America/New_York',),
  '1850581':('America/Chicago',),
  '55913732':('America/Sao_Paulo',),
  '1850588':('America/Chicago',),
  '390437':('Europe/Rome',),
- '390923':('Europe/Rome',),
- '55913731':('America/Sao_Paulo',),
+ '390435':('Europe/Rome',),
  '390922':('Europe/Rome',),
  '52938':('America/Mexico_City',),
  '52936':('America/Mexico_City',),
  '52937':('America/Mexico_City',),
  '52934':('America/Mexico_City',),
  '52932':('America/Mexico_City',),
  '52933':('America/Mexico_City',),
- '1308872':('America/Chicago',),
  '1270629':('America/Chicago',),
  '1270628':('America/Chicago',),
  '1308874':('America/Denver',),
  '1270622':('America/Chicago',),
- '1308728':('America/Chicago',),
  '55813974':('America/Sao_Paulo',),
  '1907677':('America/Juneau',),
  '1423768':('America/New_York',),
  '1423764':('America/New_York',),
  '1423765':('America/New_York',),
- '1418204':('America/Toronto',),
- '1812689':('America/New_York',),
- '1812683':('America/New_York',),
+ '1423760':('America/New_York',),
  '1812682':('America/Chicago',),
  '1605745':('America/Denver',),
  '1605747':('America/Chicago',),
  '1605217':('America/Chicago',),
  '1605743':('America/Chicago',),
  '62401':('Asia/Makassar',),
  '62403':('Asia/Jayapura', 'Asia/Makassar'),
@@ -5826,46 +4881,37 @@
  '1423503':('America/New_York',),
  '52756':('America/Mexico_City',),
  '52757':('America/Mexico_City',),
  '52754':('America/Mexico_City',),
  '1423507':('America/New_York',),
  '1709753':('America/St_Johns',),
  '1709754':('America/St_Johns',),
- '1620488':('America/Chicago',),
- '1620378':('America/Chicago',),
  '390884':('Europe/Rome',),
  '390885':('Europe/Rome',),
  '390882':('Europe/Rome',),
  '390883':('Europe/Rome',),
  '390881':('Europe/Rome',),
- '1250956':('America/Vancouver',),
- '1250954':('America/Vancouver',),
- '1250952':('America/Vancouver',),
+ '62865':('Asia/Jakarta',),
  '1620376':('America/Denver',),
  '7336':('Asia/Almaty',),
- '1574936':('America/New_York',),
- '1574935':('America/New_York',),
  '62927':('Asia/Jayapura',),
  '1701523':('America/Denver',),
  '1701527':('America/Chicago',),
- '1423447':('America/Chicago',),
  '55919807':('America/Sao_Paulo',),
  '55919806':('America/Sao_Paulo',),
  '55919805':('America/Sao_Paulo',),
  '55919804':('America/Sao_Paulo',),
  '55919803':('America/Sao_Paulo',),
  '55919802':('America/Sao_Paulo',),
  '55919801':('America/Sao_Paulo',),
  '691370':('Pacific/Kosrae',),
  '55919809':('America/Sao_Paulo',),
  '55919808':('America/Sao_Paulo',),
- '55813446':('America/Sao_Paulo',),
+ '55813194':('America/Sao_Paulo',),
  '1605964':('America/Denver',),
- '1606242':('America/New_York',),
- '1606248':('America/New_York',),
  '55913355':('America/Sao_Paulo',),
  '521653':('America/Mazatlan',),
  '55913351':('America/Sao_Paulo',),
  '55913353':('America/Sao_Paulo',),
  '55913352':('America/Sao_Paulo',),
  '8637':('Asia/Shanghai',),
  '8635':('Asia/Shanghai',),
@@ -5885,66 +4931,54 @@
  '86722':('Asia/Shanghai',),
  '56':('America/Santiago', 'Pacific/Easter'),
  '62920':('Asia/Jakarta',),
  '53':('America/Havana',),
  '1541447':('America/Los_Angeles',),
  '1541444':('America/Los_Angeles',),
  '1541440':('America/Los_Angeles',),
+ '1541441':('America/Los_Angeles',),
  '1219374':('America/Chicago',),
- '1418859':('America/Toronto',),
- '1418588':('America/Toronto',),
- '1418589':('America/Toronto',),
- '1418854':('America/Toronto',),
- '1418587':('America/Toronto',),
- '1418856':('America/Toronto',),
- '1418851':('America/Toronto',),
- '1418853':('America/Toronto',),
- '856':('Asia/Vientiane',),
+ '421':('Europe/Bratislava',),
+ '420':('Europe/Prague',),
+ '423':('Europe/Vaduz',),
  '1850640':('America/Chicago',),
- '1850643':('America/New_York',),
- '1850644':('America/New_York',),
- '853':('Asia/Shanghai',),
- '590':('America/Guadeloupe', 'America/Halifax', 'America/Marigot'),
- '55813709':('America/Sao_Paulo',),
+ '1423':('America/Chicago',),
  '1219595':('America/Chicago',),
  '1907442':('America/Juneau',),
  '1907443':('America/Juneau',),
  '55813701':('America/Sao_Paulo',),
  '55813705':('America/Sao_Paulo',),
- '55813707':('America/Sao_Paulo',),
- '1785380':('America/Chicago',),
  '5593991':('America/Sao_Paulo',),
  '1424':('America/Los_Angeles',),
- '55813228':('America/Sao_Paulo',),
- '55813229':('America/Sao_Paulo',),
+ '441757':('Europe/London',),
+ '441756':('Europe/London',),
  '55813561':('America/Sao_Paulo',),
  '55813563':('America/Sao_Paulo',),
  '55813562':('America/Sao_Paulo',),
  '52231':('America/Mexico_City',),
  '52233':('America/Mexico_City',),
  '52232':('America/Mexico_City',),
  '52235':('America/Mexico_City',),
  '52237':('America/Mexico_City',),
  '52236':('America/Mexico_City',),
  '52238':('America/Mexico_City',),
  '2432':('Africa/Lubumbashi',),
  '2431':('Africa/Kinshasa',),
  '2436':('Africa/Kinshasa',),
  '2435':('Africa/Kinshasa',),
- '55813227':('America/Sao_Paulo',),
+ '441758':('Europe/London',),
  '1775298':('America/Los_Angeles',),
  '1775525':('America/Los_Angeles',),
  '7833':('Europe/Moscow',),
  '7834':('Europe/Moscow',),
  '7835':('Europe/Moscow',),
  '7836':('Europe/Moscow',),
  '55913434':('America/Sao_Paulo',),
  '52588':('America/Mexico_City',),
  '1605553':('America/Chicago',),
- '55913284':('America/Sao_Paulo',),
  '1775742':('America/Los_Angeles',),
  '1775746':('America/Los_Angeles',),
  '1775747':('America/Los_Angeles',),
  '1807':('America/Toronto',),
  '1806':('America/Chicago',),
  '1805':('America/Los_Angeles',),
  '1804':('America/New_York',),
@@ -5956,182 +4990,144 @@
  '1270830':('America/Chicago',),
  '1270831':('America/Chicago',),
  '1270384':('America/Chicago',),
  '44129':('Europe/London',),
  '1270388':('America/Chicago',),
  '1270389':('America/Chicago',),
  '44121':('Europe/London',),
- '1574893':('America/New_York',),
- '1574892':('America/New_York',),
  '1574896':('America/Chicago',),
- '1574546':('America/New_York',),
  '55913288':('America/Sao_Paulo',),
  '1949':('America/Los_Angeles',),
  '521419':('America/Mexico_City',),
  '521418':('America/Mexico_City',),
  '521417':('America/Mexico_City',),
  '1940':('America/Chicago',),
- '521414':('America/Mexico_City',),
+ '1941':('America/New_York',),
  '521413':('America/Mexico_City',),
  '521412':('America/Mexico_City',),
  '521411':('America/Mexico_City',),
  '1541948':('America/Los_Angeles',),
  '1541942':('America/Los_Angeles',),
  '1541941':('America/Los_Angeles',),
  '1541947':('America/Los_Angeles',),
  '1541944':('America/Los_Angeles',),
  '521732':('America/Mexico_City',),
  '521733':('America/Mexico_City',),
- '1606589':('America/New_York',),
  '521731':('America/Mexico_City',),
  '521736':('America/Mexico_City',),
  '521737':('America/Mexico_City',),
  '521734':('America/Mexico_City',),
- '420':('Europe/Prague',),
+ '521735':('America/Mexico_City',),
  '521738':('America/Mexico_City',),
  '521739':('America/Mexico_City',),
- '423':('Europe/Vaduz',),
  '62232':('Asia/Jakarta',),
  '62233':('Asia/Jakarta',),
  '62231':('Asia/Jakarta',),
  '1423247':('America/New_York',),
  '1423246':('America/New_York',),
  '1423245':('America/New_York',),
- '62963':('Asia/Jakarta',),
  '1219845':('America/Chicago',),
- '1606723':('America/New_York',),
  '1208789':('America/Denver',),
  '1208788':('America/Denver',),
  '1208783':('America/Los_Angeles',),
  '1208782':('America/Denver',),
  '1208787':('America/Denver',),
  '1208785':('America/Denver',),
  '1208784':('America/Los_Angeles',),
- '62484':('Asia/Makassar',),
  '1541610':('America/Los_Angeles',),
  '1541617':('America/Los_Angeles',),
  '1541618':('America/Los_Angeles',),
  '1234':('America/New_York',),
  '1208254':('America/Denver',),
  '1208525':('America/Denver',),
  '1208524':('America/Denver',),
  '1208523':('America/Denver',),
- '1208522':('America/Denver',),
+ '1231':('America/New_York',),
  '1208521':('America/Denver',),
  '1208520':('America/Denver',),
  '1239':('America/New_York',),
  '1208529':('America/Denver',),
  '1208528':('America/Denver',),
  '1219299':('America/Chicago',),
- '1574699':('America/New_York',),
  '35122':('Europe/Lisbon',),
  '35121':('Europe/Lisbon',),
- '55913751':('America/Sao_Paulo',),
  '55913796':('America/Sao_Paulo',),
  '1850250':('America/Chicago',),
- '1850251':('America/New_York',),
  '1850256':('America/Chicago',),
  '1850258':('America/Chicago',),
  '1850259':('America/Chicago',),
  '1907388':('America/Juneau',),
- '1423837':('America/Chicago',),
  '52914':('America/Mexico_City',),
  '52916':('America/Mexico_City',),
  '52917':('America/Mexico_City',),
  '52913':('America/Mexico_City',),
  '52918':('America/Mexico_City',),
  '52919':('America/Mexico_City',),
- '1250597':('America/Vancouver',),
- '1250596':('America/Vancouver',),
- '1250595':('America/Vancouver',),
- '1250594':('America/Vancouver',),
- '1250592':('America/Vancouver',),
- '1250591':('America/Vancouver',),
- '1250590':('America/Vancouver',),
- '1250598':('America/Vancouver',),
- '1906387':('America/New_York',),
+ '7395':('Asia/Irkutsk',),
+ '55813912':('America/Sao_Paulo',),
+ '994':('Asia/Baku',),
  '62534':('Asia/Jakarta',),
  '86898':('Asia/Shanghai',),
  '62537':('Asia/Jakarta',),
  '86891':('Asia/Shanghai',),
  '86892':('Asia/Shanghai',),
  '86893':('Asia/Shanghai',),
  '86894':('Asia/Shanghai',),
  '86895':('Asia/Shanghai',),
  '86896':('Asia/Shanghai',),
  '86897':('Asia/Shanghai',),
  '1':('America/Anguilla', 'America/Antigua', 'America/Barbados', 'America/Boise', 'America/Cayman', 'America/Chicago', 'America/Denver', 'America/Dominica', 'America/Edmonton', 'America/Grand_Turk', 'America/Grenada', 'America/Halifax', 'America/Jamaica', 'America/Juneau', 'America/Los_Angeles', 'America/Lower_Princes', 'America/Montserrat', 'America/Nassau', 'America/New_York', 'America/Phoenix', 'America/Port_of_Spain', 'America/Puerto_Rico', 'America/Santo_Domingo', 'America/St_Johns', 'America/St_Kitts', 'America/St_Lucia', 'America/St_Thomas', 'America/St_Vincent', 'America/Toronto', 'America/Tortola', 'America/Vancouver', 'America/Winnipeg', 'Atlantic/Bermuda', 'Pacific/Guam', 'Pacific/Honolulu', 'Pacific/Pago_Pago', 'Pacific/Saipan'),
- '1418263':('America/Toronto',),
- '1418262':('America/Toronto',),
- '1418261':('America/Toronto',),
+ '1423746':('America/New_York',),
+ '1423744':('America/New_York',),
  '1423745':('America/New_York',),
- '1418266':('America/Toronto',),
- '1250627':('America/Vancouver',),
- '1418264':('America/Toronto',),
- '1250629':('America/Vancouver',),
- '1418269':('America/Toronto',),
- '1418268':('America/Toronto',),
+ '1423743':('America/New_York',),
  '998':('Asia/Tashkent',),
  '1605765':('America/Chicago',),
  '1605763':('America/Chicago',),
- '1906524':('America/New_York',),
  '52771':('America/Mexico_City',),
  '52772':('America/Mexico_City',),
  '1423521':('America/New_York',),
  '52774':('America/Mexico_City',),
  '52775':('America/Mexico_City',),
  '52776':('America/Mexico_City',),
- '1906523':('America/New_York',),
+ '1423525':('America/New_York',),
  '52778':('America/Mexico_City',),
  '52779':('America/Mexico_City',),
  '62423':('Asia/Makassar',),
  '62422':('Asia/Makassar',),
  '62421':('Asia/Makassar',),
  '62420':('Asia/Makassar',),
- '86597':('Asia/Shanghai',),
  '86596':('Asia/Shanghai',),
  '1605498':('America/Chicago',),
- '1620356':('America/Chicago',),
- '1620357':('America/Chicago',),
- '1620355':('America/Chicago',),
- '1250979':('America/Vancouver',),
- '1250974':('America/Vancouver',),
+ '1208639':('America/Denver',),
  '441838':('Europe/London',),
  '441830':('Europe/London',),
  '441832':('Europe/London',),
  '441833':('Europe/London',),
  '441834':('Europe/London',),
  '441835':('Europe/London',),
  '441837':('Europe/London',),
  '55943311':('America/Sao_Paulo',),
- '1605940':('America/Chicago',),
+ '55943312':('America/Sao_Paulo',),
+ '1605941':('America/Chicago',),
  '1605946':('America/Chicago',),
  '55943315':('America/Sao_Paulo',),
  '1605945':('America/Chicago',),
  '55943319':('America/Sao_Paulo',),
  '55914141':('America/Sao_Paulo',),
  '55813708':('America/Sao_Paulo',),
  '86701':('Asia/Shanghai',),
- '1605543':('America/Chicago',),
- '1574372':('America/New_York',),
  '1541420':('America/Los_Angeles',),
  '1541426':('America/Los_Angeles',),
- '1418877':('America/Toronto',),
- '1418875':('America/Toronto',),
- '1418872':('America/Toronto',),
- '1418873':('America/Toronto',),
- '1418871':('America/Toronto',),
- '1418878':('America/Toronto',),
  '8610':('Asia/Shanghai',),
  '8613':('Asia/Shanghai',),
  '8618':('Asia/Shanghai',),
  '160533':('America/Chicago',),
  '1850623':('America/Chicago',),
  '1850622':('America/Chicago',),
- '1850627':('America/New_York',),
  '1850626':('America/Chicago',),
  '1850624':('America/Chicago',),
  '521273':('America/Mexico_City',),
  '521272':('America/Mexico_City',),
  '521271':('America/Mexico_City',),
  '521276':('America/Mexico_City',),
  '521275':('America/Mexico_City',),
@@ -6142,27 +5138,15 @@
  '441581':('Europe/London',),
  '441582':('Europe/London',),
  '441583':('Europe/London',),
  '441584':('Europe/London',),
  '441586':('Europe/London',),
  '441588':('Europe/London',),
  '1907463':('America/Juneau',),
- '55813762':('America/Sao_Paulo',),
- '55813761':('America/Sao_Paulo',),
  '1907465':('America/Juneau',),
- '1250368':('America/Vancouver',),
- '1250364':('America/Vancouver',),
- '1250365':('America/Vancouver',),
- '1250367':('America/Vancouver',),
- '1250360':('America/Vancouver',),
- '1250361':('America/Vancouver',),
- '1250362':('America/Vancouver',),
- '1250363':('America/Vancouver',),
- '691950':('Pacific/Truk',),
- '1219472':('America/Chicago',),
  '55813581':('America/Sao_Paulo',),
  '7816':('Europe/Moscow',),
  '1208365':('America/Denver',),
  '7814':('Europe/Moscow',),
  '7815':('Europe/Moscow',),
  '7812':('Europe/Moscow',),
  '7813':('Europe/Moscow',),
@@ -6179,26 +5163,23 @@
  '55913412':('America/Sao_Paulo',),
  '55913411':('America/Sao_Paulo',),
  '1208362':('America/Denver',),
  '55817916':('America/Sao_Paulo',),
  '1775762':('America/Los_Angeles',),
  '1605539':('America/Chicago',),
  '1605532':('America/Chicago',),
- '1219476':('America/Chicago',),
  '1829':('America/Halifax',),
  '1828':('America/New_York',),
  '1825':('America/Edmonton',),
- '1812725':('America/New_York',),
- '1812723':('America/New_York',),
- '55813136':('America/Sao_Paulo',),
+ '1820':('America/Los_Angeles',),
+ '441449':('Europe/London',),
  '1920':('America/Chicago',),
  '1925':('America/Los_Angeles',),
  '1928':('America/Denver',),
  '1929':('America/New_York',),
- '55813138':('America/Sao_Paulo',),
  '521478':('America/Mexico_City',),
  '1541967':('America/Los_Angeles',),
  '1541966':('America/Los_Angeles',),
  '1541961':('America/Los_Angeles',),
  '1541963':('America/Los_Angeles',),
  '1541962':('America/Los_Angeles',),
  '521471':('America/Mexico_City',),
@@ -6208,42 +5189,30 @@
  '1541968':('America/Los_Angeles',),
  '521477':('America/Mexico_City',),
  '521476':('America/Mexico_City',),
  '390781':('Europe/Rome',),
  '390783':('Europe/Rome',),
  '390782':('Europe/Rome',),
  '390785':('Europe/Rome',),
- '1270773':('America/Chicago',),
+ '1541505':('America/Los_Angeles',),
  '390789':('Europe/Rome',),
  '1423265':('America/New_York',),
  '62747':('Asia/Jakarta',),
  '1423267':('America/New_York',),
  '1423266':('America/New_York',),
  '521718':('America/Mexico_City',),
  '521719':('America/Mexico_City',),
  '1423263':('America/New_York',),
  '1423262':('America/New_York',),
- '521714':('America/Mexico_City', 'America/Tijuana'),
  '521715':('America/Mexico_City',),
  '521716':('America/Mexico_City',),
  '521717':('America/Mexico_City',),
  '521711':('America/Mexico_City',),
  '521712':('America/Mexico_City',),
  '521713':('America/Mexico_City',),
- '1620728':('America/Chicago',),
- '34859':('Europe/Madrid',),
- '34858':('Europe/Madrid',),
- '1620723':('America/Chicago',),
- '34854':('Europe/Madrid',),
- '34857':('Europe/Madrid',),
- '34856':('Europe/Madrid',),
- '34851':('Europe/Madrid',),
- '34850':('Europe/Madrid',),
- '1620725':('America/Chicago',),
- '1620724':('America/Chicago',),
  '55943787':('America/Sao_Paulo',),
  '55943786':('America/Sao_Paulo',),
  '55943785':('America/Sao_Paulo',),
  '60':('Asia/Kuching',),
  '61':('Antarctica/Macquarie', 'Australia/Adelaide', 'Australia/Eucla', 'Australia/Lord_Howe', 'Australia/Perth', 'Australia/Sydney', 'Indian/Christmas', 'Indian/Cocos'),
  '62':('Asia/Jakarta', 'Asia/Jayapura', 'Asia/Makassar'),
  '63':('Asia/Manila',),
@@ -6261,70 +5230,65 @@
  '506':('America/Costa_Rica',),
  '507':('America/Panama',),
  '504':('America/Tegucigalpa',),
  '1541636':('America/Los_Angeles',),
  '502':('America/Guatemala',),
  '503':('America/El_Salvador',),
  '1541633':('America/Los_Angeles',),
- '501':('America/Belize',),
+ '1541632':('America/Los_Angeles',),
  '1212':('America/New_York',),
  '1213':('America/Los_Angeles',),
  '1210':('America/Chicago',),
- '1216':('America/New_York',),
+ '1208505':('America/Denver',),
  '1217':('America/Chicago',),
  '1214':('America/Chicago',),
  '1215':('America/New_York',),
  '1218':('America/Chicago',),
- '1219728':('America/Chicago',),
+ '1219':('America/New_York',),
  '1701265':('America/Chicago',),
  '1701261':('America/Chicago',),
  '5581998':('America/Sao_Paulo',),
  '5581999':('America/Sao_Paulo',),
  '5581994':('America/Sao_Paulo',),
  '5581995':('America/Sao_Paulo',),
  '5581996':('America/Sao_Paulo',),
  '5581997':('America/Sao_Paulo',),
  '5581991':('America/Sao_Paulo',),
  '5581992':('America/Sao_Paulo',),
  '5581993':('America/Sao_Paulo',),
  '1775888':('America/Los_Angeles',),
- '1907892':('America/Juneau',),
+ '1423307':('America/New_York',),
  '1775883':('America/Los_Angeles',),
  '1775882':('America/Los_Angeles',),
  '1775887':('America/Los_Angeles',),
  '1775886':('America/Los_Angeles',),
  '1775885':('America/Los_Angeles',),
  '1775884':('America/Los_Angeles',),
- '55813128':('America/Sao_Paulo',),
  '7831':('Europe/Moscow',),
  '35818':('Europe/Mariehamn',),
  '35819':('Europe/Helsinki',),
  '35813':('Europe/Helsinki',),
  '35816':('Europe/Helsinki',),
  '35817':('Europe/Helsinki',),
  '35814':('Europe/Helsinki',),
  '35815':('Europe/Helsinki',),
  '52972':('America/Mexico_City',),
  '52971':('America/Mexico_City',),
- '1812539':('America/New_York',),
- '1812533':('America/New_York',),
- '1812535':('America/New_York',),
  '441455':('Europe/London',),
  '1423892':('America/New_York',),
- '1208882':('America/Los_Angeles',),
+ '1423893':('America/New_York',),
  '1423722':('America/New_York',),
  '1701766':('America/Chicago',),
- '1418248':('America/Toronto',),
+ '1423725':('America/New_York',),
  '1423894':('America/New_York',),
  '1423727':('America/New_York',),
  '1423728':('America/New_York',),
- '1250642':('America/Vancouver',),
- '1418247':('America/Toronto',),
+ '97623':('Asia/Ulaanbaatar',),
  '1423899':('America/New_York',),
- '97625':('Asia/Ulaanbaatar',),
+ '441452':('Europe/London',),
  '97624':('Asia/Hovd',),
  '3487':('Europe/Madrid',),
  '55813249':('America/Sao_Paulo',),
  '55813241':('America/Sao_Paulo',),
  '55813242':('America/Sao_Paulo',),
  '55813243':('America/Sao_Paulo',),
  '55813244':('America/Sao_Paulo',),
@@ -6338,203 +5302,171 @@
  '62410':('Asia/Makassar',),
  '62915':('Asia/Jakarta', 'Asia/Jayapura'),
  '52791':('America/Mexico_City',),
  '62411':('Asia/Makassar',),
  '52763':('America/Mexico_City',),
  '62417':('Asia/Makassar',),
  '62414':('Asia/Makassar',),
- '1250914':('America/Vancouver',),
  '390331':('Europe/Rome',),
  '390332':('Europe/Rome',),
  '441852':('Europe/London',),
  '441851':('Europe/London',),
  '441856':('Europe/London',),
  '441857':('Europe/London',),
  '441854':('Europe/London',),
  '441855':('Europe/London',),
  '441858':('Europe/London',),
  '441859':('Europe/London',),
- '1574970':('America/New_York',),
- '1574971':('America/New_York',),
  '55943337':('America/Sao_Paulo',),
  '55943335':('America/Sao_Paulo',),
  '55943332':('America/Sao_Paulo',),
  '55943333':('America/Sao_Paulo',),
  '55943331':('America/Sao_Paulo',),
- '1606932':('America/New_York',),
  '1308327':('America/Denver',),
- '1308324':('America/Chicago',),
  '24345':('Africa/Kinshasa',),
- '1308221':('America/Chicago',),
- '1812882':('America/New_York',),
- '1812885':('America/New_York',),
- '1812886':('America/New_York',),
  '1219757':('America/Chicago',),
  '1541408':('America/Los_Angeles',),
  '8671':('Asia/Shanghai',),
  '8677':('Asia/Shanghai',),
  '1701385':('America/Chicago',),
  '1219755':('America/Chicago',),
  '8679':('Asia/Shanghai',),
  '1701388':('America/Chicago',),
  '1850607':('America/Chicago',),
- '1850606':('America/New_York',),
- '55813318':('America/Sao_Paulo',),
- '55813319':('America/Sao_Paulo',),
- '55813648':('America/Sao_Paulo',),
+ '441667':('Europe/London',),
+ '441666':('Europe/London',),
+ '441661':('Europe/London',),
  '521294':('America/Mexico_City',),
  '521297':('America/Mexico_City',),
  '521296':('America/Mexico_City',),
  '1867645':('America/Winnipeg',),
- '55813644':('America/Sao_Paulo',),
- '55813311':('America/Sao_Paulo',),
- '1907581':('Pacific/Honolulu',),
- '441668':('Europe/London',),
- '55813642':('America/Sao_Paulo',),
+ '55813312':('America/Sao_Paulo',),
+ '1907586':('America/Juneau',),
+ '55813316':('America/Sao_Paulo',),
+ '1564':('America/Los_Angeles',),
+ '55813641':('America/Sao_Paulo',),
+ '55813314':('America/Sao_Paulo',),
  '55813745':('America/Sao_Paulo',),
- '1250347':('America/Edmonton',),
+ '55813744':('America/Sao_Paulo',),
  '1250344':('America/Edmonton',),
  '55813746':('America/Sao_Paulo',),
  '1250342':('America/Edmonton',),
  '55813743':('America/Sao_Paulo',),
- '1250341':('America/Edmonton',),
+ '55813742':('America/Sao_Paulo',),
  '55813748':('America/Sao_Paulo',),
- '1785838':('America/Chicago',),
- '1785830':('America/Chicago',),
- '1785832':('America/Chicago',),
- '1785836':('America/Chicago',),
  '52899':('America/Mexico_City',),
  '52891':('America/Mexico_City',),
  '52892':('America/Mexico_City',),
  '52894':('America/Mexico_City',),
  '52897':('America/Mexico_City',),
- '55813861':('America/Sao_Paulo',),
  '1906753':('America/Chicago',),
  '1270415':('America/Chicago',),
  '86919':('Asia/Shanghai',),
  '86915':('Asia/Shanghai',),
- '1418968':('America/Toronto',),
+ '86914':('Asia/Shanghai',),
  '86917':('Asia/Shanghai',),
  '86916':('Asia/Shanghai',),
  '86911':('Asia/Shanghai',),
  '86913':('Asia/Shanghai',),
  '86912':('Asia/Shanghai',),
  '1775784':('America/Los_Angeles',),
  '1775786':('America/Los_Angeles',),
  '1775787':('America/Los_Angeles',),
  '1775782':('America/Los_Angeles',),
  '1775783':('America/Los_Angeles',),
- '1418388':('America/Toronto',),
  '1849':('America/Halifax',),
  '1848':('America/New_York',),
  '1843':('America/New_York',),
- '1418383':('America/Toronto',),
  '1847':('America/Chicago',),
- '1418385':('America/Toronto',),
  '1845':('America/New_York',),
- '1418387':('America/Toronto',),
- '1418962':('America/Toronto',),
- '1418963':('America/Toronto',),
  '521415':('America/Mexico_City',),
- '1941':('America/New_York',),
+ '521414':('America/Mexico_City',),
+ '1947':('America/New_York',),
  '52635':('America/Mazatlan',),
  '52634':('America/Mazatlan',),
- '52637':('America/Mazatlan',),
+ '521451':('America/Mexico_City',),
  '52636':('America/Mazatlan',),
  '52631':('America/Mazatlan',),
  '521456':('America/Mexico_City',),
  '521455':('America/Mexico_City',),
  '521454':('America/Mexico_City',),
+ '1906':('America/New_York',),
+ '1907':('America/Adak', 'America/Anchorage'),
  '521459':('America/Mexico_City',),
  '521458':('America/Mexico_City',),
  '1902':('America/Halifax',),
- '1903':('America/Chicago',),
+ '52638':('America/Mazatlan',),
  '1901':('America/Chicago',),
  '1541988':('America/Los_Angeles',),
  '1541981':('America/Los_Angeles',),
  '1541980':('America/Los_Angeles',),
- '441808':('Europe/London',),
- '1606549':('America/New_York',),
- '1606546':('America/New_York',),
- '1606545':('America/New_York',),
- '1620257':('America/Chicago',),
- '1620251':('America/Chicago',),
  '1423288':('America/New_York',),
  '1423286':('America/New_York',),
  '1423283':('America/New_York',),
  '1423282':('America/New_York',),
- '1620259':('America/Chicago',),
- '55813055':('America/Sao_Paulo',),
- '1785587':('America/Chicago',),
+ '441508':('Europe/London',),
  '44161':('Europe/London',),
- '1606768':('America/New_York',),
  '1208746':('America/Los_Angeles',),
  '1208745':('America/Denver',),
  '1208743':('America/Los_Angeles',),
  '6895':('Pacific/Tahiti',),
  '6894':('Pacific/Tahiti',),
- '55913004':('America/Sao_Paulo',),
- '55813109':('America/Sao_Paulo',),
+ '441501':('Europe/London',),
  '6898':('Pacific/Tahiti',),
  '599416':('America/Kralendijk',),
- '55913003':('America/Sao_Paulo',),
- '1208569':('America/Denver',),
+ '1279':('America/Los_Angeles',),
+ '618':('Australia/Adelaide', 'Australia/Perth'),
  '612':('Australia/Sydney',),
  '1208290':('America/Los_Angeles',),
- '1219707':('America/Chicago',),
+ '1272':('America/New_York',),
  '1208292':('America/Los_Angeles',),
- '1219253':('America/New_York',),
  '617':('Australia/Sydney',),
  '1276':('America/New_York',),
  '55913276':('America/Sao_Paulo',),
  '55913277':('America/Sao_Paulo',),
  '55913274':('America/Sao_Paulo',),
  '55913275':('America/Sao_Paulo',),
- '55813107':('America/Sao_Paulo',),
+ '55913272':('America/Sao_Paulo',),
  '55913273':('America/Sao_Paulo',),
  '55913271':('America/Sao_Paulo',),
  '521697':('America/Mazatlan',),
  '1701242':('America/Chicago',),
  '55913278':('America/Sao_Paulo',),
- '1701241':('America/Chicago',),
- '1208866':('America/Denver',),
+ '55913279':('America/Sao_Paulo',),
  '55813106':('America/Sao_Paulo',),
- '55914400':('America/Sao_Paulo',),
+ '521696':('America/Mazatlan',),
  '441689':('Europe/London',),
  '441688':('Europe/London',),
  '441683':('Europe/London',),
  '441681':('Europe/London',),
- '521735':('America/Mexico_City',),
+ '441680':('Europe/London',),
  '441687':('Europe/London',),
  '441686':('Europe/London',),
  '441685':('Europe/London',),
  '441684':('Europe/London',),
- '55813105':('America/Sao_Paulo',),
- '1850297':('America/New_York',),
- '1850294':('America/New_York',),
  '1850292':('America/Chicago',),
+ '1850291':('America/Chicago',),
  '55813104':('America/Sao_Paulo',),
  '55813103':('America/Sao_Paulo',),
  '52958':('America/Mexico_City',),
  '1541210':('America/Los_Angeles',),
  '52951':('America/Mexico_City',),
  '52953':('America/Mexico_City',),
  '52954':('America/Mexico_City',),
  '1541218':('America/Los_Angeles',),
  '1775428':('America/Los_Angeles',),
- '55813102':('America/Sao_Paulo',),
  '55813101':('America/Sao_Paulo',),
  '62234':('Asia/Jakarta',),
  '1775423':('America/Los_Angeles',),
  '1907349':('America/Juneau',),
  '55813482':('America/Sao_Paulo',),
- '1907346':('America/Juneau',),
- '441888':('Europe/London',),
- '1907344':('America/Juneau',),
- '1907343':('America/Juneau',),
+ '55813483':('America/Sao_Paulo',),
+ '1907345':('America/Juneau',),
+ '55813481':('America/Sao_Paulo',),
+ '55813486':('America/Sao_Paulo',),
  '55813487':('America/Sao_Paulo',),
  '55813484':('America/Sao_Paulo',),
  '1423708':('America/New_York',),
  '1423878':('America/New_York',),
  '1423702':('America/New_York',),
  '1423875':('America/New_York',),
  '1423876':('America/New_York',),
@@ -6549,249 +5481,194 @@
  '1605721':('America/Denver',),
  '1605724':('America/Chicago',),
  '1605725':('America/Chicago',),
  '55813268':('America/Sao_Paulo',),
  '55813269':('America/Sao_Paulo',),
  '55813266':('America/Sao_Paulo',),
  '55813267':('America/Sao_Paulo',),
+ '55813264':('America/Sao_Paulo',),
  '55813265':('America/Sao_Paulo',),
  '1907694':('America/Juneau',),
  '1907696':('America/Juneau',),
  '9765037':('Asia/Ulaanbaatar',),
  '1906563':('America/Chicago',),
  '1219882':('America/Chicago',),
  '1219881':('America/Chicago',),
  '1219886':('America/Chicago',),
  '1219887':('America/Chicago',),
  '1219884':('America/Chicago',),
  '1219885':('America/Chicago',),
- '1250661':('America/Vancouver',),
- '1250933':('America/Vancouver',),
  '7351':('Asia/Yekaterinburg',),
  '7353':('Asia/Yekaterinburg',),
  '7352':('Asia/Yekaterinburg',),
- '1308696':('America/Chicago',),
- '1308697':('America/Chicago',),
  '62971':('Asia/Jayapura',),
- '62975':('Asia/Jakarta', 'Asia/Jayapura'),
+ '62975':('Asia/Jayapura',),
  '62979':('Asia/Jakarta',),
  '1605987':('America/Chicago',),
  '55943358':('America/Sao_Paulo',),
  '1605983':('America/Chicago',),
  '55943355':('America/Sao_Paulo',),
  '55943356':('America/Sao_Paulo',),
  '55943351':('America/Sao_Paulo',),
  '55943352':('America/Sao_Paulo',),
  '55943353':('America/Sao_Paulo',),
  '1423451':('America/New_York',),
- '1308345':('America/Chicago',),
- '1308346':('America/Chicago',),
- '1620397':('America/Chicago',),
- '62372':('Asia/Makassar',),
- '1850999':('America/New_York',),
+ '1907830':('America/Juneau',),
  '1850995':('America/Chicago',),
  '1850994':('America/Chicago',),
- '1850997':('America/New_York',),
  '68991':('Pacific/Marquesas',),
  '68990':('Pacific/Tahiti',),
  '68993':('Pacific/Tahiti',),
  '68992':('Pacific/Marquesas',),
  '68995':('Pacific/Tahiti',),
  '68994':('Pacific/Tahiti',),
  '68997':('Pacific/Gambier',),
  '68996':('Pacific/Tahiti',),
  '68998':('Pacific/Tahiti',),
- '1574333':('America/New_York',),
- '1574335':('America/New_York',),
  '1709279':('America/St_Johns',),
- '1606376':('America/New_York',),
- '1606377':('America/New_York',),
- '1606379':('America/New_York',),
- '1418838':('America/Toronto',),
- '1418839':('America/Toronto',),
- '1418529':('America/Toronto',),
- '1418832':('America/Toronto',),
- '1418833':('America/Toronto',),
- '1418527':('America/Toronto',),
- '1418836':('America/Toronto',),
- '1418837':('America/Toronto',),
- '1418834':('America/Toronto',),
- '1418835':('America/Toronto',),
  '8651':('Asia/Shanghai',),
  '8653':('Asia/Shanghai',),
  '8655':('Asia/Shanghai',),
  '8657':('Asia/Shanghai',),
  '1850377':('America/Chicago',),
  '1850376':('America/Chicago',),
  '1867667':('America/Vancouver',),
  '1867669':('America/Edmonton',),
  '1867668':('America/Vancouver',),
- '1418525':('America/Toronto',),
  '55949842':('America/Sao_Paulo',),
  '55949840':('America/Sao_Paulo',),
  '55949841':('America/Sao_Paulo',),
  '1208527':('America/Denver',),
  '55814141':('America/Sao_Paulo',),
  '1236':('America/Vancouver',),
  '55813019':('America/Sao_Paulo',),
  '55813011':('America/Sao_Paulo',),
- '1208251':('America/Denver',),
+ '55813010':('America/Sao_Paulo',),
  '55813012':('America/Sao_Paulo',),
  '55813015':('America/Sao_Paulo',),
  '55813014':('America/Sao_Paulo',),
- '1231':('America/New_York',),
- '1250320':('America/Vancouver',),
+ '1208522':('America/Denver',),
  '1785852':('America/Denver',),
  '1208253':('America/Denver',),
  '1208258':('America/Denver',),
- '1250498':('America/Vancouver',),
- '1250499':('America/Vancouver',),
- '1250492':('America/Vancouver',),
- '1250493':('America/Vancouver',),
- '1250490':('America/Vancouver',),
- '1250491':('America/Vancouver',),
- '1250497':('America/Vancouver',),
- '1250494':('America/Vancouver',),
- '1250495':('America/Vancouver',),
  '1270786':('America/Chicago',),
  '1270780':('America/Chicago',),
  '1270781':('America/Chicago',),
  '1270782':('America/Chicago',),
  '1270783':('America/Chicago',),
- '1270789':('America/New_York',),
  '86458':('Asia/Shanghai',),
  '1775237':('America/Los_Angeles',),
  '1775230':('America/Los_Angeles',),
  '1775544':('America/Los_Angeles',),
  '1775233':('America/Los_Angeles',),
  '55913456':('America/Sao_Paulo',),
  '1906779':('America/Chicago',),
  '1906774':('America/Chicago',),
  '1906776':('America/Chicago',),
  '1270439':('America/Chicago',),
  '1270432':('America/Chicago',),
  '62519':('Asia/Jakarta',),
- '86455':('Asia/Shanghai',),
  '1860':('America/New_York',),
  '1863':('America/New_York',),
  '1862':('America/New_York',),
  '1865':('America/New_York',),
  '1864':('America/New_York',),
+ '1867':('America/Fort_Nelson',),
  '1869':('America/St_Kitts',),
  '1868':('America/Port_of_Spain',),
  '86457':('Asia/Shanghai',),
  '62518':('Asia/Makassar',),
- '1250808':('America/Vancouver',),
- '1620896':('America/Chicago',),
  '1812768':('America/Chicago',),
  '62517':('Asia/Makassar',),
- '1574834':('America/New_York',),
- '1418364':('America/Toronto',),
- '1574831':('America/New_York',),
- '1574522':('America/New_York',),
  '52613':('America/Mazatlan',),
  '52612':('America/Mazatlan',),
- '1250727':('America/Vancouver',),
  '52616':('America/Tijuana',),
  '52615':('America/Mazatlan',),
  '52614':('America/Mazatlan',),
  '62566':('Asia/Jakarta',),
- '1250720':('America/Vancouver',),
+ '62567':('Asia/Jakarta',),
  '62516':('Asia/Jakarta', 'Asia/Makassar'),
  '52618':('America/Mexico_City',),
  '521923':('America/Mexico_City',),
  '521922':('America/Mexico_City',),
  '521921':('America/Mexico_City',),
  '62561':('Asia/Jakarta',),
- '1606561':('America/New_York',),
- '1606564':('America/New_York',),
- '1620271':('America/Chicago',),
  '34810':('Europe/Madrid',),
- '1620273':('America/Chicago',),
- '34812':('Europe/Madrid',),
- '1620275':('America/Chicago',),
- '1620277':('America/Chicago',),
- '1620276':('America/Chicago',),
- '62702':('Asia/Jakarta',),
- '1620278':('America/Chicago',),
- '62298':('Asia/Jakarta',),
+ '34819':('Europe/Madrid',),
  '1270898':('America/Chicago',),
  '44141':('Europe/London',),
  '44143':('Europe/London',),
  '44147':('Europe/London',),
  '1208769':('America/Los_Angeles',),
- '62482':('Asia/Makassar',),
  '1780':('America/Edmonton',),
  '1781':('America/New_York',),
+ '1782':('America/Halifax',),
  '1208762':('America/Los_Angeles',),
  '1784':('America/St_Vincent',),
+ '1785':('America/Chicago',),
  '1786':('America/New_York',),
  '1787':('America/Puerto_Rico',),
- '1219838':('America/Chicago',),
+ '1775677':('America/Los_Angeles',),
  '390161':('Europe/Rome',),
  '390163':('Europe/Rome',),
  '390165':('Europe/Rome',),
  '390166':('Europe/Rome',),
- '1219279':('America/New_York',),
  '678':('Pacific/Efate',),
  '679':('Pacific/Fiji',),
  '1701730':('America/Chicago',),
  '674':('Pacific/Nauru',),
  '351295':('Atlantic/Azores',),
  '351296':('Atlantic/Azores',),
  '677':('Pacific/Guadalcanal',),
  '670':('Asia/Dili',),
  '351291':('Europe/Lisbon',),
  '1701738':('America/Chicago',),
- '673':('Asia/Brunei',),
+ '1701739':('America/Chicago',),
  '1701228':('America/Chicago',),
  '1701220':('America/Chicago',),
  '1701221':('America/Chicago',),
  '1701222':('America/Chicago',),
  '1701223':('America/Chicago',),
  '1701224':('America/Chicago',),
  '1701225':('America/Denver',),
  '1701226':('America/Chicago',),
  '1701227':('America/Denver',),
- '1270234':('America/New_York',),
+ '86483':('Asia/Shanghai',),
  '86482':('Asia/Shanghai',),
  '1270236':('America/Chicago',),
  '1270237':('America/Chicago',),
  '1270230':('America/Chicago',),
  '1775849':('America/Los_Angeles',),
  '1775847':('America/Los_Angeles',),
  '1775843':('America/Los_Angeles',),
  '1775841':('America/Los_Angeles',),
- '1606743':('America/New_York',),
+ '62986':('Asia/Jayapura',),
  '86159':('Asia/Shanghai',),
  '86158':('Asia/Shanghai',),
  '86151':('Asia/Shanghai',),
  '86150':('Asia/Shanghai',),
  '86153':('Asia/Shanghai',),
  '86152':('Asia/Shanghai',),
  '86155':('Asia/Shanghai',),
  '86157':('Asia/Shanghai',),
- '1850653':('America/New_York',),
+ '86156':('Asia/Shanghai',),
  '1256':('America/Chicago',),
  '1208547':('America/Denver',),
  '1208814':('America/Denver',),
- '1520':('America/Denver',),
+ '1252':('America/New_York',),
  '1253':('America/Los_Angeles',),
  '1208543':('America/Denver',),
  '1208542':('America/Denver',),
  '1208549':('America/Denver',),
- '1418998':('America/Toronto',),
  '1208819':('America/Los_Angeles',),
  '1208818':('America/Los_Angeles',),
- '62980':('Asia/Jayapura',),
  '1541231':('America/Los_Angeles',),
  '1541230':('America/Los_Angeles',),
  '1541232':('America/Los_Angeles',),
  '1709489':('America/St_Johns',),
- '62981':('Asia/Jayapura',),
  '1423800':('America/New_York',),
  '521311':('America/Mazatlan',),
  '521312':('America/Mexico_City',),
  '521313':('America/Mexico_City',),
  '521314':('America/Mexico_City',),
  '521315':('America/Mexico_City',),
  '521316':('America/Mexico_City',),
@@ -6800,56 +5677,56 @@
  '62522':('Asia/Jakarta',),
  '55943778':('America/Sao_Paulo',),
  '521962':('America/Mexico_City',),
  '1850416':('America/Chicago',),
  '1850417':('America/Chicago',),
  '1709738':('America/St_Johns',),
  '1709739':('America/St_Johns',),
- '52653':('America/Mazatlan',),
- '52652':('America/Mazatlan',),
- '52988':('America/Mexico_City',),
+ '1906663':('America/Chicago',),
+ '521966':('America/Mexico_City',),
  '521965':('America/Mexico_City',),
  '62525':('Asia/Jakarta',),
  '55813461':('America/Sao_Paulo',),
  '55813462':('America/Sao_Paulo',),
  '55813463':('America/Sao_Paulo',),
  '55813464':('America/Sao_Paulo',),
  '55813465':('America/Sao_Paulo',),
  '55813466':('America/Sao_Paulo',),
  '55813467':('America/Sao_Paulo',),
  '55813468':('America/Sao_Paulo',),
  '1907360':('America/Juneau',),
  '62528':('Asia/Jakarta',),
  '55813204':('America/Sao_Paulo',),
  '55813205':('America/Sao_Paulo',),
- '1906663':('America/Chicago',),
  '55813207':('America/Sao_Paulo',),
  '55813201':('America/Sao_Paulo',),
  '55813202':('America/Sao_Paulo',),
  '55813203':('America/Sao_Paulo',),
+ '441636':('Europe/London',),
  '9765011':('Asia/Ulaanbaatar',),
  '1775684':('America/Los_Angeles',),
  '1775687':('America/Los_Angeles',),
  '1775686':('America/Los_Angeles',),
+ '441637':('Europe/London',),
  '1775689':('America/Los_Angeles',),
  '1775688':('America/Los_Angeles',),
- '1219864':('America/Chicago',),
+ '55819000':('America/Sao_Paulo',),
  '1219865':('America/Chicago',),
  '1219866':('America/Chicago',),
  '52424':('America/Mexico_City',),
  '52425':('America/Mexico_City',),
  '52426':('America/Mexico_City',),
- '1423855':('America/New_York',),
+ '52427':('America/Mexico_City',),
  '52421':('America/Mexico_City',),
  '52422':('America/Mexico_City',),
  '52423':('America/Mexico_City',),
- '1250686':('America/Vancouver',),
+ '1208624':('America/Denver',),
  '52428':('America/Mexico_City',),
  '52429':('America/Mexico_City',),
- '1418669':('America/Toronto',),
+ '1684':('Pacific/Pago_Pago',),
  '390374':('Europe/Rome',),
  '390375':('Europe/Rome',),
  '390376':('Europe/Rome',),
  '390377':('Europe/Rome',),
  '390371':('Europe/Rome',),
  '390372':('Europe/Rome',),
  '390373':('Europe/Rome',),
@@ -6861,70 +5738,56 @@
  '441324':('Europe/London',),
  '441325':('Europe/London',),
  '441326':('Europe/London',),
  '441327':('Europe/London',),
  '1423581':('America/New_York',),
  '1423585':('America/New_York',),
  '1423586':('America/New_York',),
- '1906233':('America/New_York',),
+ '1423587':('America/New_York',),
  '62957':('Asia/Jayapura',),
  '62956':('Asia/Jayapura',),
  '62955':('Asia/Jayapura',),
- '62952':('Asia/Jayapura',),
+ '62952':('Asia/Jakarta', 'Asia/Jayapura'),
  '62951':('Asia/Jayapura',),
  '55943379':('America/Sao_Paulo',),
  '55939924':('America/Sao_Paulo',),
  '55939922':('America/Sao_Paulo',),
- '1308367':('America/Chicago',),
+ '55939923':('America/Sao_Paulo',),
  '55939920':('America/Sao_Paulo',),
  '55939921':('America/Sao_Paulo',),
  '1270932':('America/Chicago',),
  '1541826':('America/Los_Angeles',),
  '1541821':('America/Los_Angeles',),
  '1541822':('America/Los_Angeles',),
- '1574647':('America/New_York',),
- '1574642':('America/New_York',),
  '1423323':('America/New_York',),
  '1423328':('America/New_York',),
- '1620235':('America/Chicago',),
  '1709257':('America/St_Johns',),
  '1709256':('America/St_Johns',),
- '1606354':('America/New_York',),
- '1606353':('America/New_York',),
  '1850319':('America/Chicago',),
- '62293':('Asia/Jakarta',),
- '1785393':('America/Chicago',),
- '1418660':('America/Toronto',),
+ '1867983':('America/Edmonton',),
+ '1850315':('America/Chicago',),
  '1850314':('America/Chicago',),
- '55813915':('America/Sao_Paulo',),
- '441528':('Europe/London',),
+ '55813079':('America/Sao_Paulo',),
  '441529':('Europe/London',),
- '441526':('Europe/London',),
- '441527':('Europe/London',),
- '441524':('Europe/London',),
- '441525':('Europe/London',),
- '441522':('Europe/London',),
+ '55813077':('America/Sao_Paulo',),
+ '55813076':('America/Sao_Paulo',),
+ '55813075':('America/Sao_Paulo',),
+ '55813074':('America/Sao_Paulo',),
+ '55813073':('America/Sao_Paulo',),
  '55813072':('America/Sao_Paulo',),
- '441520':('Europe/London',),
+ '55813071':('America/Sao_Paulo',),
  '1219513':('America/Chicago',),
  '52645':('America/Mazatlan',),
- '1250309':('America/Vancouver',),
- '55813912':('America/Sao_Paulo',),
- '1785309':('America/Chicago',),
- '1785877':('America/Chicago',),
- '1250306':('America/Vancouver',),
- '1250307':('America/Vancouver',),
+ '1701968':('America/Chicago',),
  '1701965':('America/Chicago',),
- '1250305':('America/Vancouver',),
+ '55913028':('America/Sao_Paulo',),
  '7413':('Asia/Magadan',),
  '7411':('Asia/Yakutsk',),
  '7416':('Asia/Yakutsk',),
  '7415':('Asia/Kamchatka',),
- '55813003':('America/Sao_Paulo',),
- '55933603':('America/Sao_Paulo',),
  '55813699':('America/Sao_Paulo',),
  '1208373':('America/Denver',),
  '55813693':('America/Sao_Paulo',),
  '55813692':('America/Sao_Paulo',),
  '55813691':('America/Sao_Paulo',),
  '1807548':('America/Winnipeg',),
  '55813695':('America/Sao_Paulo',),
@@ -6934,24 +5797,17 @@
  '1208377':('America/Denver',),
  '86951':('Asia/Shanghai',),
  '86953':('Asia/Shanghai',),
  '86952':('Asia/Shanghai',),
  '86955':('Asia/Shanghai',),
  '86954':('Asia/Shanghai',),
  '1310':('America/Los_Angeles',),
- '1812299':('America/New_York',),
- '1812294':('America/New_York',),
- '1812295':('America/New_York',),
- '1574875':('America/New_York',),
- '1418349':('America/Toronto',),
- '1418347':('America/Toronto',),
- '1418343':('America/Toronto',),
  '55813125':('America/Sao_Paulo',),
  '1812749':('America/Chicago',),
- '55813127':('America/Sao_Paulo',),
+ '1701837':('America/Chicago',),
  '521496':('America/Mexico_City',),
  '521495':('America/Mexico_City',),
  '521494':('America/Mexico_City',),
  '521493':('America/Mexico_City',),
  '521492':('America/Mexico_City',),
  '62542':('Asia/Makassar',),
  '62543':('Asia/Makassar',),
@@ -6965,53 +5821,50 @@
  '52673':('America/Mazatlan',),
  '52672':('America/Mazatlan',),
  '52675':('America/Mexico_City',),
  '52674':('America/Mexico_City',),
  '52677':('America/Mexico_City',),
  '52676':('America/Mexico_City',),
  '1541513':('America/Los_Angeles',),
- '55813129':('America/Sao_Paulo',),
- '1541515':('America/Los_Angeles',),
- '1541517':('America/Los_Angeles',),
+ '1701839':('America/Chicago',),
+ '1701838':('America/Chicago',),
  '62721':('Asia/Jakarta',),
  '62722':('Asia/Jakarta',),
  '62723':('Asia/Jakarta',),
  '62724':('Asia/Jakarta',),
  '62725':('Asia/Jakarta',),
  '62726':('Asia/Jakarta',),
  '62727':('Asia/Jakarta',),
  '62728':('Asia/Jakarta',),
  '62729':('Asia/Jakarta',),
  '34837':('Europe/Madrid',),
  '34835':('Europe/Madrid',),
+ '34833':('Europe/Madrid',),
  '34830':('Europe/Madrid',),
- '1423746':('America/New_York',),
- '1423744':('America/New_York',),
  '390143':('Europe/Rome',),
  '390142':('Europe/Rome',),
  '390141':('Europe/Rome',),
  '390144':('Europe/Rome',),
  '82':('Asia/Seoul',),
  '81':('Asia/Tokyo',),
  '86':('Asia/Shanghai', 'Asia/Urumqi'),
  '84':('Asia/Bangkok',),
- '1250624':('America/Vancouver',),
  '55943491':('America/Sao_Paulo',),
- '1250626':('America/Vancouver',),
  '1701751':('America/Chicago',),
  '1701200':('America/Chicago',),
  '1701754':('America/Chicago',),
  '1701756':('America/Chicago',),
  '1701205':('America/Chicago',),
  '1775867':('America/Los_Angeles',),
  '1208703':('America/Denver',),
  '1208706':('America/Denver',),
  '1208705':('America/Denver',),
  '1208704':('America/Los_Angeles',),
  '1208709':('America/Denver',),
+ '441594':('Europe/London',),
  '1219662':('America/Chicago',),
  '55812119':('America/Sao_Paulo',),
  '86177':('Asia/Shanghai',),
  '86176':('Asia/Shanghai',),
  '1541783':('America/Los_Angeles',),
  '1541782':('America/Los_Angeles',),
  '86173':('Asia/Shanghai',),
@@ -7020,92 +5873,87 @@
  '1502':('America/New_York',),
  '1503':('America/Los_Angeles',),
  '1501':('America/Chicago',),
  '1506':('America/Halifax',),
  '1507':('America/Chicago',),
  '1504':('America/Chicago',),
  '1505':('America/Denver',),
- '1418977':('America/Toronto',),
  '1508':('America/New_York',),
  '1509':('America/Los_Angeles',),
- '1418973':('America/Toronto',),
  '1850784':('America/Chicago',),
  '1850785':('America/Chicago',),
  '1541259':('America/Los_Angeles',),
  '1541258':('America/Los_Angeles',),
  '1270689':('America/Chicago',),
  '1270688':('America/Chicago',),
  '1270685':('America/Chicago',),
  '1270684':('America/Chicago',),
  '1270687':('America/Chicago',),
  '1270686':('America/Chicago',),
- '1270683':('America/Chicago',),
+ '1541255':('America/Los_Angeles',),
  '521378':('America/Mexico_City',),
- '521372':('America/Mexico_City',),
  '521373':('America/Mexico_City',),
  '521371':('America/Mexico_City',),
  '521376':('America/Mexico_City',),
  '521377':('America/Mexico_City',),
  '521374':('America/Mexico_City',),
  '521375':('America/Mexico_City',),
- '52342':('America/Mexico_City',),
  '1709758':('America/St_Johns',),
+ '1709759':('America/St_Johns',),
  '1850438':('America/Chicago',),
  '1850439':('America/Chicago',),
  '1850436':('America/Chicago',),
  '1850437':('America/Chicago',),
  '1850434':('America/Chicago',),
  '1850435':('America/Chicago',),
  '1850432':('America/Chicago',),
  '1850433':('America/Chicago',),
- '1850431':('America/New_York',),
+ '1709757':('America/St_Johns',),
  '5591982':('America/Sao_Paulo',),
  '5591983':('America/Sao_Paulo',),
  '1907301':('America/Juneau',),
  '5591981':('America/Sao_Paulo',),
  '1907306':('America/Juneau',),
  '5591984':('America/Sao_Paulo',),
  '5591988':('America/Sao_Paulo',),
  '5591989':('America/Sao_Paulo',),
- '55813194':('America/Sao_Paulo',),
+ '55813446':('America/Sao_Paulo',),
  '55813447':('America/Sao_Paulo',),
  '55813444':('America/Sao_Paulo',),
  '55813445':('America/Sao_Paulo',),
  '55813442':('America/Sao_Paulo',),
  '55813443':('America/Sao_Paulo',),
  '55813441':('America/Sao_Paulo',),
  '55813198':('America/Sao_Paulo',),
  '55813448':('America/Sao_Paulo',),
  '55813449':('America/Sao_Paulo',),
  '55933016':('America/Sao_Paulo',),
  '55933017':('America/Sao_Paulo',),
- '1907222':('America/Juneau',),
  '441754':('Europe/London',),
- '441757':('Europe/London',),
- '441756':('Europe/London',),
+ '55813228':('America/Sao_Paulo',),
+ '55813229':('America/Sao_Paulo',),
  '441751':('Europe/London',),
  '441750':('Europe/London',),
  '441753':('Europe/London',),
  '441752':('Europe/London',),
  '55813222':('America/Sao_Paulo',),
  '55813223':('America/Sao_Paulo',),
  '55813221':('America/Sao_Paulo',),
- '441759':('Europe/London',),
- '441758':('Europe/London',),
+ '55813226':('America/Sao_Paulo',),
+ '55813227':('America/Sao_Paulo',),
  '55813224':('America/Sao_Paulo',),
  '55813225':('America/Sao_Paulo',),
- '1250516':('America/Vancouver',),
- '1250514':('America/Vancouver',),
+ '441659':('Europe/London',),
  '1219844':('America/Chicago',),
  '52773':('America/Mexico_City',),
  '1775664':('America/Denver',),
  '55913798':('America/Sao_Paulo',),
  '55913829':('America/Sao_Paulo',),
  '55913795':('America/Sao_Paulo',),
- '1423525':('America/New_York',),
+ '52777':('America/Mexico_City',),
  '55913823':('America/Sao_Paulo',),
  '55913822':('America/Sao_Paulo',),
  '55913821':('America/Sao_Paulo',),
  '52442':('America/Mexico_City',),
  '52443':('America/Mexico_City',),
  '52441':('America/Mexico_City',),
  '52446':('America/Mexico_City',),
@@ -7117,247 +5965,191 @@
  '52449':('America/Mexico_City',),
  '390828':('Europe/Rome',),
  '7394':('Asia/Krasnoyarsk',),
  '996':('Asia/Bishkek',),
  '7391':('Asia/Krasnoyarsk',),
  '7390':('Asia/Krasnoyarsk',),
  '993':('Asia/Ashgabat',),
- '1574296':('America/New_York',),
+ '992':('Asia/Dushanbe',),
  '390823':('Europe/Rome',),
  '390824':('Europe/Rome',),
  '390825':('Europe/Rome',),
  '390827':('Europe/Rome',),
  '441342':('Europe/London',),
  '441343':('Europe/London',),
  '441340':('Europe/London',),
  '441341':('Europe/London',),
  '441346':('Europe/London',),
  '441347':('Europe/London',),
  '441344':('Europe/London',),
  '441348':('Europe/London',),
  '441349':('Europe/London',),
- '1418681':('America/Toronto',),
  '1605328':('America/Chicago',),
  '1605322':('America/Chicago',),
  '1605323':('America/Chicago',),
  '1605321':('America/Chicago',),
- '1308389':('America/Chicago',),
- '1308384':('America/Chicago',),
- '1308385':('America/Chicago',),
- '1308380':('America/Chicago',),
- '1308381':('America/Chicago',),
- '1308382':('America/Chicago',),
+ '1850872':('America/Chicago',),
  '1541808':('America/Los_Angeles',),
  '441967':('Europe/London',),
  '441964':('Europe/London',),
  '441962':('Europe/London',),
  '441963':('Europe/London',),
- '1812829':('America/New_York',),
- '1812825':('America/New_York',),
- '1812824':('America/New_York',),
- '1812822':('America/New_York',),
  '441968':('Europe/London',),
  '441969':('Europe/London',),
- '1208724':('America/Denver',),
- '1208727':('America/Denver',),
  '1208726':('America/Denver',),
- '1423307':('America/New_York',),
+ '1907892':('America/Juneau',),
  '1423305':('America/New_York',),
  '1907895':('America/Juneau',),
- '1208720':('America/Denver',),
  '1208722':('America/Denver',),
- '1418561':('America/Toronto',),
- '1418562':('America/Toronto',),
- '1418563':('America/Toronto',),
- '1418566':('America/Toronto',),
- '1418567':('America/Toronto',),
- '1606330':('America/New_York',),
- '1606337':('America/New_York',),
- '1620532':('America/Chicago',),
- '1620662':('America/Chicago',),
+ '1423847':('America/New_York',),
  '55813657':('America/Sao_Paulo',),
  '1709237':('America/St_Johns',),
  '55949880':('America/Sao_Paulo',),
- '55813304':('America/Sao_Paulo',),
+ '55949881':('America/Sao_Paulo',),
  '1219531':('America/Chicago',),
- '55813653':('America/Sao_Paulo',),
- '441508':('Europe/London',),
+ '55813301':('America/Sao_Paulo',),
+ '441759':('Europe/London',),
+ '55813055':('America/Sao_Paulo',),
  '441509':('Europe/London',),
  '1701947':('America/Chicago',),
  '55813051':('America/Sao_Paulo',),
  '55813050':('America/Sao_Paulo',),
  '55813053':('America/Sao_Paulo',),
  '55813052':('America/Sao_Paulo',),
- '441501':('Europe/London',),
+ '55913004':('America/Sao_Paulo',),
  '441502':('Europe/London',),
  '441503':('Europe/London',),
  '55813059':('America/Sao_Paulo',),
  '441505':('Europe/London',),
  '441506':('Europe/London',),
  '441507':('Europe/London',),
- '1785320':('America/Chicago',),
- '1785325':('America/Chicago',),
  '1850332':('America/Chicago',),
  '7471':('Europe/Moscow',),
  '7472':('Europe/Moscow',),
  '7473':('Europe/Moscow',),
  '7474':('Europe/Moscow',),
  '7475':('Europe/Moscow',),
+ '1339':('America/New_York',),
  '86527':('Asia/Shanghai',),
  '52878':('America/Mexico_City',),
  '52873':('America/Mexico_City',),
  '52872':('America/Mexico_City',),
  '52871':('America/Mexico_City',),
  '52877':('America/Mexico_City',),
- '7484':('Europe/Moscow',),
- '55813877':('America/Sao_Paulo',),
- '7487':('Europe/Moscow',),
- '55813874':('America/Sao_Paulo',),
- '55813873':('America/Sao_Paulo',),
  '1270472':('America/Chicago',),
  '86979':('Asia/Shanghai',),
- '1270475':('America/Chicago',),
  '86977':('Asia/Shanghai',),
  '86976':('Asia/Shanghai',),
  '86975':('Asia/Shanghai',),
  '86974':('Asia/Shanghai',),
  '86973':('Asia/Shanghai',),
  '86972':('Asia/Shanghai',),
  '86971':('Asia/Shanghai',),
  '86970':('Asia/Shanghai',),
- '1250724':('America/Vancouver',),
- '1250725':('America/Vancouver',),
- '1250726':('America/Vancouver',),
- '1418365':('America/Toronto',),
- '1418362':('America/Toronto',),
- '1250721':('America/Vancouver',),
- '1250722':('America/Vancouver',),
- '1250723':('America/Vancouver',),
- '1250729':('America/Vancouver',),
- '1418368':('America/Toronto',),
  '52389':('America/Mazatlan',),
  '52388':('America/Mexico_City',),
- '1208852':('America/Denver',),
+ '1561':('America/New_York',),
  '52381':('America/Mexico_City',),
  '52383':('America/Mexico_City',),
  '52382':('America/Mexico_City',),
  '52385':('America/Mexico_City',),
  '52384':('America/Mexico_City',),
  '52387':('America/Mexico_City',),
  '52386':('America/Mexico_City',),
  '1208850':('America/Denver',),
- '1564':('America/Los_Angeles',),
+ '1208585':('America/Denver',),
  '1775273':('America/Los_Angeles',),
  '1208587':('America/Denver',),
- '1208854':('America/Denver',),
+ '1567':('America/New_York',),
  '521963':('America/Mexico_City',),
  '52656':('America/Hermosillo',),
  '521961':('America/Mexico_City',),
- '521967':('America/Mexico_City',),
- '521966':('America/Mexico_City',),
+ '52653':('America/Mazatlan',),
+ '52652':('America/Mazatlan',),
  '52651':('America/Mazatlan',),
  '521964':('America/Mexico_City',),
  '521969':('America/Mexico_City',),
  '521968':('America/Mexico_City',),
  '52659':('America/Mazatlan',),
  '52658':('America/Tijuana',),
  '55933222':('America/Sao_Paulo',),
  '351279':('Europe/Lisbon',),
- '1620947':('America/Chicago',),
- '1620231':('America/Chicago',),
- '1620232':('America/Chicago',),
+ '62298':('Asia/Jakarta',),
  '62291':('Asia/Jakarta',),
  '62292':('Asia/Jakarta',),
- '1867983':('America/Edmonton',),
+ '62293':('Asia/Jakarta',),
  '62294':('Asia/Jakarta',),
  '62295':('Asia/Jakarta',),
  '62296':('Asia/Jakarta',),
  '62297':('Asia/Jakarta',),
- '1785528':('America/Chicago',),
- '1785527':('America/Chicago',),
- '1785524':('America/Chicago',),
- '1701952':('America/Chicago',),
  '441289':('Europe/London',),
  '441288':('Europe/London',),
  '441287':('Europe/London',),
  '441286':('Europe/London',),
  '441285':('Europe/London',),
  '441284':('Europe/London',),
  '441283':('Europe/London',),
  '441282':('Europe/London',),
  '441280':('Europe/London',),
  '9761582':('Asia/Ulaanbaatar',),
  '55939881':('America/Sao_Paulo',),
  '55939880':('America/Sao_Paulo',),
- '1308440':('America/Chicago',),
  '7845':('Europe/Moscow',),
- '1606528':('America/New_York',),
- '1606837':('America/New_York',),
- '1606836':('America/New_York',),
- '1606526':('America/New_York',),
- '1606833':('America/New_York',),
- '1606832':('America/New_York',),
- '1606523':('America/New_York',),
+ '62336':('Asia/Jakarta',),
  '52985':('America/Mexico_City',),
  '1701772':('America/Chicago',),
- '52984':('America/New_York',),
+ '52328':('America/Mexico_City',),
  '1701776':('America/Chicago',),
  '1701777':('America/Chicago',),
  '1701774':('America/Chicago',),
  '1701775':('America/Chicago',),
  '1775800':('America/Los_Angeles',),
- '521721':('America/Mexico_City',),
- '1574295':('America/New_York',),
- '1574294':('America/New_York',),
- '1574293':('America/New_York',),
- '1574291':('America/New_York',),
- '62754':('Asia/Jakarta',),
+ '62755':('Asia/Jakarta',),
+ '52988':('America/Mexico_City',),
  '1270273':('America/Chicago',),
  '1270274':('America/Chicago',),
- '55943312':('America/Sao_Paulo',),
- '1574299':('America/New_York',),
- '1606789':('America/New_York',),
- '1606788':('America/New_York',),
+ '1605940':('America/Chicago',),
  '521722':('America/Mexico_City',),
- '1606780':('America/New_York',),
- '1606783':('America/New_York',),
+ '1208725':('America/Denver',),
+ '1208724':('America/Denver',),
+ '1208727':('America/Denver',),
  '1747':('America/Los_Angeles',),
  '1740':('America/New_York',),
- '1606784':('America/New_York',),
- '1606787':('America/New_York',),
+ '1208720':('America/Denver',),
  '1743':('America/New_York',),
  '62753':('Asia/Jakarta',),
  '55812137':('America/Sao_Paulo',),
  '55812138':('America/Sao_Paulo',),
  '521726':('America/Mexico_City',),
  '62427':('Asia/Makassar',),
- '1574773':('America/New_York',),
  '1208589':('America/Denver',),
  '1208588':('America/Denver',),
  '1208859':('America/Denver',),
- '1850321':('America/New_York',),
  '1208853':('America/Denver',),
- '1561':('America/New_York',),
+ '1208852':('America/Denver',),
  '1562':('America/Los_Angeles',),
  '1563':('America/Chicago',),
  '521686':('America/Tijuana',),
  '521687':('America/Mazatlan',),
  '1208855':('America/Denver',),
- '1567':('America/New_York',),
+ '1208854':('America/Denver',),
  '1541276':('America/Los_Angeles',),
  '1541271':('America/Los_Angeles',),
+ '1541270':('America/Los_Angeles',),
  '1541273':('America/Los_Angeles',),
+ '1541272':('America/Los_Angeles',),
  '1541278':('America/Los_Angeles',),
  '521354':('America/Mexico_City',),
  '521355':('America/Mexico_City',),
  '521356':('America/Mexico_City',),
  '521357':('America/Mexico_City',),
  '521351':('America/Mexico_City',),
  '521352':('America/Mexico_City',),
  '521353':('America/Mexico_City',),
  '5634':('America/Santiago',),
  '5635':('America/Santiago',),
  '521358':('America/Mexico_City',),
  '521359':('America/Mexico_City',),
  '5632':('Pacific/Easter',),
  '5633':('America/Santiago',),
+ '55813304':('America/Sao_Paulo',),
 }
```

### Comparing `phonenumbers-8.9.8/phonenumbers/unicode_util.py` & `phonenumbers-8.9.9/phonenumbers/unicode_util.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers/util.py` & `phonenumbers-8.9.9/phonenumbers/util.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/phonenumbers.egg-info/PKG-INFO` & `phonenumbers-8.9.9/phonenumbers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: phonenumbers
-Version: 8.9.8
+Version: 8.9.9
 Summary: Python version of Google's common library for parsing, formatting, storing and validating international phone numbers.
 Home-page: https://github.com/daviddrysdale/python-phonenumbers
 Author: David Drysdale
 Author-email: dmd@lurklurk.org
 License: Apache License 2.0
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `phonenumbers-8.9.8/phonenumbers.egg-info/SOURCES.txt` & `phonenumbers-8.9.9/phonenumbers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/PKG-INFO` & `phonenumbers-8.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: phonenumbers
-Version: 8.9.8
+Version: 8.9.9
 Summary: Python version of Google's common library for parsing, formatting, storing and validating international phone numbers.
 Home-page: https://github.com/daviddrysdale/python-phonenumbers
 Author: David Drysdale
 Author-email: dmd@lurklurk.org
 License: Apache License 2.0
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `phonenumbers-8.9.8/setup.py` & `phonenumbers-8.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/__init__.py` & `phonenumbers-8.9.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/asyoutypetest.py` & `phonenumbers-8.9.9/tests/asyoutypetest.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/carriertest.py` & `phonenumbers-8.9.9/tests/carriertest.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/examplenumberstest.py` & `phonenumbers-8.9.9/tests/examplenumberstest.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/geocodertest.py` & `phonenumbers-8.9.9/tests/geocodertest.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/pb2/converttest.py` & `phonenumbers-8.9.9/tests/pb2/converttest.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/phonenumbermatchertest.py` & `phonenumbers-8.9.9/tests/phonenumbermatchertest.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/phonenumbertest.py` & `phonenumbers-8.9.9/tests/phonenumbertest.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/phonenumberutiltest.py` & `phonenumbers-8.9.9/tests/phonenumberutiltest.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/shortnumberinfotest.py` & `phonenumbers-8.9.9/tests/shortnumberinfotest.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testcarrierdata/__init__.py` & `phonenumbers-8.9.9/tests/testcarrierdata/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testcarrierdata/data0.py` & `phonenumbers-8.9.9/tests/testcarrierdata/data0.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/__init__.py` & `phonenumbers-8.9.9/tests/testdata/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_800.py` & `phonenumbers-8.9.9/tests/testdata/region_800.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_882.py` & `phonenumbers-8.9.9/tests/testdata/region_882.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_979.py` & `phonenumbers-8.9.9/tests/testdata/region_979.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_AM.py` & `phonenumbers-8.9.9/tests/testdata/region_AM.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_AO.py` & `phonenumbers-8.9.9/tests/testdata/region_AO.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_AR.py` & `phonenumbers-8.9.9/tests/testdata/region_AR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_AU.py` & `phonenumbers-8.9.9/tests/testdata/region_AU.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_BS.py` & `phonenumbers-8.9.9/tests/testdata/region_BS.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_BY.py` & `phonenumbers-8.9.9/tests/testdata/region_BY.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_CA.py` & `phonenumbers-8.9.9/tests/testdata/region_CA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_CC.py` & `phonenumbers-8.9.9/tests/testdata/region_CC.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_CN.py` & `phonenumbers-8.9.9/tests/testdata/region_CN.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_CX.py` & `phonenumbers-8.9.9/tests/testdata/region_CX.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_DE.py` & `phonenumbers-8.9.9/tests/testdata/region_DE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_FR.py` & `phonenumbers-8.9.9/tests/testdata/region_FR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_GB.py` & `phonenumbers-8.9.9/tests/testdata/region_GB.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_GG.py` & `phonenumbers-8.9.9/tests/testdata/region_GG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_IT.py` & `phonenumbers-8.9.9/tests/testdata/region_IT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_JP.py` & `phonenumbers-8.9.9/tests/testdata/region_JP.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_KR.py` & `phonenumbers-8.9.9/tests/testdata/region_KR.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_MX.py` & `phonenumbers-8.9.9/tests/testdata/region_MX.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_NZ.py` & `phonenumbers-8.9.9/tests/testdata/region_NZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_PL.py` & `phonenumbers-8.9.9/tests/testdata/region_PL.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_RE.py` & `phonenumbers-8.9.9/tests/testdata/region_RE.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_SG.py` & `phonenumbers-8.9.9/tests/testdata/region_SG.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_TA.py` & `phonenumbers-8.9.9/tests/testdata/region_TA.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_US.py` & `phonenumbers-8.9.9/tests/testdata/region_US.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_UZ.py` & `phonenumbers-8.9.9/tests/testdata/region_UZ.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testdata/region_YT.py` & `phonenumbers-8.9.9/tests/testdata/region_YT.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testgeodata/__init__.py` & `phonenumbers-8.9.9/tests/testgeodata/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testgeodata/data0.py` & `phonenumbers-8.9.9/tests/testgeodata/data0.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testmetadatatest.py` & `phonenumbers-8.9.9/tests/testmetadatatest.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testtzdata/__init__.py` & `phonenumbers-8.9.9/tests/testtzdata/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/testtzdata/data0.py` & `phonenumbers-8.9.9/tests/testtzdata/data0.py`

 * *Files identical despite different names*

### Comparing `phonenumbers-8.9.8/tests/timezonetest.py` & `phonenumbers-8.9.9/tests/timezonetest.py`

 * *Files identical despite different names*

