# Comparing `tmp/phonenumberslite-8.9.8.tar.gz` & `tmp/phonenumberslite-8.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phonenumberslite-8.9.8.tar", last modified: Sat Jun 16 06:52:50 2018, max compression
+gzip compressed data, was "dist/phonenumberslite-8.9.9.tar", last modified: Fri Jun 29 07:34:43 2018, max compression
```

## Comparing `phonenumberslite-8.9.8.tar` & `phonenumberslite-8.9.9.tar`

### file list

```diff
@@ -1,631 +1,631 @@
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/
--rw-r--r--   0 dmd        (501) staff       (20)      115 2014-12-16 15:23:29.000000 phonenumberslite-8.9.8/MANIFEST.in
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/phonenumbers/
--rw-r--r--   0 dmd        (501) staff       (20)     9853 2018-06-16 06:46:56.000000 phonenumberslite-8.9.8/phonenumbers/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)    31975 2017-04-19 13:38:31.000000 phonenumberslite-8.9.8/phonenumbers/asyoutypeformatter.py
--rw-r--r--   0 dmd        (501) staff       (20)     6352 2013-11-15 12:19:09.000000 phonenumberslite-8.9.8/phonenumbers/carrier.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/phonenumbers/data/
--rw-r--r--   0 dmd        (501) staff       (20)    10295 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)      339 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_255.py
--rw-r--r--   0 dmd        (501) staff       (20)      232 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_27.py
--rw-r--r--   0 dmd        (501) staff       (20)      228 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_30.py
--rw-r--r--   0 dmd        (501) staff       (20)      436 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_31.py
--rw-r--r--   0 dmd        (501) staff       (20)      348 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_34.py
--rw-r--r--   0 dmd        (501) staff       (20)      217 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_350.py
--rw-r--r--   0 dmd        (501) staff       (20)      454 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_351.py
--rw-r--r--   0 dmd        (501) staff       (20)      199 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_352.py
--rw-r--r--   0 dmd        (501) staff       (20)      360 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_358.py
--rw-r--r--   0 dmd        (501) staff       (20)      482 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_359.py
--rw-r--r--   0 dmd        (501) staff       (20)      328 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_36.py
--rw-r--r--   0 dmd        (501) staff       (20)      572 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_372.py
--rw-r--r--   0 dmd        (501) staff       (20)      353 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_373.py
--rw-r--r--   0 dmd        (501) staff       (20)      493 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_380.py
--rw-r--r--   0 dmd        (501) staff       (20)      754 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_381.py
--rw-r--r--   0 dmd        (501) staff       (20)      545 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_385.py
--rw-r--r--   0 dmd        (501) staff       (20)      377 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_39.py
--rw-r--r--   0 dmd        (501) staff       (20)     1480 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_43.py
--rw-r--r--   0 dmd        (501) staff       (20)      689 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_44.py
--rw-r--r--   0 dmd        (501) staff       (20)     7207 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_49.py
--rw-r--r--   0 dmd        (501) staff       (20)      226 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_505.py
--rw-r--r--   0 dmd        (501) staff       (20)      241 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_506.py
--rw-r--r--   0 dmd        (501) staff       (20)      404 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_52.py
--rw-r--r--   0 dmd        (501) staff       (20)      343 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_54.py
--rw-r--r--   0 dmd        (501) staff       (20)      224 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_55.py
--rw-r--r--   0 dmd        (501) staff       (20)      197 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_58.py
--rw-r--r--   0 dmd        (501) staff       (20)      500 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_595.py
--rw-r--r--   0 dmd        (501) staff       (20)      589 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_61.py
--rw-r--r--   0 dmd        (501) staff       (20)      589 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_62.py
--rw-r--r--   0 dmd        (501) staff       (20)      215 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_63.py
--rw-r--r--   0 dmd        (501) staff       (20)      348 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_64.py
--rw-r--r--   0 dmd        (501) staff       (20)      216 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_66.py
--rw-r--r--   0 dmd        (501) staff       (20)      230 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_675.py
--rw-r--r--   0 dmd        (501) staff       (20)      230 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_676.py
--rw-r--r--   0 dmd        (501) staff       (20)      227 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_679.py
--rw-r--r--   0 dmd        (501) staff       (20)      696 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_7.py
--rw-r--r--   0 dmd        (501) staff       (20)      479 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_81.py
--rw-r--r--   0 dmd        (501) staff       (20)      343 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_84.py
--rw-r--r--   0 dmd        (501) staff       (20)      213 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_855.py
--rw-r--r--   0 dmd        (501) staff       (20)      415 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_856.py
--rw-r--r--   0 dmd        (501) staff       (20)      269 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_90.py
--rw-r--r--   0 dmd        (501) staff       (20)      973 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_91.py
--rw-r--r--   0 dmd        (501) staff       (20)      431 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_94.py
--rw-r--r--   0 dmd        (501) staff       (20)      224 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_95.py
--rw-r--r--   0 dmd        (501) staff       (20)      236 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_971.py
--rw-r--r--   0 dmd        (501) staff       (20)      248 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_972.py
--rw-r--r--   0 dmd        (501) staff       (20)      254 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/alt_format_995.py
--rw-r--r--   0 dmd        (501) staff       (20)      509 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_800.py
--rw-r--r--   0 dmd        (501) staff       (20)      511 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_808.py
--rw-r--r--   0 dmd        (501) staff       (20)      544 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_870.py
--rw-r--r--   0 dmd        (501) staff       (20)      527 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_878.py
--rw-r--r--   0 dmd        (501) staff       (20)      557 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_881.py
--rw-r--r--   0 dmd        (501) staff       (20)     1650 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_882.py
--rw-r--r--   0 dmd        (501) staff       (20)      838 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_883.py
--rw-r--r--   0 dmd        (501) staff       (20)      522 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_888.py
--rw-r--r--   0 dmd        (501) staff       (20)      522 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_979.py
--rw-r--r--   0 dmd        (501) staff       (20)      674 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1310 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AD.py
--rw-r--r--   0 dmd        (501) staff       (20)     1871 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AE.py
--rw-r--r--   0 dmd        (501) staff       (20)      902 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AF.py
--rw-r--r--   0 dmd        (501) staff       (20)     1556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1231 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AI.py
--rw-r--r--   0 dmd        (501) staff       (20)     1981 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AL.py
--rw-r--r--   0 dmd        (501) staff       (20)     1951 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AM.py
--rw-r--r--   0 dmd        (501) staff       (20)      670 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AO.py
--rw-r--r--   0 dmd        (501) staff       (20)     7150 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1235 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AS.py
--rw-r--r--   0 dmd        (501) staff       (20)     3044 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AT.py
--rw-r--r--   0 dmd        (501) staff       (20)     3275 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AU.py
--rw-r--r--   0 dmd        (501) staff       (20)     1075 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AW.py
--rw-r--r--   0 dmd        (501) staff       (20)     1611 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AX.py
--rw-r--r--   0 dmd        (501) staff       (20)     1611 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_AZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1889 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1728 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BB.py
--rw-r--r--   0 dmd        (501) staff       (20)     3300 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BD.py
--rw-r--r--   0 dmd        (501) staff       (20)     1940 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BE.py
--rw-r--r--   0 dmd        (501) staff       (20)      757 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BF.py
--rw-r--r--   0 dmd        (501) staff       (20)     2554 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1235 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BH.py
--rw-r--r--   0 dmd        (501) staff       (20)      675 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BI.py
--rw-r--r--   0 dmd        (501) staff       (20)      951 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      699 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BL.py
--rw-r--r--   0 dmd        (501) staff       (20)     1251 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BM.py
--rw-r--r--   0 dmd        (501) staff       (20)      717 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BN.py
--rw-r--r--   0 dmd        (501) staff       (20)     1494 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BO.py
--rw-r--r--   0 dmd        (501) staff       (20)      656 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BQ.py
--rw-r--r--   0 dmd        (501) staff       (20)     3258 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1711 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BS.py
--rw-r--r--   0 dmd        (501) staff       (20)      931 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1280 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BW.py
--rw-r--r--   0 dmd        (501) staff       (20)     3067 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BY.py
--rw-r--r--   0 dmd        (501) staff       (20)      971 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_BZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1627 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1633 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1313 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CD.py
--rw-r--r--   0 dmd        (501) staff       (20)      780 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CF.py
--rw-r--r--   0 dmd        (501) staff       (20)     1059 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CG.py
--rw-r--r--   0 dmd        (501) staff       (20)     2082 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CH.py
--rw-r--r--   0 dmd        (501) staff       (20)      767 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CI.py
--rw-r--r--   0 dmd        (501) staff       (20)      645 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CK.py
--rw-r--r--   0 dmd        (501) staff       (20)     3573 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CL.py
--rw-r--r--   0 dmd        (501) staff       (20)      963 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CM.py
--rw-r--r--   0 dmd        (501) staff       (20)     7253 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CN.py
--rw-r--r--   0 dmd        (501) staff       (20)     2114 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1448 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1208 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CU.py
--rw-r--r--   0 dmd        (501) staff       (20)      710 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CV.py
--rw-r--r--   0 dmd        (501) staff       (20)     1144 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CW.py
--rw-r--r--   0 dmd        (501) staff       (20)     1644 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CX.py
--rw-r--r--   0 dmd        (501) staff       (20)     1281 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CY.py
--rw-r--r--   0 dmd        (501) staff       (20)     1951 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_CZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     5878 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_DE.py
--rw-r--r--   0 dmd        (501) staff       (20)      665 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_DJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      983 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_DK.py
--rw-r--r--   0 dmd        (501) staff       (20)     1266 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_DM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1569 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_DO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1711 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_DZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1900 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_EC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1876 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_EE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1682 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_EG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1055 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_EH.py
--rw-r--r--   0 dmd        (501) staff       (20)      850 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_ER.py
--rw-r--r--   0 dmd        (501) staff       (20)     1724 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_ES.py
--rw-r--r--   0 dmd        (501) staff       (20)     1500 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_ET.py
--rw-r--r--   0 dmd        (501) staff       (20)     2484 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_FI.py
--rw-r--r--   0 dmd        (501) staff       (20)     1021 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_FJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_FK.py
--rw-r--r--   0 dmd        (501) staff       (20)      672 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_FM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1137 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_FO.py
--rw-r--r--   0 dmd        (501) staff       (20)     2032 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_FR.py
--rw-r--r--   0 dmd        (501) staff       (20)      850 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GA.py
--rw-r--r--   0 dmd        (501) staff       (20)     5117 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GB.py
--rw-r--r--   0 dmd        (501) staff       (20)     1331 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GD.py
--rw-r--r--   0 dmd        (501) staff       (20)     1664 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GE.py
--rw-r--r--   0 dmd        (501) staff       (20)      868 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GF.py
--rw-r--r--   0 dmd        (501) staff       (20)     1706 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1483 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GH.py
--rw-r--r--   0 dmd        (501) staff       (20)      728 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GI.py
--rw-r--r--   0 dmd        (501) staff       (20)      915 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GL.py
--rw-r--r--   0 dmd        (501) staff       (20)      732 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GM.py
--rw-r--r--   0 dmd        (501) staff       (20)      979 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GN.py
--rw-r--r--   0 dmd        (501) staff       (20)      980 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GP.py
--rw-r--r--   0 dmd        (501) staff       (20)     1089 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GQ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1837 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1044 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1602 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GU.py
--rw-r--r--   0 dmd        (501) staff       (20)      929 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GW.py
--rw-r--r--   0 dmd        (501) staff       (20)      971 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_GY.py
--rw-r--r--   0 dmd        (501) staff       (20)     2482 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_HK.py
--rw-r--r--   0 dmd        (501) staff       (20)      882 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_HN.py
--rw-r--r--   0 dmd        (501) staff       (20)     2452 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_HR.py
--rw-r--r--   0 dmd        (501) staff       (20)      924 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_HT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1719 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_HU.py
--rw-r--r--   0 dmd        (501) staff       (20)     3599 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_ID.py
--rw-r--r--   0 dmd        (501) staff       (20)     3599 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_IE.py
--rw-r--r--   0 dmd        (501) staff       (20)     3179 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_IL.py
--rw-r--r--   0 dmd        (501) staff       (20)     1564 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_IM.py
--rw-r--r--   0 dmd        (501) staff       (20)     8650 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_IN.py
--rw-r--r--   0 dmd        (501) staff       (20)      621 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_IO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1210 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_IQ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1843 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_IR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1780 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_IS.py
--rw-r--r--   0 dmd        (501) staff       (20)     3308 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_IT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1830 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_JE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1505 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_JM.py
--rw-r--r--   0 dmd        (501) staff       (20)     2482 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_JO.py
--rw-r--r--   0 dmd        (501) staff       (20)    12833 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_JP.py
--rw-r--r--   0 dmd        (501) staff       (20)     1542 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_KE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1537 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_KG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1563 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_KH.py
--rw-r--r--   0 dmd        (501) staff       (20)      935 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_KI.py
--rw-r--r--   0 dmd        (501) staff       (20)      761 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_KM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1245 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_KN.py
--rw-r--r--   0 dmd        (501) staff       (20)     1339 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_KP.py
--rw-r--r--   0 dmd        (501) staff       (20)     5194 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_KR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1175 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_KW.py
--rw-r--r--   0 dmd        (501) staff       (20)     1514 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_KY.py
--rw-r--r--   0 dmd        (501) staff       (20)     1799 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_KZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1267 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_LA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1322 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_LB.py
--rw-r--r--   0 dmd        (501) staff       (20)     1291 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_LC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1661 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_LI.py
--rw-r--r--   0 dmd        (501) staff       (20)     1082 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_LK.py
--rw-r--r--   0 dmd        (501) staff       (20)     1319 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_LR.py
--rw-r--r--   0 dmd        (501) staff       (20)      751 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_LS.py
--rw-r--r--   0 dmd        (501) staff       (20)     2129 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_LT.py
--rw-r--r--   0 dmd        (501) staff       (20)     3066 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_LU.py
--rw-r--r--   0 dmd        (501) staff       (20)     1069 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_LV.py
--rw-r--r--   0 dmd        (501) staff       (20)      873 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_LY.py
--rw-r--r--   0 dmd        (501) staff       (20)     2112 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1558 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1793 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MD.py
--rw-r--r--   0 dmd        (501) staff       (20)     1487 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_ME.py
--rw-r--r--   0 dmd        (501) staff       (20)      723 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MF.py
--rw-r--r--   0 dmd        (501) staff       (20)     1051 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MG.py
--rw-r--r--   0 dmd        (501) staff       (20)      832 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MH.py
--rw-r--r--   0 dmd        (501) staff       (20)     1741 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MK.py
--rw-r--r--   0 dmd        (501) staff       (20)     1287 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_ML.py
--rw-r--r--   0 dmd        (501) staff       (20)     3206 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1778 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MN.py
--rw-r--r--   0 dmd        (501) staff       (20)      749 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1370 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MP.py
--rw-r--r--   0 dmd        (501) staff       (20)      893 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MQ.py
--rw-r--r--   0 dmd        (501) staff       (20)      845 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1184 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MS.py
--rw-r--r--   0 dmd        (501) staff       (20)     1417 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1368 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MU.py
--rw-r--r--   0 dmd        (501) staff       (20)     1312 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MV.py
--rw-r--r--   0 dmd        (501) staff       (20)     1423 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MW.py
--rw-r--r--   0 dmd        (501) staff       (20)     3655 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MX.py
--rw-r--r--   0 dmd        (501) staff       (20)    10145 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MY.py
--rw-r--r--   0 dmd        (501) staff       (20)      946 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_MZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1865 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_NA.py
--rw-r--r--   0 dmd        (501) staff       (20)      849 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_NC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1131 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_NE.py
--rw-r--r--   0 dmd        (501) staff       (20)      877 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_NF.py
--rw-r--r--   0 dmd        (501) staff       (20)     2676 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_NG.py
--rw-r--r--   0 dmd        (501) staff       (20)      830 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_NI.py
--rw-r--r--   0 dmd        (501) staff       (20)     2894 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_NL.py
--rw-r--r--   0 dmd        (501) staff       (20)     1842 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_NO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1351 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_NP.py
--rw-r--r--   0 dmd        (501) staff       (20)      639 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_NR.py
--rw-r--r--   0 dmd        (501) staff       (20)      544 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_NU.py
--rw-r--r--   0 dmd        (501) staff       (20)     2373 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_NZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1220 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_OM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1561 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_PA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1894 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_PE.py
--rw-r--r--   0 dmd        (501) staff       (20)      964 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_PF.py
--rw-r--r--   0 dmd        (501) staff       (20)     1158 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_PG.py
--rw-r--r--   0 dmd        (501) staff       (20)     2440 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_PH.py
--rw-r--r--   0 dmd        (501) staff       (20)     3443 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_PK.py
--rw-r--r--   0 dmd        (501) staff       (20)     2278 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_PL.py
--rw-r--r--   0 dmd        (501) staff       (20)      796 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_PM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1244 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_PR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1469 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_PS.py
--rw-r--r--   0 dmd        (501) staff       (20)     1847 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_PT.py
--rw-r--r--   0 dmd        (501) staff       (20)      732 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_PW.py
--rw-r--r--   0 dmd        (501) staff       (20)     2353 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_PY.py
--rw-r--r--   0 dmd        (501) staff       (20)     1062 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_QA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1335 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_RE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1919 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_RO.py
--rw-r--r--   0 dmd        (501) staff       (20)     2300 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_RS.py
--rw-r--r--   0 dmd        (501) staff       (20)     2121 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_RU.py
--rw-r--r--   0 dmd        (501) staff       (20)     1277 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_RW.py
--rw-r--r--   0 dmd        (501) staff       (20)     1819 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1060 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SB.py
--rw-r--r--   0 dmd        (501) staff       (20)      971 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SC.py
--rw-r--r--   0 dmd        (501) staff       (20)      775 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SD.py
--rw-r--r--   0 dmd        (501) staff       (20)     5804 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1596 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SG.py
--rw-r--r--   0 dmd        (501) staff       (20)      717 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SH.py
--rw-r--r--   0 dmd        (501) staff       (20)     1896 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SI.py
--rw-r--r--   0 dmd        (501) staff       (20)     1464 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SJ.py
--rw-r--r--   0 dmd        (501) staff       (20)     2668 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SK.py
--rw-r--r--   0 dmd        (501) staff       (20)      858 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SL.py
--rw-r--r--   0 dmd        (501) staff       (20)     1662 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1381 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SN.py
--rw-r--r--   0 dmd        (501) staff       (20)     1477 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1047 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SR.py
--rw-r--r--   0 dmd        (501) staff       (20)      754 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SS.py
--rw-r--r--   0 dmd        (501) staff       (20)      658 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_ST.py
--rw-r--r--   0 dmd        (501) staff       (20)     1172 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SV.py
--rw-r--r--   0 dmd        (501) staff       (20)     1233 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SX.py
--rw-r--r--   0 dmd        (501) staff       (20)     1195 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SY.py
--rw-r--r--   0 dmd        (501) staff       (20)     1270 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_SZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      425 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1402 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TC.py
--rw-r--r--   0 dmd        (501) staff       (20)      748 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TD.py
--rw-r--r--   0 dmd        (501) staff       (20)      735 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1570 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TH.py
--rw-r--r--   0 dmd        (501) staff       (20)     1583 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      590 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TK.py
--rw-r--r--   0 dmd        (501) staff       (20)     1162 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TL.py
--rw-r--r--   0 dmd        (501) staff       (20)     1247 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1103 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TN.py
--rw-r--r--   0 dmd        (501) staff       (20)     1057 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TO.py
--rw-r--r--   0 dmd        (501) staff       (20)     2448 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1509 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TT.py
--rw-r--r--   0 dmd        (501) staff       (20)      569 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TV.py
--rw-r--r--   0 dmd        (501) staff       (20)     2303 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TW.py
--rw-r--r--   0 dmd        (501) staff       (20)     1755 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_TZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     2242 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_UA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1657 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_UG.py
--rw-r--r--   0 dmd        (501) staff       (20)     2859 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_US.py
--rw-r--r--   0 dmd        (501) staff       (20)     1439 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_UY.py
--rw-r--r--   0 dmd        (501) staff       (20)     2430 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_UZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1604 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_VA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1309 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_VC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1162 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_VE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1310 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_VG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1412 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_VI.py
--rw-r--r--   0 dmd        (501) staff       (20)     3191 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_VN.py
--rw-r--r--   0 dmd        (501) staff       (20)      869 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_VU.py
--rw-r--r--   0 dmd        (501) staff       (20)      778 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_WF.py
--rw-r--r--   0 dmd        (501) staff       (20)     1030 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_WS.py
--rw-r--r--   0 dmd        (501) staff       (20)     1347 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_XK.py
--rw-r--r--   0 dmd        (501) staff       (20)     1088 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_YE.py
--rw-r--r--   0 dmd        (501) staff       (20)      833 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_YT.py
--rw-r--r--   0 dmd        (501) staff       (20)     2008 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_ZA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1370 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_ZM.py
--rw-r--r--   0 dmd        (501) staff       (20)     3290 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/data/region_ZW.py
--rw-r--r--   0 dmd        (501) staff       (20)    10966 2018-05-17 08:38:10.000000 phonenumberslite-8.9.8/phonenumbers/geocoder.py
--rw-r--r--   0 dmd        (501) staff       (20)    32671 2018-05-17 08:40:03.000000 phonenumberslite-8.9.8/phonenumbers/phonemetadata.py
--rw-r--r--   0 dmd        (501) staff       (20)    12452 2018-05-17 08:40:03.000000 phonenumberslite-8.9.8/phonenumbers/phonenumber.py
--rw-r--r--   0 dmd        (501) staff       (20)    38746 2018-05-17 08:40:03.000000 phonenumberslite-8.9.8/phonenumbers/phonenumbermatcher.py
--rw-r--r--   0 dmd        (501) staff       (20)   155085 2018-05-17 08:40:03.000000 phonenumberslite-8.9.8/phonenumbers/phonenumberutil.py
--rw-r--r--   0 dmd        (501) staff       (20)     3650 2013-11-15 12:19:10.000000 phonenumberslite-8.9.8/phonenumbers/prefix.py
--rw-r--r--   0 dmd        (501) staff       (20)     1428 2018-05-17 08:38:26.000000 phonenumberslite-8.9.8/phonenumbers/re_util.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/
--rw-r--r--   0 dmd        (501) staff       (20)     2180 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AC.py
--rw-r--r--   0 dmd        (501) staff       (20)      558 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AD.py
--rw-r--r--   0 dmd        (501) staff       (20)      696 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AE.py
--rw-r--r--   0 dmd        (501) staff       (20)      807 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AF.py
--rw-r--r--   0 dmd        (501) staff       (20)      791 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AG.py
--rw-r--r--   0 dmd        (501) staff       (20)      773 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AI.py
--rw-r--r--   0 dmd        (501) staff       (20)     1131 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AL.py
--rw-r--r--   0 dmd        (501) staff       (20)      822 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AM.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1006 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AR.py
--rw-r--r--   0 dmd        (501) staff       (20)      676 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AS.py
--rw-r--r--   0 dmd        (501) staff       (20)      737 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1360 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AU.py
--rw-r--r--   0 dmd        (501) staff       (20)      788 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AW.py
--rw-r--r--   0 dmd        (501) staff       (20)      578 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AX.py
--rw-r--r--   0 dmd        (501) staff       (20)      826 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_AZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      786 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BA.py
--rw-r--r--   0 dmd        (501) staff       (20)      565 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BB.py
--rw-r--r--   0 dmd        (501) staff       (20)     1089 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BD.py
--rw-r--r--   0 dmd        (501) staff       (20)     1212 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BE.py
--rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BF.py
--rw-r--r--   0 dmd        (501) staff       (20)      717 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1146 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BH.py
--rw-r--r--   0 dmd        (501) staff       (20)      966 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BI.py
--rw-r--r--   0 dmd        (501) staff       (20)      822 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      541 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BL.py
--rw-r--r--   0 dmd        (501) staff       (20)      777 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BM.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BN.py
--rw-r--r--   0 dmd        (501) staff       (20)      684 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BO.py
--rw-r--r--   0 dmd        (501) staff       (20)      788 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BQ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1494 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BR.py
--rw-r--r--   0 dmd        (501) staff       (20)      554 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BS.py
--rw-r--r--   0 dmd        (501) staff       (20)      684 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BT.py
--rw-r--r--   0 dmd        (501) staff       (20)      801 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BW.py
--rw-r--r--   0 dmd        (501) staff       (20)      612 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BY.py
--rw-r--r--   0 dmd        (501) staff       (20)      568 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_BZ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1044 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CA.py
--rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CC.py
--rw-r--r--   0 dmd        (501) staff       (20)      826 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CD.py
--rw-r--r--   0 dmd        (501) staff       (20)      580 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CF.py
--rw-r--r--   0 dmd        (501) staff       (20)      661 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1354 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CH.py
--rw-r--r--   0 dmd        (501) staff       (20)      814 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CI.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CK.py
--rw-r--r--   0 dmd        (501) staff       (20)     1650 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CL.py
--rw-r--r--   0 dmd        (501) staff       (20)      804 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CM.py
--rw-r--r--   0 dmd        (501) staff       (20)      734 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CN.py
--rw-r--r--   0 dmd        (501) staff       (20)      875 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CO.py
--rw-r--r--   0 dmd        (501) staff       (20)      891 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CR.py
--rw-r--r--   0 dmd        (501) staff       (20)      581 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CU.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CV.py
--rw-r--r--   0 dmd        (501) staff       (20)      788 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CW.py
--rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CX.py
--rw-r--r--   0 dmd        (501) staff       (20)      705 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CY.py
--rw-r--r--   0 dmd        (501) staff       (20)      768 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_CZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      706 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_DE.py
--rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_DJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      746 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_DK.py
--rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_DM.py
--rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_DO.py
--rw-r--r--   0 dmd        (501) staff       (20)      785 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_DZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      579 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_EC.py
--rw-r--r--   0 dmd        (501) staff       (20)     2417 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_EE.py
--rw-r--r--   0 dmd        (501) staff       (20)      824 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_EG.py
--rw-r--r--   0 dmd        (501) staff       (20)      572 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_EH.py
--rw-r--r--   0 dmd        (501) staff       (20)      678 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_ER.py
--rw-r--r--   0 dmd        (501) staff       (20)     1620 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_ES.py
--rw-r--r--   0 dmd        (501) staff       (20)      588 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_ET.py
--rw-r--r--   0 dmd        (501) staff       (20)      707 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_FI.py
--rw-r--r--   0 dmd        (501) staff       (20)      749 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_FJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_FK.py
--rw-r--r--   0 dmd        (501) staff       (20)      576 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_FM.py
--rw-r--r--   0 dmd        (501) staff       (20)      591 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_FO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1553 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_FR.py
--rw-r--r--   0 dmd        (501) staff       (20)      588 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1338 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GB.py
--rw-r--r--   0 dmd        (501) staff       (20)      773 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GD.py
--rw-r--r--   0 dmd        (501) staff       (20)      844 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GE.py
--rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GF.py
--rw-r--r--   0 dmd        (501) staff       (20)      636 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GG.py
--rw-r--r--   0 dmd        (501) staff       (20)      856 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GH.py
--rw-r--r--   0 dmd        (501) staff       (20)     1286 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GI.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GL.py
--rw-r--r--   0 dmd        (501) staff       (20)      566 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GM.py
--rw-r--r--   0 dmd        (501) staff       (20)      676 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GN.py
--rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GP.py
--rw-r--r--   0 dmd        (501) staff       (20)      719 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GR.py
--rw-r--r--   0 dmd        (501) staff       (20)      829 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GT.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GU.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GW.py
--rw-r--r--   0 dmd        (501) staff       (20)      860 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_GY.py
--rw-r--r--   0 dmd        (501) staff       (20)     1155 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_HK.py
--rw-r--r--   0 dmd        (501) staff       (20)      793 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_HN.py
--rw-r--r--   0 dmd        (501) staff       (20)     1134 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_HR.py
--rw-r--r--   0 dmd        (501) staff       (20)      799 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_HT.py
--rw-r--r--   0 dmd        (501) staff       (20)      727 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_HU.py
--rw-r--r--   0 dmd        (501) staff       (20)      831 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_ID.py
--rw-r--r--   0 dmd        (501) staff       (20)     1249 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_IE.py
--rw-r--r--   0 dmd        (501) staff       (20)      848 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_IL.py
--rw-r--r--   0 dmd        (501) staff       (20)      720 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_IM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1625 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_IN.py
--rw-r--r--   0 dmd        (501) staff       (20)      860 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_IQ.py
--rw-r--r--   0 dmd        (501) staff       (20)     1368 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_IR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1007 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_IS.py
--rw-r--r--   0 dmd        (501) staff       (20)     1220 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_IT.py
--rw-r--r--   0 dmd        (501) staff       (20)      658 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_JE.py
--rw-r--r--   0 dmd        (501) staff       (20)      796 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_JM.py
--rw-r--r--   0 dmd        (501) staff       (20)      860 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_JO.py
--rw-r--r--   0 dmd        (501) staff       (20)      554 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_JP.py
--rw-r--r--   0 dmd        (501) staff       (20)     1594 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_KE.py
--rw-r--r--   0 dmd        (501) staff       (20)      796 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_KG.py
--rw-r--r--   0 dmd        (501) staff       (20)      810 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_KH.py
--rw-r--r--   0 dmd        (501) staff       (20)      725 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_KI.py
--rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_KM.py
--rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_KN.py
--rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_KP.py
--rw-r--r--   0 dmd        (501) staff       (20)      929 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_KR.py
--rw-r--r--   0 dmd        (501) staff       (20)      686 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_KW.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_KY.py
--rw-r--r--   0 dmd        (501) staff       (20)      841 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_KZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_LA.py
--rw-r--r--   0 dmd        (501) staff       (20)      579 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_LB.py
--rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_LC.py
--rw-r--r--   0 dmd        (501) staff       (20)      602 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_LI.py
--rw-r--r--   0 dmd        (501) staff       (20)      560 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_LK.py
--rw-r--r--   0 dmd        (501) staff       (20)      837 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_LR.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_LS.py
--rw-r--r--   0 dmd        (501) staff       (20)      760 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_LT.py
--rw-r--r--   0 dmd        (501) staff       (20)      712 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_LU.py
--rw-r--r--   0 dmd        (501) staff       (20)     1143 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_LV.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_LY.py
--rw-r--r--   0 dmd        (501) staff       (20)      572 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MA.py
--rw-r--r--   0 dmd        (501) staff       (20)      579 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MC.py
--rw-r--r--   0 dmd        (501) staff       (20)      786 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MD.py
--rw-r--r--   0 dmd        (501) staff       (20)      697 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_ME.py
--rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MF.py
--rw-r--r--   0 dmd        (501) staff       (20)      564 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MG.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MH.py
--rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MK.py
--rw-r--r--   0 dmd        (501) staff       (20)     1470 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_ML.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MM.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MN.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MO.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MP.py
--rw-r--r--   0 dmd        (501) staff       (20)      574 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MQ.py
--rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MR.py
--rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MS.py
--rw-r--r--   0 dmd        (501) staff       (20)      705 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MT.py
--rw-r--r--   0 dmd        (501) staff       (20)      594 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MU.py
--rw-r--r--   0 dmd        (501) staff       (20)      726 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MV.py
--rw-r--r--   0 dmd        (501) staff       (20)      810 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MW.py
--rw-r--r--   0 dmd        (501) staff       (20)      761 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MX.py
--rw-r--r--   0 dmd        (501) staff       (20)      952 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MY.py
--rw-r--r--   0 dmd        (501) staff       (20)      594 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_MZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      599 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_NA.py
--rw-r--r--   0 dmd        (501) staff       (20)      904 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_NC.py
--rw-r--r--   0 dmd        (501) staff       (20)      813 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_NE.py
--rw-r--r--   0 dmd        (501) staff       (20)      568 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_NF.py
--rw-r--r--   0 dmd        (501) staff       (20)      793 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_NG.py
--rw-r--r--   0 dmd        (501) staff       (20)      739 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_NI.py
--rw-r--r--   0 dmd        (501) staff       (20)     1035 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_NL.py
--rw-r--r--   0 dmd        (501) staff       (20)      743 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_NO.py
--rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_NP.py
--rw-r--r--   0 dmd        (501) staff       (20)      566 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_NR.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_NU.py
--rw-r--r--   0 dmd        (501) staff       (20)      901 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_NZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      552 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_OM.py
--rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_PA.py
--rw-r--r--   0 dmd        (501) staff       (20)      568 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_PE.py
--rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_PF.py
--rw-r--r--   0 dmd        (501) staff       (20)      741 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_PG.py
--rw-r--r--   0 dmd        (501) staff       (20)      565 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_PH.py
--rw-r--r--   0 dmd        (501) staff       (20)      599 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_PK.py
--rw-r--r--   0 dmd        (501) staff       (20)      773 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_PL.py
--rw-r--r--   0 dmd        (501) staff       (20)      678 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_PM.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_PR.py
--rw-r--r--   0 dmd        (501) staff       (20)      675 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_PS.py
--rw-r--r--   0 dmd        (501) staff       (20)      699 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_PT.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_PW.py
--rw-r--r--   0 dmd        (501) staff       (20)      565 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_PY.py
--rw-r--r--   0 dmd        (501) staff       (20)      589 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_QA.py
--rw-r--r--   0 dmd        (501) staff       (20)      574 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_RE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1043 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_RO.py
--rw-r--r--   0 dmd        (501) staff       (20)      602 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_RS.py
--rw-r--r--   0 dmd        (501) staff       (20)      595 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_RU.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_RW.py
--rw-r--r--   0 dmd        (501) staff       (20)     1045 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SA.py
--rw-r--r--   0 dmd        (501) staff       (20)      650 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SB.py
--rw-r--r--   0 dmd        (501) staff       (20)      638 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SC.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SD.py
--rw-r--r--   0 dmd        (501) staff       (20)     1316 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SE.py
--rw-r--r--   0 dmd        (501) staff       (20)      748 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SG.py
--rw-r--r--   0 dmd        (501) staff       (20)      582 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SH.py
--rw-r--r--   0 dmd        (501) staff       (20)      711 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SI.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      747 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SK.py
--rw-r--r--   0 dmd        (501) staff       (20)      808 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SL.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SM.py
--rw-r--r--   0 dmd        (501) staff       (20)     1279 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SN.py
--rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SO.py
--rw-r--r--   0 dmd        (501) staff       (20)      561 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SR.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_ST.py
--rw-r--r--   0 dmd        (501) staff       (20)      793 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SV.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SX.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SY.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_SZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_TC.py
--rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_TD.py
--rw-r--r--   0 dmd        (501) staff       (20)      587 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_TG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1672 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_TH.py
--rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_TJ.py
--rw-r--r--   0 dmd        (501) staff       (20)      581 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_TL.py
--rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_TM.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_TN.py
--rw-r--r--   0 dmd        (501) staff       (20)      574 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_TO.py
--rw-r--r--   0 dmd        (501) staff       (20)     1767 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_TR.py
--rw-r--r--   0 dmd        (501) staff       (20)      554 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_TT.py
--rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_TV.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_TW.py
--rw-r--r--   0 dmd        (501) staff       (20)      808 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_TZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      956 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_UA.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_UG.py
--rw-r--r--   0 dmd        (501) staff       (20)     1618 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_US.py
--rw-r--r--   0 dmd        (501) staff       (20)      707 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_UY.py
--rw-r--r--   0 dmd        (501) staff       (20)      833 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_UZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      558 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_VA.py
--rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_VC.py
--rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_VE.py
--rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_VG.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_VI.py
--rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_VN.py
--rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_VU.py
--rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_WF.py
--rw-r--r--   0 dmd        (501) staff       (20)      710 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_WS.py
--rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_XK.py
--rw-r--r--   0 dmd        (501) staff       (20)      558 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_YE.py
--rw-r--r--   0 dmd        (501) staff       (20)      567 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_YT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1188 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_ZA.py
--rw-r--r--   0 dmd        (501) staff       (20)      575 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_ZM.py
--rw-r--r--   0 dmd        (501) staff       (20)      976 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/phonenumbers/shortdata/region_ZW.py
--rw-r--r--   0 dmd        (501) staff       (20)    20748 2018-05-17 08:40:03.000000 phonenumberslite-8.9.8/phonenumbers/shortnumberinfo.py
--rw-r--r--   0 dmd        (501) staff       (20)     4947 2018-05-17 08:38:10.000000 phonenumberslite-8.9.8/phonenumbers/timezone.py
--rw-r--r--   0 dmd        (501) staff       (20)    18939 2013-11-15 12:19:10.000000 phonenumberslite-8.9.8/phonenumbers/unicode_util.py
--rw-r--r--   0 dmd        (501) staff       (20)     5865 2016-01-29 10:59:27.000000 phonenumberslite-8.9.8/phonenumbers/util.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/phonenumberslite.egg-info/
--rw-r--r--   0 dmd        (501) staff       (20)        1 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/phonenumberslite.egg-info/dependency_links.txt
--rw-r--r--   0 dmd        (501) staff       (20)      928 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/phonenumberslite.egg-info/PKG-INFO
--rw-r--r--   0 dmd        (501) staff       (20)    20341 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/phonenumberslite.egg-info/SOURCES.txt
--rw-r--r--   0 dmd        (501) staff       (20)       13 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/phonenumberslite.egg-info/top_level.txt
--rw-r--r--   0 dmd        (501) staff       (20)      928 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/PKG-INFO
--rw-r--r--   0 dmd        (501) staff       (20)       67 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/setup.cfg
--rwxr-xr-x   0 dmd        (501) staff       (20)     3319 2017-09-15 12:46:57.000000 phonenumberslite-8.9.8/setup.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/tests/
--rw-r--r--   0 dmd        (501) staff       (20)      585 2013-10-11 17:19:49.000000 phonenumberslite-8.9.8/tests/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)    67545 2018-05-17 08:38:10.000000 phonenumberslite-8.9.8/tests/asyoutypetest.py
--rw-r--r--   0 dmd        (501) staff       (20)     5419 2013-11-15 12:19:10.000000 phonenumberslite-8.9.8/tests/carriertest.py
--rw-r--r--   0 dmd        (501) staff       (20)    18579 2018-05-17 08:40:03.000000 phonenumberslite-8.9.8/tests/examplenumberstest.py
--rw-r--r--   0 dmd        (501) staff       (20)    11403 2018-05-17 08:40:03.000000 phonenumberslite-8.9.8/tests/geocodertest.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/tests/pb2/
--rw-r--r--   0 dmd        (501) staff       (20)      127 2015-10-07 18:13:06.000000 phonenumberslite-8.9.8/tests/pb2/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)     2564 2018-05-19 06:37:56.000000 phonenumberslite-8.9.8/tests/pb2/converttest.py
--rw-r--r--   0 dmd        (501) staff       (20)    49214 2018-05-17 08:40:03.000000 phonenumberslite-8.9.8/tests/phonenumbermatchertest.py
--rwxr-xr-x   0 dmd        (501) staff       (20)     7615 2018-05-17 08:38:10.000000 phonenumberslite-8.9.8/tests/phonenumbertest.py
--rwxr-xr-x   0 dmd        (501) staff       (20)   187153 2018-05-17 14:56:20.000000 phonenumberslite-8.9.8/tests/phonenumberutiltest.py
--rw-r--r--   0 dmd        (501) staff       (20)    19975 2018-05-17 08:40:03.000000 phonenumberslite-8.9.8/tests/shortnumberinfotest.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/tests/testcarrierdata/
--rw-r--r--   0 dmd        (501) staff       (20)      847 2018-06-16 06:46:07.000000 phonenumberslite-8.9.8/tests/testcarrierdata/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)     1056 2018-06-16 06:46:07.000000 phonenumberslite-8.9.8/tests/testcarrierdata/data0.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/tests/testdata/
--rw-r--r--   0 dmd        (501) staff       (20)     2186 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)      520 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_800.py
--rw-r--r--   0 dmd        (501) staff       (20)      527 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_882.py
--rw-r--r--   0 dmd        (501) staff       (20)      533 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_979.py
--rw-r--r--   0 dmd        (501) staff       (20)      436 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_AD.py
--rw-r--r--   0 dmd        (501) staff       (20)      440 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_AE.py
--rw-r--r--   0 dmd        (501) staff       (20)      731 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_AM.py
--rw-r--r--   0 dmd        (501) staff       (20)      746 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_AO.py
--rw-r--r--   0 dmd        (501) staff       (20)     2450 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_AR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1247 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_AU.py
--rw-r--r--   0 dmd        (501) staff       (20)      420 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_BB.py
--rw-r--r--   0 dmd        (501) staff       (20)      511 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_BR.py
--rw-r--r--   0 dmd        (501) staff       (20)     1072 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_BS.py
--rw-r--r--   0 dmd        (501) staff       (20)      945 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_BY.py
--rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_CA.py
--rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_CC.py
--rw-r--r--   0 dmd        (501) staff       (20)     1083 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_CN.py
--rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_CX.py
--rw-r--r--   0 dmd        (501) staff       (20)     2079 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_DE.py
--rw-r--r--   0 dmd        (501) staff       (20)      671 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_FR.py
--rw-r--r--   0 dmd        (501) staff       (20)     2140 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_GB.py
--rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_GG.py
--rw-r--r--   0 dmd        (501) staff       (20)      502 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_HU.py
--rw-r--r--   0 dmd        (501) staff       (20)     1308 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_IT.py
--rw-r--r--   0 dmd        (501) staff       (20)     1990 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_JP.py
--rw-r--r--   0 dmd        (501) staff       (20)     3617 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_KR.py
--rw-r--r--   0 dmd        (501) staff       (20)     2808 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_MX.py
--rw-r--r--   0 dmd        (501) staff       (20)     1503 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_NZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      909 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_PL.py
--rw-r--r--   0 dmd        (501) staff       (20)     1091 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_RE.py
--rw-r--r--   0 dmd        (501) staff       (20)      382 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_SE.py
--rw-r--r--   0 dmd        (501) staff       (20)     1221 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_SG.py
--rw-r--r--   0 dmd        (501) staff       (20)      668 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_TA.py
--rw-r--r--   0 dmd        (501) staff       (20)     1640 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_US.py
--rw-r--r--   0 dmd        (501) staff       (20)      921 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_UZ.py
--rw-r--r--   0 dmd        (501) staff       (20)      777 2018-06-16 06:46:01.000000 phonenumberslite-8.9.8/tests/testdata/region_YT.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/tests/testgeodata/
--rw-r--r--   0 dmd        (501) staff       (20)      847 2018-06-16 06:46:07.000000 phonenumberslite-8.9.8/tests/testgeodata/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)     1881 2018-06-16 06:46:07.000000 phonenumberslite-8.9.8/tests/testgeodata/data0.py
--rw-r--r--   0 dmd        (501) staff       (20)     2317 2017-07-24 12:06:48.000000 phonenumberslite-8.9.8/tests/testmetadatatest.py
-drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-16 06:52:50.000000 phonenumberslite-8.9.8/tests/testtzdata/
--rw-r--r--   0 dmd        (501) staff       (20)      835 2018-06-16 06:46:08.000000 phonenumberslite-8.9.8/tests/testtzdata/__init__.py
--rw-r--r--   0 dmd        (501) staff       (20)     1112 2018-06-16 06:46:08.000000 phonenumberslite-8.9.8/tests/testtzdata/data0.py
--rw-r--r--   0 dmd        (501) staff       (20)     5914 2013-11-15 12:19:10.000000 phonenumberslite-8.9.8/tests/timezonetest.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/
+-rw-r--r--   0 dmd        (501) staff       (20)      115 2014-12-16 15:23:29.000000 phonenumberslite-8.9.9/MANIFEST.in
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/phonenumbers/
+-rw-r--r--   0 dmd        (501) staff       (20)     9853 2018-06-29 07:26:49.000000 phonenumberslite-8.9.9/phonenumbers/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)    31975 2017-04-19 13:38:31.000000 phonenumberslite-8.9.9/phonenumbers/asyoutypeformatter.py
+-rw-r--r--   0 dmd        (501) staff       (20)     6352 2013-11-15 12:19:09.000000 phonenumberslite-8.9.9/phonenumbers/carrier.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/phonenumbers/data/
+-rw-r--r--   0 dmd        (501) staff       (20)    10295 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)      339 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_255.py
+-rw-r--r--   0 dmd        (501) staff       (20)      232 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_27.py
+-rw-r--r--   0 dmd        (501) staff       (20)      228 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_30.py
+-rw-r--r--   0 dmd        (501) staff       (20)      436 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_31.py
+-rw-r--r--   0 dmd        (501) staff       (20)      348 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_34.py
+-rw-r--r--   0 dmd        (501) staff       (20)      217 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_350.py
+-rw-r--r--   0 dmd        (501) staff       (20)      454 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_351.py
+-rw-r--r--   0 dmd        (501) staff       (20)      199 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_352.py
+-rw-r--r--   0 dmd        (501) staff       (20)      360 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_358.py
+-rw-r--r--   0 dmd        (501) staff       (20)      482 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_359.py
+-rw-r--r--   0 dmd        (501) staff       (20)      328 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_36.py
+-rw-r--r--   0 dmd        (501) staff       (20)      572 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_372.py
+-rw-r--r--   0 dmd        (501) staff       (20)      353 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_373.py
+-rw-r--r--   0 dmd        (501) staff       (20)      493 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_380.py
+-rw-r--r--   0 dmd        (501) staff       (20)      754 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_381.py
+-rw-r--r--   0 dmd        (501) staff       (20)      545 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_385.py
+-rw-r--r--   0 dmd        (501) staff       (20)      377 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_39.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1480 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_43.py
+-rw-r--r--   0 dmd        (501) staff       (20)      689 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_44.py
+-rw-r--r--   0 dmd        (501) staff       (20)     7207 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_49.py
+-rw-r--r--   0 dmd        (501) staff       (20)      226 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_505.py
+-rw-r--r--   0 dmd        (501) staff       (20)      241 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_506.py
+-rw-r--r--   0 dmd        (501) staff       (20)      404 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_52.py
+-rw-r--r--   0 dmd        (501) staff       (20)      343 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_54.py
+-rw-r--r--   0 dmd        (501) staff       (20)      224 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_55.py
+-rw-r--r--   0 dmd        (501) staff       (20)      197 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_58.py
+-rw-r--r--   0 dmd        (501) staff       (20)      500 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_595.py
+-rw-r--r--   0 dmd        (501) staff       (20)      589 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_61.py
+-rw-r--r--   0 dmd        (501) staff       (20)      589 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_62.py
+-rw-r--r--   0 dmd        (501) staff       (20)      215 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_63.py
+-rw-r--r--   0 dmd        (501) staff       (20)      348 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_64.py
+-rw-r--r--   0 dmd        (501) staff       (20)      216 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_66.py
+-rw-r--r--   0 dmd        (501) staff       (20)      230 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_675.py
+-rw-r--r--   0 dmd        (501) staff       (20)      230 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_676.py
+-rw-r--r--   0 dmd        (501) staff       (20)      227 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_679.py
+-rw-r--r--   0 dmd        (501) staff       (20)      696 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_7.py
+-rw-r--r--   0 dmd        (501) staff       (20)      479 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_81.py
+-rw-r--r--   0 dmd        (501) staff       (20)      343 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_84.py
+-rw-r--r--   0 dmd        (501) staff       (20)      213 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_855.py
+-rw-r--r--   0 dmd        (501) staff       (20)      415 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_856.py
+-rw-r--r--   0 dmd        (501) staff       (20)      269 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_90.py
+-rw-r--r--   0 dmd        (501) staff       (20)      973 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_91.py
+-rw-r--r--   0 dmd        (501) staff       (20)      431 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_94.py
+-rw-r--r--   0 dmd        (501) staff       (20)      224 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_95.py
+-rw-r--r--   0 dmd        (501) staff       (20)      236 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_971.py
+-rw-r--r--   0 dmd        (501) staff       (20)      248 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_972.py
+-rw-r--r--   0 dmd        (501) staff       (20)      254 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/alt_format_995.py
+-rw-r--r--   0 dmd        (501) staff       (20)      509 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_800.py
+-rw-r--r--   0 dmd        (501) staff       (20)      511 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_808.py
+-rw-r--r--   0 dmd        (501) staff       (20)      544 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_870.py
+-rw-r--r--   0 dmd        (501) staff       (20)      527 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_878.py
+-rw-r--r--   0 dmd        (501) staff       (20)      557 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_881.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1650 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_882.py
+-rw-r--r--   0 dmd        (501) staff       (20)      838 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_883.py
+-rw-r--r--   0 dmd        (501) staff       (20)      522 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_888.py
+-rw-r--r--   0 dmd        (501) staff       (20)      522 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_979.py
+-rw-r--r--   0 dmd        (501) staff       (20)      674 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1310 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AD.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1871 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      902 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1556 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1231 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1981 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AL.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1951 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      670 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     7150 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1235 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3044 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3275 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1075 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1611 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AX.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1611 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_AZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1889 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1728 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BB.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3300 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BD.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1940 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      757 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2554 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1235 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      675 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      951 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      699 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BL.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1251 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      717 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BN.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1494 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      656 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BQ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3258 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1711 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      931 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1280 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3067 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      971 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_BZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1627 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1633 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1313 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      780 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1059 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2082 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      767 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      645 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3573 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      963 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     7253 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CN.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2114 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1448 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1208 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      710 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CV.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1144 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1644 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CX.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1281 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1951 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_CZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     5878 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_DE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      665 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_DJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      983 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_DK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1266 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_DM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1569 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_DO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1711 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_DZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1900 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_EC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1876 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_EE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1682 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_EG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1055 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_EH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      850 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_ER.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1724 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_ES.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1500 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_ET.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2484 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_FI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1021 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_FJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_FK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      672 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_FM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1137 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_FO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2032 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_FR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      850 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     5117 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GB.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1331 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GD.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1664 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      868 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1706 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1483 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      728 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      915 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      732 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      979 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      980 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GP.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1089 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GQ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1837 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1044 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1602 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      929 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      971 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_GY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2482 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_HK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      882 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_HN.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2452 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_HR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      924 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_HT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1719 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_HU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3599 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_ID.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3599 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_IE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3179 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_IL.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1564 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_IM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     8650 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_IN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      621 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_IO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1210 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_IQ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1843 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_IR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1780 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_IS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3308 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_IT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1830 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_JE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1505 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_JM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2482 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_JO.py
+-rw-r--r--   0 dmd        (501) staff       (20)    12833 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_JP.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1542 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_KE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1545 2018-06-29 07:26:49.000000 phonenumberslite-8.9.9/phonenumbers/data/region_KG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1563 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_KH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      935 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_KI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      761 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_KM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1245 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_KN.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1339 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_KP.py
+-rw-r--r--   0 dmd        (501) staff       (20)     5194 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_KR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1175 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_KW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1514 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_KY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1799 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_KZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1267 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_LA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1322 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_LB.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1291 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_LC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1661 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_LI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1082 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_LK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1319 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_LR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      751 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_LS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2129 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_LT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3066 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_LU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1069 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_LV.py
+-rw-r--r--   0 dmd        (501) staff       (20)      873 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_LY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2112 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1558 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1793 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MD.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1487 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_ME.py
+-rw-r--r--   0 dmd        (501) staff       (20)      723 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1051 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      832 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MH.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1741 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1287 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_ML.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3206 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1778 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      749 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1370 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MP.py
+-rw-r--r--   0 dmd        (501) staff       (20)      893 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MQ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      845 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1184 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1417 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1368 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1312 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MV.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1423 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3655 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MX.py
+-rw-r--r--   0 dmd        (501) staff       (20)    10145 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      946 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_MZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1865 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_NA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      849 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_NC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1131 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_NE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      877 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_NF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2676 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_NG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      830 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_NI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2894 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_NL.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1842 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_NO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1351 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_NP.py
+-rw-r--r--   0 dmd        (501) staff       (20)      639 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_NR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      666 2018-06-29 07:26:49.000000 phonenumberslite-8.9.9/phonenumbers/data/region_NU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2373 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_NZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1220 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_OM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1561 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_PA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1894 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_PE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      964 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_PF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1158 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_PG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2440 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_PH.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3443 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_PK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2278 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_PL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      796 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_PM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1244 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_PR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1469 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_PS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1847 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_PT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      732 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_PW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2353 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_PY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1062 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_QA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1335 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_RE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1919 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_RO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2300 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_RS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2121 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_RU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1277 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_RW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1819 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1060 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SB.py
+-rw-r--r--   0 dmd        (501) staff       (20)      971 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      775 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SD.py
+-rw-r--r--   0 dmd        (501) staff       (20)     5794 2018-06-29 07:26:49.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1596 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      717 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SH.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1896 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1464 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2668 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      858 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SL.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1662 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1381 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SN.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1477 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1047 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      754 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      658 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_ST.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1172 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SV.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1233 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SX.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1195 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1270 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_SZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      425 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1402 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      748 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      735 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1570 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TH.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1583 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      590 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1162 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TL.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1247 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1103 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TN.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1057 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2448 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1509 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      569 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TV.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2303 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1755 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_TZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2242 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_UA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1657 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_UG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2859 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_US.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1439 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_UY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2430 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_UZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1604 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_VA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1309 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_VC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1162 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_VE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1310 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_VG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1412 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_VI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3319 2018-06-29 07:26:49.000000 phonenumberslite-8.9.9/phonenumbers/data/region_VN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      869 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_VU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      778 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_WF.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1030 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_WS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1347 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_XK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1088 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_YE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      833 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_YT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2008 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_ZA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1370 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_ZM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3290 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/data/region_ZW.py
+-rw-r--r--   0 dmd        (501) staff       (20)    10966 2018-05-17 08:38:10.000000 phonenumberslite-8.9.9/phonenumbers/geocoder.py
+-rw-r--r--   0 dmd        (501) staff       (20)    32671 2018-05-17 08:40:03.000000 phonenumberslite-8.9.9/phonenumbers/phonemetadata.py
+-rw-r--r--   0 dmd        (501) staff       (20)    12452 2018-05-17 08:40:03.000000 phonenumberslite-8.9.9/phonenumbers/phonenumber.py
+-rw-r--r--   0 dmd        (501) staff       (20)    38746 2018-05-17 08:40:03.000000 phonenumberslite-8.9.9/phonenumbers/phonenumbermatcher.py
+-rw-r--r--   0 dmd        (501) staff       (20)   155085 2018-05-17 08:40:03.000000 phonenumberslite-8.9.9/phonenumbers/phonenumberutil.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3650 2013-11-15 12:19:10.000000 phonenumberslite-8.9.9/phonenumbers/prefix.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1428 2018-05-17 08:38:26.000000 phonenumberslite-8.9.9/phonenumbers/re_util.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/
+-rw-r--r--   0 dmd        (501) staff       (20)     2180 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      558 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      696 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      807 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      791 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      773 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1137 2018-06-29 07:26:49.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      822 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1004 2018-06-29 07:26:49.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      676 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      737 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1360 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      788 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      578 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AX.py
+-rw-r--r--   0 dmd        (501) staff       (20)      826 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_AZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      786 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      565 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BB.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1089 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BD.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1212 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      717 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1146 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      966 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      822 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      541 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      777 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      684 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      788 2018-06-29 07:25:36.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BQ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1494 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      554 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      684 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      801 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      612 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      568 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_BZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1044 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      826 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      580 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      661 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1354 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      814 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1650 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      804 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      734 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      875 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      891 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      581 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CV.py
+-rw-r--r--   0 dmd        (501) staff       (20)      788 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CX.py
+-rw-r--r--   0 dmd        (501) staff       (20)      705 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      768 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_CZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      706 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_DE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_DJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      746 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_DK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_DM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_DO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      785 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_DZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      579 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_EC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2419 2018-06-29 07:26:49.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_EE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      824 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_EG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      572 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_EH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      678 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_ER.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1620 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_ES.py
+-rw-r--r--   0 dmd        (501) staff       (20)      588 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_ET.py
+-rw-r--r--   0 dmd        (501) staff       (20)      707 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_FI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      749 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_FJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_FK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      576 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_FM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      591 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_FO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1551 2018-06-29 07:26:49.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_FR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      588 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1338 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GB.py
+-rw-r--r--   0 dmd        (501) staff       (20)      773 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      844 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      636 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      856 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GH.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1286 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      566 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      676 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GP.py
+-rw-r--r--   0 dmd        (501) staff       (20)      719 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      829 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      860 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_GY.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1155 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_HK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      793 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_HN.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1134 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_HR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      799 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_HT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      727 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_HU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      831 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_ID.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1249 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_IE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      848 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_IL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      720 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_IM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1625 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_IN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      860 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_IQ.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1368 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_IR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1007 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_IS.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1220 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_IT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      658 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_JE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      796 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_JM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      860 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_JO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      554 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_JP.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1594 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_KE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      796 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_KG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      810 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_KH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      725 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_KI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_KM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_KN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_KP.py
+-rw-r--r--   0 dmd        (501) staff       (20)      929 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_KR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      686 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_KW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_KY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      841 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_KZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_LA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      579 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_LB.py
+-rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_LC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      602 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_LI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      560 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_LK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      837 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_LR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_LS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      760 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_LT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      712 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_LU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1143 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_LV.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_LY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      572 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      579 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      786 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      697 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_ME.py
+-rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      564 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MK.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1470 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_ML.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MP.py
+-rw-r--r--   0 dmd        (501) staff       (20)      574 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MQ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      705 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      594 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      726 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MV.py
+-rw-r--r--   0 dmd        (501) staff       (20)      810 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      761 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MX.py
+-rw-r--r--   0 dmd        (501) staff       (20)      952 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      594 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_MZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      599 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_NA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      904 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_NC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      813 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_NE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      568 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_NF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      793 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_NG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      739 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_NI.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1035 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_NL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      743 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_NO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_NP.py
+-rw-r--r--   0 dmd        (501) staff       (20)      566 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_NR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      676 2018-06-29 07:26:49.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_NU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      901 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_NZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      552 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_OM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_PA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      568 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_PE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_PF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      741 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_PG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      565 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_PH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      599 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_PK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      773 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_PL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      678 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_PM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_PR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      675 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_PS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      699 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_PT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_PW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      565 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_PY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      589 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_QA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      574 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_RE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1043 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_RO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      602 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_RS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      595 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_RU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_RW.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1045 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      650 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SB.py
+-rw-r--r--   0 dmd        (501) staff       (20)      638 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SD.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1316 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      748 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      582 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      711 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      747 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      808 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SM.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1279 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SO.py
+-rw-r--r--   0 dmd        (501) staff       (20)      561 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_ST.py
+-rw-r--r--   0 dmd        (501) staff       (20)      793 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SV.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SX.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_SZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_TC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      547 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_TD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      587 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_TG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1672 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_TH.py
+-rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_TJ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      581 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_TL.py
+-rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_TM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_TN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      574 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_TO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1767 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_TR.py
+-rw-r--r--   0 dmd        (501) staff       (20)      554 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_TT.py
+-rw-r--r--   0 dmd        (501) staff       (20)      559 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_TV.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_TW.py
+-rw-r--r--   0 dmd        (501) staff       (20)      808 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_TZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      956 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_UA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_UG.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1618 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_US.py
+-rw-r--r--   0 dmd        (501) staff       (20)      707 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_UY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      833 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_UZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      558 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_VA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_VC.py
+-rw-r--r--   0 dmd        (501) staff       (20)      573 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_VE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      562 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_VG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_VI.py
+-rw-r--r--   0 dmd        (501) staff       (20)      556 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_VN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      548 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_VU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      549 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_WF.py
+-rw-r--r--   0 dmd        (501) staff       (20)      710 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_WS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      570 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_XK.py
+-rw-r--r--   0 dmd        (501) staff       (20)      558 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_YE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      567 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_YT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1188 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_ZA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      575 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_ZM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      984 2018-06-29 07:26:49.000000 phonenumberslite-8.9.9/phonenumbers/shortdata/region_ZW.py
+-rw-r--r--   0 dmd        (501) staff       (20)    20748 2018-05-17 08:40:03.000000 phonenumberslite-8.9.9/phonenumbers/shortnumberinfo.py
+-rw-r--r--   0 dmd        (501) staff       (20)     4947 2018-05-17 08:38:10.000000 phonenumberslite-8.9.9/phonenumbers/timezone.py
+-rw-r--r--   0 dmd        (501) staff       (20)    18939 2013-11-15 12:19:10.000000 phonenumberslite-8.9.9/phonenumbers/unicode_util.py
+-rw-r--r--   0 dmd        (501) staff       (20)     5865 2016-01-29 10:59:27.000000 phonenumberslite-8.9.9/phonenumbers/util.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/phonenumberslite.egg-info/
+-rw-r--r--   0 dmd        (501) staff       (20)        1 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/phonenumberslite.egg-info/dependency_links.txt
+-rw-r--r--   0 dmd        (501) staff       (20)      928 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/phonenumberslite.egg-info/PKG-INFO
+-rw-r--r--   0 dmd        (501) staff       (20)    20341 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/phonenumberslite.egg-info/SOURCES.txt
+-rw-r--r--   0 dmd        (501) staff       (20)       13 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/phonenumberslite.egg-info/top_level.txt
+-rw-r--r--   0 dmd        (501) staff       (20)      928 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/PKG-INFO
+-rw-r--r--   0 dmd        (501) staff       (20)       67 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/setup.cfg
+-rwxr-xr-x   0 dmd        (501) staff       (20)     3319 2017-09-15 12:46:57.000000 phonenumberslite-8.9.9/setup.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/tests/
+-rw-r--r--   0 dmd        (501) staff       (20)      585 2013-10-11 17:19:49.000000 phonenumberslite-8.9.9/tests/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)    67545 2018-05-17 08:38:10.000000 phonenumberslite-8.9.9/tests/asyoutypetest.py
+-rw-r--r--   0 dmd        (501) staff       (20)     5419 2013-11-15 12:19:10.000000 phonenumberslite-8.9.9/tests/carriertest.py
+-rw-r--r--   0 dmd        (501) staff       (20)    18579 2018-05-17 08:40:03.000000 phonenumberslite-8.9.9/tests/examplenumberstest.py
+-rw-r--r--   0 dmd        (501) staff       (20)    11403 2018-05-17 08:40:03.000000 phonenumberslite-8.9.9/tests/geocodertest.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/tests/pb2/
+-rw-r--r--   0 dmd        (501) staff       (20)      127 2015-10-07 18:13:06.000000 phonenumberslite-8.9.9/tests/pb2/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2564 2018-05-19 06:37:56.000000 phonenumberslite-8.9.9/tests/pb2/converttest.py
+-rw-r--r--   0 dmd        (501) staff       (20)    49214 2018-05-17 08:40:03.000000 phonenumberslite-8.9.9/tests/phonenumbermatchertest.py
+-rwxr-xr-x   0 dmd        (501) staff       (20)     7615 2018-05-17 08:38:10.000000 phonenumberslite-8.9.9/tests/phonenumbertest.py
+-rwxr-xr-x   0 dmd        (501) staff       (20)   187153 2018-05-17 14:56:20.000000 phonenumberslite-8.9.9/tests/phonenumberutiltest.py
+-rw-r--r--   0 dmd        (501) staff       (20)    19975 2018-05-17 08:40:03.000000 phonenumberslite-8.9.9/tests/shortnumberinfotest.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/tests/testcarrierdata/
+-rw-r--r--   0 dmd        (501) staff       (20)      847 2018-06-29 07:25:43.000000 phonenumberslite-8.9.9/tests/testcarrierdata/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1056 2018-06-29 07:25:43.000000 phonenumberslite-8.9.9/tests/testcarrierdata/data0.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/tests/testdata/
+-rw-r--r--   0 dmd        (501) staff       (20)     2186 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)      520 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_800.py
+-rw-r--r--   0 dmd        (501) staff       (20)      527 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_882.py
+-rw-r--r--   0 dmd        (501) staff       (20)      533 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_979.py
+-rw-r--r--   0 dmd        (501) staff       (20)      436 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_AD.py
+-rw-r--r--   0 dmd        (501) staff       (20)      440 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_AE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      731 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_AM.py
+-rw-r--r--   0 dmd        (501) staff       (20)      746 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_AO.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2450 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_AR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1247 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_AU.py
+-rw-r--r--   0 dmd        (501) staff       (20)      420 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_BB.py
+-rw-r--r--   0 dmd        (501) staff       (20)      511 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_BR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1072 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_BS.py
+-rw-r--r--   0 dmd        (501) staff       (20)      945 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_BY.py
+-rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_CA.py
+-rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_CC.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1083 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_CN.py
+-rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_CX.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2079 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_DE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      671 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_FR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2140 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_GB.py
+-rw-r--r--   0 dmd        (501) staff       (20)      513 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_GG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      502 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_HU.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1308 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_IT.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1990 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_JP.py
+-rw-r--r--   0 dmd        (501) staff       (20)     3617 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_KR.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2808 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_MX.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1503 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_NZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      909 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_PL.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1091 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_RE.py
+-rw-r--r--   0 dmd        (501) staff       (20)      382 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_SE.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1221 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_SG.py
+-rw-r--r--   0 dmd        (501) staff       (20)      668 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_TA.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1640 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_US.py
+-rw-r--r--   0 dmd        (501) staff       (20)      921 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_UZ.py
+-rw-r--r--   0 dmd        (501) staff       (20)      777 2018-06-29 07:25:37.000000 phonenumberslite-8.9.9/tests/testdata/region_YT.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/tests/testgeodata/
+-rw-r--r--   0 dmd        (501) staff       (20)      847 2018-06-29 07:25:43.000000 phonenumberslite-8.9.9/tests/testgeodata/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1881 2018-06-29 07:25:43.000000 phonenumberslite-8.9.9/tests/testgeodata/data0.py
+-rw-r--r--   0 dmd        (501) staff       (20)     2317 2017-07-24 12:06:48.000000 phonenumberslite-8.9.9/tests/testmetadatatest.py
+drwxr-xr-x   0 dmd        (501) staff       (20)        0 2018-06-29 07:34:43.000000 phonenumberslite-8.9.9/tests/testtzdata/
+-rw-r--r--   0 dmd        (501) staff       (20)      835 2018-06-29 07:25:44.000000 phonenumberslite-8.9.9/tests/testtzdata/__init__.py
+-rw-r--r--   0 dmd        (501) staff       (20)     1112 2018-06-29 07:25:44.000000 phonenumberslite-8.9.9/tests/testtzdata/data0.py
+-rw-r--r--   0 dmd        (501) staff       (20)     5914 2013-11-15 12:19:10.000000 phonenumberslite-8.9.9/tests/timezonetest.py
```

### Comparing `phonenumberslite-8.9.8/phonenumbers/__init__.py` & `phonenumberslite-8.9.9/phonenumbers/__init__.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/asyoutypeformatter.py` & `phonenumberslite-8.9.9/phonenumbers/asyoutypeformatter.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/carrier.py` & `phonenumberslite-8.9.9/phonenumbers/carrier.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/__init__.py` & `phonenumberslite-8.9.9/phonenumbers/data/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/alt_format_372.py` & `phonenumberslite-8.9.9/phonenumbers/data/alt_format_372.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/alt_format_381.py` & `phonenumberslite-8.9.9/phonenumbers/data/alt_format_381.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/alt_format_385.py` & `phonenumberslite-8.9.9/phonenumbers/data/alt_format_385.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/alt_format_43.py` & `phonenumberslite-8.9.9/phonenumbers/data/alt_format_43.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/alt_format_44.py` & `phonenumberslite-8.9.9/phonenumbers/data/alt_format_44.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/alt_format_49.py` & `phonenumberslite-8.9.9/phonenumbers/data/alt_format_49.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/alt_format_61.py` & `phonenumberslite-8.9.9/phonenumbers/data/alt_format_61.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/alt_format_62.py` & `phonenumberslite-8.9.9/phonenumbers/data/alt_format_62.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/alt_format_7.py` & `phonenumberslite-8.9.9/phonenumbers/data/alt_format_7.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/alt_format_91.py` & `phonenumberslite-8.9.9/phonenumbers/data/alt_format_91.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_870.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_870.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_878.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_878.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_881.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_881.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_882.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_882.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_883.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_883.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_888.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_888.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_979.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_979.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AC.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AD.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AD.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AE.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AF.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AG.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AI.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AL.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AO.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AR.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AS.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AT.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AU.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AW.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AX.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AX.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_AZ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_AZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BA.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BB.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BB.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BD.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BD.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BE.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BF.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BG.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BH.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BI.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BJ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BJ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BL.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BN.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BO.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BQ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BQ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BR.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BS.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BT.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BW.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BY.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_BZ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_BZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CA.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CC.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CD.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CD.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CF.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CG.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CH.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CI.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CK.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CL.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CN.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CO.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CR.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CU.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CV.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CV.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CW.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CX.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CX.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CY.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_CZ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_CZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_DE.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_DE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_DJ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_DJ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_DK.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_DK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_DM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_DM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_DO.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_DO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_DZ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_DZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_EC.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_EC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_EE.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_EE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_EG.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_EG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_EH.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_EH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_ER.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_ER.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_ES.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_ES.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_ET.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_ET.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_FI.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_FI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_FJ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_FJ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_FK.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_FK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_FM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_FM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_FO.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_FO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_FR.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_FR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GA.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GB.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GB.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GD.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GD.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GE.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GF.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GG.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GH.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GI.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GL.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GN.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GP.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GP.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GQ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GQ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GR.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GT.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GU.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GW.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_GY.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_GY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_HK.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_HK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_HN.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_HN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_HR.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_HR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_HT.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_HT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_HU.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_HU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_ID.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_ID.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_IE.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_IE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_IL.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_IL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_IM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_IM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_IN.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_IN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_IO.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_IO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_IQ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_IQ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_IR.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_IR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_IS.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_IS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_IT.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_IT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_JE.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_JE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_JM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_JM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_JO.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_JO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_JP.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_JP.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_KE.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_KE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_KG.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_KG.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_KH.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_KH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_KI.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_KI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_KM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_KM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_KN.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_KN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_KP.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_KP.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_KR.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_KR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_KW.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_KW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_KY.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_KY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_KZ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_KZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_LA.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_LA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_LB.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_LB.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_LC.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_LC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_LI.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_LI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_LK.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_LK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_LR.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_LR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_LS.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_LS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_LT.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_LT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_LU.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_LU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_LV.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_LV.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_LY.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_LY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MA.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MC.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MD.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MD.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_ME.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_ME.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MF.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MG.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MH.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MK.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_ML.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_ML.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MN.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MO.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MP.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MP.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MQ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MQ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MR.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MS.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MT.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MU.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MV.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MV.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MW.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MX.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MX.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MY.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_MZ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_MZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_NA.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_NA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_NC.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_NC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_NE.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_NE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_NF.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_NF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_NG.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_NG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_NI.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_NI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_NL.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_NL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_NO.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_NO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_NP.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_NP.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_NR.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_NR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_NU.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_PW.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_NZ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_NZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_OM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_OM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_PA.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_PA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_PE.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_PE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_PF.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_PF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_PG.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_PG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_PH.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_PH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_PK.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_PK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_PL.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_PL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_PM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_PM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_PR.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_PR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_PS.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_PS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_PT.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_PT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_PW.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_PA.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_PY.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_PY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_QA.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_QA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_RE.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_RE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_RO.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_RO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_RS.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_RS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_RU.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_RU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_RW.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_RW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SA.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SB.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SB.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SC.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SD.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SD.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SE.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SE.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SG.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SH.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SI.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SJ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SJ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SK.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SL.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SN.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SO.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SR.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SS.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_ST.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_ST.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SV.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SV.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SX.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SX.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SY.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_SZ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_SZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_TC.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_TC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_TD.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_TD.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_TG.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_TG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_TH.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_TH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_TJ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_TJ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_TK.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_TK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_TL.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_TL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_TM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_TM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_TN.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_TN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_TO.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_TO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_TR.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_TR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_TT.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_TT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_TV.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_TV.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_TW.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_TW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_TZ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_TZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_UA.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_UA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_UG.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_UG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_US.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_US.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_UY.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_UY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_UZ.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_UZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_VA.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_VA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_VC.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_VC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_VE.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_VE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_VG.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_VG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_VI.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_VI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_VN.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_VN.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_VU.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_VU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_WF.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_WF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_WS.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_WS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_XK.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_XK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_YE.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_YE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_YT.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_YT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_ZA.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_ZA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_ZM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_ZM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/data/region_ZW.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_ZW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/geocoder.py` & `phonenumberslite-8.9.9/phonenumbers/geocoder.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/phonemetadata.py` & `phonenumberslite-8.9.9/phonenumbers/phonemetadata.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/phonenumber.py` & `phonenumberslite-8.9.9/phonenumbers/phonenumber.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/phonenumbermatcher.py` & `phonenumberslite-8.9.9/phonenumbers/phonenumbermatcher.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/phonenumberutil.py` & `phonenumberslite-8.9.9/phonenumbers/phonenumberutil.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/prefix.py` & `phonenumberslite-8.9.9/phonenumbers/prefix.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/re_util.py` & `phonenumberslite-8.9.9/phonenumbers/re_util.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/__init__.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AC.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AD.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AD.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AE.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AF.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AG.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AI.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AL.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CH.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AM.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AO.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AR.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AR.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AS.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AT.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AU.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AW.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AX.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AX.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_AZ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BA.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BB.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BB.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BD.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BD.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BE.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BF.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BG.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BH.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BI.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BJ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BJ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BL.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BM.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BN.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BO.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BQ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BQ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BR.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BS.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BT.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BW.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BY.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_BZ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_BZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CA.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CC.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CD.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CD.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CF.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CG.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CH.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_IS.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CI.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CK.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CL.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CM.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CN.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CO.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CR.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CU.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CV.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CV.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CW.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CX.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CX.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CY.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_CZ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_CZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_DE.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_DE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_DJ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_DJ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_DK.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_DK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_DM.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_DM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_DO.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_DO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_DZ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_DZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_EC.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_EC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_EE.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_EE.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_EG.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_EG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_EH.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_EH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_ER.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_ER.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_ES.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_ES.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_ET.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_ET.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_FI.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_FI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_FJ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_FJ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_FK.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_FK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_FM.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_FM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_FO.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_FO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_FR.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_FR.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GA.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GB.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GB.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GD.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GD.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GE.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GF.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GG.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GH.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GI.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GL.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GM.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GN.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GP.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GP.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GR.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GT.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GU.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GW.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_GY.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_GY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_HK.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_HK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_HN.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_HN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_HR.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_HR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_HT.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_HT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_HU.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_HU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_ID.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_ID.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_IE.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_IE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_IL.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_IL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_IM.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_IM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_IN.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_IN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_IQ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_IQ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_IR.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_IR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_IS.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_LV.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_IT.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_IT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_JE.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_JE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_JM.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_JM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_JO.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_JO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_JP.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_JP.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_KE.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_KE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_KG.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_KG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_KH.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_KH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_KI.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_KI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_KM.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_KM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_KN.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_KN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_KP.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_KP.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_KR.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_KR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_KW.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_KW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_KY.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_KY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_KZ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_KZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_LA.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_LA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_LB.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_LB.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_LC.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_LC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_LI.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_LI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_LK.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_LK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_LR.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_LR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_LS.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_LS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_LT.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_LT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_LU.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_LU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_LV.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_ZA.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_LY.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_LY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MA.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MC.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MD.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MD.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_ME.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_ME.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MF.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MG.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MH.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MK.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_ML.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_ML.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MM.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MN.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MO.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MP.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MP.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MQ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MQ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MR.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MS.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MT.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MU.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MV.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MV.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MW.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MX.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MX.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MY.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_MZ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_MZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_NA.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_NA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_NC.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_NC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_NE.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_NE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_NF.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_NF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_NG.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_NG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_NI.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_NI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_NL.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_NL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_NO.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_NO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_NP.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_NP.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_NR.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_NR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_NU.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SZ.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_NZ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_NZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_OM.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_OM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_PA.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_PH.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_PE.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_PE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_PF.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_PF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_PG.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_PG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_PH.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_VU.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_PK.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_PK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_PL.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_PL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_PM.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_PM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_PR.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_PR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_PS.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_PS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_PT.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_PT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_PW.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_PW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_PY.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_PY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_QA.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_QA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_RE.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_RE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_RO.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_RO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_RS.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_RS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_RU.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_RU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_RW.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_RW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SA.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SB.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SB.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SC.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SD.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SD.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SE.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SG.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SH.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SI.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SI.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SJ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SJ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SK.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SL.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SM.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SN.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SO.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SR.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_ST.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_ST.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SV.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SV.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SX.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SX.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SY.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_SY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_SZ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_UG.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_TC.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_TC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_TD.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_TD.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_TG.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_TG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_TH.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_TH.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_TJ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_TJ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_TL.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_TL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_TM.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_TM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_TN.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_TN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_TO.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_TO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_TR.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_TR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_TT.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_TT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_TV.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_TV.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_TW.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_TW.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_TZ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_TZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_UA.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_UA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_UG.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_VI.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_US.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_US.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_UY.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_UY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_UZ.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_UZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_VA.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_VA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_VC.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_VC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_VE.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_VE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_VG.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_VG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_VI.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_YE.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_VN.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_VN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_VU.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_NU.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_WF.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_WF.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_WS.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_WS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_XK.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_XK.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_YE.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_ZM.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_YT.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_YT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_ZA.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_AL.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_ZM.py` & `phonenumberslite-8.9.9/phonenumbers/data/region_NU.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortdata/region_ZW.py` & `phonenumberslite-8.9.9/phonenumbers/shortdata/region_ZW.py`

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

### Comparing `phonenumberslite-8.9.8/phonenumbers/shortnumberinfo.py` & `phonenumberslite-8.9.9/phonenumbers/shortnumberinfo.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/timezone.py` & `phonenumberslite-8.9.9/phonenumbers/timezone.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/unicode_util.py` & `phonenumberslite-8.9.9/phonenumbers/unicode_util.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumbers/util.py` & `phonenumberslite-8.9.9/phonenumbers/util.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/phonenumberslite.egg-info/PKG-INFO` & `phonenumberslite-8.9.9/phonenumberslite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: phonenumberslite
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

### Comparing `phonenumberslite-8.9.8/phonenumberslite.egg-info/SOURCES.txt` & `phonenumberslite-8.9.9/phonenumberslite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/PKG-INFO` & `phonenumberslite-8.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: phonenumberslite
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

### Comparing `phonenumberslite-8.9.8/setup.py` & `phonenumberslite-8.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/__init__.py` & `phonenumberslite-8.9.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/asyoutypetest.py` & `phonenumberslite-8.9.9/tests/asyoutypetest.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/carriertest.py` & `phonenumberslite-8.9.9/tests/carriertest.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/examplenumberstest.py` & `phonenumberslite-8.9.9/tests/examplenumberstest.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/geocodertest.py` & `phonenumberslite-8.9.9/tests/geocodertest.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/pb2/converttest.py` & `phonenumberslite-8.9.9/tests/pb2/converttest.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/phonenumbermatchertest.py` & `phonenumberslite-8.9.9/tests/phonenumbermatchertest.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/phonenumbertest.py` & `phonenumberslite-8.9.9/tests/phonenumbertest.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/phonenumberutiltest.py` & `phonenumberslite-8.9.9/tests/phonenumberutiltest.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/shortnumberinfotest.py` & `phonenumberslite-8.9.9/tests/shortnumberinfotest.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testcarrierdata/__init__.py` & `phonenumberslite-8.9.9/tests/testcarrierdata/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testcarrierdata/data0.py` & `phonenumberslite-8.9.9/tests/testcarrierdata/data0.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/__init__.py` & `phonenumberslite-8.9.9/tests/testdata/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_800.py` & `phonenumberslite-8.9.9/tests/testdata/region_800.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_882.py` & `phonenumberslite-8.9.9/tests/testdata/region_882.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_979.py` & `phonenumberslite-8.9.9/tests/testdata/region_979.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_AM.py` & `phonenumberslite-8.9.9/tests/testdata/region_AM.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_AO.py` & `phonenumberslite-8.9.9/tests/testdata/region_AO.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_AR.py` & `phonenumberslite-8.9.9/tests/testdata/region_AR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_AU.py` & `phonenumberslite-8.9.9/tests/testdata/region_AU.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_BS.py` & `phonenumberslite-8.9.9/tests/testdata/region_BS.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_BY.py` & `phonenumberslite-8.9.9/tests/testdata/region_BY.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_CA.py` & `phonenumberslite-8.9.9/tests/testdata/region_CA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_CC.py` & `phonenumberslite-8.9.9/tests/testdata/region_CC.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_CN.py` & `phonenumberslite-8.9.9/tests/testdata/region_CN.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_CX.py` & `phonenumberslite-8.9.9/tests/testdata/region_CX.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_DE.py` & `phonenumberslite-8.9.9/tests/testdata/region_DE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_FR.py` & `phonenumberslite-8.9.9/tests/testdata/region_FR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_GB.py` & `phonenumberslite-8.9.9/tests/testdata/region_GB.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_GG.py` & `phonenumberslite-8.9.9/tests/testdata/region_GG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_IT.py` & `phonenumberslite-8.9.9/tests/testdata/region_IT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_JP.py` & `phonenumberslite-8.9.9/tests/testdata/region_JP.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_KR.py` & `phonenumberslite-8.9.9/tests/testdata/region_KR.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_MX.py` & `phonenumberslite-8.9.9/tests/testdata/region_MX.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_NZ.py` & `phonenumberslite-8.9.9/tests/testdata/region_NZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_PL.py` & `phonenumberslite-8.9.9/tests/testdata/region_PL.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_RE.py` & `phonenumberslite-8.9.9/tests/testdata/region_RE.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_SG.py` & `phonenumberslite-8.9.9/tests/testdata/region_SG.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_TA.py` & `phonenumberslite-8.9.9/tests/testdata/region_TA.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_US.py` & `phonenumberslite-8.9.9/tests/testdata/region_US.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_UZ.py` & `phonenumberslite-8.9.9/tests/testdata/region_UZ.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testdata/region_YT.py` & `phonenumberslite-8.9.9/tests/testdata/region_YT.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testgeodata/__init__.py` & `phonenumberslite-8.9.9/tests/testgeodata/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testgeodata/data0.py` & `phonenumberslite-8.9.9/tests/testgeodata/data0.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testmetadatatest.py` & `phonenumberslite-8.9.9/tests/testmetadatatest.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testtzdata/__init__.py` & `phonenumberslite-8.9.9/tests/testtzdata/__init__.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/testtzdata/data0.py` & `phonenumberslite-8.9.9/tests/testtzdata/data0.py`

 * *Files identical despite different names*

### Comparing `phonenumberslite-8.9.8/tests/timezonetest.py` & `phonenumberslite-8.9.9/tests/timezonetest.py`

 * *Files identical despite different names*

