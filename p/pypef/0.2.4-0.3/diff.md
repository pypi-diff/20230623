# Comparing `tmp/pypef-0.2.4.tar.gz` & `tmp/pypef-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypef-0.2.4.tar", last modified: Mon May  8 14:22:13 2023, max compression
+gzip compressed data, was "pypef-0.3.tar", last modified: Fri Jun 23 08:52:35 2023, max compression
```

## Comparing `pypef-0.2.4.tar` & `pypef-0.3.tar`

### file list

```diff
@@ -1,637 +1,641 @@
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:13.573596 pypef-0.2.4/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    20254 2022-07-09 09:31:17.000000 pypef-0.2.4/LICENSE.md
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)       72 2022-07-09 09:31:17.000000 pypef-0.2.4/MANIFEST.in
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1287 2023-05-08 14:22:13.572097 pypef-0.2.4/PKG-INFO
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    24749 2023-01-22 13:21:24.000000 pypef-0.2.4/README.md
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:04.241560 pypef-0.2.4/pypef/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1004 2023-05-08 13:28:24.000000 pypef-0.2.4/pypef/__init__.py
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:04.350055 pypef-0.2.4/pypef/dca/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2020-12-13 17:44:24.000000 pypef-0.2.4/pypef/dca/__init__.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    29920 2023-05-07 14:00:14.000000 pypef-0.2.4/pypef/dca/encoding.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    41769 2023-05-08 13:38:48.000000 pypef-0.2.4/pypef/dca/hybrid_model.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     5289 2023-05-05 17:45:20.000000 pypef-0.2.4/pypef/dca/run.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    21434 2023-05-08 13:27:58.000000 pypef-0.2.4/pypef/main.py
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:04.399057 pypef-0.2.4/pypef/ml/
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:12.755968 pypef-0.2.4/pypef/ml/AAindex/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      594 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ANDN920101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      917 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ARGP820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      540 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ARGP820102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      674 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ARGP820103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      451 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      489 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      469 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      469 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      836 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1161 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      771 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      664 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      945 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      794 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1054 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      794 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980115.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980116.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      511 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980117.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980118.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      470 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980119.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      451 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980120.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1030 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      818 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      640 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      704 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      639 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      620 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      620 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      512 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1186 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BAEK050101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2418 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BASU050101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2485 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BASU050102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2873 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BASU050103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      846 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BEGF750101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      891 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BEGF750102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      649 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BEGF750103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BHAR880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1002 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BIGC670101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2753 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BIOV880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2581 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BIOV880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      949 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BLAM930101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1880 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BLAS910101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      790 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BROC820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      640 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BROC820102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1419 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BULH740101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BULH740102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      811 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BUNA790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      543 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BUNA790102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BUNA790103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      938 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BURA740101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BURA740102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2179 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CASG920101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      977 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CEDJ970101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1016 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CEDJ970102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      993 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CEDJ970103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1021 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CEDJ970104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      755 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CEDJ970105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1069 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM820102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1425 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      597 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      546 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      697 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      968 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      518 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      524 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      978 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOC750101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1042 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOC760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1264 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOC760102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1659 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOC760103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      913 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOC760104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1066 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1273 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780201.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1425 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780202.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1011 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780203.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780204.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      542 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780205.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780206.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780207.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      656 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780208.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      612 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780209.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      963 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780210.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      531 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780211.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780212.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      733 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780213.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      538 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780214.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780215.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1099 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780216.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1520 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CIDH920101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1844 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CIDH920102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2110 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CIDH920103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2479 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CIDH920104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2440 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CIDH920105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      439 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/COHE430101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2467 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1882 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1968 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1838 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1882 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2012 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2228 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2119 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      585 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/COSI940101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1140 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/COWR900101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      963 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CRAJ730101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      659 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CRAJ730102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      825 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CRAJ730103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      780 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/DAWD720101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1038 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/DAYM780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      605 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/DAYM780201.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1472 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/DESM900101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2134 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/DESM900102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/DIGM050101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1899 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/EISD840101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1471 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/EISD860101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      590 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/EISD860102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1824 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/EISD860103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1497 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ENGD860101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FASG760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      444 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FASG760102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      447 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FASG760103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      435 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FASG760104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      454 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FASG760105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2291 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FASG890101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2454 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ830101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      642 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1053 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1328 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      931 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      766 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1169 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      767 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      657 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1142 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      865 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      721 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      778 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FINA770101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      843 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FINA910101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1071 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FINA910102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      827 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FINA910103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      802 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FINA910104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      537 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FODM020101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      628 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      995 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1276 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1256 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      759 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      823 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      807 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1000 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      826 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      936 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      610 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GARJ730101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      902 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      531 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      490 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      882 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      923 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      681 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1165 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1030 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      529 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      962 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1098 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      592 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      623 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      641 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      754 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1017 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GOLD730101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1054 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GOLD730102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      499 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GRAR740101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2266 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GRAR740102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      941 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GRAR740103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1884 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GUOD860101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2253 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GUYH850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1976 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GUYH850102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1867 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GUYH850103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1686 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GUYH850104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1275 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GUYH850105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1005 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/HARY940101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      538 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/HOPA770101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1453 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/HOPT810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/HUTJ700101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      772 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/HUTJ700102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      646 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/HUTJ700103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1307 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      706 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1017 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      889 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      629 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      590 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      573 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1171 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JACR890101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1346 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JANJ780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1885 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JANJ780102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1582 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JANJ780103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1240 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JANJ790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1625 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JANJ790102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      897 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JOND750101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      686 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JOND750102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      964 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JOND920101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      496 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JOND920102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      887 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JUKT750101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      842 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JUNJ780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2297 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JURD980101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1090 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KANM800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1397 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KANM800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1356 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KANM800103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1078 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KANM800104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      972 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARP850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1731 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARP850102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      457 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARP850103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      536 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      532 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      591 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      526 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      528 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      573 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      564 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      564 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      559 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      563 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      547 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      565 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160115.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      567 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160116.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      622 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160117.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160118.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160119.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160120.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160121.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160122.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      458 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KHAG800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1837 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KIDA850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      611 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KIMC930101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      527 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KLEP840101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KOEP990101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      511 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KOEP990102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1073 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KRIW710101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2101 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KRIW790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1518 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KRIW790102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1016 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KRIW790103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1615 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KUHL950101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      808 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KUMS000101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      871 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KUMS000102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      557 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KUMS000103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KUMS000104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2155 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KYTJ820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      626 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LAWE840101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1272 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1019 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM760102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      577 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM760103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM760104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1035 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM760105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1124 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM760106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      999 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM760107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      919 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      811 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM780102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1073 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM780103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      917 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM780104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      916 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM780105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1092 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM780106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      525 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEWP710101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1861 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LIFS790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      761 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LIFS790102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1004 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LIFS790103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2391 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MANP780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1301 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MAXF760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      723 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MAXF760102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MAXF760103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      772 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MAXF760104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      690 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MAXF760105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      631 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MAXF760106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      764 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MCMT640101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      674 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MEEJ800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1236 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MEEJ800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1625 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MEEJ810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1431 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MEEJ810102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2320 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MEIH800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2423 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MEIH800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2265 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MEIH800103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      548 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MITS020101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2621 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MIYS850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2635 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MIYS990101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2617 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MIYS990102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2726 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MIYS990103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2703 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MIYS990104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2552 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MIYS990105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      839 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MONM990101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      629 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MONM990201.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1157 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MUNV940101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1128 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MUNV940102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1631 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MUNV940103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      889 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MUNV940104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      845 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MUNV940105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2035 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NADH010101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2467 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NADH010102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2556 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NADH010103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2296 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NADH010104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1688 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NADH010105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      822 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NADH010106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NADH010107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      888 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAGK730101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      782 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAGK730102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      925 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAGK730103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      989 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      756 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      682 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      581 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      673 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      578 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      682 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      545 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      862 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      779 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      668 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      524 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      894 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      660 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      829 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      834 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      829 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      935 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2079 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NISK800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2601 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NISK860101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1331 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NOZY710101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1313 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OLSK800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      880 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ONEK900101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      927 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ONEK900102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1871 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM770101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      672 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM770102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2350 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM770103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM770104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM770105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      588 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM850102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      542 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM850103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM850104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM850105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      973 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1298 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1060 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1362 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      966 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1184 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      638 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      599 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      878 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      875 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      598 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      898 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      621 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      632 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810115.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      632 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810116.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2385 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PARJ860101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1697 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PARS000101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      724 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PARS000102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2257 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PLIV810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1028 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONJ960101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2346 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2238 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2244 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      550 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      909 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1315 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2169 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2388 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP930101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      535 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PRAM820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      579 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PRAM820102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PRAM820103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1575 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PRAM900101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1115 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PRAM900102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PRAM900103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1269 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PRAM900104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1271 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PTIO830101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1637 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PTIO830102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2481 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PUNT030101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2221 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PUNT030102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      584 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      844 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1127 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1363 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      952 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      996 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      778 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      671 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880115.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880116.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      522 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880117.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880118.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1277 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880119.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1622 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880120.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1450 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880121.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      712 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880122.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880123.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880124.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880125.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      540 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880126.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      535 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880127.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880128.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880129.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880130.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      881 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880131.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1185 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880132.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1205 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880133.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1184 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880134.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1039 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880135.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      641 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880136.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880137.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880138.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880139.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1980 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS770101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2148 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS770102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1487 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS770103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1155 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      591 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      635 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      612 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      647 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1630 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1357 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1089 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1097 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      728 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      967 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1245 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2735 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      504 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      628 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      585 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      630 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880115.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880116.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880117.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1109 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      508 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1261 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      854 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1192 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1327 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      496 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      668 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      488 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      654 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      507 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      582 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      712 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1940 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1107 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROSG850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2469 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROSG850102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1630 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROSM880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1823 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROSM880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      506 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROSM880103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1197 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROSM880104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2001 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROSM880105.txt
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:13.464594 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_12_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_0_4.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_1_3.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_2_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_14_0_3.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_14_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_15_0_3.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_16_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_17_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_17_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_0_3.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_2_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_3_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_1_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_2_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_3_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_4_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_4_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_5_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_2_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_3_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_4_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_8_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_0_7.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_1_4.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_2_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_3_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1015 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SIMZ760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      456 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SNEP660101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      476 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SNEP660102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SNEP660103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      457 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SNEP660104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1158 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SUEM840101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      684 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SUEM840102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      494 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SUYM030101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1839 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SWER830101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1093 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TAKK010101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1097 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      605 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      758 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      821 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      647 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      607 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      669 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      597 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      656 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1100 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1036 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TSAJ990101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1040 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TSAJ990102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VASM830101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VASM830102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      578 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VASM830103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      565 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VELV850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1083 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VENT840101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      974 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VHEG790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2392 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VINM940101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2006 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VINM940102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1701 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VINM940103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      705 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VINM940104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1118 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WARP780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      679 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WEBA780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2230 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WERD780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      626 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WERD780102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      631 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WERD780103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      624 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WERD780104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      834 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WILM950101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      659 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WILM950102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      619 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WILM950103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WILM950104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      856 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WIMW960101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1497 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WOEC730101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1070 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WOLR790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1105 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WOLR810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2072 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WOLS870101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      749 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WOLS870102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      623 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WOLS870103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      607 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/YANJ020101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      771 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/YUTK870101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      685 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/YUTK870102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      711 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/YUTK870103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      711 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/YUTK870104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      758 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZASB820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1677 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZHOH040101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1180 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZHOH040102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2314 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZHOH040103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZIMJ680101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      642 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZIMJ680102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZIMJ680103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      562 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZIMJ680104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZIMJ680105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2020-12-13 17:44:24.000000 pypef-0.2.4/pypef/ml/__init__.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     5068 2022-07-02 13:59:04.000000 pypef-0.2.4/pypef/ml/parallelization.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    57666 2023-05-05 21:32:40.000000 pypef-0.2.4/pypef/ml/regression.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    10200 2023-05-05 18:28:24.000000 pypef-0.2.4/pypef/ml/run.py
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:13.561594 pypef-0.2.4/pypef/utils/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2020-12-13 17:44:24.000000 pypef-0.2.4/pypef/utils/__init__.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    16275 2023-05-05 17:16:29.000000 pypef-0.2.4/pypef/utils/directed_evolution.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    18749 2023-05-08 09:38:22.000000 pypef-0.2.4/pypef/utils/learning_test_sets.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    19505 2023-05-07 16:51:51.000000 pypef-0.2.4/pypef/utils/low_n_mutation_extrapolation.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    18168 2023-05-07 09:07:01.000000 pypef-0.2.4/pypef/utils/prediction_sets.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    17404 2023-05-08 10:45:26.000000 pypef-0.2.4/pypef/utils/run.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     4142 2023-05-05 17:20:37.000000 pypef-0.2.4/pypef/utils/sto2a2m.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    12585 2023-05-08 13:38:48.000000 pypef-0.2.4/pypef/utils/variant_data.py
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:04.301058 pypef-0.2.4/pypef.egg-info/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1287 2023-05-08 14:22:01.000000 pypef-0.2.4/pypef.egg-info/PKG-INFO
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    21140 2023-05-08 14:22:04.000000 pypef-0.2.4/pypef.egg-info/SOURCES.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)        1 2023-05-08 14:22:01.000000 pypef-0.2.4/pypef.egg-info/dependency_links.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)       46 2023-05-08 14:22:01.000000 pypef-0.2.4/pypef.egg-info/entry_points.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)       96 2023-05-08 14:22:01.000000 pypef-0.2.4/pypef.egg-info/requires.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)        6 2023-05-08 14:22:01.000000 pypef-0.2.4/pypef.egg-info/top_level.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      105 2022-07-01 13:45:38.000000 pypef-0.2.4/requirements.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)       38 2023-05-08 14:22:13.574097 pypef-0.2.4/setup.cfg
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2129 2023-05-08 10:04:52.000000 pypef-0.2.4/setup.py
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:35.204268 pypef-0.3/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    20254 2022-07-09 09:31:17.000000 pypef-0.3/LICENSE.md
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)       72 2022-07-09 09:31:17.000000 pypef-0.3/MANIFEST.in
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1285 2023-06-23 08:52:35.200769 pypef-0.3/PKG-INFO
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    28270 2023-06-21 09:33:59.000000 pypef-0.3/README.md
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:06.293491 pypef-0.3/pypef/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1002 2023-06-22 13:24:04.000000 pypef-0.3/pypef/__init__.py
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:06.645495 pypef-0.3/pypef/dca/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2020-12-13 17:44:24.000000 pypef-0.3/pypef/dca/__init__.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     5949 2023-06-21 12:24:22.000000 pypef-0.3/pypef/dca/dca_run.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    26612 2023-06-22 08:00:42.000000 pypef-0.3/pypef/dca/gremlin_inference.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    46823 2023-06-18 11:12:50.000000 pypef-0.3/pypef/dca/hybrid_model.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    31392 2023-06-15 16:19:10.000000 pypef-0.3/pypef/dca/plmc_encoding.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    23529 2023-06-13 19:31:08.000000 pypef-0.3/pypef/main.py
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:06.801492 pypef-0.3/pypef/ml/
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:33.124768 pypef-0.3/pypef/ml/AAindex/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      594 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ANDN920101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      917 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ARGP820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      540 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ARGP820102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      674 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ARGP820103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      451 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      489 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      469 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      469 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      836 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1161 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      771 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      664 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      945 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      794 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1054 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      794 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980115.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980116.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      511 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980117.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980118.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      470 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980119.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      451 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AURR980120.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1030 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      818 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      640 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      704 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      639 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      620 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      620 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      512 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/AVBF000109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1186 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BAEK050101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2418 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BASU050101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2485 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BASU050102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2873 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BASU050103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      846 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BEGF750101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      891 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BEGF750102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      649 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BEGF750103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BHAR880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1002 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BIGC670101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2753 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BIOV880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2581 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BIOV880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      949 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BLAM930101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1880 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BLAS910101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      790 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BROC820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      640 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BROC820102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1419 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BULH740101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BULH740102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      811 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BUNA790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      543 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BUNA790102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BUNA790103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      938 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BURA740101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/BURA740102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2179 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CASG920101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      977 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CEDJ970101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1016 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CEDJ970102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      993 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CEDJ970103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1021 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CEDJ970104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      755 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CEDJ970105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1069 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM820102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1425 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      597 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      546 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      697 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      968 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      518 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      524 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHAM830108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      978 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOC750101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1042 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOC760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1264 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOC760102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1659 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOC760103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      913 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOC760104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1066 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1273 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780201.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1425 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780202.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1011 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780203.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780204.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      542 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780205.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780206.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780207.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      656 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780208.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      612 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780209.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      963 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780210.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      531 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780211.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780212.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      733 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780213.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      538 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780214.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780215.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1099 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CHOP780216.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1520 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CIDH920101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1844 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CIDH920102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2110 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CIDH920103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2479 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CIDH920104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2440 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CIDH920105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      439 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/COHE430101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2467 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1882 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1968 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1838 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1882 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2012 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2228 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2119 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CORJ870108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      585 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/COSI940101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1140 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/COWR900101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      963 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CRAJ730101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      659 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CRAJ730102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      825 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/CRAJ730103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      780 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/DAWD720101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1038 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/DAYM780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      605 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/DAYM780201.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1472 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/DESM900101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2134 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/DESM900102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/DIGM050101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1899 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/EISD840101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1471 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/EISD860101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      590 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/EISD860102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1824 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/EISD860103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1497 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ENGD860101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FASG760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      444 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FASG760102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      447 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FASG760103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      435 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FASG760104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      454 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FASG760105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2291 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FASG890101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2454 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ830101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      642 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1053 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1328 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      931 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      766 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1169 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      767 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      657 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1142 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      865 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      721 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FAUJ880113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      778 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FINA770101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      843 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FINA910101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1071 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FINA910102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      827 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FINA910103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      802 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FINA910104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      537 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FODM020101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      628 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      995 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1276 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1256 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      759 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      823 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      807 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1000 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      826 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      936 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/FUKS010112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      610 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GARJ730101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      902 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      531 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      490 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      882 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      923 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      681 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1165 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1030 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      529 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      962 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1098 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEIM800111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      592 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      623 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      641 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      754 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GEOR030109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1017 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GOLD730101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1054 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GOLD730102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      499 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GRAR740101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2266 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GRAR740102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      941 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GRAR740103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1884 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GUOD860101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2253 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GUYH850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1976 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GUYH850102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1867 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GUYH850103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1686 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GUYH850104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1275 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/GUYH850105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1005 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/HARY940101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      538 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/HOPA770101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1453 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/HOPT810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/HUTJ700101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      772 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/HUTJ700102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      646 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/HUTJ700103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1307 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      706 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1017 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      889 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      629 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      590 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      573 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ISOY800108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1171 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JACR890101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1346 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JANJ780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1885 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JANJ780102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1582 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JANJ780103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1240 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JANJ790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1625 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JANJ790102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      897 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JOND750101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      686 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JOND750102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      964 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JOND920101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      496 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JOND920102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      887 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JUKT750101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      842 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JUNJ780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2297 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/JURD980101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1090 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KANM800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1397 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KANM800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1356 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KANM800103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1078 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KANM800104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      972 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARP850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1731 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARP850102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      457 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARP850103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      536 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      532 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      591 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      526 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      528 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      573 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      564 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      564 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      559 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      563 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      547 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      565 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160115.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      567 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160116.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      622 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160117.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160118.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160119.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160120.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160121.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KARS160122.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      458 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KHAG800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1837 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KIDA850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      611 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KIMC930101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      527 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KLEP840101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KOEP990101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      511 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KOEP990102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1073 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KRIW710101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2101 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KRIW790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1518 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KRIW790102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1016 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KRIW790103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1615 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KUHL950101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      808 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KUMS000101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      871 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KUMS000102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      557 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KUMS000103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KUMS000104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2155 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/KYTJ820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      626 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LAWE840101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1272 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1019 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM760102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      577 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM760103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM760104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1035 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM760105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1124 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM760106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      999 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM760107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      919 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      811 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM780102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1073 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM780103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      917 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM780104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      916 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM780105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1092 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEVM780106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      525 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LEWP710101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1861 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LIFS790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      761 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LIFS790102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1004 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/LIFS790103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2391 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MANP780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1301 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MAXF760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      723 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MAXF760102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MAXF760103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      772 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MAXF760104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      690 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MAXF760105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      631 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MAXF760106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      764 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MCMT640101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      674 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MEEJ800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1236 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MEEJ800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1625 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MEEJ810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1431 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MEEJ810102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2320 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MEIH800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2423 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MEIH800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2265 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MEIH800103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      548 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MITS020101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2621 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MIYS850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2635 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MIYS990101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2617 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MIYS990102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2726 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MIYS990103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2703 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MIYS990104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2552 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MIYS990105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      839 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MONM990101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      629 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MONM990201.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1157 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MUNV940101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1128 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MUNV940102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1631 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MUNV940103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      889 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MUNV940104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      845 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/MUNV940105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2035 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NADH010101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2467 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NADH010102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2556 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NADH010103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2296 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NADH010104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1688 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NADH010105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      822 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NADH010106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NADH010107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      888 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAGK730101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      782 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAGK730102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      925 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAGK730103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      989 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      756 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      682 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      581 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      673 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      578 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      682 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      545 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      862 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      779 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      668 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      524 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH900113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      894 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      660 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      829 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      834 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      829 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      935 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NAKH920108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2079 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NISK800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2601 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NISK860101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1331 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/NOZY710101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1313 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OLSK800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      880 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ONEK900101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      927 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ONEK900102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1871 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM770101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      672 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM770102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2350 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM770103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM770104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM770105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      588 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM850102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      542 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM850103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM850104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/OOBM850105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      973 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1298 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1060 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1362 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      966 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1184 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      638 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      599 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      878 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      875 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      598 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      898 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      621 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      632 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810115.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      632 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PALJ810116.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2385 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PARJ860101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1697 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PARS000101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      724 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PARS000102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2257 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PLIV810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1028 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONJ960101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2346 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2238 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2244 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      550 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      909 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1315 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2169 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP800108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2388 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PONP930101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      535 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PRAM820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      579 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PRAM820102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PRAM820103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1575 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PRAM900101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1115 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PRAM900102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PRAM900103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1269 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PRAM900104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1271 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PTIO830101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1637 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PTIO830102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2481 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PUNT030101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2221 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/PUNT030102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      584 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      844 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1127 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1363 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      952 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      996 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      778 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      671 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880115.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880116.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      522 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880117.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880118.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1277 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880119.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1622 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880120.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1450 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880121.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      712 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880122.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880123.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880124.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880125.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      540 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880126.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      535 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880127.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880128.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880129.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880130.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      881 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880131.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1185 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880132.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1205 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880133.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1184 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880134.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1039 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880135.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      641 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880136.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880137.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880138.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/QIAN880139.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1980 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS770101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2148 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS770102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1487 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS770103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1155 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      591 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      635 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      612 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      647 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RACS820114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1630 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1357 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1089 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1097 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      728 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      967 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1245 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2735 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RADA880108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      504 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      628 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      585 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      630 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880115.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880116.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/RICJ880117.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1109 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      508 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1261 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      854 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1192 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1327 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      496 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      668 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      488 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      654 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      507 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      582 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      712 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB760113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1940 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROBB790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1107 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROSG850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2469 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROSG850102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1630 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROSM880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1823 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROSM880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      506 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROSM880103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1197 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROSM880104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2001 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ROSM880105.txt
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:34.729297 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_12_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_0_4.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_1_3.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_2_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_14_0_3.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_14_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_15_0_3.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_16_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_17_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_17_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_0_3.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_2_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_3_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_1_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_2_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_3_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_4_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_4_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_5_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_2_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_3_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_4_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_8_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_0_7.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_1_4.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_2_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_3_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1015 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SIMZ760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      456 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SNEP660101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      476 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SNEP660102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SNEP660103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      457 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SNEP660104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1158 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SUEM840101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      684 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SUEM840102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      494 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SUYM030101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1839 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/SWER830101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1093 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TAKK010101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1097 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      605 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      758 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      821 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      647 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      607 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      669 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      597 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      656 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1100 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TANS770110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1036 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TSAJ990101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1040 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/TSAJ990102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VASM830101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VASM830102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      578 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VASM830103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      565 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VELV850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1083 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VENT840101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      974 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VHEG790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2392 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VINM940101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2006 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VINM940102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1701 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VINM940103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      705 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/VINM940104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1118 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WARP780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      679 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WEBA780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2230 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WERD780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      626 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WERD780102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      631 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WERD780103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      624 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WERD780104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      834 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WILM950101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      659 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WILM950102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      619 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WILM950103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WILM950104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      856 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WIMW960101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1497 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WOEC730101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1070 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WOLR790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1105 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WOLR810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2072 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WOLS870101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      749 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WOLS870102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      623 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/WOLS870103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      607 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/YANJ020101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      771 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/YUTK870101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      685 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/YUTK870102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      711 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/YUTK870103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      711 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/YUTK870104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      758 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZASB820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1677 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZHOH040101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1180 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZHOH040102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2314 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZHOH040103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZIMJ680101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      642 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZIMJ680102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZIMJ680103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      562 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZIMJ680104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2021-11-13 22:27:22.000000 pypef-0.3/pypef/ml/AAindex/ZIMJ680105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2020-12-13 17:44:24.000000 pypef-0.3/pypef/ml/__init__.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    10148 2023-06-22 08:25:04.000000 pypef-0.3/pypef/ml/ml_run.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     5068 2022-07-02 13:59:04.000000 pypef-0.3/pypef/ml/parallelization.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    46544 2023-06-22 09:06:50.000000 pypef-0.3/pypef/ml/regression.py
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:35.170768 pypef-0.3/pypef/utils/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2020-12-13 17:44:24.000000 pypef-0.3/pypef/utils/__init__.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    16959 2023-06-22 08:44:57.000000 pypef-0.3/pypef/utils/directed_evolution.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    16653 2023-06-05 11:31:37.000000 pypef-0.3/pypef/utils/learning_test_sets.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    19555 2023-06-08 12:17:07.000000 pypef-0.3/pypef/utils/low_n_mutation_extrapolation.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2238 2023-06-08 12:17:07.000000 pypef-0.3/pypef/utils/performance.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     3712 2023-06-14 07:07:14.000000 pypef-0.3/pypef/utils/plot.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    18580 2023-06-11 17:16:59.000000 pypef-0.3/pypef/utils/prediction_sets.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     4362 2023-06-22 08:26:56.000000 pypef-0.3/pypef/utils/sto2a2m.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1872 2023-06-08 12:17:07.000000 pypef-0.3/pypef/utils/to_file.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    17756 2023-06-22 09:31:05.000000 pypef-0.3/pypef/utils/utils_run.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    15786 2023-06-22 15:38:45.000000 pypef-0.3/pypef/utils/variant_data.py
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-06-23 08:52:06.423021 pypef-0.3/pypef.egg-info/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1285 2023-06-23 08:51:58.000000 pypef-0.3/pypef.egg-info/PKG-INFO
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    21259 2023-06-23 08:52:06.000000 pypef-0.3/pypef.egg-info/SOURCES.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)        1 2023-06-23 08:51:58.000000 pypef-0.3/pypef.egg-info/dependency_links.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)       46 2023-06-23 08:51:58.000000 pypef-0.3/pypef.egg-info/entry_points.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      107 2023-06-23 08:51:58.000000 pypef-0.3/pypef.egg-info/requires.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)        6 2023-06-23 08:51:58.000000 pypef-0.3/pypef.egg-info/top_level.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      117 2023-06-11 11:08:13.000000 pypef-0.3/requirements.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)       38 2023-06-23 08:52:35.205300 pypef-0.3/setup.cfg
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2149 2023-06-22 14:53:59.000000 pypef-0.3/setup.py
```

### Comparing `pypef-0.2.4/LICENSE.md` & `pypef-0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/PKG-INFO` & `pypef-0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypef
-Version: 0.2.4
+Version: 0.3
 Summary: A command-line interface (CLI) tool for performing data-driven protein engineering by building machine learning (ML)-trained regression models from sequence variant fitness data (in CSV format) based on different techniques for protein sequence encoding. Next to building pure ML models, 'hybrid modeling' is also possible using a blended model optimized for predictive contributions of a statistical and an ML-based prediction.
 Home-page: https://github.com/niklases/PyPEF
 Author: Niklas Siedhoff & Alexander-Maurice Illig
 Author-email: n.siedhoff@biotec.rwth-aachen.de
 License: CC BY-NC-SA 4.0
 Keywords: Pythonic Protein Engineering Framework
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pypef-0.2.4/README.md` & `pypef-0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 This repository contains the source files and supplementary information for the PyPEF framework, which is described in<br>
 
 Niklas E. Siedhoff<sup>*1,§*</sup>, Alexander-Maurice Illig<sup>*1,§*</sup>, Ulrich Schwaneberg<sup>*1,2*</sup>, Mehdi D. Davari<sup>*3,\**</sup>, <br>
 PyPEF – An Integrated Framework for Data-Driven Protein Engineering, *J. Chem. Inf. Model.* 2021, 61, 3463-3476 <br>
-https://doi.org/10.1021/acs.jcim.1c00099<br>
+https://doi.org/10.1021/acs.jcim.1c00099 <br>
 
 as well as additional framework features described in the preprint<br>
 
 Alexander-Maurice Illig<sup>*1,§*</sup>, Niklas E. Siedhoff<sup>*1,§*</sup>, Ulrich Schwaneberg<sup>*1,2*</sup>, Mehdi D. Davari<sup>*3,\**</sup>, <br>
 A hybrid model combining evolutionary probability and machine learning leverages data-driven protein engineering, *To be published*<br>
 Preprint available at bioRxiv: https://doi.org/10.1101/2022.06.07.495081.
 
@@ -31,22 +31,29 @@
 - [Setting Up the Scripts Yourself](#set-up)
 - [Preprocessing for DCA-based Sequence Encoding](#dca-preprocessing)
 - [API Usage for Sequence Encoding](#api-usage)
 ---
 
 <a name="pypef"></a>
 # PyPEF: Pythonic Protein Engineering Framework
+[![PyPI version](https://img.shields.io/pypi/v/PyPEF?color=blue)](https://pypi.org/project/pypef/)
+[![Python version](https://img.shields.io/pypi/pyversions/PyPEF)](https://pypi.org/project/pypef/)
 
-a framework written in Python 3 for performing sequence-based machine learning-assisted protein engineering to predict a protein's fitness from its sequence. Written by Niklas Siedhoff and Alexander-Maurice Illig.
+a framework written in Python 3 for performing sequence-based machine learning-assisted protein engineering to predict a protein's fitness from its sequence using different forms of sequence encoding:
+- One-hot encoding
+- Amino acid descriptor sets (taken from AAindex database) encoding
+- Direct coupling analysis (amino acid coevolution based on multiple sequence alignments) encoding
+
+Written by Niklas Siedhoff and Alexander-Maurice Illig.
 
 <p align="center">
     <img src="workflow/test_dataset_aneh/exemplary_validation_color_plot.png" alt="drawing" width="500"/>
 </p>
 
-Protein engineering by rational or random approaches generates data that can aid the construction of self-learned sequence-function landscapes to predict beneficial variants by using probabilistic methods that can screen the unexplored sequence space with uncertainty *in silico*. Such predictive methods can be applied for increasing the success/effectivity of an engineering campaign while partly offering the prospect to reveal (higher-order) epistatic effects. Here we present an engineering framework termed PyPEF for assisting the supervised training and testing of regression models for predicting beneficial combinations of (identified) amino acid substitutions using machine learning algorithms from the [Scikit-learn](https://github.com/scikit-learn/scikit-learn) package. As training input, the developed framework requires the variant sequences and the corresponding screening results (fitness labels) of the identified variants as CSV (or FASTA-like datasets following a self-defined convention). Using linear or nonlinear regression methods (partial least squares (PLS), Ridge, Lasso, Elastic net, support vector machines (SVR), random forest (RF), and multilayer perceptron (MLP)-based regression), PyPEF trains on the given learning data while optimizing model hyperparameters (default: five-fold cross-validation) and can compute model performances on left-out test data. As sequences are encoded using amino acid descriptor sets taken from the [AAindex database](https://www.genome.jp/aaindex/), finding the best index-dependent encoding for a specific test set can be seen as a hyperparameter search on the test set. In addition, one-hot and [direct coupling analysis](https://en.wikipedia.org/wiki/Direct_coupling_analysis)-based feature generation are implemented as sequence encoding techniques, which often outperform AAindex-based encoding techniques. Finally, the selected or best identified encoding technique and regression model can be used to perform directed evolution walks *in silico* (see [Church-lab implementation](https://github.com/churchlab/UniRep) or the [reimplementation](https://github.com/ivanjayapurna/low-n-protein-engineering)) or to predict natural diverse or recombinant variant sequences that subsequently are to be designed and validated in the wet-lab.
+Protein engineering by rational or random approaches generates data that can aid the construction of self-learned sequence-function landscapes to predict beneficial variants by using probabilistic methods that can screen the unexplored sequence space with uncertainty *in silico*. Such predictive methods can be applied for increasing the success/effectivity of an engineering campaign while partly offering the prospect to reveal (higher-order) epistatic effects. Here we present an engineering framework termed PyPEF for assisting the supervised training and testing of regression models for predicting beneficial combinations of (identified) amino acid substitutions using machine learning algorithms from the [Scikit-learn](https://github.com/scikit-learn/scikit-learn) package. As training input, the developed framework requires the variant sequences and the corresponding screening results (fitness labels) of the identified variants as CSV (or FASTA-Like (FASL) datasets following a self-defined convention). Using linear or nonlinear regression methods (partial least squares (PLS), Ridge, Lasso, Elastic net, support vector machines (SVR), random forest (RF), and multilayer perceptron (MLP)-based regression), PyPEF trains on the given learning data while optimizing model hyperparameters (default: five-fold cross-validation) and can compute model performances on left-out test data. As sequences are encoded using amino acid descriptor sets taken from the [AAindex database](https://www.genome.jp/aaindex/), finding the best index-dependent encoding for a specific test set can be seen as a hyperparameter search on the test set. In addition, one-hot and [direct coupling analysis](https://en.wikipedia.org/wiki/Direct_coupling_analysis)-based feature generation are implemented as sequence encoding techniques, which often outperform AAindex-based encoding techniques. Finally, the selected or best identified encoding technique and regression model can be used to perform directed evolution walks *in silico* (see [Church-lab implementation](https://github.com/churchlab/UniRep) or the [reimplementation](https://github.com/ivanjayapurna/low-n-protein-engineering)) or to predict natural diverse or recombinant variant sequences that subsequently are to be designed and validated in the wet-lab.
 
 For detailed information, please refer to the above-mentioned publications and related Supporting Information.
 
 The workflow procedure is explained in the [Jupyter notebook](/workflow/Workflow_PyPEF.ipynb) (.ipynb) protocol (see
 Tutorial section below).
 
 <img src="workflow/Splitting_Workflow.png" alt="drawing" width="1000"/>
@@ -61,30 +68,47 @@
 
 After successful installation, PyPEF should work by calling `pypef` in the shell:
 
 ```
 pypef --help
 ```
 
-The detailed routine for setting up a new virtual environment with Anaconda, installing the necessary Python packages for that environment, and running the Jupyter notebook tutorial can be found below in the Tutorial section. Further, executable files for running PyPEF on a single core are available at https://github.com/niklases/PyPEF/releases/tag/v0.2.3-alpha.
+The detailed routine for setting up a new virtual environment with Anaconda, installing the necessary Python packages for that environment, and running the Jupyter notebook tutorial can be found below in the Tutorial section.
 
 <a name="requirements"></a>
 ## Requirements
 - Python >=3.9
-    - numpy
-    - pandas
-    - tqdm
-    - docopt
-    - matplotlib
+    - numpy 
     - scipy
-    - adjustText
+    - pandas
     - scikit-learn
+    - tensorflow 
+    - ray[default]
+    - matplotlib
+    - tqdm
     - biopython
     - schema
-    - ray[default] (<2.0.0)
+    - docopt
+    - adjustText
+
+If errors occur with third-party packages, you can check the required Python version dependencies (if available); also, as a rule of thumb, it is often helpful to use the second most recent Python version instead of the latest, since development for the latest version is often ongoing:
+
+[![Python version](https://img.shields.io/pypi/pyversions/numpy?label=numpy%3A%20python)](https://github.com/numpy/numpy)
+[![Python version](https://img.shields.io/pypi/pyversions/scipy?label=scipy%3A%20python)](https://github.com/scipy/scipy)
+[![Python version](https://img.shields.io/pypi/pyversions/pandas?label=pandas%3A%20python)](https://github.com/pandas-dev/pandas)
+[![Python version](https://img.shields.io/pypi/pyversions/scikit-learn?label=scikit-learn%3A%20python)](https://github.com/scikit-learn/scikit-learn)
+[![Python version](https://img.shields.io/pypi/pyversions/tensorflow?label=tensorflow%3A%20python)](https://github.com/tensorflow/tensorflow)
+[![Python version](https://img.shields.io/pypi/pyversions/ray?label=ray%3A%20python)](https://github.com/ray-project/ray)
+[![Python version](https://img.shields.io/pypi/pyversions/matplotlib?label=matplotlib%3A%20python)](https://github.com/matplotlib/matplotlib)
+[![Python version](https://img.shields.io/pypi/pyversions/tqdm?label=tqdm%3A%20python)](https://github.com/tqdm/tqdm)
+[![Python version](https://img.shields.io/pypi/pyversions/biopython?label=biopython%3A%20python)](https://github.com/biopython/biopython)
+[![Python version](https://img.shields.io/pypi/pyversions/schema?label=schema%3A%20python)](https://github.com/keleshev/schema)
+[![Python version](https://img.shields.io/pypi/pyversions/docopt?label=docopt%3A%20python)](https://github.com/docopt/docopt)
+[![Python version](https://img.shields.io/pypi/pyversions/adjusttext?label=adjusttext%3A%20python)](https://github.com/Phlya/adjustText)
+
 
 <a name="examples"></a>
 ## Running Examples
 Printing the help function:   
 ```
 pypef --help
 ```
@@ -92,25 +116,25 @@
 Creating sets for model learning and testing:
 ```
 pypef mklsts -w WT_SEQUENCE.FASTA -i VARIANT-FITNESS_DATA.CSV 
 ```
 
 Training and testing a model (encoding technique = {`aaidx`, `onehot`, `dca`}, regression model = {`pls`, `ridge`, `lasso`, `elasticnet`, `svr`, `rf`, `mlp`}):
 ```
-pypef ml -e aaidx -l LEARNING_SET.FASTA -t TEST_SET.FASTA --regressor pls 
+pypef ml -e aaidx -l LEARNING_SET.FASL -t TEST_SET.FASL --regressor pls 
 ```
 
 Show the model performance(s) (reads and prints the created Model_Results.txt file):
 ```
 pypef ml --show
 ```
 
 Load a trained model, predict fitness of test sequences using that model, and plot the measured versus the predicted fitness values:
 ```
-pypef ml -e aaidx -m MODEL -f TEST_SET.FASTA
+pypef ml -e aaidx -m MODEL -t TEST_SET.FASL
 ```
 `-m MODEL`is the saved model Pickle file name, for `-e aaidx` this will be the AAindex to use for encoding, e.g. `-m ARGP820101`, for `-e onehot` it will be `-m ONEHOTMODEL` and for `-e dca` it will be `-m DCAMODEL`.
 
 Load a trained model and use it for predicting the fitness of sequences of a prediction set (with unknown corresponding fitness):
 ```
 pypef ml -e aaidx -m MODEL -p PREDICTION_SET.FASTA
 ```
@@ -133,37 +157,56 @@
 Encoding a variant-fitness CSV file and writing it to a new CSV file (for the different encodings, also specify the AAindex name with the `-m` option next to `-e aaidx`):
 
 ```
 pypef encode -i VARIANT-FITNESS_DATA.CSV -w WT_SEQUENCE.FASTA -e aaidx
 ```
 
 Using the created variant-encoded sequence-fitness CSV file for a simulated "low *N*" engineering task:
+
 ```
 pypef ml low_n -i VARIANT-FITNESS-ENCODING_DATA.CSV --regressor pls
 ```
 
 Using the created variant-encoded sequence-fitness CSV file for a simulated "mutation extrapolation" task (requires higher/deeply-substituted variants):
 ```
 pypef ml extrapolation -i VARIANT-FITNESS-ENCODING_DATA.CSV --regressor pls
 ```
 
 The use of the hybrid model (`pypef hybrid`) - instead of a pure ML model (`pypef ml`) as described in the steps above - is quite similar in terms of commands, but does not require the definition of the `-e`/`--encoding` and the `--regressor` flags, since it depends only on the DCA-based encoding technique and (so far) only uses Ridge regression for modeling. However, DCA-based encoding of sequences always requires a parameter file as input, which comes from the preprocessing of a query-specific multiple sequence alignment (MSA) and results in the parameter file generated by [plmc](https://github.com/debbiemarkslab/plmc). E.g. for training a model on a learning set and testing it on a test set, the command for hybrid modeling is:
 
 ```
-pypef hybrid -l LEARNING_SET.FASTA -t TEST_SET.FASTA --params PLMC_FILE.params
+pypef hybrid -l LEARNING_SET.FASL -t TEST_SET.FASL --params PLMC_FILE.params
 ``` 
 
+Also, it is now possible to infer DCA model parameters using [GREMLIN](https://www.pnas.org/doi/10.1073/pnas.1314045110)'s [TensorFlow implementation](https://github.com/sokrypton/GREMLIN_CPP/blob/master/GREMLIN_TF.ipynb) and a generated MSA in FASTA or A2M format:
+
+```
+pypef param_inference --msa MSA.fasta -w WT_SEQUENCE.FASTA --opt_iter 250
+``` 
+
+For getting coupling information and highly evolved amino acids:
+```
+pypef save_msa_info --msa MSA.fasta -w WT_SEQUENCE.FASTA --opt_iter 250
+```
+
+Using saved GREMLIN model for testing:
+
+```
+pypef hybrid -l LEARNING_SET.FASL -t TEST_SET.FASL --params GREMLIN
+``` 
+
+
 Sample files for testing PyPEF routines are provided in the workflow directory, which are also used when running the notebook tutorial. PyPEF's package dependencies are linked [here](https://github.com/niklases/PyPEF/network/dependencies).
 Further, for designing your own API based on the PyPEF workflow, modules can be adapted from the [source code](/pypef).
 
 As standard input files, PyPEF requires the target protein wild-type sequence in [FASTA](https://en.wikipedia.org/wiki/FASTA) format and variant-fitness data in [CSV](https://en.wikipedia.org/wiki/Comma-separated_values) format to split the collected variant-fitness data in learning and test sets that resemble the aligned FASTA format and additionally contain lines indicating the fitness of each corresponding variant (see [ANEH sample files](workflow/test_dataset_aneh), [avGFP sample files](workflow/test_dataset_avgfp), and [MERGE SSM & DMS files](https://github.com/Protein-Engineering-Framework/MERGE/tree/main/Data/_variant_fitness_wtseq)).
 
 <a name="tutorial"></a>
 ## Tutorial
-Before starting running the tutorial, it is a good idea to set-up a new Python environment using Anaconda, https://www.anaconda.com/, e.g. using [Anaconda](https://www.anaconda.com/products/individual) ([Anaconda3-2020.11-Linux-x86_64.sh installer download](https://repo.anaconda.com/archive/Anaconda3-2020.11-Linux-x86_64.sh)) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
+Before starting running the tutorial, it is a good idea to set up a new Python environment using Anaconda, https://www.anaconda.com/, e.g. using [Anaconda](https://www.anaconda.com/products/individual) ([Anaconda3-2020.11-Linux-x86_64.sh installer download](https://repo.anaconda.com/archive/Anaconda3-2020.11-Linux-x86_64.sh)) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
 Change to the download directory and run the installation, e.g. in Linux:
 
 ```
 bash Anaconda3-2020.11-Linux-x86_64.sh
 ```
 
 After accepting all steps, the conda setup should also be written to your `~/.bashrc`file, so that you can call anaconda typing `conda`.
@@ -308,48 +351,62 @@
 python3 ./pypef/main.py
 ```
 
 <a name="dca-preprocessing"></a>
 ## Preprocessing for DCA-based Sequence Encoding
 
 1. Downloading sequence database (e.g. UniRef100):
-```
-wget https://ftp.uniprot.org/pub/databases/uniprot/uniref/uniref100/uniref100.fasta.gz
-```
+   ```
+   wget https://ftp.uniprot.org/pub/databases/uniprot/uniref/uniref100/uniref100.fasta.gz
+   ```
 
 2. Extracting sequence database:
-```
-gunzip uniref100.fasta.gz
-```
+   ```
+   gunzip uniref100.fasta.gz
+   ```
 
 3. After [installing jackhmmer as part of the HMMER package](http://hmmer.org/documentation.html), construct an MSA for your target sequence provided in FASTA format (and for example set `--incT` to half the sequence length (0.5*L*) and the number of used CPUs for computing):
-```
-jackhmmer --incT 199 --cpu 16 --noali -A ANEH_jhmmer.sto Sequence_WT_ANEH.fasta /path/to/uniref100.fasta
-```
+   ```
+   jackhmmer --incT 199 --cpu 16 --noali -A ANEH_jhmmer.sto Sequence_WT_ANEH.fasta /path/to/uniref100.fasta
+   ```
 
 4. Convert the created MSA from [Stockholm](https://en.wikipedia.org/wiki/Stockholm_format) (.sto) format to [A2M](https://en.wikipedia.org/wiki/FASTA_format#Extensions) format:
-```
-pypef sto2a2m --sto ANEH_jhmmer.sto
-```
-
-5. After [installing plmc](https://github.com/debbiemarkslab/plmc#compilation), generate the evolutionary coupling file, which is used for encoding sequences. For example, set `-le` to the value output by `sto2a2m`:
-
-```
-plmc -o ANEH_72.6.params -le 72.6 -m 100 -g -f WT_ANEH ANEH_jhmmer.a2m
-```
-
-Done! The output parameter (.params) file can be used for encoding sequences with the DCA-based encoding technique (`-e dca`) by providing it to PyPEF; e.g. for pure ML modeling:
-```
-pypef ml -e dca -l LS.fasta -t TS.fasta --regressor pls --params ANEH_72.6.params
-```
-Or for hybrid modeling:
-```
-pypef hybrid -l LS.fasta -t TS.fasta --params ANEH_72.6.params
-```
+   ```
+   pypef sto2a2m --sto ANEH_jhmmer.sto
+   ```
+   
+5. Now you can follow approaches 5.1 (using GREMLIN; implemented in TensorFlow) or 5.2 (using plmc; extern parameter generation in C). 
+
+    5.1. Running GREMLIN on the generated MSA (in FASTA or A2M format):
+    ```
+    pypef param_inference --msa ANEH_jhmmer.a2m -w WT_SEQUENCE.FASTA --opt_iter 250
+    ```
+    The pickled GREMLIN file can then be used for encoding new/test sequences:
+    ```
+    pypef ml -e dca -l LS.fasl -t TS.fasl --regressor pls --params GREMLIN
+    ```
+    Or for hybrid modeling:
+    ```
+    pypef hybrid -l LS.fasl -t TS.fasl --params GREMLIN
+    ```
+
+    5.2 After [installing plmc](https://github.com/debbiemarkslab/plmc#compilation), generate the evolutionary coupling file, which is used for encoding sequences. For example, set `-le` to the value output by `sto2a2m`:
+    ```
+    plmc -o ANEH_72.6.params -le 72.6 -m 100 -g -f WT_ANEH ANEH_jhmmer.a2m
+    ```
+    
+    The output parameter (.params) file can be used for encoding sequences with the DCA-based encoding technique (`-e dca`) by providing it to PyPEF; e.g. for pure ML modeling:
+    ```
+    pypef ml -e dca -l LS.fasl -t TS.fasl --regressor pls --params ANEH_72.6.params
+    ```
+    Or for hybrid modeling:
+    ```
+    pypef hybrid -l LS.fasl -t TS.fasl --params ANEH_72.6.params
+    ```
 
 <a name="api-usage"></a>
 ## API Usage for Sequence Encoding
-For script-based encoding of sequences using PyPEF and the available AAindex-, OneHot- or DCA-based techniques, the classes and corresponding functions can be imported, i.e. `OneHotEncoding`, `AAIndexEncoding`, `DCAEncoding`, and `DCAHybridModel`. In addition, implemented functions for CV-based tuning of regression models can be used to train and validate models, eventually deriving them to obtain performances on retained data for testing. An exemplary script for CV-based (low-*N*) tuning of models and using them for testing is provided at [workflow/api_encoding_train_test.py](workflow/api_encoding_train_test.py).
+For script-based encoding of sequences using PyPEF and the available AAindex-, OneHot- or DCA-based techniques, the classes and corresponding functions can be imported, i.e. `OneHotEncoding`, `AAIndexEncoding`, `GREMLIN` (DCA),  `PLMC` (DCA), and `DCAHybridModel`. In addition, implemented functions for CV-based tuning of regression models can be used to train and validate models, eventually deriving them to obtain performances on retained data for testing. An exemplary script for CV-based (low-*N*) tuning of models and using them for testing is provided at [workflow/api_encoding_train_test.py](workflow/api_encoding_train_test.py).
 
 <p align="center">
     <img src="workflow/low_N_avGFP_extrapolation.png" alt="drawing" width="500"/>
 </p>
```

### Comparing `pypef-0.2.4/pypef/__init__.py` & `pypef-0.3/pypef/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
 # 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
 # 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
 # *Corresponding author
 # §Equal contribution
 
 
-__version__ = '0.2.4-alpha'
+__version__ = '0.3-alpha'
```

### Comparing `pypef-0.2.4/pypef/dca/encoding.py` & `pypef-0.3/pypef/dca/plmc_encoding.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,55 +12,64 @@
 # https://doi.org/10.1021/acs.jcim.1c00099
 # Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
 # 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
 # 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
 # *Corresponding author
 # §Equal contribution
 
-# Contains Python code used for the approach presented in our 'hybrid modeling' paper
-# Preprint available at: https://doi.org/10.1101/2022.06.07.495081
-# Code available at: https://github.com/Protein-Engineering-Framework/Hybrid_Model
-
-# The included class 'CouplingsModel' has been taken from the script 'model.py' as part of the
-# EVmutation module (https://github.com/debbiemarkslab/EVmutation) written by Thomas Hopf in the
-# labs of Debora Marks and Chris Sander at Harvard Medical School and modified (shortened).
-# See also: https://doi.org/10.1038/nbt.3769
-# Hopf, T. A., Ingraham, J. B., Poelwijk, F.J., Schärfe, C.P.I., Springer, M., Sander, C., & Marks, D. S. (2016).
-# Mutation effects predicted from sequence co-variation. Nature Biotechnology, in press.
-
 """
+Contains Python code used for the approach presented in our 'hybrid modeling' paper
+Preprint available at: https://doi.org/10.1101/2022.06.07.495081
+Code available at: https://github.com/Protein-Engineering-Framework/Hybrid_Model
+
 The included class 'CouplingsModel' has been taken from the script 'model.py' as part of the
 EVmutation module (https://github.com/debbiemarkslab/EVmutation) written by Thomas Hopf in the
 labs of Debora Marks and Chris Sander at Harvard Medical School and modified (shortened).
-
-See also:
+See also: https://doi.org/10.1038/nbt.3769
 Hopf, T. A., Ingraham, J. B., Poelwijk, F.J., Schärfe, C.P.I., Springer, M., Sander, C., & Marks, D. S. (2016).
 Mutation effects predicted from sequence co-variation. Nature Biotechnology, in press.
+
+References:
+[1] Hopf, T. A., Ingraham, J. B., Poelwijk, F.J., Schärfe, C.P.I., Springer, M., Sander, C., & Marks, D. S.
+    Mutation effects predicted from sequence co-variation.
+    Nature Biotechnology, 35, 2017, 128–135
+    https://doi.org/10.1038/nbt.3769
+[2] Hopf T. A., Green A. G., Schubert B., et al.
+    The EVcouplings Python framework for coevolutionary sequence analysis.
+    Bioinformatics 35, 2019, 1582–1584
+    https://doi.org/10.1093/bioinformatics/bty862
+[3] Ekeberg, M., Lövkvist, C., Lan, Y., Weigt, M., & Aurell, E.
+    Improved contact prediction in proteins: Using pseudolikelihoods to infer Potts models.
+    Physical Review E, 87(1), 2013, 012707. doi:10.1103/PhysRevE.87.012707
+    https://doi.org/10.1103/PhysRevE.87.012707
 """
 
 
-from collections.abc import Iterable  # originally imported 'from collections'
+import os
+from collections.abc import Iterable
 import logging
 logger = logging.getLogger('pypef.dca.encoding')
 
 import numpy as np
 import ray
 from tqdm import tqdm
+import pickle
+
 from pypef.utils.variant_data import amino_acids
 
 
 _SLICE = np.s_[:]
-# np.warnings.filterwarnings('error', category=np.VisibleDeprecationWarning)  # DEV
+# np.warnings.filterwarnings('error', category=np.VisibleDeprecationWarning)
 
 class InvalidVariantError(Exception):
     """
     Description
     -----------
     Exception raised when entered variant does not follow the required scheme
-    (integer enclosed by two one letter code representations of amino acids).
+    (integer enclosed by two one-letter code representations of amino acids).
 
     Attributes
     ----------
     variant: str
         Variant that causes the error
     message: str
         Explanation of the error
@@ -104,16 +113,16 @@
 
 
 def is_valid_substitution(substitution: str) -> bool:
     """
     Description
     -----------
     A substitution has to follow the scheme:
-    First character: (wild-type/substituted) amino acid in one letter code representation
-    Last character: (introduced) amino acid in one letter code representation
+    First character: (wild-type/substituted) amino acid in one-letter code representation
+    Last character: (introduced) amino acid in one-letter code representation
     In between: position (of substitution)
 
     If the entered substitution does not follow this scheme (integer enclosed by two one
     letter code representations of amino acids) return False, else return True.
 
     Parameters
     -----------
@@ -141,15 +150,15 @@
 
 def is_valid_variant(variant: str, separator='/') -> bool:
     """
     Description
     -----------
     Gets the single substitutions of the variant and checks if they follow the required scheme.
 
-    If the entered substitution does not follow this scheme (integer enclosed by two one
+    If the entered substitution does not follow this scheme (integer enclosed by two one-
     letter code representations of amino acids) return False, else return True.
 
     Parameters
     ----------
     variant : str
         Joined string of integers enclosed by two letters representing the wild type
         and variant amino acid in the single letter code. -> Check separator
@@ -194,15 +203,15 @@
     Class to store parameters of pairwise undirected graphical model of sequences
     and compute evolutionary couplings, sequence statistical energies, etc.
     """
     def __init__(
             self,
             filename,
             precision="float32",
-            verbose: bool = True,
+            verbose: bool = False,
             **kwargs
     ):
         """
         Initializes the object with raw values read from binary .Jij file
 
         Parameters
         ----------
@@ -212,14 +221,15 @@
             Symbols corresponding to model states (e.g. "-ACGT").
         precision : {"float32", "float64"}, default: "float32"
             Sets if input file has single (float32) or double precision (float64)
         """
         self.index_map = None
         self._target_seq = None
         self._index_list = None
+        self.x_wt = None
         self.verbose = verbose
         try:
             self.__read_plmc_v2(filename, precision)
         except TypeError or FileNotFoundError:
             raise SystemError(
                 "Did not find (specified) PLMC parameter file. "
                 "The parameter file is required for DCA-based "
@@ -283,24 +293,24 @@
                 if num not in self.index_list:
                     not_valid.append(num)
                 else:
                     valid.append(num)
             self.wt_aa_pos = []
             for aa, pos in zip(self._target_seq, self.index_list):
                 self.wt_aa_pos.append(str(aa) + str(pos))
-            logger.info(f'Evaluating gap content of PLMC parameter file... '
-                  f'First amino acid position used in the MSA (PLMC params file) is '
-                  f'{self._target_seq[0]}{self.index_list[0]} and the last position '
-                  f'used is {self._target_seq[-1]}{self.index_list[-1]}.')
-            if len(not_valid) > 0:
-                logger.info(f'Further, non-included positions are:\n{str(not_valid)[1:-1]}')
             if self.verbose:
-                    logger.info(f'Summary of all effective positions represented in the MSA '
-                                f'based on wild-type sequence ({len(valid)} encoded positions):\n'
-                                f'{str([aa_pos for aa_pos in self.wt_aa_pos])[1:-1]}'.replace("'", ""))
+                logger.info(f'Evaluating gap content of PLMC parameter file... '
+                            f'First amino acid position used in the MSA (PLMC params file) is '
+                            f'{self._target_seq[0]}{self.index_list[0]} and the last position '
+                            f'used is {self._target_seq[-1]}{self.index_list[-1]}.')
+                if len(not_valid) > 0:
+                    logger.info(f'Further, non-included positions are:\n{str(not_valid)[1:-1]}')
+                logger.info(f'Summary of all effective positions represented in the MSA '
+                            f'based on wild-type sequence ({len(valid)} encoded positions):\n'
+                            f'{str([aa_pos for aa_pos in self.wt_aa_pos])[1:-1]}'.replace("'", ""))
 
             # single site frequencies f_i and fields h_i
             self.f_i, = np.fromfile(
                 f, dtype=(precision, (self.L, self.num_symbols)), count=1
             )
 
             self.h_i, = np.fromfile(
@@ -487,15 +497,15 @@
         """
         Quick access to h_i matrix with automatic index mapping.
         See __2d_access for explanation of parameters.
         """
         return self.__2d_access(self.h_i, i, A_i)
 
 
-class DCAEncoding(CouplingsModel):
+class PLMC(CouplingsModel):
     """
     Class for performing the 'DCA encoding'.
 
     Attributes
     ----------
     params_file: str
         Binary parameter file outputted by PLMC.
@@ -506,14 +516,16 @@
             params_file: str,
             separator: str = '/',
             verbose: bool = True
     ):
         super().__init__(filename=params_file)  # inherit functions and variables from class CouplingsModel
         self.verbose = verbose
         self.separator = separator
+        target_seq, index = self.get_target_seq_and_index()
+        self.x_wt = self.collect_encoded_sequences(target_seq[0] + str(index[0]) + target_seq[0])
 
     def _get_position_internal(self, position: int):
         """
         Description
         -----------
         Returns the "internal position" of an amino acid, e.g., D19V is the desired substitution,
         but the fasta sequence starts from residue 3, i.e., the first two residues are "missing".
@@ -589,15 +601,15 @@
         """
         Checks whether the amino acid to substitute of the variant matches
         the amino acid of the wild type at this position.
         """
         if substitution[:-1] not in self.wt_aa_pos:
             wild_type_aa, position, A_i = self._unpack_substitution(substitution)
             raise SystemError(
-                f"The variant naming scheme is not fitting to the DCAEncoding "
+                f"The variant naming scheme is not fitting to the PLMC "
                 f"scheme. Substitution {substitution} of variant {variant} has "
                 f"the amino acid {wild_type_aa} at position {position}, which "
                 f"does not match the wild type sequence used as target for DCA-"
                 f"based coupling parameter file generation. See summary of "
                 f"(effective) wild-type positions and amino acids above. Please "
                 f"check your input variant data or generate a new parameter file "
                 f"for encoding."
@@ -613,34 +625,34 @@
         ----------
         variant : str
             Joined string of integers enclosed by two letters representing the wild type
             and variant amino acid in the single letter code. -> Check separator
 
         Returns
         -------
-        X_var : np.ndarray
+        x_var : np.ndarray
             Encoded sequence of the variant.
         """
         sequence = self.target_seq.copy()
         for substitution in get_single_substitutions(variant, self.separator):  # e.g. A123C/D234E --> A123C, D234C
             wild_type_aa, position, A_i = self._unpack_substitution(substitution)
 
             i = self._get_position_internal(position)
             if not i:
                 raise EffectiveSiteError(position, variant, self.verbose)
 
             self.check_substitution_naming_against_wt(substitution, variant)
             i_mapped = self.index_map[i]
             sequence[i_mapped] = A_i
 
-        X_var = np.zeros(sequence.size, dtype=float)
+        x_var = np.zeros(sequence.size, dtype=float)
         for idx, (i, A_i) in enumerate(zip(self.index_list, sequence)):
-            X_var[idx] = self.hi(i, A_i) + 0.5 * self.Ji(i, A_i, sequence)
+            x_var[idx] = self.hi(i, A_i) + 0.5 * self.Ji(i, A_i, sequence)
 
-        return X_var
+        return x_var
 
     def collect_encoded_sequences(self, variants: list) -> np.ndarray:
         """
         Description
         -----------
         Collects all encoded sequences based on input variant names.
 
@@ -659,152 +671,188 @@
             Internal array/list position for variants that could not be
             encoded due to the underlying MSA (inter-gap threshold for
             computing of local and coupling PLMC parameters). These list
             positions must then be removed for the corresponding fitness
             arrays/lists for training and testing the model.
         """
         encoded_sequences = []
-        if len(variants) == 1:  # do not show progress bar for single variant
+        if len(np.atleast_1d(variants)) == 1:  # do not show progress bar for single variant
             set_silence = True  # thus, also not for directed evolution
         else:
             set_silence = False
-        for i, variant in enumerate(tqdm(variants, disable=set_silence)):
+        for i, variant in enumerate(tqdm(np.atleast_1d(variants), disable=set_silence)):
             try:
                 encoded_sequences.append(self.encode_variant(variant))
             except EffectiveSiteError:
                 encoded_sequences.append([None])
 
         return np.array(encoded_sequences, dtype='object')
 
 
 """
-Below: Some helper functions to run the DCAEncoding class and get 
+Below: Some helper functions to run the PLMC class and get 
 the encoded sequences in parallel (threading) using Ray and
 to construct a pandas.DataFrame to store the encoded sequences 
 (features) and the associated fitness values in a CSV file.
 """
 
 
+def save_plmc_dca_encoding_model(params_file, substitution_sep='/'):
+    """
+    Just converts plmc params from raw binary to
+    Pickle-saved PLMC class.
+    """
+    logger.info("Transforming the provided plmc params file "
+                "to a PLMC Pickle file (Pickles/PLMC).")
+    plmc = PLMC(
+        params_file=params_file,
+        separator=substitution_sep,
+        verbose=False
+    )
+    try:
+        os.mkdir('Pickles')
+    except FileExistsError:
+        pass
+    pickle.dump({
+        'model': plmc,
+        'model_type': 'PLMCpureDCA',
+        'beta_1': None,
+        'beta_2': None,
+        'spearman_rho': None,
+        'regressor': None
+    },
+        open(f'Pickles/PLMC', 'wb')
+    )
+
+
 def get_encoded_sequence(
         variant: str,
-        dca_encode: DCAEncoding
+        dca_encode: PLMC
 ):
     """
     Description
     -----------
     Gets encoded sequence based on input variant name and a preexisting
-    DCAEncoding instance.
+    PLMC instance.
 
     Parameters
     ----------
     variant: str
         Variant name, e.g. 'A13E', or 'D127F'. Wild-type sequence
         is defined by substitution to itself, e.g. 'F17F'.
-    dca_encode: DCAEncoding class object
-        For encoding sequences, see above: class DCAEncoding.
+    dca_encode: PLMC class object
+        For encoding sequences, see above: class PLMC.
     """
     try:
         encoded_seq = dca_encode.encode_variant(variant)
     except EffectiveSiteError:  # position not included in processed MSA
         return
 
     return encoded_seq
 
 
 @ray.remote
 def _get_data_parallel(
         variants: list,
+        sequences: list,
         fitnesses: list,
-        dca_encode: DCAEncoding,
+        dca_encode: PLMC,
         data: list
 ) -> list:
     """
     Description
     -----------
     Get the variant name, the associated fitness value, and its ("DCA"-)encoded sequence.
 
     Parameters
     ----------
     variants : list
         List of strings containing the variants to be encoded.
     fitnesses : list
         List of floats (1d) containing the fitness values associated to the variants.
     dca_encode : object
-        Initialized 'DCAEncoding' class object.
+        Initialized 'PLMC' class object.
     data : manager.list()
         Manager.list() object to store the output of multiple processors.
 
     Returns
     -------
     data : manager.list()
         Filled list with variant names, fitnesses, and encoded sequence.
     """
-    for i, (variant, fitness) in enumerate(zip(variants, fitnesses)):
+    for i, (variant, sequence, fitness) in enumerate(zip(variants, sequences, fitnesses)):
         try:
-            data.append([variant, dca_encode.encode_variant(variant), fitness])
+            data.append([variant, sequence, dca_encode.encode_variant(variant), fitness])
         except EffectiveSiteError:  # do not append non-encoded sequences and
-            pass                 # associated fitness values
+            pass                    # associated fitness values
 
     return data
 
 
 def get_dca_data_parallel(
         variants: list,
+        sequences: list,
         fitnesses: list,
-        dca_encode: DCAEncoding,
+        dca_encode: PLMC,
         threads: int,
-) -> tuple[list, list, list]:
+        verbose=True
+) -> tuple[list, list, list, list]:
     """
     Description
     -----------
     This function allows to generate the encoded sequences based on the variants
     given in 'csv_file' in a parallel manner.
 
     Parameters
     ----------
     variants: list (or np.ndarray)
         Variant names.
     fitnesses: list (or np.ndarray)
         Variant-associated fitness values.
     dca_encode : object
-        Initialized 'DCAEncoding' class object.
+        Initialized 'PLMC' class object.
     threads : int
         Number of processes to be used for parallel execution.
         n_cores = 1 defines no threading (not using Ray).
 
     Returns
     -------
     data: numpy.ndarray
         Filled numpy array including variant names, fitnesses, and encoded sequences.
     non_effective_subs: list
         List of variant names that cannot be used for modelling as they are not effective
         positions in the underlying MSA used for generating local and coupling terms.
     """
-    logger.info(f'{len(variants)} input variants. Encoding variant sequences. '
-                f'This might take some time...')
+    if verbose:
+        logger.info(f'{len(variants)} input variants. Encoding variant sequences using parameters '
+                    f'taken from plmc generated file. This might take some time...')
 
     idxs_nan = np.array([i for i, b in enumerate(np.isnan(fitnesses)) if b])  # find fitness NaNs
     if idxs_nan.size > 0:  # remove NaNs if present
         logger.info(f'Fitness NaNs are: {idxs_nan}')
         fitnesses = np.delete(fitnesses, idxs_nan)
         variants = np.delete(variants, idxs_nan)
 
-    variants_split = np.array_split(variants, threads)    # split array in n_cores pieces
-    fitnesses_split = np.array_split(fitnesses, threads)  # for parallelization
+    variants_split = np.array_split(variants, threads)    # split array in n_cores parts
+    sequences_split = np.array_split(sequences, threads)  # for Ray parallelization
+    fitnesses_split = np.array_split(fitnesses, threads)
     results = ray.get([
         _get_data_parallel.remote(
             variants_split[i],
+            sequences_split[i],
             fitnesses_split[i],
             dca_encode,
             []
         ) for i in range(len(variants_split))
     ])
-    data = [item for sublist in results for item in sublist]  # fusing all the individual results
 
+    data = [item for sublist in results for item in sublist]  # fusing all the individual results
     variants = [item[0] for item in data]
-    encoded_sequences = [item[1] for item in data]
-    fitnesses = [item[2] for item in data]
-
-    logger.info(f'{len(data)} variants after NaN-valued and non-effective '
-                f'site-substituted variant (EffectiveSiteError) dropping.')
+    sequences = [item[1] for item in data]
+    xs = [item[2] for item in data]
+    fitnesses = [item[3] for item in data]
+
+    if verbose:
+        logger.info(f'{len(data)} variants after NaN-valued and non-effective '
+                    f'site-substituted variant (EffectiveSiteError) dropping.')
 
-    return variants, encoded_sequences, fitnesses
+    return variants, sequences, xs, fitnesses
```

### Comparing `pypef-0.2.4/pypef/dca/hybrid_model.py` & `pypef-0.3/pypef/dca/hybrid_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,48 +33,56 @@
 import numpy as np
 import sklearn.base
 from scipy.stats import spearmanr
 from sklearn.linear_model import Ridge
 from sklearn.model_selection import GridSearchCV, train_test_split
 from scipy.optimize import differential_evolution
 
-import pypef.dca.encoding
-from pypef.utils.variant_data import get_sequences_from_file, remove_nan_encoded_positions
-from pypef.dca.encoding import DCAEncoding, get_dca_data_parallel, get_encoded_sequence, EffectiveSiteError
-from pypef.ml.regression import predictions_out, plot_y_true_vs_y_pred
+from pypef.utils.variant_data import (
+    get_sequences_from_file, get_seqs_from_var_name,
+    remove_nan_encoded_positions, get_wt_sequence, split_variants
+)
+
+from pypef.dca.plmc_encoding import PLMC, get_dca_data_parallel, get_encoded_sequence, EffectiveSiteError
+from pypef.utils.to_file import predictions_out
+from pypef.utils.plot import plot_y_true_vs_y_pred
+import pypef.dca.gremlin_inference
+from pypef.dca.gremlin_inference import GREMLIN
 
-# np.warnings.filterwarnings('error', category=np.VisibleDeprecationWarning) # DEV
+# np.warnings.filterwarnings('error', category=np.VisibleDeprecationWarning)  # DEV
 
 
 class DCAHybridModel:
     alphas = np.logspace(-6, 6, 100)  # Grid for the parameter 'alpha'.
     parameter_range = [(0, 1), (0, 1)]  # Parameter range of 'beta_1' and 'beta_2' with lb <= x <= ub
+    # TODO: Implementation of other regression techniques (CVRegression models)
 
     def __init__(
             self,
             alphas=alphas,
             parameter_range=None,
-            X_train: np.ndarray = None,
+            x_train: np.ndarray = None,
             y_train: np.ndarray = None,
-            X_test: np.ndarray = None,  # not necessary for training
+            x_test: np.ndarray = None,  # not necessary for training
             y_test: np.ndarray = None,  # not necessary for training
-            X_wt = None
+            x_wt=None
     ):
         if parameter_range is None:
             parameter_range = parameter_range
         self._alphas = alphas
         self._parameter_range = parameter_range
-        self.X_train = X_train
+        self.x_train = x_train
         self.y_train = y_train
-        self.X_test = X_test
+        self.x_test = x_test
         self.y_test = y_test
-        self.X = np.concatenate((X_train, X_test), axis=0) if self.X_test is not None else self.X_train
+        self.X = np.concatenate((x_train, x_test), axis=0) if self.x_test is not None else self.x_train
         self.y = np.concatenate((y_train, y_test), axis=0) if self.y_test is not None else self.y_train
-        self.x_wild_type = X_wt
+        self.x_wild_type = x_wt
         self._spearmanr_dca = self._spearmanr_dca()
+        self.beta_1, self.beta_2, self.regressor = self.settings(self.x_train, self.y_train)
 
     @staticmethod
     def spearmanr(
             y1: np.ndarray,
             y2: np.ndarray
     ) -> float:
         """
@@ -109,37 +117,37 @@
 
         Returns
         -------
         Standardized version of 'x'.
         """
         return np.subtract(x, np.mean(x, axis=axis)) / np.std(x, axis=axis, ddof=1)
 
-    def _delta_X(
+    def _delta_x(
             self,
-            X: np.ndarray
+            x: np.ndarray
     ) -> np.ndarray:
         """
         Substracts for each variant the encoded wild-type sequence
         from its encoded sequence.
         
         Parameters
         ----------
-        X : np.ndarray
-            Array of encoded variant sequences.
+        x : np.ndarray
+            Array of encoded variant sequences (matrix X).
 
         Returns
         -------
         Array of encoded variant sequences with substracted encoded
         wild-type sequence.
         """
-        return np.subtract(X, self.x_wild_type)
+        return np.subtract(x, self.x_wild_type)
 
-    def _delta_E(
+    def _delta_e(
             self,
-            X: np.ndarray
+            x: np.ndarray
     ) -> np.ndarray:
         """
         Calculates the difference of the statistical energy 'dE'
         of the variant and wild-type sequence.
 
         dE = E (variant) - E (wild-type)
         with E = \sum_{i} h_i (o_i) + \sum_{i<j} J_{ij} (o_i, o_j)
@@ -150,55 +158,55 @@
             Array of the encoded variant sequences.
 
         Returns
         -------
         Difference of the statistical energy between variant 
         and wild-type.
         """
-        return np.sum(self._delta_X(X), axis=1)
+        return np.sum(self._delta_x(x), axis=1)
 
     def _spearmanr_dca(self) -> float:
         """
         Returns
         -------
         Spearman's rank correlation coefficient of the full
         data and the statistical DCA predictions (difference
         of statistical energies). Used to adjust the sign
         of hybrid predictions, i.e.
             beta_1 * y_dca + beta_2 * y_ridge
         or
             beta_1 * y_dca - beta_2 * y_ridge.
         """
-        y_dca = self._delta_E(self.X)
+        y_dca = self._delta_e(self.X)
         return self.spearmanr(self.y, y_dca)
 
     def ridge_predictor(
             self,
-            X_train: np.ndarray,
+            x_train: np.ndarray,
             y_train: np.ndarray,
     ) -> object:
         """
         Sets the parameter 'alpha' for ridge regression.
 
         Parameters
         ----------
-        X_train : np.ndarray
+        x_train : np.ndarray
             Array of the encoded sequences for training.
         y_train : np.ndarray
             Associated fitness values to the sequences present
-            in 'X_train'.
+            in 'x_train'.
 
         Returns
         -------
-        Ridge object trained on 'X_train' and 'y_train' (cv=5)
+        Ridge object trained on 'x_train' and 'y_train' (cv=5)
         with optimized 'alpha'. 
         """
         grid = GridSearchCV(Ridge(), {'alpha': self._alphas}, cv=5)
-        grid.fit(X_train, y_train)
-        return Ridge(**grid.best_params_).fit(X_train, y_train)
+        grid.fit(x_train, y_train)
+        return Ridge(**grid.best_params_).fit(x_train, y_train)
 
     def _y_hybrid(
             self,
             y_dca: np.ndarray,
             y_ridge: np.ndarray,
             beta_1: float,
             beta_2: float
@@ -261,30 +269,30 @@
         """
         loss = lambda b: -np.abs(self.spearmanr(y, b[0] * y_dca + b[1] * y_ridge))
         minimizer = differential_evolution(loss, bounds=self.parameter_range, tol=1e-4)
         return minimizer.x
 
     def settings(
             self,
-            X_train: np.ndarray,
+            x_train: np.ndarray,
             y_train: np.ndarray,
             train_size_fit=0.66,
             random_state=42
     ) -> tuple:
         """
         Get the adjusted parameters 'beta_1', 'beta_2', and the
         tuned regressor of the hybrid model.
 
         Parameters
         ----------
-        X_train : np.ndarray
+        x_train : np.ndarray
             Encoded sequences of the variants in the training set.
         y_train : np.ndarray
             Fitness values of the variants in the training set.
-        X_test : np.ndarray
+        x_test : np.ndarray
             Encoded sequences of the variants in the testing set.
         y_test : np.ndarray
             Fitness values of the variants in the testing set.
         train_size_train : float [0,1] (default 0.66)
             Fraction to split training set into another
             training and testing set.
         random_state : int (default=224)
@@ -293,15 +301,15 @@
         Returns
         -------
         Tuple containing the adjusted parameters 'beta_1' and 'beta_2',
         as well as the tuned regressor of the hybrid model.
         """
         try:
             X_ttrain, X_ttest, y_ttrain, y_ttest = train_test_split(
-                X_train, y_train,
+                x_train, y_train,
                 train_size=train_size_fit,
                 random_state=random_state
             )
 
         except ValueError:
             """
             Not enough sequences to construct a sub-training and sub-testing 
@@ -319,55 +327,55 @@
 
         If this is not given -> return parameter setting for 'EVmutation' model.
         """
         y_ttrain_min_cv = int(0.2 * len(y_ttrain))  # 0.2 because of five-fold cross validation (1/5)
         if y_ttrain_min_cv < 2:
             return 1.0, 0.0, None
 
-        y_dca_ttest = self._delta_E(X_ttest)
+        y_dca_ttest = self._delta_e(X_ttest)
 
         ridge = self.ridge_predictor(X_ttrain, y_ttrain)
         y_ridge_ttest = ridge.predict(X_ttest)
 
         beta1, beta2 = self._adjust_betas(y_ttest, y_dca_ttest, y_ridge_ttest)
         return beta1, beta2, ridge
 
     def hybrid_prediction(
             self,
-            X: np.ndarray,
+            x: np.ndarray,
             reg: object,  # any regression-based estimator (from sklearn)
             beta_1: float,
             beta_2: float
     ) -> np.ndarray:
         """
         Use the regressor 'reg' and the parameters 'beta_1'
         and 'beta_2' for constructing a hybrid model and
         predicting the fitness associates of 'X'.
 
         Parameters
         ----------
-        X : np.ndarray
-            Encoded sequences used for prediction.
+        x : np.ndarray
+            Encoded sequences X used for prediction.
         reg : object
             Tuned ridge regressor for the hybrid model.
         beta_1 : float
             Float for regulating EVmutation model contribution.
         beta_2 : float
             Float for regulating Ridge regressor contribution.
 
         Returns
         -------
         Predicted fitness associates of 'X' using the
         hybrid model.
         """
-        y_dca = self._delta_E(X)
+        y_dca = self._delta_e(x)
         if reg is None:
             y_ridge = np.random.random(len(y_dca))  # in order to suppress error
         else:
-            y_ridge = reg.predict(X)
+            y_ridge = reg.predict(x)
         # adjusting: + or - on all data --> +-beta_1 * y_dca + beta_2 * y_ridge
         return self._y_hybrid(y_dca, y_ridge, beta_1, beta_2)
 
     def split_performance(
             self,
             train_size: float = 0.8,
             n_runs: int = 10,
@@ -395,17 +403,17 @@
             Contains information about hybrid model parameters
             and performance results.
         """
         data = {}
         np.random.seed(seed)
 
         for r, random_state in enumerate(np.random.randint(100, size=n_runs)):
-            X_train, X_test, y_train, y_test = train_test_split(
+            x_train, x_test, y_train, y_test = train_test_split(
                 self.X, self.y, train_size=train_size, random_state=random_state)
-            beta_1, beta_2, reg = self.settings(X_train, y_train)
+            beta_1, beta_2, reg = self.settings(x_train, y_train)
             if beta_2 == 0.0:
                 alpha = np.nan
             else:
                 if save_model:
                     pickle.dumps(reg)
                 alpha = reg.alpha
             data.update(
@@ -413,65 +421,36 @@
                     {
                         'no_run': r,
                         'n_y_train': len(y_train),
                         'n_y_test': len(y_test),
                         'rnd_state': random_state,
                         'spearman_rho': self.spearmanr(
                             y_test, self.hybrid_prediction(
-                                X_test, reg, beta_1, beta_2
+                                x_test, reg, beta_1, beta_2
                             )
                         ),
                         'beta_1': beta_1,
                         'beta_2': beta_2,
                         'alpha': alpha
                     }
                 }
             )
 
         return data
 
-    def ls_ts_performance(
-            self,
-            data=None
-    ):
-        if data is None:
-            data = {}
+    def ls_ts_performance(self):
         beta_1, beta_2, reg = self.settings(
-            X_train=self.X_train,
+            x_train=self.x_train,
             y_train=self.y_train
         )
-        if reg is None:
-            alpha_ = 'None'
-        else:
-            alpha_ = f'{reg.alpha:.3f}'
-        logger.info(f'Beta 1 (DCA): {beta_1:.3f}, Beta 2 (ML): {beta_2:.3f} ( '
-              f'regressor: Ridge(alpha={alpha_}))')
-        if beta_2 == 0.0:
-            alpha = np.nan
-        else:
-            alpha = reg.alpha
-        data.update(
-            {f'ls_ts':
-                {
-                    'n_y_train': len(self.y_train),
-                    'n_y_test': len(self.y_test),
-                    'spearman_rho': self.spearmanr(
-                        self.y_test, self.hybrid_prediction(
-                            self.X_test, reg, beta_1, beta_2
-                        )
-                    ),
-                    'beta_1': beta_1,
-                    'beta_2': beta_2,
-                    'regressor': reg,
-                    'alpha': alpha
-                }
-            }
+        spearman_r = self.spearmanr(
+            self.y_test,
+            self.hybrid_prediction(self.x_test, reg, beta_1, beta_2)
         )
-
-        return data, self.hybrid_prediction(self.X_test, reg, beta_1, beta_2)
+        return spearman_r, reg, beta_1, beta_2
 
     def train_and_test(
             self,
             train_percent_fit: float = 0.66,
             random_state: int = 42
     ):
         """
@@ -508,25 +487,25 @@
             To determine, if spearmanr_dca (i.e. DCA correlation) and measured
             fitness values is positive (>= 0) or negative (< 0).
         test_spearman_r : float
             Achieved performance in terms of Spearman's rank correlation
             between measured and predicted test set variant fitness values.
         """
         beta_1, beta_2, reg = self.settings(
-            X_train=self.X_train,
+            x_train=self.x_train,
             y_train=self.y_train,
             train_size_fit=train_percent_fit,
             random_state=random_state
         )
 
         if len(self.y_test) > 0:
             test_spearman_r = self.spearmanr(
                 self.y_test,
                 self.hybrid_prediction(
-                    self.X_test, reg, beta_1, beta_2
+                    self.x_test, reg, beta_1, beta_2
                 )
             )
         else:
             test_spearman_r = None
         return beta_1, beta_2, reg, self._spearmanr_dca, test_spearman_r
 
     def get_train_sizes(self) -> np.ndarray:
@@ -562,30 +541,291 @@
             training set = train_size and size of the
             test set = N_variants - train_size.
         """
         data = {}
         for t, train_size in enumerate(train_sizes):
             logger.info(f'{t + 1}/{len(train_sizes)}:{train_size}')
             data.update(self.split_performance(train_size=train_size, n_runs=n_runs))
-
         return data
 
 
 """
 Below: Some helper functions that call or are dependent on the DCAHybridModel class.
 """
 
 
+def check_model_type(model: dict | DCAHybridModel | PLMC | GREMLIN):
+    """
+    Checks type/instance of model.
+    """
+    if type(model) == dict:
+        try:
+            model = model['model']
+        except KeyError:
+            raise SystemError("Unknown model dictionary taken from Pickle file.")
+    if type(model) == pypef.dca.plmc_encoding.PLMC:
+        return 'PLMC'
+    elif type(model) == pypef.dca.hybrid_model.DCAHybridModel:
+        return 'Hybrid'
+    elif type(model) == pypef.dca.gremlin_inference.GREMLIN:
+        return 'GREMLIN'
+    elif isinstance(model, sklearn.base.BaseEstimator):
+        raise SystemError("Loaded an sklearn ML model. For pure ML-based modeling the "
+                          "\'ml\' flag has to be used instead of the \'hybrid\' flag.")
+    else:
+        raise SystemError('Unknown model/unknown Pickle file.')
+
+
+def get_model_path(model: str):
+    try:
+        if isfile(model):
+            model_path = model
+        elif isfile(f'Pickles/{model}'):
+            model_path = f'Pickles/{model}'
+        else:
+            raise SystemError("Did not find specified model file.")
+        return model_path
+    except TypeError:
+        raise SystemError("No provided model. "
+                          "Specify a model for DCA-based encoding.")
+
+
+def get_model_and_type(params_file: str, substitution_sep: str = '/'):
+    file_path = get_model_path(params_file)
+    try:
+        with open(file_path, 'rb') as read_pkl_file:
+            model = pickle.load(read_pkl_file)
+            model_type = check_model_type(model)
+    except pickle.UnpicklingError:
+        model_type = 'PLMC_Params'
+
+    if model_type == 'PLMC_Params':
+        model = PLMC(
+            params_file=params_file,
+            separator=substitution_sep,
+            verbose=False
+        )
+        model_type = 'PLMC'
+
+    else:  # --> elif model_type in ['PLMC', 'GREMLIN', 'Hybrid']:
+        model = model['model']
+
+    return model, model_type
+
+
+def save_model_to_dict_pickle(
+        model: DCAHybridModel | PLMC | GREMLIN,
+        model_type: str | None = None,
+        beta_1: float | None = None,
+        beta_2: float | None = None,
+        spearman_r: float | None = None,
+        regressor: sklearn.base.BaseEstimator = None
+):
+    try:
+        os.mkdir('Pickles')
+    except FileExistsError:
+        pass
+
+    if model_type is None:
+        model_type = 'MODEL'
+    # else:
+    #    model_type += '_MODEL'
+    logger.info(f'Save model as Pickle file... {model_type}')
+    pickle.dump(
+        {
+            'model': model,
+            'model_type': model_type,
+            'beta_1': beta_1,
+            'beta_2': beta_2,
+            'spearman_rho': spearman_r,
+            'regressor': regressor
+        },
+        open(f'Pickles/{model_type}', 'wb')
+    )
+
+
+global_model = None
+global_model_type = None
+
+
+def plmc_or_gremlin_encoding(
+        variants,
+        sequences,
+        ys_true,
+        params_file,
+        substitution_sep='/',
+        threads=1,
+        verbose=True,
+        use_global_model=False
+):
+    """
+    Decides based on the params file input type which DCA encoding to be performed, i.e.,
+    GREMLIN or PLMC.
+    If use_global_model==True, to avoid each time pickle model file getting loaded, which
+    is quite inefficient when performing directed evolution, i.e., encoding of single
+    sequences, a global model is stored at the first evolution step and used in the
+    subsequent steps.
+    """
+    global global_model, global_model_type
+    if ys_true is None:
+        ys_true = np.zeros(np.shape(sequences))
+    if use_global_model:
+        if global_model is None:
+            global_model, global_model_type = get_model_and_type(params_file, substitution_sep)
+            model, model_type = global_model, global_model_type
+        else:
+            model, model_type = global_model, global_model_type
+    else:
+        model, model_type = get_model_and_type(params_file, substitution_sep)
+    if model_type == 'PLMC':
+        xs, x_wt, variants, sequences, ys_true = plmc_encoding(
+            model, variants, sequences, ys_true, threads, verbose
+        )
+    elif model_type == 'GREMLIN':
+        if verbose:
+            logger.info(f"Following positions are frequent gap positions in the MSA "
+                        f"and cannot be considered for effective modeling, i.e., "
+                        f"substitutions at these positions are removed as these would be "
+                        f"predicted as wild type:\n{[gap + 1 for gap in model.gaps]}.\n"
+                        f"Effective positions (N={len(model.v_idx)}) are:\n"
+                        f"{[v_pos + 1 for v_pos in model.v_idx]}")
+        xs, x_wt, variants, sequences, ys_true = gremlin_encoding(
+            model, variants, sequences, ys_true,
+            shift_pos=1, substitution_sep=substitution_sep
+        )
+    else:
+        raise SystemError(
+            f"Found a {model_type.lower()} model as input. Please train a new "
+            f"hybrid model on the provided LS/TS datasets."
+        )
+    assert len(xs) == len(variants) == len(sequences) == len(ys_true)
+    return xs, variants, sequences, ys_true, x_wt, model, model_type
+
+
+def gremlin_encoding(gremlin: GREMLIN, variants, sequences, ys_true, shift_pos=1, substitution_sep='/'):
+    """
+     Gets X and x_wt for DCA prediction: delta_Hamiltonian respectively
+     delta_E = np.subtract(X, x_wt), with X = encoded sequences of variants.
+     Also removes variants, sequences, and y_trues at MSA gap positions.
+    """
+    variants, sequences, ys_true = np.atleast_1d(variants), np.atleast_1d(sequences), np.atleast_1d(ys_true)
+    variants, sequences, ys_true = remove_gap_pos(
+        gremlin.gaps, variants, sequences, ys_true,
+        shift_pos=shift_pos, substitution_sep=substitution_sep
+    )
+    try:
+        xs = gremlin.get_score(sequences, encode=True)
+    except SystemError:
+        xs = []
+    x_wt = gremlin.get_score(np.atleast_1d(gremlin.wt_seq), encode=True)
+    return xs, x_wt, variants, sequences, ys_true
+
+
+def plmc_encoding(plmc: PLMC, variants, sequences, ys_true, threads=1, verbose=False):
+    """
+    Gets X and x_wt for DCA prediction: delta_E = np.subtract(X, x_wt),
+    with X = encoded sequences of variants.
+    Also removes variants, sequences, and y_trues at MSA gap positions.
+    """
+    target_seq, index = plmc.get_target_seq_and_index()
+    wt_name = target_seq[0] + str(index[0]) + target_seq[0]
+    if verbose:
+        logger.info(f"Using to-self-substitution '{wt_name}' as wild type reference. "
+                    f"Encoding variant sequences. This might take some time...")
+    x_wt = get_encoded_sequence(wt_name, plmc)
+    if threads > 1:
+        # Hyperthreading, NaNs are already being removed by the called function
+        variants, sequences, xs, ys_true = get_dca_data_parallel(
+            variants, sequences, ys_true, plmc, threads, verbose=verbose)
+    else:
+        x_ = plmc.collect_encoded_sequences(variants)
+        # NaNs must still be removed
+        xs, variants, sequences, ys_true = remove_nan_encoded_positions(
+            x_, variants, sequences, ys_true
+        )
+    return xs, x_wt, variants, sequences, ys_true
+
+
+def remove_gap_pos(
+        gaps,
+        variants,
+        sequences,
+        fitnesses,
+        shift_pos=1,
+        substitution_sep='/'
+):
+    """
+    Remove gap postions from input variants, sequences, and fitness values
+    based on input gaps (gap positions).
+    Note that by default, gap positions are shifted by +1 to match the input
+    variant identifiers (e.g., variant A123C is removed if gap pos is 122; (122 += 1).
+
+    Returns
+    -----------
+    variants_v
+        Variants with substitutions at valid sequence positions, i.e., at non-gap positions
+    sequences_v
+        Sequences of variants with substitutions at valid sequence positions, i.e., at non-gap positions
+    fitnesses_v
+        Fitness values of variants with substitutions at valid sequence positions, i.e., at non-gap positions
+    """
+    variants_v, sequences_v, fitnesses_v = [], [], []
+    valid = []
+    for i, variant in enumerate(variants):
+        variant = variant.split(substitution_sep)
+        for var in variant:
+            if int(var[1:-1]) not in [gap + shift_pos for gap in gaps]:
+                if i not in valid:
+                    valid.append(i)
+                    variants_v.append(variants[i])
+                    sequences_v.append(sequences[i])
+                    fitnesses_v.append(fitnesses[i])
+    return variants_v, sequences_v, fitnesses_v
+
+
+def get_delta_e_statistical_model(
+        x_test: np.ndarray,
+        x_wt: np.ndarray
+):
+    """
+    Description
+    -----------
+    Delta_E means difference in evolutionary energy in plmc terms.
+    In other words, this is the delta of the sum of Hamiltonian-encoded
+    sequences of local fields and couplings of encoded sequence and wild-type
+    sequence in GREMLIN terms.
+
+    Parameters
+    -----------
+    x_test: np.ndarray [2-dim]
+        Encoded sequences to be subtracted by x_wt to compute delta E.
+    x_wt: np.ndarray [1-dim]
+        Encoded wild-type sequence.
+
+    Returns
+    -----------
+    delta_e: np.ndarray [1-dim]
+        Summed subtracted encoded sequences.
+
+    """
+    delta_x = np.subtract(x_test, x_wt)
+    delta_e = np.sum(delta_x, axis=1)
+    return delta_e
+
+
 def generate_model_and_save_pkl(
-        xs: list,
-        ys: list,
-        dca_encoder: DCAEncoding,
+        variants,
+        ys_true,
+        params_file,
+        wt,
         train_percent_fit: float = 0.66,  # percent of all data: 0.8 * 0.66
         test_percent: float = 0.2,
-        random_state: int = 42
+        random_state: int = 42,
+        substitution_sep = '/',
+        threads=1
 ):
     """
     Description
     -----------
     Save (Ridge) regression model (trained and with tuned alpha parameter)
     with betas (beta_1 and beta_2) as dictionary-structured pickle file.
 
@@ -598,44 +838,43 @@
         Percent of DataFrame data to train on.
         The remaining data is used for validation.
     random_state: int
         Random seed for splitting in train and test data for reproducing results.
 
     Returns
     ----------
-    None
+    ()
         Just saving model parameters as pickle file.
     """
+    wt_seq = get_wt_sequence(wt)
+    variants_splitted = split_variants(variants, substitution_sep)
+    variants, ys_true, sequences = get_seqs_from_var_name(wt_seq, variants_splitted, ys_true)
 
-    # getting target (WT) sequence and encoding it to provide it as
-    # relative value for pure DCA based predictions (difference in sums
-    # of sequence encodings: variant - WT)
-    target_seq, index = dca_encoder.get_target_seq_and_index()
-    wt_name = target_seq[0] + str(index[0]) + target_seq[0]
-    x_wt = get_encoded_sequence(wt_name, dca_encoder)
+    xs, variants, sequences, ys_true, x_wt, model, model_type = plmc_or_gremlin_encoding(
+        variants, sequences, ys_true, params_file, substitution_sep, threads)
 
     logger.info(
-        f'Train size (fitting): {train_percent_fit*100:.1f} % of training data '
-        f'({((1 - test_percent)*train_percent_fit)*100:.1f} % of all data),\n'
-        f'Train size validation: {(1 - train_percent_fit)*100:.1f} % of training data '
-        f'({((1 - test_percent)*(1 - train_percent_fit))*100:.1f} % of all data),\n'
-        f'Test size: {test_percent*100:.1f} % ({test_percent*100:.1f} % of all data),\n'
-        f'(Random state: {random_state})...\n'
+        f'Train size (fitting): {train_percent_fit * 100:.1f} % of training data '
+        f'({((1 - test_percent) * train_percent_fit) * 100:.1f} % of all data)\n'
+        f'Train size validation: {(1 - train_percent_fit) * 100:.1f} % of training data '
+        f'({((1 - test_percent) * (1 - train_percent_fit)) * 100:.1f} % of all data)\n'
+        f'Test size: {test_percent * 100:.1f} % ({test_percent * 100:.1f} % of all data)\n'
+        f'Using random state: {random_state}...\n'
     )
 
-    X_train, X_test, y_train, y_test = train_test_split(
-        xs, ys, test_size=test_percent, random_state=random_state
+    x_train, x_test, y_train, y_test = train_test_split(
+        xs, ys_true, test_size=test_percent, random_state=random_state
     )
 
     hybrid_model = DCAHybridModel(
-        X_train=X_train,
+        x_train=x_train,
         y_train=y_train,
-        X_test=X_test,
+        x_test=x_test,
         y_test=y_test,
-        X_wt=x_wt
+        x_wt=x_wt
     )
 
     beta_1, beta_2, reg, spearman_dca, test_spearman_r = hybrid_model.train_and_test(
         train_percent_fit=train_percent_fit,
         random_state=random_state
     )
     if reg is None:
@@ -649,77 +888,26 @@
         f'regressor: Ridge(alpha={alpha_}))\n'
         f'Test performance: Spearman\'s rho = {test_spearman_r:.3f}'
     )
     try:
         os.mkdir('Pickles')
     except FileExistsError:
         pass
-    logger.info(f'Save model as Pickle file... HYBRIDMODEL')
-    pickle.dump(
-        {
-            'model': hybrid_model,
-            'beta_1': beta_1,
-            'beta_2': beta_2,
-            'spearman_rho': test_spearman_r,
-            'regressor': reg
-        },
-        open('Pickles/HYBRIDMODEL', 'wb')
-    )
-
-
-def check_model_type(model):
-    """
-    Checks type/instance of loaded Pickle file.
-    """
-    if type(model) == pypef.dca.encoding.DCAEncoding:
-        return 'DCAMODEL'
-    elif type(model) == pypef.dca.hybrid_model.DCAHybridModel:
-        return 'HYBRIDMODEL'
-    elif isinstance(model, sklearn.base.BaseEstimator):
-        raise SystemError("Loaded an sklearn ML model. For pure ML-based modeling the "
-                          "\'ml\' flag has to be used instead of the \'hybrid\' flag.")
-    else:
-        raise SystemError('Unknown model/unknown Pickle file.')
-
-
-def get_delta_e_statistical_model(
-        x_test: np.ndarray,
-        x_wt: np.ndarray
-):
-    """
-    Description
-    -----------
-
-
-    Parameters
-    -----------
-    x_test: np.ndarray [2-dim]
-        Encoded sequences to be subtracted by x_wt to compute delta E.
-    x_wt: np.ndarray [1-dim]
-        Encoded wild-type sequence.
-
-    Returns
-    -----------
-    delta_e: np.ndarray [1-dim]
-        Summed subtracted encoded sequences.
-
-    """
-    delta_x = np.subtract(x_test, x_wt)
-    delta_e = np.sum(delta_x, axis=1)
-
-    return delta_e
-
+    model_name = f'HYBRID{model_type.lower()}'
+    save_model_to_dict_pickle(hybrid_model, model_name, beta_1, beta_2, test_spearman_r, reg)
 
 
 def performance_ls_ts(
         ls_fasta: str | None,
         ts_fasta: str | None,
         threads: int,
         params_file: str,
-        separator: str
+        model_pickle_file: str | None = None,
+        substitution_sep: str = '/',
+        label=False
 ):
     """
     Description
     -----------
     Computes performance based on a (linear) regression model trained
     on the training set by optimizing model hyperparameters based on
     validation performances on training subsets (default: 5-fold CV)
@@ -736,139 +924,121 @@
         of the tuned regressor for test set entries (performance metric of
         measured and predicted fitness values).
     threads: int
         Number of threads to use for parallel computing using Ray.
     params_file: str
         PLMC parameter file (containing evolutionary, i.e. MSA-based local
         and coupling terms.
+    model: str
+        Model to load for TS prediction.
     separator: str
         Character to split the variant to obtain the single substitutions
         (default='/').
 
-
     Returns
     -----------
     None
         Just plots test results (predicted fitness vs. measured fitness)
         using def plot_y_true_vs_y_pred.
     """
-    dca_encoder = DCAEncoding(
-        params_file=params_file,
-        separator=separator,
-        verbose=False
-    )
-    # DCA prediction: delta E = np.subtract(X, self.x_wild_type),
-    # with X = encoded sequence of any variant -->
-    # getting wild-type name und subsequently x_wild_type
-    # to provide it for the DCAHybridModel
-    target_seq, index = dca_encoder.get_target_seq_and_index()
-    wt_name = target_seq[0] + str(index[0]) + target_seq[0]
-    logger.info(f'Using to-self-substitution \'{wt_name}\' as wild type reference.')
-    x_wt = get_encoded_sequence(wt_name, dca_encoder)
+    test_sequences, test_variants, y_test = get_sequences_from_file(ts_fasta)
+
     if ls_fasta is not None and ts_fasta is not None:
-        _, train_variants, y_train = get_sequences_from_file(ls_fasta)
-        _, test_variants, y_test = get_sequences_from_file(ts_fasta)
+        train_sequences, train_variants, y_train = get_sequences_from_file(ls_fasta)
+        x_train, train_variants, train_sequences, y_train, x_wt, _, model_type = plmc_or_gremlin_encoding(
+            train_variants, train_sequences, y_train, params_file, substitution_sep, threads
+        )
 
-        if threads > 1:
-            # Hyperthreading, NaNs are already being removed by the called function
-            train_variants, x_train, y_train = get_dca_data_parallel(
-                train_variants, y_train, dca_encoder, threads)
-            test_variants, x_test, y_test = get_dca_data_parallel(
-                test_variants, y_test, dca_encoder, threads)
-        else:
-            x_train_ = dca_encoder.collect_encoded_sequences(train_variants)
-            x_test_ = dca_encoder.collect_encoded_sequences(test_variants)
-            # NaNs must still be removed
-            x_train, train_variants, y_train = remove_nan_encoded_positions(x_train_, train_variants, y_train)
-            x_test, test_variants, y_test = remove_nan_encoded_positions(x_test_, test_variants, y_test)
-        assert len(x_train) == len(train_variants) == len(y_train)
-        assert len(x_test) == len(test_variants) == len(y_test)
+        x_test, test_variants, test_sequences, y_test, *_ = plmc_or_gremlin_encoding(
+            test_variants, test_sequences, y_test, params_file, substitution_sep, threads, verbose=False
+        )
+
+        logger.info(f"\nInitial training set variants: {len(train_sequences)}. "
+                    f"Remaining: {len(train_variants)} (after removing "
+                    f"substitutions at gap positions).\nInitial test set "
+                    f"variants: {len(test_sequences)}. Remaining: {len(test_variants)} "
+                    f"(after removing substitutions at gap positions)."
+                    )
 
         hybrid_model = DCAHybridModel(
-            X_train=np.array(x_train),
+            x_train=np.array(x_train),
             y_train=np.array(y_train),
-            X_test=np.array(x_test),
+            x_test=np.array(x_test),
             y_test=np.array(y_test),
-            X_wt=x_wt
+            x_wt=x_wt
         )
-        data, y_pred = hybrid_model.ls_ts_performance()
-        result = data['ls_ts']
-        test_spearman_r = result['spearman_rho']
-        beta_1 = result['beta_1']
-        beta_2 = result['beta_2']
-        reg = result['regressor']
+        model_name = f'HYBRID{model_type.lower()}'
+
+        spearman_r, reg, beta_1, beta_2 = hybrid_model.ls_ts_performance()
+        ys_pred = hybrid_model.hybrid_prediction(np.array(x_test), reg, beta_1, beta_2)
+
         if reg is None:
             alpha_ = 'None'
         else:
             alpha_ = f'{reg.alpha:.3f}'
         logger.info(
             f'Individual model weights and regressor hyperparameters:\n'
             f'Hybrid model individual model contributions: Beta1 (DCA): '
             f'{beta_1:.3f}, Beta2 (ML): {beta_2:.3f} (regressor: '
-            f'Ridge(alpha={alpha_}))\nTesting performance...\nSpearman\'s '
-            f'rho = {test_spearman_r:.3f}'
-        )
-        try:
-            os.mkdir('Pickles')
-        except FileExistsError:
-            pass
-        logger.info(f'Save model as Pickle file... HYBRIDMODEL')
-        pickle.dump(
-            {
-                'model': hybrid_model,
-                'beta_1': beta_1,
-                'beta_2': beta_2,
-                'spearman_rho': test_spearman_r,
-                'regressor': reg
-            },
-            open('Pickles/HYBRIDMODEL', 'wb')
+            f'Ridge(alpha={alpha_}))\nTesting performance...'
         )
 
-    elif ts_fasta is not None:
-        logger.info('No learning set provided, falling back to statistical DCA model: '
-                    'no adjustments of individual hybrid model parameters (beta_1 and beta_2).')
-        _, test_variants, y_test = get_sequences_from_file(ts_fasta)
-        if threads > 1:
-            test_variants, x_test, y_test = get_dca_data_parallel(
-                test_variants, y_test, dca_encoder, threads)
-        else:
-            x_test_ = dca_encoder.collect_encoded_sequences(test_variants)
-            x_test, y_test, test_variants = remove_nan_encoded_positions(x_test_, y_test, test_variants)
+        save_model_to_dict_pickle(hybrid_model, model_name, beta_1, beta_2, spearman_r, reg)
 
-        delta_e = get_delta_e_statistical_model(x_test, x_wt)
+    elif ts_fasta is not None and model_pickle_file is not None and params_file is not None:
+        logger.info(f'Taking model from saved model (Pickle file): {model_pickle_file}...')
 
-        spearman_rho = spearmanr(y_test, delta_e)
-        logger.info(f'Spearman Rho = {spearman_rho[0]:.3f}')
+        model, model_type = get_model_and_type(model_pickle_file)
 
-        logger.info(f'Save model as Pickle file... DCAMODEL')
-        pickle.dump(
-            {
-                'model': dca_encoder,
-                'beta_1': None,
-                'beta_2': None,
-                'spearman_rho': spearman_rho,
-                'regressor': None
-            },
-            open('Pickles/DCAMODEL', 'wb')
+        if model_type != 'Hybrid':  # same as below in next elif
+            x_test, test_variants, test_sequences, y_test, x_wt, *_ = plmc_or_gremlin_encoding(
+                test_variants, test_sequences, y_test, model_pickle_file, substitution_sep, threads, False)
+            ys_pred = get_delta_e_statistical_model(x_test, x_wt)
+        else:  # Hybrid model input requires params from plmc or GREMLIN model
+            beta_1, beta_2, reg = model.beta_1, model.beta_2, model.regressor
+            x_test, test_variants, test_sequences, y_test, *_ = plmc_or_gremlin_encoding(
+                test_variants, test_sequences, y_test, params_file,
+                substitution_sep, threads, False
+            )
+            ys_pred = model.hybrid_prediction(x_test, reg, beta_1, beta_2)
+
+    elif ts_fasta is not None and model_pickle_file is None:  # no LS provided --> statistical modeling / no ML
+        logger.info(f'No learning set provided, falling back to statistical DCA model: '
+                    f'no adjustments of individual hybrid model parameters (beta_1 and beta_2).')
+        test_sequences, test_variants, y_test = get_sequences_from_file(ts_fasta)
+        x_test, test_variants, test_sequences, y_test, x_wt, model, model_type = plmc_or_gremlin_encoding(
+            test_variants, test_sequences, y_test, params_file, substitution_sep, threads
         )
 
+        logger.info(f"Initial test set variants: {len(test_sequences)}. "
+                    f"Remaining: {len(test_variants)} (after removing "
+                    f"substitutions at gap positions).")
+
+        ys_pred = get_delta_e_statistical_model(x_test, x_wt)
+
+        save_model_to_dict_pickle(model, model_type, None, None, spearmanr(y_test, ys_pred)[0], None)
+
     else:
-        logger.info('No Test Set given for performance estimation.')
+        raise SystemError('No Test Set given for performance estimation.')
+
+    spearman_rho = spearmanr(y_test, ys_pred)
+    logger.info(f'Spearman Rho = {spearman_rho[0]:.3f}')
+
+    plot_y_true_vs_y_pred(
+        np.array(y_test), np.array(ys_pred), np.array(test_variants), label=label, hybrid=True
+    )
 
 
-def predict_ps(  # also predicting "pmult" dirs
+def predict_ps(  # also predicting "pmult" dict directories
         prediction_dict: dict,
-        params_file: str,
         threads: int,
         separator: str,
         model_pickle_file: str,
-        test_set: str = None,
+        params_file: str = None,
         prediction_set: str = None,
-        figure: str = None,
-        label: bool = False,
         negative: bool = False
 ):
     """
     Description
     -----------
     Predicting the fitness of sequences of a prediction set
     or multiple prediction sets that were exemplary created with
@@ -906,190 +1076,138 @@
     negative: bool = False
         If true, negative defines improved variants having a reduced/negative
         fitness compared to wild type.
 
 
     Returns
     -----------
-    None
+    ()
         Writes sorted predictions to files (for [--drecomb] [--trecomb]
         [--qarecomb] [--qirecomb] [--ddiverse] [--tdiverse] [--qdiverse]
         in the respective created folders).
 
     """
-    if threads > 1:  # silent DCA encoding
-        dca_encoder = DCAEncoding(params_file, separator=separator, verbose=False)
-    else:
-        dca_encoder = DCAEncoding(params_file, separator=separator)
-    logger.info(f'Taking regression model from saved model (Pickle file): {model_pickle_file}...')
-    model_data = pickle.load(open(f'Pickles/{model_pickle_file}', "rb"))
-    model = model_data['model']
-    test_spearman_r = model_data['spearman_rho']
-    beta_1 = model_data['beta_1']
-    beta_2 = model_data['beta_2']
-    reg = model_data['regressor']
+    logger.info(f'Taking model from saved model (Pickle file): {model_pickle_file}...')
 
-    if check_model_type(model) == 'DCAMODEL':
-        pass
-    elif check_model_type(model) == 'HYBRIDMODEL':
+    model, model_type = get_model_and_type(model_pickle_file)
+
+    if model_type == 'PLMC':
+        logger.info(f'No hybrid model provided – falling back to a statistical DCA model.')
+    elif model_type == 'Hybrid':
+        beta_1, beta_2, reg = model.beta_1, model.beta_2, model.regressor
         if reg is None:
             alpha_ = 'None'
         else:
             alpha_ = f'{reg.alpha:.3f}'
         logger.info(
             f'Individual model weights and regressor hyperparameters:\n'
             f'Hybrid model individual model contributions: Beta1 (DCA): {beta_1:.3f}, '
-            f'Beta2 (ML): {beta_2:.3f} (regressor: Ridge(alpha={alpha_})), '
-            f'Train->Test performance: Spearman\'s rho = {test_spearman_r:.3f}.'
+            f'Beta2 (ML): {beta_2:.3f} (regressor: Ridge(alpha={alpha_})).'
         )
 
     pmult = [
         'Recomb_Double_Split', 'Recomb_Triple_Split', 'Recomb_Quadruple_Split',
         'Recomb_Quintuple_Split', 'Diverse_Double_Split', 'Diverse_Triple_Split',
         'Diverse_Quadruple_Split'
     ]
     if True in prediction_dict.values():
         for ps, path in zip(prediction_dict.values(), pmult):
             if ps:  # if True, run prediction in this directory, e.g. for drecomb
                 logger.info(f'Running predictions for variant-sequence files in directory {path}...')
                 all_y_v_pred = []
                 files = [f for f in listdir(path) if isfile(join(path, f)) if f.endswith('.fasta')]
                 for i, file in enumerate(files):  # collect and predict for each file in the directory
-                    logger.info(f'Encoding files ({i+1}/{len(files)}) for prediction...\n')
+                    logger.info(f'Encoding files ({i + 1}/{len(files)}) for prediction...\n')
                     file_path = os.path.join(path, file)
                     sequences, variants, _ = get_sequences_from_file(file_path)
-                    if threads > 1:  # parallel execution
-                        # NaNs are already being removed by the called function
-                        variants, xs, _ = get_dca_data_parallel(
-                            variants, list(np.zeros(len(variants))), dca_encoder, threads)
-                    else:  # single thread execution
-                        xs = dca_encoder.collect_encoded_sequences(variants)
-                        # NaNs must still be removed
-                        xs, variants = remove_nan_encoded_positions(xs, variants)
-                    assert len(xs) == len(variants)
-                    if check_model_type(model) == 'DCAMODEL':
-                        target_seq, index = dca_encoder.get_target_seq_and_index()
-                        wt_name = target_seq[0] + str(index[0]) + target_seq[0]
-                        x_wt = get_encoded_sequence(wt_name, dca_encoder)
-                        ys_pred = get_delta_e_statistical_model(xs, x_wt)
-                    elif check_model_type(model) == 'HYBRIDMODEL':
-                        ys_pred = model.hybrid_prediction(xs, reg, beta_1, beta_2)
+                    if model_type != 'Hybrid':
+                        x_test, test_variants, x_wt, *_ = plmc_or_gremlin_encoding(
+                            variants, sequences, None, model, threads=threads, verbose=False,
+                            substitution_sep=separator)
+                        ys_pred = get_delta_e_statistical_model(x_test, x_wt)
+                    else:  # Hybrid model input requires params from plmc or GREMLIN model
+                        ##encoding_model, encoding_model_type = get_model_and_type(params_file)
+                        x_test, test_variants, *_ = plmc_or_gremlin_encoding(
+                            variants, sequences, None, params_file,
+                            threads=threads, verbose=False, substitution_sep=separator
+                        )
+                        ys_pred = model.hybrid_prediction(x_test, reg, beta_1, beta_2)
                     for k, y in enumerate(ys_pred):
                         all_y_v_pred.append((ys_pred[k], variants[k]))
                 if negative:  # sort by fitness value
                     all_y_v_pred = sorted(all_y_v_pred, key=lambda x: x[0], reverse=False)
                 else:
                     all_y_v_pred = sorted(all_y_v_pred, key=lambda x: x[0], reverse=True)
                 predictions_out(
                     predictions=all_y_v_pred,
-                    model='hybrid',
-                    prediction_set=prediction_set,
+                    model='Hybrid',
+                    prediction_set=f'Top{path}',
                     path=path
                 )
-            else:  # check next task to do, e.g. predicting triple substituted variants, e.g. trecomb
+            else:  # check next task to do, e.g., predicting triple substituted variants, e.g. trecomb
                 continue
 
     elif prediction_set is not None:
         sequences, variants, _ = get_sequences_from_file(prediction_set)
         # NaNs are already being removed by the called function
-        if threads > 1:
-            # NaNs are already being removed by the called function
-            variants, xs, _ = get_dca_data_parallel(
-                variants, list(np.zeros(len(variants))), dca_encoder, threads)
-        else:
-            xs = dca_encoder.collect_encoded_sequences(variants)
-            # NaNs must still be removed
-            xs, variants = remove_nan_encoded_positions(xs, variants)
-        assert len(xs) == len(variants)
-        if prediction_set is not None:
-            if check_model_type(model) == 'DCAMODEL':
-                target_seq, index = dca_encoder.get_target_seq_and_index()
-                wt_name = target_seq[0] + str(index[0]) + target_seq[0]
-                x_wt = get_encoded_sequence(wt_name, dca_encoder)
-                y_pred = get_delta_e_statistical_model(xs, x_wt)
-            elif check_model_type(model) == 'HYBRIDMODEL':
-                y_pred = model.hybrid_prediction(xs, reg, beta_1, beta_2)
-            y_v_pred = zip(y_pred, variants)
-            y_v_pred = sorted(y_v_pred, key=lambda x: x[0], reverse=True)
-            predictions_out(
-                predictions=y_v_pred,
-                model='hybrid',
-                prediction_set=prediction_set
-            )
-    elif test_set is not None or figure is not None:
-        if test_set is not None:
-            loaded_set = test_set
-        else:
-            loaded_set = figure
-        sequences, variants, y_true = get_sequences_from_file(loaded_set)
-        # NaNs are already being removed by the called function
-        try:
-            if threads > 1:
-                variants, xs, y_test = get_dca_data_parallel(
-                    variants, y_true, dca_encoder, threads)
-            else:
-                # NaNs must still be removed
-                xs_ = dca_encoder.collect_encoded_sequences(variants)
-                xs, variants, y_test = remove_nan_encoded_positions(xs_, variants, y_true)
-            assert len(xs) == len(variants) == len(y_test)
-        except IndexError:
-            raise SystemError(
-                "Potentially, you provided a prediction set for plotting the figure "
-                "instead of a test set (including measured fitness values, i.e. y_true)."
+        if model_type != 'Hybrid':  # statistical DCA model
+            xs, variants, _, _, x_wt, *_ = plmc_or_gremlin_encoding(
+                variants, sequences, None, params_file,
+                threads=threads, verbose=False, substitution_sep=separator)
+            ys_pred = get_delta_e_statistical_model(xs, x_wt)
+        else:  # Hybrid model input requires params from plmc or GREMLIN model
+            xs, variants, *_ = plmc_or_gremlin_encoding(
+                variants, sequences, None, params_file,
+                threads=threads, verbose=True, substitution_sep=separator
             )
-        if check_model_type(model) == 'DCAMODEL':
-            target_seq, index = dca_encoder.get_target_seq_and_index()
-            wt_name = target_seq[0] + str(index[0]) + target_seq[0]
-            x_wt = get_encoded_sequence(wt_name, dca_encoder)
-            y_pred = get_delta_e_statistical_model(xs, x_wt)
-        elif check_model_type(model) == 'HYBRIDMODEL':
-            y_pred = model.hybrid_prediction(xs, reg, beta_1, beta_2)
-        logger.info('Testing performance...\n'
-                    f'Spearman\'s rho = {spearmanr(y_test, y_pred)[0]:.3f} (N_test = {len(y_pred)})')
-        if figure is not None:
-            plot_y_true_vs_y_pred(
-                np.array(y_test), np.array(y_pred), np.array(variants), label, hybrid=True
-            )
-    else:
-        raise SystemError(
-            'Define set(s) for prediction (e.g. \'-p PS.fasta\' or '
-            'created prediction set folder, e.g. \'--pmult --drecomb\')'
+            ys_pred = model.hybrid_prediction(xs, reg, beta_1, beta_2)
+        assert len(xs) == len(variants)
+        y_v_pred = zip(ys_pred, variants)
+        y_v_pred = sorted(y_v_pred, key=lambda x: x[0], reverse=True)
+        predictions_out(
+            predictions=y_v_pred,
+            model='Hybrid',
+            prediction_set=f'Top{prediction_set}'
         )
 
 
 def predict_directed_evolution(
-        encoder: DCAEncoding,
+        encoder: str,
         variant: str,
+        sequence: str,
         hybrid_model_data_pkl: str
 ) -> Union[str, list]:
     """
     Perform directed in silico evolution and predict the fitness of a
     (randomly) selected variant using the hybrid model. This function opens
     the stored DCAHybridModel and the model parameters to predict the fitness
-    of the variant encoded herein using the DCAEncoding class. If the variant
+    of the variant encoded herein using the PLMC class. If the variant
     cannot be encoded (based on the PLMC params file), returns 'skip'. Else,
     returning the predicted fitness value and the variant name.
     """
-    try:
-        x = encoder.encode_variant(variant)
-    except EffectiveSiteError:
-        return 'skip'
-
-    model_dict = pickle.load(open(os.path.join('Pickles', hybrid_model_data_pkl), "rb"))
-    model = model_dict['model']
-    reg = model_dict['regressor']
-    beta_1 = model_dict['beta_1']
-    beta_2 = model_dict['beta_2']
-    if check_model_type(model) == 'DCAMODEL':
-        target_seq, index = encoder.get_target_seq_and_index()
-        wt_name = target_seq[0] + str(index[0]) + target_seq[0]
-        x_wt = get_encoded_sequence(wt_name, encoder)
-        y_pred = get_delta_e_statistical_model(np.atleast_2d(x), x_wt)[0]  # [0] only for unpacking from list
-    elif check_model_type(model) == 'HYBRIDMODEL':
-        y_pred = model.hybrid_prediction(  # 2d as only single variant
-            X=np.atleast_2d(x),  # e.g., np.atleast_2d(3.0) --> array([[3.]])
-            reg=reg,  # RidgeRegressor
-            beta_1=beta_1,  # DCA model prediction weight
-            beta_2=beta_2  # ML model prediction weight
-        )[0]  # [0] only for unpacking from list
+    if hybrid_model_data_pkl is not None:
+        model, model_type = get_model_and_type(hybrid_model_data_pkl)
+    else:
+        model_type = 'StatisticalModel'  # any name != 'Hybrid'
+
+    if model_type != 'Hybrid':  # statistical DCA model
+        xs, variant, _, _, x_wt, *_ = plmc_or_gremlin_encoding(
+            variant, sequence, None, encoder, verbose=False, use_global_model=True)
+        if not list(xs):
+            return 'skip'
+        y_pred = get_delta_e_statistical_model(xs, x_wt)
+    else:  # model_type == 'Hybrid': Hybrid model input requires params from PLMC or GREMLIN model
+        xs, variant, *_ = plmc_or_gremlin_encoding(
+            variant, sequence, None, encoder, verbose=False, use_global_model=True
+        )
+        if not list(xs):
+            return 'skip'
+        try:
+            y_pred = model.hybrid_prediction(np.atleast_2d(xs), model.regressor, model.beta_1, model.beta_2)[0]
+        except ValueError:
+            raise SystemError(
+                "Probably a different model was used for encoding than for modeling; "
+                "e.g. using a HYBRIDgremlin model in combination with parameters taken from a PLMC file."
+            )
+    y_pred = float(y_pred)
 
-    return [(y_pred, variant[1:])]
+    return [(y_pred, variant[0][1:])]
```

### Comparing `pypef-0.2.4/pypef/main.py` & `pypef-0.3/pypef/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 Modeling options
 ----------------
     I. Pure ML modeling
     -------------------
         PyPEF provides three encoding options for training machine learning models, i.e.
         regression models trained by supervised learning:
 
-            1. DCA: Direct coupling analysis (DCA) based on evolutionary couplings (input
-                       coupling parameter file generated by the C framework PLMC).
+            1. DCA: Direct coupling analysis (DCA) based on evolutionary couplings (input:
+                       coupling parameter file generated by the C framework plmc) or
+                       generating parameters using TensorFlow-based GREMLIN (input: MSA).
 
             2. AAidx: Based on AAindex descriptors (566 amino acid descriptor files
                        taken from the AAindex database).
 
             3. OneHot: One-hot encoding representing the occurrence of an
                        amino acid at a sequence position as a single 1 and 19 0's.
 
@@ -58,166 +59,179 @@
 
     II. Hybrid modeling
     -------------------
         Constructing a hybrid model that combines pure statistical DCA-based prediction (a
         variant's relative 'evolutionary energy' to the wild type) and DCA-encoding based
         training of a ML model similar to pure ML modeling option I.1.
         Based on features generated from the direct coupling analysis (.params file output
-        using the plmc framework). Individual model contributions are optimization only based on
-        Spearman's correlation coefficient and thus, only variant fitness ranks are to be considered
-        for evaluating model performance, not the exact predicted fitness value. For regression,
+        using the plmc framework or provided MSA and running GREMLIN).
+        Individual model contributions are optimization only based on Spearman's correlation
+        coefficient and thus, only variant fitness ranks are to be considered for evaluating
+        model performance, not the exact predicted fitness value. For regression, up to now
         only L2-regularized linear regression (Ridge regression) is provided as modeling option.
 
 
-Running example of training, testing, and inferring a pure ML model for predictions
------------------------------------------------------------------------------------
+Running example of training, testing, and using a pure ML model for prediction
+------------------------------------------------------------------------------
 Exemplary running of PyPEF for training a pure ML model using encoding option 2
 based on features generated from the AAIndex database (566 amino acid descriptor
 indices taken from the AAIndex database).
  1. Create files for training and testing from variant-fitness CSV data:
        pypef mklsts -i variant_and_fitness.csv -w wt_sequence.fasta
  2. Train and validate models:
-        pypef ml -e aaidx -l LS.fasta -t TS.fasta --regressor pls
- 3. Plot the test set entries against test set predictions (creates PNG figure, MODEL12345 is
-    the chosen AAindex, e.g. FAUJ880104):
-        pypef ml -e aaidx -m MODEL12345 -f TS.fasta --label
+        pypef ml -e onehot -l LS.fasta -t TS.fasta --regressor pls
+ 3. Plot the test set entries against test set predictions (creates PNG figure, MODEL is
+    the chosen AAindex, the ML-DCA model, or here the ONEHOT model):
+        pypef ml -e onehot -m ONEHOT -t TS.fasta
  4. Create files for prediction:
     - Single file:
         pypef mkps -w wt_sequence.fasta -i variant_fitness.csv
     - Recombinant/diverse prediction files:
         pypef mkps -w wt_sequence.fasta -i variant_fitness.csv
             [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
             [--ddiverse] [--tdiverse] [--qdiverse]
  5. Predict (unknown/new) variants:
     - Single file:
-        pypef ml -e aaidx -m MODEL12345 -p Prediction_Set.fasta
+        pypef ml -e aaidx -m MODEL -p Prediction_Set.fasta
     - Recombinant/diverse prediction files in created prediction set folders:
-        pypef ml -e aaidx -m MODEL12345 --pmult [--drecomb] [...] [--qdiverse]
+        pypef ml -e aaidx -m MODEL --pmult [--drecomb] [...] [--qdiverse]
     - Directed evolution – for performing and plotting in silico evolution trajectories:
-        pypef ml -e aaidx directevo -m MODEL12345 [...]
+        pypef ml -e aaidx directevo -m MODEL [...]
 Note: The commands for hybrid modeling are very similar to the commands for pure ML modeling,
-see pypef [-h] for possible commands.
+see pypef -h for possible commands.
 
+For generating DCA parameters using GREMLIN, you have to provide an MSA in FASTA or A2M format:
+pypef param_inference --msa MSA_FILE --wt WT_FASTA [--opt_iter 100]
 
-Additional helpful commands for data conversion
+
+Helpful commands for data conversion
 -----------------------------------------------
 Creation of learning and test sets – splitting CSV variant-fitness data:
-        pypef mklsts --wt WT_SEQ --input CSV_FILE
+        pypef mklsts --wt WT_FASTA --input CSV_FILE
             [--drop THRESHOLD] [--numrnd NUMBER]
 
 Creation of prediction sets from CSV data (using single-substituted variant data):
-        pypef mkps --wt WT_SEQ --input CSV_FILE
+        pypef mkps --wt WT_FASTA --input CSV_FILE
             [--drop THRESHOLD] [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
             [--ddiverse] [--tdiverse] [--qdiverse]
 
 Encoding a CSV file (for further performance studies such as "low N" or
 "mutational extrapolation" engineering tasks:
-        pypef encode --input CSV_FILE --encoding ENCODING_TECHNIQUE --wt WT_SEQ
-            [--params PLMC_FILE] [--y_wt WT_FITNESS] [--model MODEL12345] [--nofft]
+        pypef encode --input CSV_FILE --encoding ENCODING_TECHNIQUE --wt WT_FASTA
+            [--params PARAM_FILE] [--y_wt WT_FITNESS] [--model MODEL] [--nofft]
             [--threads THREADS] [--sep CSV_COLUMN_SEPARATOR] [--fitness_key FITNESS_KEY]
 
 Converting a STO alignment file to A2M format:
         pypef sto2a2m --sto STO_MSA_FILE
             [--inter_gap INTER_GAP] [--intra_gap INTRA_GAP]
 
 
 Usage:
-    pypef mklsts --wt WT_SEQ --input CSV_FILE
-        [--drop THRESHOLD] [--numrnd NUMBER]
-    pypef mkps --wt WT_SEQ --input CSV_FILE
-        [--drop THRESHOLD] [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
+    pypef mklsts --wt WT_FASTA --input CSV_FILE
+        [--drop THRESHOLD] [--sep CSV_COLUMN_SEPARATOR] [--mutation_sep MUTATION_SEPARATOR] [--numrnd NUMBER]
+    pypef mkps --wt WT_FASTA [--input CSV_FILE]
+        [--drop THRESHOLD] [--ssm] [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
         [--ddiverse] [--tdiverse] [--qdiverse]
-    pypef encode --input CSV_FILE --encoding ENCODING_TECHNIQUE --wt WT_SEQ
-        [--params PLMC_FILE] [--y_wt WT_FITNESS] [--model MODEL12345] [--nofft]
+    pypef param_inference
+        [--msa MSA_FILE] [--params PARAM_FILE]
+        [--wt WT_FASTA] [--opt_iter N_ITER]
+    pypef save_msa_info --msa MSA_FILE --wt WT_FASTA
+        [--opt_iter N_ITER]
+    pypef encode --input CSV_FILE --encoding ENCODING_TECHNIQUE --wt WT_FASTA
+        [--params PARAM_FILE] [--y_wt WT_FITNESS] [--model MODEL] [--nofft]
         [--threads THREADS]
         [--sep CSV_COLUMN_SEPARATOR] [--fitness_key FITNESS_KEY]
+    pypef reformat_csv --input CSV_FILE
+        [--sep CSV_COLUMN_SEPARATOR] [--mutation_sep MUTATION_SEPARATOR] [--fitness_key FITNESS_KEY]
     pypef shift_pos --input CSV_FILE --offset OFFSET
         [--sep CSV_COLUMN_SEPARATOR] [--mutation_sep MUTATION_SEPARATOR] [--fitness_key FITNESS_KEY]
     pypef sto2a2m --sto STO_MSA_FILE [--inter_gap INTER_GAP] [--intra_gap INTRA_GAP]
-    pypef hybrid --params PLMC_FILE --ts TEST_SET
+    pypef hybrid --ts TEST_SET
+        [--model MODEL] [--params PARAM_FILE]
         [--ls LEARNING_SET] [--label] [--threads THREADS]
-    pypef hybrid --model MODEL --params PLMC_FILE
-        [--ts TEST_SET]
-        [--figure TS_FOR_PLOTTING] [--label]
+    pypef hybrid --model MODEL --params PARAM_FILE
+        [--ts TEST_SET] [--label]
         [--ps PREDICTION_SET] [--pmult] [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
                                         [--ddiverse] [--tdiverse] [--qdiverse] [--negative]
         [--threads THREADS]
-    pypef hybrid directevo --wt WT_SEQ --model MODEL12345 --params PLMC_FILE
+    pypef hybrid directevo --wt WT_FASTA --params PARAM_FILE
+        [--model MODEL]
         [--input CSV_FILE] [--y_wt WT_FITNESS] [--numiter NUM_ITER]
         [--numtraj NUM_TRAJ] [--temp TEMPERATURE]
         [--negative] [--usecsv] [--csvaa] [--drop THRESHOLD]
-    pypef hybrid train_and_save --input CSV_FILE --params PLMC_FILE
+    pypef hybrid train_and_save --input CSV_FILE --params PARAM_FILE --wt WT_FASTA
         [--fit_size REL_LEARN_FIT_SIZE] [--test_size REL_TEST_SIZE]
         [--threads THREADS] [--sep CSV_COLUMN_SEPARATOR]
         [--fitness_key FITNESS_KEY] [--rnd_state RND_STATE]
     pypef hybrid low_n --input ENCODED_CSV_FILE
     pypef hybrid extrapolation --input ENCODED_CSV_FILE
         [--conc]
     pypef ml --encoding ENCODING_TECHNIQUE --ls LEARNING_SET --ts TEST_SET
-        [--save NUMBER] [--regressor TYPE] [--nofft] [--all] [--params PLMC_FILE]
-        [--sort METRIC_INT] [--threads THREADS]
+        [--save NUMBER] [--regressor TYPE] [--nofft] [--all] [--params PARAM_FILE]
+        [--sort METRIC_INT] [--threads THREADS] [--label]
+    pypef ml --encoding ENCODING_TECHNIQUE --model MODEL --ts TEST_SET
+        [--nofft] [--params PARAM_FILE] [--threads THREADS] [--label]
     pypef ml --show
         [MODELS]
-    pypef ml --encoding ENCODING_TECHNIQUE --model MODEL12345 --figure TS_FOR_PLOTTING
-        [--label] [--color] [--y_wt WT_FITNESS] [--nofft] [--params PLMC_FILE] [--threads THREADS]
-    pypef ml --encoding ENCODING_TECHNIQUE --model MODEL12345 --ps PREDICTION_SET
-        [--params PLMC_FILE] [--threads THREADS] [--nofft] [--negative]
-    pypef ml --encoding ENCODING_TECHNIQUE --model MODEL12345 --pmult
+    pypef ml --encoding ENCODING_TECHNIQUE --model MODEL --ps PREDICTION_SET
+        [--params PARAM_FILE] [--threads THREADS] [--nofft] [--negative]
+    pypef ml --encoding ENCODING_TECHNIQUE --model MODEL --pmult
         [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
         [--ddiverse] [--tdiverse] [--qdiverse]
-        [--regressor TYPE] [--nofft] [--negative] [--params PLMC_FILE] [--threads THREADS]
-    pypef ml --encoding ENCODING_TECHNIQUE directevo --model MODEL12345 --wt WT_SEQ
+        [--regressor TYPE] [--nofft] [--negative] [--params PARAM_FILE] [--threads THREADS]
+    pypef ml --encoding ENCODING_TECHNIQUE directevo --model MODEL --wt WT_FASTA
         [--input CSV_FILE] [--y_wt WT_FITNESS] [--numiter NUM_ITER] [--numtraj NUM_TRAJ] [--temp TEMPERATURE]
-        [--nofft] [--negative] [--usecsv] [--csvaa] [--drop THRESHOLD] [--params PLMC_FILE]
+        [--nofft] [--negative] [--usecsv] [--csvaa] [--drop THRESHOLD] [--params PARAM_FILE]
     pypef ml low_n --input ENCODED_CSV_FILE
         [--regressor TYPE]
     pypef ml extrapolation --input ENCODED_CSV_FILE
         [--regressor TYPE] [--conc]
 
 
 Options:
   --all                             Finally training on all data [default: False].
-  --color                           Color the plot for "true" and "false" predictions
-                                    quarters [default: False].
   --conc                            Concatenating mutational level variants for predicting variants
                                     from next higher level [default: False].
   --csvaa                           Directed evolution csv amino acid substitutions,
                                     requires flag "--usecsv" [default: False].
   --ddiverse                        Create/predict double natural diverse variants [default: False].
   --drecomb                         Create/predict double recombinants [default: False].
   -d --drop THRESHOLD               Below threshold variants will be discarded from the
                                     data [default: -9E09].
   -e --encoding ENCODING_TECHNIQUE  Sets technique used for encoding sequences for constructing regression models;
                                     choose between 'aaidx' (AAIndex-based encoding), 'onehot' (OneHot-based encoding),
-                                    and 'dca' (DCA-based encoding) [default: aaidx].
-  -f --figure VS_FOR_PLOTTING       Validation set for plotting using a trained model.
+                                    and DCA encoding using Gremlin/plmc (DCA-based encoding) [default: onehot].
   --fitness_key FITNESS_KEY         Label of CSV fitness column. Else uses second column.
   -h --help                         Show this screen [default: False].
   -i --input CSV_FILE               Input data file in .csv format.
   --inter_gap INTER_GAP             Fraction to delete all positions with more than
                                     'inter_gap' * 100 % gaps (columnar trimming) [default: 0.3].
   --intra_gap INTRA_GAP             Fraction to delete all sequences with more than
                                     'intra_gap' * 100 % gaps after being columnar trimmed
                                     (line trimming) [default: 0.5].
   --label                           Label the plot instances [default: False].
   -l --ls LEARNING_SET              Input learning set in .fasta format.
-  -m --model MODEL12345             Model (pickle file) for plotting of validation or for
+  -m --model MODEL                  Model (pickle file) for plotting of validation or for
                                     performing predictions.
+  --msa MSA_FILE                    Multiple sequence alignment (MSA) ins FASTA or A2M format for
+                                    inferring DCA parameters.
   --mutation_sep MUTATION_SEP       Mutation separator [default: /].
   --mutation_extrapolation          Mutation extrapolation [default: False].
   --negative                        Set if more negative values define better variants [default: False].
   --nofft                           Raw sequence input, i.e., no FFT for establishing protein spectra
                                     as vector inputs, only implemented as option for AAindex-based
                                     sequence encoding [default: False].
   -n --numrnd NUMBER                Number of randomly created Learning and Validation
                                     datasets [default: 0].
   --numiter NUM_ITER                Number of mutation iterations per evolution trajectory [default: 5].
   --numtraj NUM_TRAJ                Number of trajectories, i.e., evolution pathways [default: 5].
   -o --offset OFFSET                Offset for shifting substitution positions of the input CSV file [default: 0].
-  --params PLMC_FILE                Input PLMC couplings parameter file.
+  --opt_iter N_ITER                 Number of iterations for GREMLIN-based optimization of local fields
+                                    and couplings [default: 100].
+  --params PARAM_FILE               Input PLMC couplings parameter file.
   -u --pmult                        Predict for all prediction files in folder for recombinants
                                     or for diverse variants [default: False].
   -p --ps PREDICTION_SET            Prediction set for performing predictions using a trained Model.
   --qdiverse                        Create quadruple natural diverse variants [default: False].
   --qarecomb                        Create/predict quadruple recombinants [default: False].
   --qirecomb                        Create/predict quintuple recombinants [default: False].
   --regressor TYPE                  Type of regression (R.) to use, options: PLS CV R.: pls,
@@ -228,18 +242,20 @@
   --rnd_state RND_STATE             Sets the random state for reproduction, only implemented
                                     for hybrid train_and_save [default: 42].
   -s --save NUMBER                  Number of models to be saved as pickle files [default: 5].
   --sep CSV_COLUMN_SEPARATOR        CSV Column separator [default: ;].
   --show                            Show achieved model performances from Model_Results.txt.
   --sort METRIC_INT                 Rank models based on metric {1: R^2, 2: RMSE, 3: NRMSE,
                                     4: Pearson's r, 5: Spearman's rho} [default: 1].
+  --ssm                             Create single-saturation mutagenesis prediction set (does not
+                                    require CSV input) [default: False].
   --sto STO_MSA_FILE                The input MSA file in STO (Stockholm) format.
   --tdiverse                        Create/predict triple natural diverse variants [default: False].
   --temp TEMPERATURE                "Temperature" of Metropolis-Hastings criterion [default: 0.01]
-  --threads THREADS                  Parallel computing of training and validation of models.
+  --threads THREADS                 Parallel computing of training and validation of models.
                                     Number of threads used in parallel computing, by default
                                     no hyperthreading.
   --fit_size REL_LEARN_FIT_SIZE     Relative size of the train set for initial fitting. The remaining data
                                     for training is used for hyperparameter optimization on train subsets
                                     used for validation, while in sum the total data for training is
                                     training data = train_fit data + train_test(validation) data
                                                   = all data - test data.
@@ -248,123 +264,137 @@
   --test_size REL_TEST_SIZE         Relative size of the test set; if set to 0.0 the trained model
                                     will not be tested [default: 0.2].
   --trecomb                         Create/predict triple recombinants [default: False].
   --usecsv                          Perform directed evolution on single variant csv position
                                     data [default: False].
   -t --ts TEST_SET                  Input validation set in .fasta format.
   --version                         Show version [default: False].
-  -w --wt WT_SEQ                    Input file (in FASTA format) for wild-type sequence.
+  -w --wt WT_FASTA                  Input wild-type sequence file (in FASTA format).
   --wt_pos WT_POSITION              Row position of encoded wild-type in encoding CSV file (0-indexed) [default: 0].
   -y --y_wt WT_FITNESS              Fitness value (y) of wild-type [default: 1.0].
   encode                            Encoding [default: False].
   hybrid                            Hybrid modeling based on DCA-derived sequence encoding [default: False].
   ml                                Pure machine learning modeling based on encoded sequences [default: False].
   MODELS                            Number of saved models to show [default: 5].
   onehot                            OneHot-based encoding [default: False].
+  param_inference                   Inferring DCA params using the GREMLIN approach [default: False].
+  reformat_csv                      Reformat input CSV with indicated column and mutation separators to default
+                                    CSV style (column separator ';' and mutation separator '/') [default: False.]
+  save_msa_info                     Optimize local fields and couplings of MSA based on GREMLIN DCA approach and
+                                    save resulting coupling matrix and highly coevolved amino acids.
   shift_pos                         Shift positions of all variant substitutions of the input CSV
-                                    file [default: False.]
+                                    file (identical to reformat_csv when setting --offset to 0) [default: False.]
   sto2a2m                           Transform multiple sequence alignment from STO format to
                                     A2M format [default: False].
 """
 
+
+from os import environ
+try:
+    environ['TF_CPP_MIN_LOG_LEVEL'] = '2'  # only print TensorFlow errors, set to '0' or comment
+except KeyError:                           # lines for seeing TensorFlow infos and warnings
+    pass
+
 from sys import argv, version_info
 from pypef import __version__
 if version_info[0] < 3 or version_info[1] < 9:
     raise SystemError(f"The current version of PyPEF (v {__version__}) "
                       f"requires at least Python 3.9 or higher.")
 
 import time
 from datetime import timedelta
 import logging
 
 from docopt import docopt
 from schema import Schema, SchemaError, Optional, Or, Use
 
-
-from pypef.ml.run import run_pypef_pure_ml
-from pypef.dca.run import run_pypef_hybrid_modeling
-from pypef.utils.run import run_pypef_utils
-
+from pypef.ml.ml_run import run_pypef_pure_ml
+from pypef.dca.dca_run import run_pypef_hybrid_modeling
+from pypef.utils.utils_run import run_pypef_utils
 
 logger = logging.getLogger("pypef")
 logger.setLevel(logging.INFO)
 
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
 
 formatter = logging.Formatter(
-    "%(asctime)s,%(msecs)03d %(levelname)s %(filename)s:%(lineno)d -- %(message)s",
+    "%(asctime)s.%(msecs)03d %(levelname)s %(filename)s:%(lineno)d -- %(message)s",
     "%Y-%m-%d %H:%M:%S"
 )
 ch.setFormatter(formatter)
 logger.addHandler(ch)
 
 
 schema = Schema({
     Optional('--all'): bool,
-    Optional('--color'): bool,
     Optional('--conc'): bool,
     Optional('--csvaa'): bool,
     Optional('--ddiverse'): bool,
     Optional('--drecomb'): bool,
     Optional('--drop'): Use(float),
     Optional('--encoding'): Use(str),
-    Optional('--figure'): Or(None, str),
     Optional('--fitness_key'): Or(None, str),
     Optional('--fit_size'): Use(float),
     Optional('--help'): bool,
     Optional('--input'): Or(None, str),
     Optional('--inter_gap'): Use(float),
     Optional('--intra_gap'): Use(float),
     Optional('--label'): bool,
     Optional('--ls'): Or(None, str),
-    Optional('--model'): Or(None, str),  # str, Or(None, str),
+    Optional('--model'): Or(None, str),
+    Optional('--msa'): Or(None, str),
     Optional('--mutation_sep'): Or(None, str),
     Optional('--negative'): bool,
     Optional('--nofft'): bool,
     Optional('--numrnd'): Use(int),
     Optional('--numiter'): Use(int),
     Optional('--numtraj'): Use(int),
     Optional('--offset'): Use(int),
+    Optional('--opt_iter'): Use(int),
     Optional('--params'): Or(None, str),
     Optional('--pmult'): bool,
     Optional('--ps'): Or(None, str),
     Optional('--qdiverse'): bool,
     Optional('--qarecomb'): bool,
     Optional('--qirecomb'): bool,
     Optional('--regressor'): Or(None, str),
     Optional('--rnd_splits'): Use(int),
     Optional('--rnd_state'): Use(int),
     Optional('--save'): Use(int),
     Optional('--sep'): Or(None, str),
     Optional('--show'): Use(int),
     Optional('--sort'): Use(int),
+    Optional('--ssm'): bool,
     Optional('--sto'): Or(None, str),
     Optional('--tdiverse'): bool,
     Optional('--temp'): Use(float),
     Optional('--test_size'): Use(float),
     Optional('--threads'): Or(None, Use(int)),
     Optional('--train_size'): Use(float),
     Optional('--trecomb'): bool,
     Optional('--usecsv'): bool,
     Optional('--ts'): Or(None, str),
     Optional('--wt'): Or(None, str),
     Optional('--wt_pos'): Use(int),
     Optional('--y_wt'): Or(None, Use(float)),
     Optional('aaidx'): bool,
+    Optional('param_inference'): bool,
     Optional('hybrid'): bool,
     Optional('directevo'): bool,
     Optional('encode'): bool,
     Optional('extrapolation'): bool,
     Optional('low_n'): bool,
     Optional('mklsts'): bool,
     Optional('mkps'): bool,
     Optional('ml'): bool,
     Optional('MODELS'): Or(None, Use(int)),
     Optional('onehot'): bool,
+    Optional('reformat_csv'): bool,
+    Optional('save_msa_info'): bool,
     Optional('shift_pos'): bool,
     Optional('sto2a2m'): bool,
     Optional('train_and_save'): bool,
 })
 
 
 def validate(args):
@@ -372,29 +402,35 @@
         args = schema.validate(args)
         return args
     except SchemaError as e:
         exit(e)
 
 
 def run_main():
+    """
+    Entry point for pip-installed version.
+    """
     arguments = docopt(__doc__, version=__version__)
     start_time = time.time()
     logger.debug(f'main.py __name__: {__name__}, version: {__version__}')
     logger.debug(str(argv)[1:-1].replace("\'", "").replace(",", ""))
     logger.debug(f'\n{arguments}')
     arguments = validate(arguments)
     if arguments['directevo']:
         run_pypef_utils(arguments)
     elif arguments['ml']:
         run_pypef_pure_ml(arguments)
-    elif arguments['hybrid']:
+    elif arguments['hybrid'] or arguments['param_inference'] or arguments['save_msa_info']:
         run_pypef_hybrid_modeling(arguments)
     else:
         run_pypef_utils(arguments)
 
     elapsed = str(timedelta(seconds=time.time()-start_time)).split(".")[0]
     elapsed = f'{elapsed.split(":")[0]} h {elapsed.split(":")[1]} min {elapsed.split(":")[2]} s'
     logger.info(f'Done! (Run time: {elapsed})')
 
 
 if __name__ == '__main__':
+    """
+    Entry point for direct file run.
+    """
     run_main()
```

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ANDN920101.txt` & `pypef-0.3/pypef/ml/AAindex/ANDN920101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ARGP820101.txt` & `pypef-0.3/pypef/ml/AAindex/ARGP820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ARGP820102.txt` & `pypef-0.3/pypef/ml/AAindex/ARGP820102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ARGP820103.txt` & `pypef-0.3/pypef/ml/AAindex/ARGP820103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AURR980108.txt` & `pypef-0.3/pypef/ml/AAindex/AURR980108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AURR980109.txt` & `pypef-0.3/pypef/ml/AAindex/AURR980109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AURR980110.txt` & `pypef-0.3/pypef/ml/AAindex/AURR980110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AURR980111.txt` & `pypef-0.3/pypef/ml/AAindex/AURR980111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AURR980112.txt` & `pypef-0.3/pypef/ml/AAindex/AURR980112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AURR980113.txt` & `pypef-0.3/pypef/ml/AAindex/AURR980113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AURR980114.txt` & `pypef-0.3/pypef/ml/AAindex/AURR980114.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AURR980115.txt` & `pypef-0.3/pypef/ml/AAindex/AURR980115.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AVBF000101.txt` & `pypef-0.3/pypef/ml/AAindex/AVBF000101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AVBF000102.txt` & `pypef-0.3/pypef/ml/AAindex/AVBF000102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AVBF000103.txt` & `pypef-0.3/pypef/ml/AAindex/AVBF000103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AVBF000104.txt` & `pypef-0.3/pypef/ml/AAindex/AVBF000104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AVBF000105.txt` & `pypef-0.3/pypef/ml/AAindex/AVBF000105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AVBF000106.txt` & `pypef-0.3/pypef/ml/AAindex/AVBF000106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AVBF000107.txt` & `pypef-0.3/pypef/ml/AAindex/AVBF000107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AVBF000108.txt` & `pypef-0.3/pypef/ml/AAindex/AVBF000108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/AVBF000109.txt` & `pypef-0.3/pypef/ml/AAindex/AVBF000109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BAEK050101.txt` & `pypef-0.3/pypef/ml/AAindex/BAEK050101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BASU050101.txt` & `pypef-0.3/pypef/ml/AAindex/BASU050101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BASU050102.txt` & `pypef-0.3/pypef/ml/AAindex/BASU050102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BASU050103.txt` & `pypef-0.3/pypef/ml/AAindex/BASU050103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BEGF750101.txt` & `pypef-0.3/pypef/ml/AAindex/BEGF750101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BEGF750102.txt` & `pypef-0.3/pypef/ml/AAindex/BEGF750102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BEGF750103.txt` & `pypef-0.3/pypef/ml/AAindex/BEGF750103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BHAR880101.txt` & `pypef-0.3/pypef/ml/AAindex/BHAR880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BIGC670101.txt` & `pypef-0.3/pypef/ml/AAindex/BIGC670101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BIOV880101.txt` & `pypef-0.3/pypef/ml/AAindex/BIOV880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BIOV880102.txt` & `pypef-0.3/pypef/ml/AAindex/BIOV880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BLAM930101.txt` & `pypef-0.3/pypef/ml/AAindex/BLAM930101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BLAS910101.txt` & `pypef-0.3/pypef/ml/AAindex/BLAS910101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BROC820101.txt` & `pypef-0.3/pypef/ml/AAindex/BROC820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BROC820102.txt` & `pypef-0.3/pypef/ml/AAindex/BROC820102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BULH740101.txt` & `pypef-0.3/pypef/ml/AAindex/BULH740101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BULH740102.txt` & `pypef-0.3/pypef/ml/AAindex/BULH740102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BUNA790101.txt` & `pypef-0.3/pypef/ml/AAindex/BUNA790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BUNA790102.txt` & `pypef-0.3/pypef/ml/AAindex/BUNA790102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BUNA790103.txt` & `pypef-0.3/pypef/ml/AAindex/BUNA790103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BURA740101.txt` & `pypef-0.3/pypef/ml/AAindex/BURA740101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/BURA740102.txt` & `pypef-0.3/pypef/ml/AAindex/BURA740102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CASG920101.txt` & `pypef-0.3/pypef/ml/AAindex/CASG920101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CEDJ970101.txt` & `pypef-0.3/pypef/ml/AAindex/CEDJ970101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CEDJ970102.txt` & `pypef-0.3/pypef/ml/AAindex/CEDJ970102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CEDJ970103.txt` & `pypef-0.3/pypef/ml/AAindex/CEDJ970103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CEDJ970104.txt` & `pypef-0.3/pypef/ml/AAindex/CEDJ970104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CEDJ970105.txt` & `pypef-0.3/pypef/ml/AAindex/CEDJ970105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHAM810101.txt` & `pypef-0.3/pypef/ml/AAindex/CHAM810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHAM820101.txt` & `pypef-0.3/pypef/ml/AAindex/CHAM820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHAM820102.txt` & `pypef-0.3/pypef/ml/AAindex/CHAM820102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHAM830101.txt` & `pypef-0.3/pypef/ml/AAindex/CHAM830101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHAM830102.txt` & `pypef-0.3/pypef/ml/AAindex/CHAM830102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHAM830103.txt` & `pypef-0.3/pypef/ml/AAindex/CHAM830103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHAM830104.txt` & `pypef-0.3/pypef/ml/AAindex/CHAM830104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHAM830105.txt` & `pypef-0.3/pypef/ml/AAindex/CHAM830105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHAM830106.txt` & `pypef-0.3/pypef/ml/AAindex/CHAM830106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHAM830107.txt` & `pypef-0.3/pypef/ml/AAindex/CHAM830107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHAM830108.txt` & `pypef-0.3/pypef/ml/AAindex/CHAM830108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOC750101.txt` & `pypef-0.3/pypef/ml/AAindex/CHOC750101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOC760101.txt` & `pypef-0.3/pypef/ml/AAindex/CHOC760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOC760102.txt` & `pypef-0.3/pypef/ml/AAindex/CHOC760102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOC760103.txt` & `pypef-0.3/pypef/ml/AAindex/CHOC760103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOC760104.txt` & `pypef-0.3/pypef/ml/AAindex/CHOC760104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780101.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780201.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780201.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780202.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780202.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780203.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780203.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780204.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780204.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780205.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780205.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780206.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780206.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780207.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780207.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780208.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780208.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780209.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780209.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780210.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780210.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780211.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780211.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780212.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780212.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780213.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780213.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780214.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780214.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780215.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780215.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CHOP780216.txt` & `pypef-0.3/pypef/ml/AAindex/CHOP780216.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CIDH920101.txt` & `pypef-0.3/pypef/ml/AAindex/CIDH920101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CIDH920102.txt` & `pypef-0.3/pypef/ml/AAindex/CIDH920102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CIDH920103.txt` & `pypef-0.3/pypef/ml/AAindex/CIDH920103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CIDH920104.txt` & `pypef-0.3/pypef/ml/AAindex/CIDH920104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CIDH920105.txt` & `pypef-0.3/pypef/ml/AAindex/CIDH920105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CORJ870101.txt` & `pypef-0.3/pypef/ml/AAindex/CORJ870101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CORJ870102.txt` & `pypef-0.3/pypef/ml/AAindex/CORJ870102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CORJ870103.txt` & `pypef-0.3/pypef/ml/AAindex/CORJ870103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CORJ870104.txt` & `pypef-0.3/pypef/ml/AAindex/CORJ870104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CORJ870105.txt` & `pypef-0.3/pypef/ml/AAindex/CORJ870105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CORJ870106.txt` & `pypef-0.3/pypef/ml/AAindex/CORJ870106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CORJ870107.txt` & `pypef-0.3/pypef/ml/AAindex/CORJ870107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CORJ870108.txt` & `pypef-0.3/pypef/ml/AAindex/CORJ870108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/COSI940101.txt` & `pypef-0.3/pypef/ml/AAindex/COSI940101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/COWR900101.txt` & `pypef-0.3/pypef/ml/AAindex/COWR900101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CRAJ730101.txt` & `pypef-0.3/pypef/ml/AAindex/CRAJ730101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CRAJ730102.txt` & `pypef-0.3/pypef/ml/AAindex/CRAJ730102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/CRAJ730103.txt` & `pypef-0.3/pypef/ml/AAindex/CRAJ730103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/DAWD720101.txt` & `pypef-0.3/pypef/ml/AAindex/DAWD720101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/DAYM780101.txt` & `pypef-0.3/pypef/ml/AAindex/DAYM780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/DAYM780201.txt` & `pypef-0.3/pypef/ml/AAindex/DAYM780201.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/DESM900101.txt` & `pypef-0.3/pypef/ml/AAindex/DESM900101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/DESM900102.txt` & `pypef-0.3/pypef/ml/AAindex/DESM900102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/DIGM050101.txt` & `pypef-0.3/pypef/ml/AAindex/DIGM050101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/EISD840101.txt` & `pypef-0.3/pypef/ml/AAindex/EISD840101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/EISD860101.txt` & `pypef-0.3/pypef/ml/AAindex/EISD860101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/EISD860102.txt` & `pypef-0.3/pypef/ml/AAindex/EISD860102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/EISD860103.txt` & `pypef-0.3/pypef/ml/AAindex/EISD860103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ENGD860101.txt` & `pypef-0.3/pypef/ml/AAindex/ENGD860101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FASG760101.txt` & `pypef-0.3/pypef/ml/AAindex/FASG760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FASG890101.txt` & `pypef-0.3/pypef/ml/AAindex/FASG890101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FAUJ830101.txt` & `pypef-0.3/pypef/ml/AAindex/FAUJ830101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FAUJ880101.txt` & `pypef-0.3/pypef/ml/AAindex/FAUJ880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FAUJ880102.txt` & `pypef-0.3/pypef/ml/AAindex/FAUJ880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FAUJ880103.txt` & `pypef-0.3/pypef/ml/AAindex/FAUJ880103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FAUJ880104.txt` & `pypef-0.3/pypef/ml/AAindex/FAUJ880104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FAUJ880105.txt` & `pypef-0.3/pypef/ml/AAindex/FAUJ880105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FAUJ880106.txt` & `pypef-0.3/pypef/ml/AAindex/FAUJ880106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FAUJ880107.txt` & `pypef-0.3/pypef/ml/AAindex/FAUJ880107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FAUJ880108.txt` & `pypef-0.3/pypef/ml/AAindex/FAUJ880108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FAUJ880109.txt` & `pypef-0.3/pypef/ml/AAindex/FAUJ880109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FAUJ880110.txt` & `pypef-0.3/pypef/ml/AAindex/FAUJ880110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FAUJ880111.txt` & `pypef-0.3/pypef/ml/AAindex/FAUJ880111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FAUJ880112.txt` & `pypef-0.3/pypef/ml/AAindex/FAUJ880112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FAUJ880113.txt` & `pypef-0.3/pypef/ml/AAindex/FAUJ880113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FINA770101.txt` & `pypef-0.3/pypef/ml/AAindex/FINA770101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FINA910101.txt` & `pypef-0.3/pypef/ml/AAindex/FINA910101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FINA910102.txt` & `pypef-0.3/pypef/ml/AAindex/FINA910102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FINA910103.txt` & `pypef-0.3/pypef/ml/AAindex/FINA910103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FINA910104.txt` & `pypef-0.3/pypef/ml/AAindex/FINA910104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FODM020101.txt` & `pypef-0.3/pypef/ml/AAindex/FODM020101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FUKS010101.txt` & `pypef-0.3/pypef/ml/AAindex/FUKS010101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FUKS010102.txt` & `pypef-0.3/pypef/ml/AAindex/FUKS010102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FUKS010103.txt` & `pypef-0.3/pypef/ml/AAindex/FUKS010103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FUKS010104.txt` & `pypef-0.3/pypef/ml/AAindex/FUKS010104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FUKS010105.txt` & `pypef-0.3/pypef/ml/AAindex/FUKS010105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FUKS010106.txt` & `pypef-0.3/pypef/ml/AAindex/FUKS010106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FUKS010107.txt` & `pypef-0.3/pypef/ml/AAindex/FUKS010107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FUKS010108.txt` & `pypef-0.3/pypef/ml/AAindex/FUKS010108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FUKS010109.txt` & `pypef-0.3/pypef/ml/AAindex/FUKS010109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FUKS010110.txt` & `pypef-0.3/pypef/ml/AAindex/FUKS010110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FUKS010111.txt` & `pypef-0.3/pypef/ml/AAindex/FUKS010111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/FUKS010112.txt` & `pypef-0.3/pypef/ml/AAindex/FUKS010112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GARJ730101.txt` & `pypef-0.3/pypef/ml/AAindex/GARJ730101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEIM800101.txt` & `pypef-0.3/pypef/ml/AAindex/GEIM800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEIM800102.txt` & `pypef-0.3/pypef/ml/AAindex/GEIM800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEIM800104.txt` & `pypef-0.3/pypef/ml/AAindex/GEIM800104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEIM800105.txt` & `pypef-0.3/pypef/ml/AAindex/GEIM800105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEIM800106.txt` & `pypef-0.3/pypef/ml/AAindex/GEIM800106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEIM800107.txt` & `pypef-0.3/pypef/ml/AAindex/GEIM800107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEIM800108.txt` & `pypef-0.3/pypef/ml/AAindex/GEIM800108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEIM800109.txt` & `pypef-0.3/pypef/ml/AAindex/GEIM800109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEIM800110.txt` & `pypef-0.3/pypef/ml/AAindex/GEIM800110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEIM800111.txt` & `pypef-0.3/pypef/ml/AAindex/GEIM800111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEOR030101.txt` & `pypef-0.3/pypef/ml/AAindex/GEOR030101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEOR030102.txt` & `pypef-0.3/pypef/ml/AAindex/GEOR030102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEOR030103.txt` & `pypef-0.3/pypef/ml/AAindex/GEOR030103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEOR030104.txt` & `pypef-0.3/pypef/ml/AAindex/GEOR030104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEOR030105.txt` & `pypef-0.3/pypef/ml/AAindex/GEOR030105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEOR030106.txt` & `pypef-0.3/pypef/ml/AAindex/GEOR030106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEOR030107.txt` & `pypef-0.3/pypef/ml/AAindex/GEOR030107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEOR030108.txt` & `pypef-0.3/pypef/ml/AAindex/GEOR030108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GEOR030109.txt` & `pypef-0.3/pypef/ml/AAindex/GEOR030109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GOLD730101.txt` & `pypef-0.3/pypef/ml/AAindex/GOLD730101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GOLD730102.txt` & `pypef-0.3/pypef/ml/AAindex/GOLD730102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GRAR740102.txt` & `pypef-0.3/pypef/ml/AAindex/GRAR740102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GRAR740103.txt` & `pypef-0.3/pypef/ml/AAindex/GRAR740103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GUOD860101.txt` & `pypef-0.3/pypef/ml/AAindex/GUOD860101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GUYH850101.txt` & `pypef-0.3/pypef/ml/AAindex/GUYH850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GUYH850102.txt` & `pypef-0.3/pypef/ml/AAindex/GUYH850102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GUYH850103.txt` & `pypef-0.3/pypef/ml/AAindex/GUYH850103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GUYH850104.txt` & `pypef-0.3/pypef/ml/AAindex/GUYH850104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/GUYH850105.txt` & `pypef-0.3/pypef/ml/AAindex/GUYH850105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/HARY940101.txt` & `pypef-0.3/pypef/ml/AAindex/HARY940101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/HOPA770101.txt` & `pypef-0.3/pypef/ml/AAindex/HOPA770101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/HOPT810101.txt` & `pypef-0.3/pypef/ml/AAindex/HOPT810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/HUTJ700101.txt` & `pypef-0.3/pypef/ml/AAindex/HUTJ700101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/HUTJ700102.txt` & `pypef-0.3/pypef/ml/AAindex/HUTJ700102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/HUTJ700103.txt` & `pypef-0.3/pypef/ml/AAindex/HUTJ700103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ISOY800101.txt` & `pypef-0.3/pypef/ml/AAindex/ISOY800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ISOY800102.txt` & `pypef-0.3/pypef/ml/AAindex/ISOY800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ISOY800103.txt` & `pypef-0.3/pypef/ml/AAindex/ISOY800103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ISOY800104.txt` & `pypef-0.3/pypef/ml/AAindex/ISOY800104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ISOY800105.txt` & `pypef-0.3/pypef/ml/AAindex/ISOY800105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ISOY800106.txt` & `pypef-0.3/pypef/ml/AAindex/ISOY800106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ISOY800107.txt` & `pypef-0.3/pypef/ml/AAindex/ISOY800107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ISOY800108.txt` & `pypef-0.3/pypef/ml/AAindex/ISOY800108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/JACR890101.txt` & `pypef-0.3/pypef/ml/AAindex/JACR890101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/JANJ780101.txt` & `pypef-0.3/pypef/ml/AAindex/JANJ780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/JANJ780102.txt` & `pypef-0.3/pypef/ml/AAindex/JANJ780102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/JANJ780103.txt` & `pypef-0.3/pypef/ml/AAindex/JANJ780103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/JANJ790101.txt` & `pypef-0.3/pypef/ml/AAindex/JANJ790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/JANJ790102.txt` & `pypef-0.3/pypef/ml/AAindex/JANJ790102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/JOND750101.txt` & `pypef-0.3/pypef/ml/AAindex/JOND750101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/JOND750102.txt` & `pypef-0.3/pypef/ml/AAindex/JOND750102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/JOND920101.txt` & `pypef-0.3/pypef/ml/AAindex/JOND920101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/JUKT750101.txt` & `pypef-0.3/pypef/ml/AAindex/JUKT750101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/JUNJ780101.txt` & `pypef-0.3/pypef/ml/AAindex/JUNJ780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/JURD980101.txt` & `pypef-0.3/pypef/ml/AAindex/JURD980101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KANM800101.txt` & `pypef-0.3/pypef/ml/AAindex/KANM800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KANM800102.txt` & `pypef-0.3/pypef/ml/AAindex/KANM800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KANM800103.txt` & `pypef-0.3/pypef/ml/AAindex/KANM800103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KANM800104.txt` & `pypef-0.3/pypef/ml/AAindex/KANM800104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARP850101.txt` & `pypef-0.3/pypef/ml/AAindex/KARP850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARP850102.txt` & `pypef-0.3/pypef/ml/AAindex/KARP850102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160101.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160102.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160103.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160104.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160105.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160106.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160107.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160108.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160109.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160110.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160111.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160112.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160113.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160114.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160114.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160115.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160115.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160116.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160116.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160117.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160117.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160118.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160118.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160119.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160119.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160120.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160120.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160121.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160121.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KARS160122.txt` & `pypef-0.3/pypef/ml/AAindex/KARS160122.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KIDA850101.txt` & `pypef-0.3/pypef/ml/AAindex/KIDA850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KIMC930101.txt` & `pypef-0.3/pypef/ml/AAindex/KIMC930101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KLEP840101.txt` & `pypef-0.3/pypef/ml/AAindex/KLEP840101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KOEP990101.txt` & `pypef-0.3/pypef/ml/AAindex/KOEP990101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KRIW710101.txt` & `pypef-0.3/pypef/ml/AAindex/KRIW710101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KRIW790101.txt` & `pypef-0.3/pypef/ml/AAindex/KRIW790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KRIW790102.txt` & `pypef-0.3/pypef/ml/AAindex/KRIW790102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KRIW790103.txt` & `pypef-0.3/pypef/ml/AAindex/KRIW790103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KUHL950101.txt` & `pypef-0.3/pypef/ml/AAindex/KUHL950101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KUMS000101.txt` & `pypef-0.3/pypef/ml/AAindex/KUMS000101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KUMS000102.txt` & `pypef-0.3/pypef/ml/AAindex/KUMS000102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KUMS000103.txt` & `pypef-0.3/pypef/ml/AAindex/KUMS000103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KUMS000104.txt` & `pypef-0.3/pypef/ml/AAindex/KUMS000104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/KYTJ820101.txt` & `pypef-0.3/pypef/ml/AAindex/KYTJ820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LAWE840101.txt` & `pypef-0.3/pypef/ml/AAindex/LAWE840101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LEVM760101.txt` & `pypef-0.3/pypef/ml/AAindex/LEVM760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LEVM760102.txt` & `pypef-0.3/pypef/ml/AAindex/LEVM760102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LEVM760103.txt` & `pypef-0.3/pypef/ml/AAindex/LEVM760103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LEVM760104.txt` & `pypef-0.3/pypef/ml/AAindex/LEVM760104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LEVM760105.txt` & `pypef-0.3/pypef/ml/AAindex/LEVM760105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LEVM760106.txt` & `pypef-0.3/pypef/ml/AAindex/LEVM760106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LEVM760107.txt` & `pypef-0.3/pypef/ml/AAindex/LEVM760107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LEVM780101.txt` & `pypef-0.3/pypef/ml/AAindex/LEVM780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LEVM780102.txt` & `pypef-0.3/pypef/ml/AAindex/LEVM780102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LEVM780103.txt` & `pypef-0.3/pypef/ml/AAindex/LEVM780103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LEVM780104.txt` & `pypef-0.3/pypef/ml/AAindex/LEVM780104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LEVM780105.txt` & `pypef-0.3/pypef/ml/AAindex/LEVM780105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LEVM780106.txt` & `pypef-0.3/pypef/ml/AAindex/LEVM780106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LEWP710101.txt` & `pypef-0.3/pypef/ml/AAindex/LEWP710101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LIFS790101.txt` & `pypef-0.3/pypef/ml/AAindex/LIFS790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LIFS790102.txt` & `pypef-0.3/pypef/ml/AAindex/LIFS790102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/LIFS790103.txt` & `pypef-0.3/pypef/ml/AAindex/LIFS790103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MANP780101.txt` & `pypef-0.3/pypef/ml/AAindex/MANP780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MAXF760101.txt` & `pypef-0.3/pypef/ml/AAindex/MAXF760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MAXF760102.txt` & `pypef-0.3/pypef/ml/AAindex/MAXF760102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MAXF760103.txt` & `pypef-0.3/pypef/ml/AAindex/MAXF760103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MAXF760104.txt` & `pypef-0.3/pypef/ml/AAindex/MAXF760104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MAXF760105.txt` & `pypef-0.3/pypef/ml/AAindex/MAXF760105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MAXF760106.txt` & `pypef-0.3/pypef/ml/AAindex/MAXF760106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MCMT640101.txt` & `pypef-0.3/pypef/ml/AAindex/MCMT640101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MEEJ800101.txt` & `pypef-0.3/pypef/ml/AAindex/MEEJ800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MEEJ800102.txt` & `pypef-0.3/pypef/ml/AAindex/MEEJ800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MEEJ810101.txt` & `pypef-0.3/pypef/ml/AAindex/MEEJ810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MEEJ810102.txt` & `pypef-0.3/pypef/ml/AAindex/MEEJ810102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MEIH800101.txt` & `pypef-0.3/pypef/ml/AAindex/MEIH800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MEIH800102.txt` & `pypef-0.3/pypef/ml/AAindex/MEIH800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MEIH800103.txt` & `pypef-0.3/pypef/ml/AAindex/MEIH800103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MITS020101.txt` & `pypef-0.3/pypef/ml/AAindex/MITS020101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MIYS850101.txt` & `pypef-0.3/pypef/ml/AAindex/MIYS850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MIYS990101.txt` & `pypef-0.3/pypef/ml/AAindex/MIYS990101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MIYS990102.txt` & `pypef-0.3/pypef/ml/AAindex/MIYS990102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MIYS990103.txt` & `pypef-0.3/pypef/ml/AAindex/MIYS990103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MIYS990104.txt` & `pypef-0.3/pypef/ml/AAindex/MIYS990104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MIYS990105.txt` & `pypef-0.3/pypef/ml/AAindex/MIYS990105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MONM990101.txt` & `pypef-0.3/pypef/ml/AAindex/MONM990101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MONM990201.txt` & `pypef-0.3/pypef/ml/AAindex/MONM990201.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MUNV940101.txt` & `pypef-0.3/pypef/ml/AAindex/MUNV940101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MUNV940102.txt` & `pypef-0.3/pypef/ml/AAindex/MUNV940102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MUNV940103.txt` & `pypef-0.3/pypef/ml/AAindex/MUNV940103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MUNV940104.txt` & `pypef-0.3/pypef/ml/AAindex/MUNV940104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/MUNV940105.txt` & `pypef-0.3/pypef/ml/AAindex/MUNV940105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NADH010101.txt` & `pypef-0.3/pypef/ml/AAindex/NADH010101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NADH010102.txt` & `pypef-0.3/pypef/ml/AAindex/NADH010102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NADH010103.txt` & `pypef-0.3/pypef/ml/AAindex/NADH010103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NADH010104.txt` & `pypef-0.3/pypef/ml/AAindex/NADH010104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NADH010105.txt` & `pypef-0.3/pypef/ml/AAindex/NADH010105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NADH010106.txt` & `pypef-0.3/pypef/ml/AAindex/NADH010106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NADH010107.txt` & `pypef-0.3/pypef/ml/AAindex/NADH010107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAGK730101.txt` & `pypef-0.3/pypef/ml/AAindex/NAGK730101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAGK730102.txt` & `pypef-0.3/pypef/ml/AAindex/NAGK730102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAGK730103.txt` & `pypef-0.3/pypef/ml/AAindex/NAGK730103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH900101.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH900101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH900102.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH900102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH900103.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH900103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH900104.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH900104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH900105.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH900105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH900106.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH900106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH900107.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH900107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH900108.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH900108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH900109.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH900109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH900110.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH900110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH900111.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH900111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH900112.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH900112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH900113.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH900113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH920101.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH920101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH920102.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH920102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH920103.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH920103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH920104.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH920104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH920105.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH920105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH920106.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH920106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH920107.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH920107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NAKH920108.txt` & `pypef-0.3/pypef/ml/AAindex/NAKH920108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NISK800101.txt` & `pypef-0.3/pypef/ml/AAindex/NISK800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NISK860101.txt` & `pypef-0.3/pypef/ml/AAindex/NISK860101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/NOZY710101.txt` & `pypef-0.3/pypef/ml/AAindex/NOZY710101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/OLSK800101.txt` & `pypef-0.3/pypef/ml/AAindex/OLSK800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ONEK900101.txt` & `pypef-0.3/pypef/ml/AAindex/ONEK900101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ONEK900102.txt` & `pypef-0.3/pypef/ml/AAindex/ONEK900102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/OOBM770101.txt` & `pypef-0.3/pypef/ml/AAindex/OOBM770101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/OOBM770102.txt` & `pypef-0.3/pypef/ml/AAindex/OOBM770102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/OOBM770103.txt` & `pypef-0.3/pypef/ml/AAindex/OOBM770103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/OOBM770104.txt` & `pypef-0.3/pypef/ml/AAindex/OOBM770104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/OOBM770105.txt` & `pypef-0.3/pypef/ml/AAindex/OOBM770105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/OOBM850101.txt` & `pypef-0.3/pypef/ml/AAindex/OOBM850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/OOBM850102.txt` & `pypef-0.3/pypef/ml/AAindex/OOBM850102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/OOBM850103.txt` & `pypef-0.3/pypef/ml/AAindex/OOBM850103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/OOBM850104.txt` & `pypef-0.3/pypef/ml/AAindex/OOBM850104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/OOBM850105.txt` & `pypef-0.3/pypef/ml/AAindex/OOBM850105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810101.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810102.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810103.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810104.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810105.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810106.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810107.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810108.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810109.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810110.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810111.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810112.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810113.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810114.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810114.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810115.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810115.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PALJ810116.txt` & `pypef-0.3/pypef/ml/AAindex/PALJ810116.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PARJ860101.txt` & `pypef-0.3/pypef/ml/AAindex/PARJ860101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PARS000101.txt` & `pypef-0.3/pypef/ml/AAindex/PARS000101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PARS000102.txt` & `pypef-0.3/pypef/ml/AAindex/PARS000102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PLIV810101.txt` & `pypef-0.3/pypef/ml/AAindex/PLIV810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PONJ960101.txt` & `pypef-0.3/pypef/ml/AAindex/PONJ960101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PONP800101.txt` & `pypef-0.3/pypef/ml/AAindex/PONP800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PONP800102.txt` & `pypef-0.3/pypef/ml/AAindex/PONP800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PONP800103.txt` & `pypef-0.3/pypef/ml/AAindex/PONP800103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PONP800104.txt` & `pypef-0.3/pypef/ml/AAindex/PONP800104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PONP800105.txt` & `pypef-0.3/pypef/ml/AAindex/PONP800105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PONP800106.txt` & `pypef-0.3/pypef/ml/AAindex/PONP800106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PONP800107.txt` & `pypef-0.3/pypef/ml/AAindex/PONP800107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PONP800108.txt` & `pypef-0.3/pypef/ml/AAindex/PONP800108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PONP930101.txt` & `pypef-0.3/pypef/ml/AAindex/PONP930101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PRAM820101.txt` & `pypef-0.3/pypef/ml/AAindex/PRAM820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PRAM820102.txt` & `pypef-0.3/pypef/ml/AAindex/PRAM820102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PRAM820103.txt` & `pypef-0.3/pypef/ml/AAindex/PRAM820103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PRAM900101.txt` & `pypef-0.3/pypef/ml/AAindex/PRAM900101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PRAM900102.txt` & `pypef-0.3/pypef/ml/AAindex/PRAM900102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PRAM900103.txt` & `pypef-0.3/pypef/ml/AAindex/PRAM900103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PRAM900104.txt` & `pypef-0.3/pypef/ml/AAindex/PRAM900104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PTIO830101.txt` & `pypef-0.3/pypef/ml/AAindex/PTIO830101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PTIO830102.txt` & `pypef-0.3/pypef/ml/AAindex/PTIO830102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PUNT030101.txt` & `pypef-0.3/pypef/ml/AAindex/PUNT030101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/PUNT030102.txt` & `pypef-0.3/pypef/ml/AAindex/PUNT030102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880101.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880102.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880103.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880104.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880105.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880106.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880107.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880108.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880109.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880110.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880111.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880112.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880113.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880114.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880114.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880115.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880115.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880116.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880116.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880117.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880117.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880118.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880118.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880119.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880119.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880120.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880120.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880121.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880121.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880122.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880122.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880123.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880123.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880124.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880124.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880125.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880125.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880126.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880126.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880127.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880127.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880128.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880128.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880129.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880129.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880130.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880130.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880131.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880131.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880132.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880132.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880133.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880133.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880134.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880134.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880135.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880135.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880136.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880136.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880137.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880137.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880138.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880138.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/QIAN880139.txt` & `pypef-0.3/pypef/ml/AAindex/QIAN880139.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS770101.txt` & `pypef-0.3/pypef/ml/AAindex/RACS770101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS770102.txt` & `pypef-0.3/pypef/ml/AAindex/RACS770102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS770103.txt` & `pypef-0.3/pypef/ml/AAindex/RACS770103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS820101.txt` & `pypef-0.3/pypef/ml/AAindex/RACS820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS820102.txt` & `pypef-0.3/pypef/ml/AAindex/RACS820102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS820103.txt` & `pypef-0.3/pypef/ml/AAindex/RACS820103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS820104.txt` & `pypef-0.3/pypef/ml/AAindex/RACS820104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS820105.txt` & `pypef-0.3/pypef/ml/AAindex/RACS820105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS820106.txt` & `pypef-0.3/pypef/ml/AAindex/RACS820106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS820107.txt` & `pypef-0.3/pypef/ml/AAindex/RACS820107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS820108.txt` & `pypef-0.3/pypef/ml/AAindex/RACS820108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS820109.txt` & `pypef-0.3/pypef/ml/AAindex/RACS820109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS820110.txt` & `pypef-0.3/pypef/ml/AAindex/RACS820110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS820111.txt` & `pypef-0.3/pypef/ml/AAindex/RACS820111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS820112.txt` & `pypef-0.3/pypef/ml/AAindex/RACS820112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS820113.txt` & `pypef-0.3/pypef/ml/AAindex/RACS820113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RACS820114.txt` & `pypef-0.3/pypef/ml/AAindex/RACS820114.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RADA880101.txt` & `pypef-0.3/pypef/ml/AAindex/RADA880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RADA880102.txt` & `pypef-0.3/pypef/ml/AAindex/RADA880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RADA880103.txt` & `pypef-0.3/pypef/ml/AAindex/RADA880103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RADA880104.txt` & `pypef-0.3/pypef/ml/AAindex/RADA880104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RADA880105.txt` & `pypef-0.3/pypef/ml/AAindex/RADA880105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RADA880106.txt` & `pypef-0.3/pypef/ml/AAindex/RADA880106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RADA880107.txt` & `pypef-0.3/pypef/ml/AAindex/RADA880107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RADA880108.txt` & `pypef-0.3/pypef/ml/AAindex/RADA880108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RICJ880101.txt` & `pypef-0.3/pypef/ml/AAindex/RICJ880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RICJ880102.txt` & `pypef-0.3/pypef/ml/AAindex/RICJ880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RICJ880106.txt` & `pypef-0.3/pypef/ml/AAindex/RICJ880106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RICJ880107.txt` & `pypef-0.3/pypef/ml/AAindex/RICJ880107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RICJ880109.txt` & `pypef-0.3/pypef/ml/AAindex/RICJ880109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RICJ880111.txt` & `pypef-0.3/pypef/ml/AAindex/RICJ880111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/RICJ880115.txt` & `pypef-0.3/pypef/ml/AAindex/RICJ880115.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROBB760101.txt` & `pypef-0.3/pypef/ml/AAindex/ROBB760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROBB760103.txt` & `pypef-0.3/pypef/ml/AAindex/ROBB760103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROBB760104.txt` & `pypef-0.3/pypef/ml/AAindex/ROBB760104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROBB760105.txt` & `pypef-0.3/pypef/ml/AAindex/ROBB760105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROBB760106.txt` & `pypef-0.3/pypef/ml/AAindex/ROBB760106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROBB760108.txt` & `pypef-0.3/pypef/ml/AAindex/ROBB760108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROBB760110.txt` & `pypef-0.3/pypef/ml/AAindex/ROBB760110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROBB760112.txt` & `pypef-0.3/pypef/ml/AAindex/ROBB760112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROBB760113.txt` & `pypef-0.3/pypef/ml/AAindex/ROBB760113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROBB790101.txt` & `pypef-0.3/pypef/ml/AAindex/ROBB790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROSG850101.txt` & `pypef-0.3/pypef/ml/AAindex/ROSG850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROSG850102.txt` & `pypef-0.3/pypef/ml/AAindex/ROSG850102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROSM880101.txt` & `pypef-0.3/pypef/ml/AAindex/ROSM880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROSM880102.txt` & `pypef-0.3/pypef/ml/AAindex/ROSM880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROSM880104.txt` & `pypef-0.3/pypef/ml/AAindex/ROSM880104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ROSM880105.txt` & `pypef-0.3/pypef/ml/AAindex/ROSM880105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/SIMZ760101.txt` & `pypef-0.3/pypef/ml/AAindex/SIMZ760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/SNEP660103.txt` & `pypef-0.3/pypef/ml/AAindex/SNEP660103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/SUEM840101.txt` & `pypef-0.3/pypef/ml/AAindex/SUEM840101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/SUEM840102.txt` & `pypef-0.3/pypef/ml/AAindex/SUEM840102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/SWER830101.txt` & `pypef-0.3/pypef/ml/AAindex/SWER830101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/TAKK010101.txt` & `pypef-0.3/pypef/ml/AAindex/TAKK010101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/TANS770101.txt` & `pypef-0.3/pypef/ml/AAindex/TANS770101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/TANS770102.txt` & `pypef-0.3/pypef/ml/AAindex/TANS770102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/TANS770103.txt` & `pypef-0.3/pypef/ml/AAindex/TANS770103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/TANS770104.txt` & `pypef-0.3/pypef/ml/AAindex/TANS770104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/TANS770105.txt` & `pypef-0.3/pypef/ml/AAindex/TANS770105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/TANS770106.txt` & `pypef-0.3/pypef/ml/AAindex/TANS770106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/TANS770107.txt` & `pypef-0.3/pypef/ml/AAindex/TANS770107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/TANS770108.txt` & `pypef-0.3/pypef/ml/AAindex/TANS770108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/TANS770109.txt` & `pypef-0.3/pypef/ml/AAindex/TANS770109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/TANS770110.txt` & `pypef-0.3/pypef/ml/AAindex/TANS770110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/TSAJ990101.txt` & `pypef-0.3/pypef/ml/AAindex/TSAJ990101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/TSAJ990102.txt` & `pypef-0.3/pypef/ml/AAindex/TSAJ990102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/VASM830101.txt` & `pypef-0.3/pypef/ml/AAindex/VASM830101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/VASM830102.txt` & `pypef-0.3/pypef/ml/AAindex/VASM830102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/VASM830103.txt` & `pypef-0.3/pypef/ml/AAindex/VASM830103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/VELV850101.txt` & `pypef-0.3/pypef/ml/AAindex/VELV850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/VENT840101.txt` & `pypef-0.3/pypef/ml/AAindex/VENT840101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/VHEG790101.txt` & `pypef-0.3/pypef/ml/AAindex/VHEG790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/VINM940101.txt` & `pypef-0.3/pypef/ml/AAindex/VINM940101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/VINM940102.txt` & `pypef-0.3/pypef/ml/AAindex/VINM940102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/VINM940103.txt` & `pypef-0.3/pypef/ml/AAindex/VINM940103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/VINM940104.txt` & `pypef-0.3/pypef/ml/AAindex/VINM940104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WARP780101.txt` & `pypef-0.3/pypef/ml/AAindex/WARP780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WEBA780101.txt` & `pypef-0.3/pypef/ml/AAindex/WEBA780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WERD780101.txt` & `pypef-0.3/pypef/ml/AAindex/WERD780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WERD780102.txt` & `pypef-0.3/pypef/ml/AAindex/WERD780102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WERD780103.txt` & `pypef-0.3/pypef/ml/AAindex/WERD780103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WERD780104.txt` & `pypef-0.3/pypef/ml/AAindex/WERD780104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WILM950101.txt` & `pypef-0.3/pypef/ml/AAindex/WILM950101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WILM950102.txt` & `pypef-0.3/pypef/ml/AAindex/WILM950102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WILM950103.txt` & `pypef-0.3/pypef/ml/AAindex/WILM950103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WILM950104.txt` & `pypef-0.3/pypef/ml/AAindex/WILM950104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WIMW960101.txt` & `pypef-0.3/pypef/ml/AAindex/WIMW960101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WOEC730101.txt` & `pypef-0.3/pypef/ml/AAindex/WOEC730101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WOLR790101.txt` & `pypef-0.3/pypef/ml/AAindex/WOLR790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WOLR810101.txt` & `pypef-0.3/pypef/ml/AAindex/WOLR810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WOLS870101.txt` & `pypef-0.3/pypef/ml/AAindex/WOLS870101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WOLS870102.txt` & `pypef-0.3/pypef/ml/AAindex/WOLS870102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/WOLS870103.txt` & `pypef-0.3/pypef/ml/AAindex/WOLS870103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/YANJ020101.txt` & `pypef-0.3/pypef/ml/AAindex/YANJ020101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/YUTK870101.txt` & `pypef-0.3/pypef/ml/AAindex/YUTK870101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/YUTK870102.txt` & `pypef-0.3/pypef/ml/AAindex/YUTK870102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/YUTK870103.txt` & `pypef-0.3/pypef/ml/AAindex/YUTK870103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/YUTK870104.txt` & `pypef-0.3/pypef/ml/AAindex/YUTK870104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ZASB820101.txt` & `pypef-0.3/pypef/ml/AAindex/ZASB820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ZHOH040101.txt` & `pypef-0.3/pypef/ml/AAindex/ZHOH040101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ZHOH040102.txt` & `pypef-0.3/pypef/ml/AAindex/ZHOH040102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ZHOH040103.txt` & `pypef-0.3/pypef/ml/AAindex/ZHOH040103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ZIMJ680101.txt` & `pypef-0.3/pypef/ml/AAindex/ZIMJ680101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ZIMJ680102.txt` & `pypef-0.3/pypef/ml/AAindex/ZIMJ680102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ZIMJ680103.txt` & `pypef-0.3/pypef/ml/AAindex/ZIMJ680103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ZIMJ680104.txt` & `pypef-0.3/pypef/ml/AAindex/ZIMJ680104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/AAindex/ZIMJ680105.txt` & `pypef-0.3/pypef/ml/AAindex/ZIMJ680105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/parallelization.py` & `pypef-0.3/pypef/ml/parallelization.py`

 * *Files identical despite different names*

### Comparing `pypef-0.2.4/pypef/ml/regression.py` & `pypef-0.3/pypef/ml/regression.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # https://doi.org/10.1021/acs.jcim.1c00099
 # Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
 # 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
 # 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
 # *Corresponding author
 # §Equal contribution
 
-
 """
 Main modules for regression/ML including feature generation
 (i.e. sequence encoding), cross-validation-based hyperparameter
 tuning, prediction, and plotting routines.
 """
 
 
@@ -29,48 +28,59 @@
 
 import logging
 logger = logging.getLogger('pypef.ml.regression')
 import matplotlib
 matplotlib.use('Agg')  # no plt.show(), just save plot
 import matplotlib.pyplot as plt
 import numpy as np
-from scipy import stats
 import pickle
 from tqdm import tqdm  # progress bars
-from adjustText import adjust_text
 from sklearn.model_selection import LeaveOneOut
 from sklearn.model_selection import KFold
-from sklearn.metrics import mean_squared_error, r2_score
+from sklearn.metrics import mean_squared_error
 from sklearn.model_selection import GridSearchCV  # default: refit=True
 
 # import regression models
 from sklearn.cross_decomposition import PLSRegression
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.svm import SVR
 from sklearn.neural_network import MLPRegressor
 from sklearn.linear_model import Ridge, Lasso, ElasticNet
 
 from pypef.utils.variant_data import (
-    amino_acids, get_sequences_from_file,
-    remove_nan_encoded_positions, get_basename
+    amino_acids, get_sequences_from_file, get_basename
 )
-from pypef.dca.encoding import DCAEncoding, get_dca_data_parallel
+from pypef.utils.plot import plot_y_true_vs_y_pred
+from pypef.utils.performance import get_performances
+from pypef.dca.hybrid_model import plmc_or_gremlin_encoding
 
 import warnings
 warnings.filterwarnings(action='ignore', category=RuntimeWarning, module='numpy')
 # ignoring warnings of PLS regression when using n_components
 warnings.filterwarnings(action='ignore', category=RuntimeWarning, module='sklearn')
 warnings.filterwarnings(action='ignore', category=UserWarning, module='sklearn')
 warnings.filterwarnings(action='ignore', category=DeprecationWarning, module='sklearn')
 # FutureWarning: The default of 'normalize' will be set to False in version 1.2 and deprecated in version 1.4.
 # If you wish to scale the data, use Pipeline with a StandardScaler in a preprocessing stage.
 # sklearn: The default value of 'normalize' should be changed to False in linear models where now normalize=True
 warnings.filterwarnings(action='ignore', category=FutureWarning, module='sklearn')
 
 
+# globals
+x_train = None
+x_test = None
+y_train = None
+y_test = None
+train_variants = None
+test_variants = None
+train_sequences = None
+test_sequences = None
+model_type = None
+
+
 def read_models(number):
     """
     reads the models found in the file Model_Results.txt.
     If no model was trained, the .txt file does not exist.
     """
     try:
         ls = ""
@@ -327,14 +337,15 @@
 
     def collect_encoded_sequences(self, silence=False) -> list:
         encoded_sequences = []
         for sequence in tqdm(self.sequences, disable=silence):
             encoded_sequences.append(self.one_hot_encode_sequence(sequence))
         return np.array(encoded_sequences)
 
+
 def pls_loocv(
         x_train: np.ndarray,
         y_train: np.ndarray
 ) -> Union[tuple[str, str], tuple[PLSRegression, dict]]:
     """
     PLS regression with LOOCV n_components tuning as described by Cadet et al.
     https://doi.org/10.1186/s12859-018-2407-8
@@ -533,49 +544,46 @@
         couplings_file: str = None,
         threads: int = 1  # for parallelization of DCA-based encoding
 ):
     """
     returns the sorted list of all the model parameters and the
     performance values (R2 etc.) from function get_performances.
     """
+    global x_train, y_train, train_variants, train_sequences, \
+        x_test, y_test, test_variants, test_sequences, \
+        model_type
     encoding = encoding.lower()
     performance_list = []
     train_sequences, train_variants, y_train = get_sequences_from_file(train_set)
     test_sequences, test_variants, y_test = get_sequences_from_file(test_set)
     if encoding == 'onehot':  # OneHot-based encoding
         x_onehot_train = OneHotEncoding(train_sequences)
         x_onehot_test = OneHotEncoding(test_sequences)
         x_train = x_onehot_train.collect_encoded_sequences()
         x_test = x_onehot_test.collect_encoded_sequences()
         r2, rmse, nrmse, pearson_r, spearman_rho, regression_model, \
             params = get_regressor_performances(x_train, x_test, y_train, y_test, regressor, verbose=True)
         if r2 is not None:  # get_regressor_performances() returns None for metrics if MSE can't be calculated
             performance_list.append([
-                'ONEHOTMODEL', r2, rmse, nrmse, pearson_r,
+                encoding.upper(), r2, rmse, nrmse, pearson_r,
                 spearman_rho, regression_model, params
             ])
-    elif encoding == 'dca':
-        if threads > 1:  # NaNs are already being removed by the called function
-            dca_encoder = DCAEncoding(couplings_file, verbose=False)
-            logger.info('Parallel encoding (runs DCA encoding silent, '
-                        'no information about non-encoded variant positions)...')
-            train_variants, x_train, y_train = get_dca_data_parallel(train_variants, y_train, dca_encoder, threads)
-            test_variants, x_test, y_test = get_dca_data_parallel(test_variants, y_test, dca_encoder, threads)
-        else:
-            dca_encoder = DCAEncoding(couplings_file)
-            x_train_ = dca_encoder.collect_encoded_sequences(train_variants)
-            x_test_ = dca_encoder.collect_encoded_sequences(test_variants)
-            # NaNs must still be removed
-            x_train, y_train = remove_nan_encoded_positions(x_train_, y_train)
-            x_test, y_test = remove_nan_encoded_positions(x_test_, y_test)
+    elif encoding == 'dca':  # 'plmc' or encoding == 'gremlin':
+        x_train, train_variants, train_sequences, y_train, x_wt, model, model_type = plmc_or_gremlin_encoding(
+            train_variants, train_sequences, y_train, couplings_file, threads=threads
+        )
+        x_test, test_variants, test_sequences, y_test, x_wt, model, model_type = plmc_or_gremlin_encoding(
+            test_variants, test_sequences, y_test, couplings_file, threads=threads
+        )
+
         r2, rmse, nrmse, pearson_r, spearman_rho, regression_model, \
             params = get_regressor_performances(x_train, x_test, y_train, y_test, regressor, verbose=True)
         if r2 is not None:  # get_regressor_performances() returns None for metrics if MSE can't be calculated
             performance_list.append([
-                'DCAMLMODEL', r2, rmse, nrmse, pearson_r,
+                encoding.upper(), r2, rmse, nrmse, pearson_r,
                 spearman_rho, regression_model, params
             ])
 
     else:  # AAindex-based encoding
         aa_indices = [file for file in os.listdir(path_aaindex_dir()) if file.endswith('.txt')]
         # loop over the 566 AAindex entries, encode with each AAindex and test performance
         # can be seen as a AAindex hyperparameter search on the test set  --> also see CV performance
@@ -614,15 +622,15 @@
 
     return performance_list
 
 
 def formatted_output(
         performance_list,
         no_fft=False,
-        minimum_r2=0.0
+        minimum_r2=-1E9
 ):
     """
     Takes the sorted list from function r2_list and writes the model names with an R2 ≥ 0
     as well as the corresponding parameters for each model so that the user gets
     a list (Model_Results.txt) of the top ranking models for the given validation set.
     """
 
@@ -636,15 +644,15 @@
             value3.append('{:f}'.format(val3))
             value4.append('{:f}'.format(val4))
             value5.append('{:f}'.format(val5))
             regression_model.append(r_m.upper())
             params.append(pam)
 
     if len(value) == 0:  # Criterion of not finding suitable model is defined by Minimum_R2
-        raise ValueError('No model with positive R2.')
+        raise SystemError(f'No model with minimum R2 ({minimum_r2}).')
 
     data = np.array([index, value, value2, value3, value4, value5, regression_model, params]).T
     col_width = max(len(str(value)) for row in data for value in row[:-1]) + 5
 
     head = ['Index', 'R2', 'RMSE', 'NRMSE', 'Pearson\'s r', 'Spearman\'s rho', 'Regression', 'Model parameters']
     with open('Model_Results.txt', 'w') as f:
         if no_fft is not False:
@@ -697,53 +705,14 @@
                 y_predicted_total.append(float(values))
         except UserWarning:
             continue
 
     return y_test_total, y_predicted_total
 
 
-def get_performances(
-        y_true: list,
-        y_pred: list
-) -> tuple[float, float, float, float, float]:
-    """
-    Description
-    -----------
-    Gets performance metrics (R^2, RMSE, NRMSE, Pearson's r, Spearman's rho)
-    between y_true and y_pred.
-
-    Parameters
-    -----------
-    y_true: list
-        Measured fitness values.
-    y_pred: list
-        Predicted fitness values.
-
-    Returns
-    -----------
-    r_squared: float
-    rmse: float
-    nrmse: float
-    pearson_r: float
-    spearman_rho: float
-    """
-    y_true = list(y_true)
-    y_pred = list(y_pred)
-    r_squared = r2_score(y_true, y_pred)
-    rmse = np.sqrt(mean_squared_error(y_true, y_pred))
-    stddev = np.std(y_true, ddof=1)
-    nrmse = rmse / stddev
-    with warnings.catch_warnings():  # catching RunTime warning when there's no variance in an array,
-        warnings.simplefilter("ignore")  # e.g. [2, 2, 2, 2] which would mean divide by zero
-        pearson_r = np.corrcoef(y_true, y_pred)[0][1]
-        spearman_rho = stats.spearmanr(y_true, y_pred)[0]
-
-    return r_squared, rmse, nrmse, pearson_r, spearman_rho
-
-
 def get_regressor(
         regressor: str,
         parameter: dict
 ):
     """
     Returns the tuned CVRegressor with the tuned hyperparameters.
     Regression options are
@@ -798,244 +767,246 @@
     else:
         raise SystemError("Did not find specified regression model as valid option. "
                           "See '--help' for valid regression model options.")
 
     return regressor_
 
 
+def encode_based_on_type(
+        encoding: str,
+        variants,
+        sequences,
+        y_true=None,
+        couplings_file=None,
+        idx=None,
+        threads=1,
+        no_fft=True,
+        substitution_sep='/',
+        verbose=True
+):
+    if y_true is None:
+        y_true = np.zeros(np.shape(sequences))
+    if encoding == 'aaidx':  # AAindex encoding technique
+        encoder = AAIndexEncoding(full_aaidx_txt_path(idx), list(np.atleast_1d(sequences)))
+        if no_fft is False:  # use FFT on encoded sequences (default)
+            x, _ = encoder.collect_encoded_sequences()
+        else:  # use raw encoding (no FFT used on encoded sequences)
+            _, x = encoder.collect_encoded_sequences()
+    elif encoding == 'onehot':  # OneHot encoding technique
+        encoder = OneHotEncoding(sequences)
+        x = encoder.collect_encoded_sequences()
+    elif encoding == 'dca':  # PLMC or GREMLIN-based encoding
+        x, variants, sequences, y_true, x_wt, model, model_type = plmc_or_gremlin_encoding(
+            variants, sequences, y_true, couplings_file, substitution_sep, threads, verbose
+        )
+    else:
+        raise SystemError("Unknown encoding option.")
+
+    assert len(x) == len(variants) == len(sequences) == len(y_true)
+    return x, variants, sequences, y_true
+
+
+def crossval_on_all(x_train, x_test, y_train, y_test, regressor: str, parameter, idx=None, no_fft=False):
+    """
+    Use e.g. 80 %  of all data for learning (hyperparameter tuning via validation)
+    and e.g. 20 % for testing 5 times for 5-fold cross validation.
+    """
+    name = get_basename(idx)
+    cv_filename = os.path.join('CV_performance', f'{name}_{regressor.upper()}_CV_Results.txt')
+    try:
+        os.remove(cv_filename)
+    except FileNotFoundError:
+        pass
+    file = open(cv_filename, 'w')
+    file.write('5-fold cross-validated performance of top '
+               'models for validation set across all data.\n\n')
+    if no_fft:
+        file.write("No FFT used in this model construction, performance represents"
+                   " model accuracies on raw encoded sequence data.\n\n")
+    file.close()
+
+    x = np.concatenate([x_train, x_test])
+    y = np.concatenate([y_train, y_test])
+
+    regressor_ = get_regressor(regressor, parameter)
+    # perform 5-fold cross-validation on all data (on X and Y)
+    n_samples = 5
+    y_test_total, y_predicted_total = cross_validation(x, y, regressor_, n_samples)
+
+    r_squared, rmse, nrmse, pearson_r, spearman_rho = \
+        get_performances(y_test_total, y_predicted_total)
+
+    with open(cv_filename, 'a') as f:
+        f.write('Regression type: {}; Parameter: {}; Encoding index: {}\n'.format(
+            regressor.upper(), parameter, name))
+        f.write('R2 = {:.5f}; RMSE = {:.5f}; NRMSE = {:.5f}; Pearson\'s r = {:.5f};'
+                ' Spearman\'s rho = {:.5f}\n\n'.format(r_squared, rmse, nrmse, pearson_r, spearman_rho))
+
+    figure, ax = plt.subplots()
+    legend = r'$R^2$' + f' = {r_squared:.3f}' + f'\nRMSE = {rmse:.3f}' + f'\nNRMSE = {nrmse:.3f}' + \
+             f'\nPearson\'s ' + r'$r$' + f' = {pearson_r:.3f}' + f'\nSpearman\'s ' + \
+             fr'$\rho$ = {spearman_rho:.3f}' + '\n' + fr'($N$ = {len(y_test_total)})'
+    ax.scatter(
+        y_test_total, y_predicted_total,
+        marker='o', s=20, linewidths=0.5, edgecolor='black', label=legend, alpha=0.8
+    )
+    ax.plot([min(y_test_total) - 1, max(y_test_total) + 1],
+            [min(y_predicted_total) - 1, max(y_predicted_total) + 1], 'k', lw=0.5)
+
+    ax.set_xlabel('Measured')
+    ax.set_ylabel('Predicted')
+    ax.legend(prop={'size': 8})
+    plt.savefig(
+        os.path.join('CV_performance', f'{name}_{regressor.upper()}_{n_samples}-fold-CV.png'),
+        dpi=500
+    )
+    plt.close('all')
+
+
 def save_model(
         path,
-        performance_list,
+        performances,
         training_set,
         test_set,
         threshold=5,
         encoding='aaidx',
         regressor='pls',
         no_fft=False,
         train_on_all=False,
         couplings_file=None,
-        threads: int = 1
+        threads: int = 1,
+        label=False
 ):
     """
     Function Save_Model saves the best -s THRESHOLD models as 'Pickle'
     files (pickle.dump), which can be loaded again for doing predictions.
     Also, in Save_Model included is the def cross_validation-based computing
     of the k-fold CV performance of the n component-optimized model on all
     data (learning + test set); by default  k  is 5 (n_samples = 5).
     Plots of the CV performance for the t best models are stored inside the
     folder CV_performance.
     """
+    global x_train, y_train, train_variants, train_sequences, \
+        x_test, y_test, test_variants, test_sequences, \
+        model_type
     logger.info('Encoding and cross validation on all data (creating folder CV_performance)...')
     regressor = regressor.lower()
     try:
         os.mkdir('CV_performance')
     except FileExistsError:
         pass
     try:
         os.mkdir('Pickles')
     except FileExistsError:
         pass
-    train_sequences, train_variants, y_train = get_sequences_from_file(training_set)
-    test_sequences, test_variants, y_test = get_sequences_from_file(test_set)
+    if encoding != 'aaidx' and x_train is not None and x_test is not None:
+        pass  # take global encodings instead of recomputing DCA encodings
+    else:
+        train_sequences, train_variants, y_train = get_sequences_from_file(training_set)
+        test_sequences, test_variants, y_test = get_sequences_from_file(test_set)
     for i, t in enumerate(range(threshold)):
         try:
-            idx = performance_list[t][0]
-            parameter = performance_list[t][7]
+            idx = performances[t][0]
+            parameter = performances[t][7]
 
-            if encoding == 'onehot' or encoding == 'dca':
-                name = idx
+            if encoding != 'aaidx' and x_train is not None and x_test is not None:
+                pass  # take global encodings instead of recomputing DCA encodings
             else:
-                name = get_basename(idx)
-            cv_filename = os.path.join('CV_performance', f'{name}_{regressor.upper()}_CV_Results.txt')
-            try:
-                os.remove(cv_filename)
-            except FileNotFoundError:
-                pass
-            file = open(cv_filename, 'w')
-            file.write('5-fold cross-validated performance of top '
-                       'models for validation set across all data.\n\n')
-            if no_fft:
-                file.write("No FFT used in this model construction, performance represents"
-                           " model accuracies on raw encoded sequence data.\n\n")
-            file.close()
-
-            # Estimating the CV performance of the n_component-fitted model on all data
-            if encoding == 'aaidx':  # AAindex encoding technique
-                x_aaidx_train = AAIndexEncoding(full_aaidx_txt_path(idx), train_sequences)
-                x_aaidx_test = AAIndexEncoding(full_aaidx_txt_path(idx), test_sequences)
-                if no_fft is False:  # use FFT on encoded sequences (default)
-                    x_train, _ = x_aaidx_train.collect_encoded_sequences()
-                    x_test, _ = x_aaidx_test.collect_encoded_sequences()
-                else:  # use raw encoding (no FFT used on encoded sequences)
-                    _, x_train = x_aaidx_train.collect_encoded_sequences()
-                    _, x_test = x_aaidx_test.collect_encoded_sequences()
-            elif encoding == 'onehot':  # OneHot encoding technique
-                x_onehot_train = OneHotEncoding(train_sequences)
-                x_onehot_test = OneHotEncoding(test_sequences)
-                x_train = x_onehot_train.collect_encoded_sequences()
-                x_test = x_onehot_test.collect_encoded_sequences()
-            else:  # DCA
-                dca_encoder = DCAEncoding(couplings_file, verbose=False)
-                if threads > 1:  # parallelization of encoding, NaNs are already being removed by the called function
-                    train_variants, x_train, y_train = get_dca_data_parallel(train_variants, y_train, dca_encoder, threads)
-                    test_variants, x_test, y_test = get_dca_data_parallel(test_variants, y_test, dca_encoder, threads)
-                else:  # encode using a single thread
-                    x_train_ = dca_encoder.collect_encoded_sequences(train_variants)
-                    x_test_ = dca_encoder.collect_encoded_sequences(test_variants)
-
-                    x_train, y_train, train_variants = remove_nan_encoded_positions(x_train_, y_train, train_variants)
-                    x_test, y_test, test_variants = remove_nan_encoded_positions(x_test_, y_test, test_variants)
-
-                    assert len(x_train) == len(y_train) == len(train_variants)
-                    assert len(x_test) == len(y_test) == len(test_variants)
-
-            x = np.concatenate([x_train, x_test])
-            y = np.concatenate([y_train, y_test])
+                x_train, train_variants, train_sequences, y_train = encode_based_on_type(
+                    encoding, train_variants, train_sequences, y_train, couplings_file, idx, threads, no_fft
+                )
+                x_test, test_variants, test_sequences, y_test = encode_based_on_type(
+                    encoding, test_variants, test_sequences, y_test, couplings_file, idx, threads, no_fft
+                )
 
+            crossval_on_all(x_train, x_test, y_train, y_test, regressor, parameter, idx, no_fft)
             regressor_ = get_regressor(regressor, parameter)
-            # perform 5-fold cross-validation on all data (on X and Y)
-            n_samples = 5
-            y_test_total, y_predicted_total = cross_validation(x, y, regressor_, n_samples)
-
-            r_squared, rmse, nrmse, pearson_r, spearman_rho = \
-                get_performances(y_test_total, y_predicted_total)
-
-            with open(cv_filename, 'a') as f:
-                f.write('Regression type: {}; Parameter: {}; Encoding index: {}\n'.format(
-                    regressor.upper(), parameter, name))
-                f.write('R2 = {:.5f}; RMSE = {:.5f}; NRMSE = {:.5f}; Pearson\'s r = {:.5f};'
-                        ' Spearman\'s rho = {:.5f}\n\n'.format(r_squared, rmse, nrmse, pearson_r, spearman_rho))
-
-            figure, ax = plt.subplots()
-            legend = r'$R^2$' + f' = {r_squared:.3f}' + f'\nRMSE = {rmse:.3f}' + f'\nNRMSE = {nrmse:.3f}' + \
-                     f'\nPearson\'s ' + r'$r$'+f' = {pearson_r:.3f}' + f'\nSpearman\'s ' + \
-                     fr'$\rho$ = {spearman_rho:.3f}' + '\n' + fr'($N$ = {len(y_test_total)})'
-            ax.scatter(
-                y_test_total, y_predicted_total,
-                marker='o', s=20, linewidths=0.5, edgecolor='black', label=legend, alpha=0.8
-            )
-            ax.plot([min(y_test_total) - 1, max(y_test_total) + 1],
-                    [min(y_predicted_total) - 1, max(y_predicted_total) + 1], 'k', lw=0.5)
-
-            ax.set_xlabel('Measured')
-            ax.set_ylabel('Predicted')
-            ax.legend(prop={'size': 8})
-            plt.savefig(os.path.join('CV_performance', f'{name}_{regressor.upper()}_{n_samples}-fold-CV.png'), dpi=300)
-            plt.close('all')
-
             if train_on_all:  # Train model hyperparameters based on all available data (training + test set)
                 # But, no generalization performance can be estimated as the model also trained on the test set
+                x = np.concatenate([x_train, x_test])
+                y = np.concatenate([y_train, y_test])
                 regressor_.fit(x, y)
             else:
                 # fit (only) on full learning set (FFT or noFFT is defined already above)
                 regressor_.fit(x_train, y_train)
-
-            y_test_pred = []  # 2D prediction array output to 1D
-            for value in regressor_.predict(x_test):
-                y_test_pred.append(float(value))
-            y_test_pred = np.array(y_test_pred)
-
+            # 2D prediction array output to 1D
+            y_test_pred = np.array(regressor_.predict(x_test)).flatten()
             plot_y_true_vs_y_pred(
                 y_true=y_test,
                 y_pred=y_test_pred,
                 variants=test_variants,
-                label=True,
+                label=label,
                 hybrid=False,
-                name=f'{name}_{regressor.upper()}_'
+                name=f'{get_basename(idx)}_{regressor.upper()}_'
             )
-
+            name = get_basename(idx)
+            if model_type in ['PLMC', 'GREMLIN'] and encoding not in ['aaidx', 'onehot']:
+                name = 'ML' + model_type.lower()
+            logger.info(f'Saving model as {name}')
             file = open(os.path.join(path, 'Pickles', name), 'wb')
             pickle.dump(regressor_, file)
             file.close()
 
         except IndexError:
-            break
+            raise IndexError
+        #    break
 
         if encoding == 'onehot' or encoding == 'dca':   # only 1 model/encoding  -->
             break                                       # no further iteration needed, thus break loop
 
 
 def predict(
-        path=None,
+        path,
+        model,
         prediction_set=None,
-        model=None,
         encoding='aaidx',
         mult_path=None,
         no_fft=False,
         variants=None,
         sequences=None,
         couplings_file=None,
-        dca_encoder: DCAEncoding = None,
-        threads: int = 1  # for parallelization of DCA-based encoding
+        threads: int = 1,  # for parallelization of DCA-based encoding
+        substitution_sep='/',
+        verbose=False
 ):
     """
     The function Predict is used to perform predictions.
     Saved pickle files of models will be loaded again:
       mod = pickle.load(file)
     and used for predicting the label y (y = mod.predict(x))
     of sequences given in the Prediction_Set.fasta.
     """
-    if model is not None:
-        # model defines pickle to load (and thus determines encoding AAidx)
-        file = open(os.path.join(path, 'Pickles', str(model)), 'rb')
-        loaded_model = pickle.load(file)
-        file.close()
-        aaidx = full_aaidx_txt_path(str(model) + '.txt')
-    else:
-        aaidx = None
-        loaded_model = None
-    if sequences is None and variants is None:  # File-based prediction with AAidx
+    # model defines pickle to load (and thus determines encoding AAidx)
+    file = open(os.path.join(path, 'Pickles', str(model)), 'rb')
+    loaded_model = pickle.load(file)
+    file.close()
+    idx = None
+    if encoding == 'aaidx':
+        idx = model + '.txt'
+    if sequences is None and variants is None:  # File-based prediction
         sequences, variants, _ = get_sequences_from_file(prediction_set, mult_path)
 
-    if encoding == 'aaidx':  # AAidx
-        # Directed evolution with AAidx, means sequences is only 1 sequence, thus
-        x_aaidx = AAIndexEncoding(aaidx, np.atleast_1d(sequences).tolist())  # at least 1D if only 1 sequence inputted
-        x, x_raw = x_aaidx.collect_encoded_sequences()
-    elif encoding == 'onehot':  # OneHot
-        x_onehot = OneHotEncoding(np.atleast_1d(sequences).tolist())
-        if len(sequences) == 1:
-            silence = True
-        else:
-            silence = False
-        x = x_onehot.collect_encoded_sequences(silence=silence)
-        x_raw = None
-    else:  # DCA
-        if dca_encoder is not None:  # use dca_encoder from directed evolution, single thread
-            x_ = dca_encoder.collect_encoded_sequences(variants)
-            x, variants = remove_nan_encoded_positions(x_, variants)
-            x_raw = None
-
-        else:
-            if threads > 1:
-                dca_encoder = DCAEncoding(couplings_file, verbose=False)
-                logger.info('Parallel encoding (runs DCA encoding silent, '
-                            'no information about non-encoded variant positions)...')
-                # parallel encoding of variants, NaNs are already being removed by the called function
-                variants, x, _ = get_dca_data_parallel(
-                    variants, list(np.zeros(len(variants))), dca_encoder, threads
-                )
-            else:  # single thread running
-                dca_encoder = DCAEncoding(couplings_file)
-                x_ = dca_encoder.collect_encoded_sequences(variants)
-                x, variants = remove_nan_encoded_positions(x_, variants)
-                x_raw = None
-        if type(x) == list:
-            if not x:
-                return 'skip'
-        elif type(x) == np.ndarray:
-            if not x.any():
-                return 'skip'
+    try:
+        x, variants, sequences, _ = encode_based_on_type(
+            encoding, variants, sequences, None, couplings_file,
+            idx, threads, no_fft, substitution_sep, verbose
+        )
+    except SystemError:
+        return 'skip'
+    if type(x) == list:
+        if not x:
+            return 'skip'
+    elif type(x) == np.ndarray:
+        if not x.any():
+            return 'skip'
 
     assert len(variants) == len(x)
 
     try:
-        if no_fft and encoding == 'aaidx':  # predict using raw AAidx encoding (without FFT)
-            ys = loaded_model.predict(x_raw)
-        else:  # predict AAidx-FFTed or onehot or DCA-based encoding
-            ys = loaded_model.predict(x)
+        ys = loaded_model.predict(x)
     except ValueError:
         raise SystemError(
             "If you used an encoding such as onehot, make sure to use the correct model, e.g. -m ONEHOT. "
             "If you used an AAindex-encoded model you likely tried to predict using a model encoded with "
             "(or without) FFT featurization ('--nofft') while the model was trained without (or with) FFT "
             "featurization so check Model_Results.txt line 1, if the models were trained with or without FFT."
         )
@@ -1045,236 +1016,69 @@
             "Check the specified model provided via the \'-m\' flag."
         )
 
     predictions = [(float(ys[i]), variants[i]) for i in range(len(ys))]  # List of tuples
 
     # Pay attention if increased negative values would define a better variant --> use negative flag
     predictions.sort()
-    predictions.reverse()
-    # if predictions array too large? if Mult_Path is not None: predictions = predictions[:100000]
-
+    predictions.reverse()  # if predictions array is too large?
     return predictions
 
 
-def predictions_out(
-        predictions,
-        model,
-        prediction_set,
-        path: str = ''
-):
-    """
-    Writes predictions (of the new sequence space) to text file(s).
-    """
-    name, value = [], []
-    for (val, nam) in predictions:
-        name.append(nam)
-        value.append('{:f}'.format(val))
-
-    data = np.array([name, value]).T
-    col_width = max(len(str(value)) for row in data for value in row) + 5
-
-    head = ['Name', 'Prediction']
-    path_ = os.path.join(path, 'Predictions_' + str(model) + '_' + str(prediction_set)[:-6] + '.txt')
-    with open(path_, 'w') as f:
-        f.write("".join(caption.ljust(col_width) for caption in head) + '\n')
-        f.write(len(head)*col_width*'-' + '\n')
-        for row in data:
-            f.write("".join(str(value).ljust(col_width) for value in row) + '\n')
-
-
-def predict_and_plot(
+def predict_ts(
         path,
-        fasta_file,
         model,
+        test_set=None,
         encoding='aaidx',
-        label=False,
-        color=False,
-        y_wt=1,
+        idx=None,
         no_fft=False,
         couplings_file=None,
-        threads: int = None
+        label=False,
+        threads: int = 1  # for parallelization of DCA-based encoding
 ):
     """
-    Function Plot is used to make plots of the validation process and
-    shows predicted (Y_pred) vs. measured/"true" (Y_true) protein fitness and
-    calculates the corresponding model performance (R2, (N)RMSE, Pearson's r).
-    Also allows colored version plotting to classify predictions in true or
-    false positive or negative predictions.
-    """
-    sequences_test, variants_test, y_test = get_sequences_from_file(fasta_file)
-    if encoding == 'aaidx':  # AAindex-based encoding
-        aaidx = full_aaidx_txt_path(str(model) + '.txt')
-        aaidx_encoded = AAIndexEncoding(aaidx, sequences_test)
-        x, x_raw = aaidx_encoded.collect_encoded_sequences()
-    elif encoding == 'onehot':  # OneHot-based encoding
-        onehot_encoded = OneHotEncoding(sequences_test)
-        x = onehot_encoded.collect_encoded_sequences()
-        x_raw = None
-    else:  # DCA
-        if threads is None:
-            threads = 1
-        dca_encoder = DCAEncoding(couplings_file)
-        x_raw = None
-        if threads > 1:  # NaNs are already being removed by the called function, for ys just filling 0's
-            variants_test, x, y_test = get_dca_data_parallel(variants_test, y_test, dca_encoder, threads)
-        else:
-            x_ = dca_encoder.collect_encoded_sequences(variants_test)
-            x, variants_test, y_test = remove_nan_encoded_positions(x_, variants_test, y_test)
-        assert len(x) == len(variants_test) == len(y_test)
+    The function Predict is used to perform predictions.
+    Saved pickle files of models will be loaded again:
+      mod = pickle.load(file)
+    and used for predicting the label y (y = mod.predict(x))
+    of sequences given in the Prediction_Set.fasta.
+    """
+    file = open(os.path.join(path, 'Pickles', str(model)), 'rb')
+    loaded_model = pickle.load(file)
+    file.close()
+    if type(loaded_model) == dict:
+        loaded_model = loaded_model['model']
+    if encoding == 'aaidx':
+        idx = model + '.txt'
+
+    sequences, variants, y_test = get_sequences_from_file(test_set)
+    x, variants, sequences, y_test, *_ = encode_based_on_type(
+        encoding, variants, sequences, y_test, couplings_file, idx, threads, no_fft
+    )
+    if type(x) == list:
+        if not x:
+            return 'skip'
+    elif type(x) == np.ndarray:
+        if not x.any():
+            return 'skip'
+    if encoding != 'aaidx':
+        idx = encoding
+
+    assert len(variants) == len(x)
 
     try:
-        file = open(os.path.join(path, 'Pickles', str(model)), 'rb')
-        model_ = pickle.load(file)
-        file.close()
-    except FileNotFoundError:
-        raise FileNotFoundError(
-            f"Did not find specified model: {str(model)}. You can define the "
-            f"threshold of models to be saved; e.g. with pypef run -l LS.fasta "
-            f"-v VS.fasta -s 10 and pay attention to capitalization of model "
-            f"names (e.g. -m PONP930101 or -m ONEHOT."
-        )
-    y_pred = []
-    try:
-        # predicting (again) with (re-)loaded model (that was trained on training or full data)
-        if no_fft and encoding == 'aaidx':  # predict using raw AAidx encoding
-            y_pred_ = model_.predict(x_raw)
-        else:  # predict AAidx-FFTed or onehot or DCA-based encoding
-            y_pred_ = model_.predict(x)
+        y_pred = loaded_model.predict(x)
+        y_pred = list(np.array(y_pred).flatten())
     except ValueError:
-        raise ValueError(
-            "You likely tried to plot a test set with (or without) "
-            "FFT featurization ('--nofft') while the model was trained "
-            "without (or with) FFT featurization. Check the Model_Results.txt "
-            "line 1, if the models were trained using FFT."
-        )
-    for y_p in y_pred_:
-        y_pred.append(float(y_p))
-    r_squared, rmse, nrmse, pearson_r, spearman_rho = \
-        get_performances(y_test, y_pred)
-    legend = '$R^2$ = {}\nRMSE = {}\nNRMSE = {}\nPearson\'s $r$ = {}\nSpearman\'s '.format(
-        round(r_squared, 3), round(rmse, 3), round(nrmse, 3), round(pearson_r, 3)) + \
-             r'$\rho$ = {}'.format(round(spearman_rho, 3)) + \
-             '\n' + r'($N$ = {})'.format(len(y_test))
-    x = np.linspace(min(y_pred), max(y_pred), 100)
-    fig, ax = plt.subplots()
-    ax.scatter(y_test, y_pred,
-               label=legend, marker='o', s=20, linewidths=0.5, edgecolor='black', alpha=0.8)
-    ax.legend(prop={'size': 8})
-    ax.plot(x, x, color='black', linewidth=0.5)  # plot diagonal line
-    if label is not False:
-        logger.info('Adjusting variant labels for plotting can take some '
-                    'time (the limit for labeling is 150 data points)...')
-        if len(y_test) < 150:
-            texts = [ax.text(y_test[i], y_pred[i], txt, fontsize=4) for i, txt in enumerate(variants_test)]
-            adjust_text(texts, only_move={'points': 'y', 'text': 'y'}, force_points=0.5, lim=250)
-        else:
-            logger.info("Terminating label process. Too many variants "
-                        "(> 150) for plotting (labels would overlap).")
-    if color is not False:
-        try:
-            y_wt = float(y_wt)
-        except TypeError:
-            raise TypeError('Needs label value of WT (y_WT) when making color plot (e.g. --color --ywt 1.0)')
-        if y_wt == 0:
-            y_wt = 1E-9  # choose a value close to zero
-        true_v, true_p, false_v, false_p = [], [], [], []
-        for i, v in enumerate(y_test):
-            if y_test[i] / y_wt >= 1 and y_pred[i] / y_wt >= 1:
-                true_v.append(y_test[i]), true_p.append(float(y_pred[i]))
-            elif y_test[i] / y_wt < 1 and y_pred[i] / y_wt < 1:
-                true_v.append(y_test[i]), true_p.append(float(y_pred[i]))
-            else:
-                false_v.append(y_test[i]), false_p.append(float(y_pred[i]))
-        try:
-            ax.scatter(true_v, true_p, color='tab:blue', marker='o', s=20, linewidths=0.5, edgecolor='black')
-        except IndexError:
-            pass
-        try:
-            ax.scatter(false_v, false_p, color='tab:red', marker='o', s=20, linewidths=0.5, edgecolor='black')
-        except IndexError:
-            pass
-        if (y_wt - min(y_test)) < (max(y_test) - y_wt):
-            limit_y_true = float(max(y_test) - y_wt)
-        else:
-            limit_y_true = float(y_wt - min(y_test))
-        limit_y_true = limit_y_true * 1.1
-        if (y_wt - min(y_pred)) < (max(y_pred) - y_wt):
-            limit_y_pred = float(max(y_pred) - y_wt)
-        else:
-            limit_y_pred = float(y_wt - min(y_pred))
-        limit_y_pred = limit_y_pred * 1.1
-        plt.vlines(x=(y_wt + limit_y_true) - (((y_wt + limit_y_true) - (y_wt - limit_y_true)) / 2),
-                   ymin=y_wt - limit_y_pred, ymax=y_wt + limit_y_pred, color='grey', linewidth=0.5)
-        plt.hlines(y=(y_wt + limit_y_pred) - (((y_wt + limit_y_pred) - (y_wt - limit_y_pred)) / 2),
-                   xmin=y_wt - limit_y_true, xmax=y_wt + limit_y_true, color='grey', linewidth=0.5)
-        crossline = np.linspace(y_wt - limit_y_true, y_wt + limit_y_true)
-        plt.plot(crossline, crossline, color='black', linewidth=0.25)
-        steps = float(abs(max(y_pred)))
-        gradient = []
-        for x in np.linspace(0, steps, 100):
-            # arr = np.linspace(x/steps, 1-x/steps, steps)
-            arr = 1 - np.linspace(x / steps, 1 - x / steps, 100)
-            gradient.append(arr)
-        gradient = np.array(gradient)
-        plt.imshow(gradient, extent=[y_wt - limit_y_true, y_wt + limit_y_true,
-                                     y_wt - limit_y_pred, y_wt + limit_y_pred],
-                   aspect='auto', alpha=0.8, cmap='coolwarm')  # RdYlGn
-        plt.xlim([y_wt - limit_y_true, y_wt + limit_y_true])
-        plt.ylim([y_wt - limit_y_pred, y_wt + limit_y_pred])
-    plt.xlabel('Measured')
-    plt.ylabel('Predicted')
-    plt.legend(prop={'size': 8})
-    plt.savefig(str(model) + '_' + str(fasta_file[:-6]) + '.png', dpi=500)
-
-
-def plot_y_true_vs_y_pred(
-        y_true: np.ndarray,
-        y_pred: np.ndarray,
-        variants: np.ndarray,  # just required for labeling
-        label=False,
-        hybrid=False,
-        name: str = ''
-):
-    """
-    Plots predicted versus true values using the hybrid model for prediction.
-    Function called by function predict_ps.
-    """
-    figure, ax = plt.subplots()
-    if hybrid:
-        spearman_rho = stats.spearmanr(y_true, y_pred)[0]
-        ax.scatter(y_true, y_pred, marker='o', s=20, linewidths=0.5, edgecolor='black', alpha=0.7,
-                   label=f'Spearman\'s ' + fr'$\rho$ = {spearman_rho:.3f}' + '\n' + fr'($N$ = {len(y_true)})')
-        file_name = name + 'DCA_Hybrid_Model_LS_TS_Performance.png'
-    else:
-        r_squared, rmse, nrmse, pearson_r, spearman_rho = get_performances(
-            y_true=y_true, y_pred=y_pred
+        raise SystemError(
+            "If you used an encoding such as onehot, make sure to use the correct model, e.g. -m ONEHOT. "
+            "If you used an AAindex-encoded model you likely tried to predict using a model encoded with "
+            "(or without) FFT featurization ('--nofft') while the model was trained without (or with) FFT "
+            "featurization so check Model_Results.txt line 1, if the models were trained with or without FFT."
         )
-        ax.scatter(
-            y_true, y_pred, marker='o', s=20, linewidths=0.5, edgecolor='black', alpha=0.7,
-            label=r'$R^2$' + f' = {r_squared:.3f}' + f'\nRMSE = {rmse:.3f}' + f'\nNRMSE = {nrmse:.3f}' +
-                  f'\nPearson\'s ' + r'$r$'+f' = {pearson_r:.3f}' + f'\nSpearman\'s ' +
-                  fr'$\rho$ = {spearman_rho:.3f}' + '\n' + fr'($N$ = {len(y_true)})'
+    except AttributeError:
+        raise SystemError(
+            "The model specified is likely a hybrid or pure statistical DCA (and no pure ML model).\n"
+            "Check the specified model provided via the \'-m\' flag."
         )
-        file_name = name + 'ML_Model_LS_TS_Performance.png'
-        x = np.linspace(min(y_pred), max(y_pred), 100)
-        ax.plot(x, x, color='black', linewidth=0.25)  # plot diagonal line
-    ax.legend(prop={'size': 8})
-    ax.set_xlabel('Measured')
-    ax.set_ylabel('Predicted')
-    logger.info('Plotting...')
-    if label:
-        logger.info('Adjusting variant labels for plotting can take some '
-                    'time (the limit for labeling is 150 data points)...')
-        if len(y_true) < 150:
-            texts = [ax.text(y_true[i], y_pred[i], txt, fontsize=4)
-                     for i, txt in enumerate(variants)]
-            adjust_text(
-                texts, only_move={'points': 'y', 'text': 'y'}, force_points=0.5, lim=250)
-        else:
-            logger.info("Terminating label process. Too many variants "
-                        "(> 150) for plotting (labels would overlap).")
-    # Uncomment for renaming new plots
-    # i = 1
-    # while os.path.isfile(file_name):
-    #     i += 1  # iterate until finding an unused file name
-    #     file_name = f'DCA_Hybrid_Model_LS_TS_Performance({i}).png'
-    plt.savefig(file_name, dpi=500)
+
+    plot_y_true_vs_y_pred(y_test, y_pred, variants, label, hybrid=False, name=f'{get_basename(idx).upper()}_')
```

### Comparing `pypef-0.2.4/pypef/ml/run.py` & `pypef-0.3/pypef/ml/ml_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,31 +12,30 @@
 # https://doi.org/10.1021/acs.jcim.1c00099
 # Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
 # 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
 # 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
 # *Corresponding author
 # §Equal contribution
 
-
 import os
 from os import listdir
 from os.path import isfile, join
 
 import logging
-logger = logging.getLogger('pypef.ml.run')
+logger = logging.getLogger('pypef.ml.ml_run')
 import ray
 from pypef.ml.parallelization import aaindex_performance_parallel
 
 # importing own modules
 from pypef.ml.regression import (
-    read_models, formatted_output, performance_list, save_model, predict,
-    predictions_out, predict_and_plot
+    read_models, formatted_output, performance_list, save_model, predict, predict_ts
 )
+from pypef.utils.to_file import predictions_out
 from pypef.utils.low_n_mutation_extrapolation import low_n, performance_mutation_extrapolation
-from pypef.utils.variant_data import absolute_path_cwd_file
+
 
 
 def run_pypef_pure_ml(arguments):
     """
     Running the program, importing all required self-made modules and
     running them dependent on user-passed input arguments using docopt
     for argument parsing.
@@ -54,15 +53,15 @@
             except TypeError:
                 print(read_models(5))
         else:
             print(read_models(5))
 
     else:
         if arguments['--ls'] is not None and arguments['--ts'] is not None:  # LS --> TS
-            if arguments['--model'] is None and arguments['--figure'] is None:
+            if arguments['--model'] is None:
                 path = os.getcwd()
                 try:
                     t_save = int(arguments['--save'])
                 except ValueError:
                     t_save = 5
                 # Parallelization of AAindex iteration if threads is not None (but int)
                 if threads > 1 and arguments['--encoding'] == 'aaidx':
@@ -87,61 +86,60 @@
                         couplings_file=arguments['--params'],  # only for DCA
                         threads=threads  # only for DCA
                     )
 
                 formatted_output(
                     performance_list=encoding_performance_list,
                     no_fft=arguments['--nofft'],
-                    minimum_r2=0.0
+                    minimum_r2=-1E9
                 )
 
                 # save_model encodes variants again (possibly change)
                 save_model(
                     path=path,
-                    performance_list=encoding_performance_list,
+                    performances=encoding_performance_list,
                     training_set=arguments['--ls'],
                     test_set=arguments['--ts'],
                     threshold=t_save,
                     encoding=arguments['--encoding'],
                     regressor=arguments['--regressor'],
                     no_fft=arguments['--nofft'],
                     train_on_all=arguments['--all'],
                     couplings_file=arguments['--params'],  # only for DCA
-                    threads=threads  # only for DCA
+                    threads=threads,  # only for DCA
+                    label=arguments['--label']
                 )
 
-        elif arguments['--figure'] is not None and arguments['--model'] is not None:  # plotting
-            path = os.getcwd()
-            predict_and_plot(
-                path=path,
-                fasta_file=arguments['--figure'],
+        # Prediction of single .fasta file
+        elif arguments['--ts'] is not None and arguments['--model'] is not None:
+            predict_ts(
+                path=os.getcwd(),
                 model=arguments['--model'],
+                test_set=arguments['--ts'],
                 encoding=arguments['--encoding'],
-                label=arguments['--label'],
-                color=arguments['--color'],
-                y_wt=arguments['--y_wt'],
                 no_fft=arguments['--nofft'],
                 couplings_file=arguments['--params'],  # only for DCA
-                threads=threads  # only for DCA
+                label=arguments['--label'],
+                threads=threads
             )
-            logger.info('\nCreated plot!\n')
 
-        # Prediction of single .fasta file
         elif arguments['--ps'] is not None and arguments['--model'] is not None:
-            path = os.getcwd()
             predictions = predict(
-                path=path,
+                path=os.getcwd(),
                 prediction_set=arguments['--ps'],
                 model=arguments['--model'],
                 encoding=arguments['--encoding'],
                 mult_path=None,
                 no_fft=arguments['--nofft'],
                 couplings_file=arguments['--params'],  # only for DCA
                 threads=threads  # only for DCA
             )
+            if predictions == 'skip' and not arguments['--params']:
+                raise SystemError("No couplings file provided. DCA-based sequence encoding "
+                                  "requires a (plmc or GREMLIN) parameter file.")
             if arguments['--negative']:
                 predictions = sorted(predictions, key=lambda x: x[0], reverse=False)
             predictions_out(
                 predictions=predictions,
                 model=arguments['--model'],
                 prediction_set=arguments['--ps']
             )
@@ -178,42 +176,42 @@
                     and arguments['--qdiverse'] is False:
                 raise SystemError('Define prediction target for --pmult, e.g. --pmult --drecomb.')
 
             for args in recombs_total:
                 predictions_total = []
                 logger.info(f'Running predictions for variant-sequence files in directory {args[1:-1]}...')
                 path_recomb = path + args
-                os.chdir(path)
-                files = [f for f in listdir(path_recomb) if isfile(join(path_recomb, f)) if f.endswith('.fasta')]
+                files = [path_recomb + f for f in listdir(path_recomb)
+                         if isfile(join(path_recomb, f)) if f.endswith('.fasta')]
                 for i, file in enumerate(files):
-                    logger.info(f'Encoding files ({i+1}/{len(files)}) for prediction...\n')
+                    logger.info(f'Encoding files ({i+1}/{len(files)}) for prediction...')
                     predictions = predict(
                         path=path,
                         prediction_set=file,
                         model=arguments['--model'],
                         encoding=arguments['--encoding'],
                         mult_path=path_recomb,
                         no_fft=arguments['--nofft'],
-                        couplings_file=absolute_path_cwd_file(arguments['--params']),  # only for DCA
+                        couplings_file=arguments['--params'],  # only for DCA
                         threads=threads  # only for DCA
                     )
                     for pred in predictions:
-                        predictions_total.append(pred)  # could implement numpy.save if array gets too large byte size
+                        predictions_total.append(pred)  # if array gets too large?
                 predictions_total = list(dict.fromkeys(predictions_total))  # removing duplicates from list
                 if arguments['--negative']:
                     predictions_total = sorted(predictions_total, key=lambda x: x[0], reverse=False)
                 else:
                     predictions_total = sorted(predictions_total, key=lambda x: x[0], reverse=True)
 
                 predictions_out(
                     predictions=predictions_total,
                     model=arguments['--model'],
-                    prediction_set='Top' + args[1:-1]
+                    prediction_set=f'Top{args[1:-1]}',
+                    path=path_recomb
                 )
-                os.chdir(path)
 
         elif arguments['extrapolation']:
             performance_mutation_extrapolation(
                 encoded_csv=arguments['--input'],
                 cv_regressor=arguments['--regressor'],
                 conc=arguments['--conc']
             )
```

### Comparing `pypef-0.2.4/pypef/utils/directed_evolution.py` & `pypef-0.3/pypef/utils/directed_evolution.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,26 @@
 # §Equal contribution
 
 """
 Modules for performing random evolution walks
 similar as presented by Biswas et al.
 """
 
+
+from __future__ import annotations
 import os
 import re
 import random
 
 import matplotlib.pyplot as plt
 import numpy as np
 import warnings
 from adjustText import adjust_text
+import logging
+logger = logging.getLogger('pypef.utils.directed_evolution')
 
 from pypef.ml.regression import predict
 from pypef.dca.hybrid_model import predict_directed_evolution
 
 # ignoring warnings of scikit-learn regression
 warnings.filterwarnings(action='ignore', category=RuntimeWarning, module='sklearn')
 warnings.filterwarnings(action='ignore', category=UserWarning, module='sklearn')
@@ -49,19 +53,19 @@
             single_vars: list,
             num_iterations: int,
             num_trajectories: int,
             amino_acids: list,
             temp: float,
             path: str,
             model: str = None,
-            no_fft=False,
-            dca_encoder=None,
-            usecsv=False,
-            csvaa=False,
-            negative=False
+            no_fft: bool = False,
+            dca_encoder: str | None = None,
+            usecsv: bool = False,
+            csvaa: bool = False,
+            negative: bool = False
     ):
         """
         Runs in silico directed evolution and plots and writes trajectories.
 
         Parameters
         ----------
         ml_or_hybrid: str
@@ -88,16 +92,16 @@
             accepting new trajectory variants
         path: str
             Just current working directory (os.getcwd())
         model: str
             Loaded Pickle file for regression/hybrid modeling.
         no_fft: bool
             If True, not using FFT for AAindex-based encoding
-        dca_encoder = None or DCAEncoding object
-            dca_encoder = DCAEncoding(
+        dca_encoder = None or PLMC object
+            dca_encoder = PLMC(
                   params_file=arguments['--plmc_params'],
                   separator=arguments['--sep']
             )
         usecsv: bool
             Using only CSV variants for recombination (but all 20 amino acids)
         csvaa: bool
             Using only CSV variants for recombination (but all amino acids that
@@ -117,15 +121,14 @@
         self.path = path
         self.model = model
         self.no_fft = no_fft  # for AAidx only
         self.dca_encoder = dca_encoder
         self.usecsv = usecsv
         self.csvaa = csvaa
         self.negative = negative
-
         self.de_step_counter = 0  # DE steps
         self.traj_counter = 0  # Trajectory counter
 
     def mutate_sequence(
             self,
             seq: str,
             prev_mut_loc: int
@@ -213,14 +216,15 @@
         # iterate through the trial mutation steps for the directed evolution trajectory
         # m = 1 (only 1 mutation per step) instead of (np.random.poisson(2) + 1)
         v_traj, s_traj, y_traj = [], [], []
         v_traj.append('WT')
         y_traj.append(self.y_wt)
         s_traj.append(self.s_wt)
         accepted = 0
+        logger.info(f"Step 0: WT --> {self.y_wt:.3f}")
         for iteration in range(self.num_iterations):  # num_iterations
             self.de_step_counter = iteration
 
             if accepted == 0:
                 prior_mutation_location = random.randint(0, len(self.s_wt))  # not really "prior" as first
             else:  # get prior mutation position
                 prior_mutation_location = int(re.findall(r"\d+", v_traj[-1])[0])
@@ -236,29 +240,34 @@
             new_full_variant = str(self.s_wt[int(new_variant[:-1])-1]) + new_variant  # full variant name, e.g. 'F17A'
             new_sequence = new_var_seq[0][1]
             # encode and predict new sequence fitness
             if self.ml_or_hybrid == 'ml':
                 predictions = predict(  # AAidx, OneHot, or DCA-based pure ML prediction
                     path=self.path,
                     model=self.model,
-                    encoding=self.encoding,
+                    encoding=self.encoding,  # TODO: check names/rename
                     variants=np.atleast_1d(new_full_variant),
                     sequences=np.atleast_1d(new_sequence),
                     no_fft=self.no_fft,
-                    dca_encoder=self.dca_encoder
+                    couplings_file=self.dca_encoder
                 )
 
             else:  # hybrid modeling and prediction
                 predictions = predict_directed_evolution(
                     encoder=self.dca_encoder,
                     variant=self.s_wt[int(new_variant[:-1]) - 1] + new_variant,
+                    sequence=new_sequence,
                     hybrid_model_data_pkl=self.model
                 )
-
-            if predictions == 'skip':  # skip if variant cannot be encoded by DCA-based encoding technique
+            if predictions != 'skip':
+                logger.info(f"Step {self.de_step_counter + 1}: "
+                            f"{self.s_wt[int(new_variant[:-1]) - 1]}{new_variant} --> {predictions[0][0]:.3f}")
+            else:  # skip if variant cannot be encoded by DCA-based encoding technique
+                logger.info(f"Step {self.de_step_counter + 1}: "
+                            f"{self.s_wt[int(new_variant[:-1]) - 1]}{new_variant} --> {predictions}")
                 continue
             new_y, new_var = predictions[0][0], predictions[0][1]  # new_var == new_variant nonetheless
             # probability function for trial sequence
             # The lower the fitness (y) of the new variant, the higher are the chances to get excluded
             with warnings.catch_warnings():  # catching Overflow warning
                 warnings.simplefilter("ignore")
                 try:
@@ -304,38 +313,39 @@
         Plots evolutionary trajectories and saves steps
         in CSV file.
         """
         s_records, v_records, y_records = self.run_de_trajectories()
         # Idea: Standardizing DCA-HybridModel predictions as just trained by Spearman's rho
         # e.g., meaning that fitness values could differ only at the 6th decimal place and only
         # predicted fitness ranks matter and not associated fitness values
-        fig, ax = plt.subplots()  # figsize=(10, 6)
+        fig, ax = plt.subplots(figsize=(10,6))  # figsize=(10, 6)
         ax.locator_params(integer=True)
         y_records_ = []
         for i, fitness_array in enumerate(y_records):
             ax.plot(np.arange(1, len(fitness_array) + 1, 1), fitness_array,
                     '-o', alpha=0.7, markeredgecolor='black', label='EvoTraj' + str(i + 1))
             y_records_.append(fitness_array)
         label_x_y_name = []
         traj_max_len = 0
         for i, v_record in enumerate(v_records):  # i = 1, 2, 3, .., ; v_record = variant label array
             for j, v in enumerate(v_record):      # j = 1, 2, 3, ..., ; v = variant name; y_records[i][j] = fitness
                 if len(v_record) > traj_max_len:
                     traj_max_len = len(v_record)
                 if i == 0:                      # j + 1 -> x-axis position shifted by 1
-                    label_x_y_name.append(ax.text(j + 1, y_records_[i][j], v, size=9))
+                    label_x_y_name.append(ax.text(j + 1, y_records_[i][j], v, size=7))
                 else:
                     if v != 'WT':  # only plot 'WT' name once at i == 0
-                        label_x_y_name.append(ax.text(j + 1, y_records_[i][j], v, size=9))
-        adjust_text(label_x_y_name, only_move={'points': 'y', 'text': 'y'}, force_points=0.5)
+                        label_x_y_name.append(ax.text(j + 1, y_records_[i][j], v, size=7))
+        adjust_text(label_x_y_name, only_move={'points': 'y', 'text': 'y'}, force_points=0.6)
         ax.legend()
         plt.xticks(np.arange(1,  traj_max_len + 1, 1), np.arange(1, traj_max_len + 1, 1))
 
         plt.ylabel('Predicted fitness')
         plt.xlabel('Mutation trial steps')
+        plt.tight_layout()
         plt.savefig(str(self.model) + '_DE_trajectories.png', dpi=500)
         plt.clf()
 
         with open(os.path.join('EvoTraj', 'Trajectories.csv'), 'w') as file:
             file.write('Trajectory;Variant;Sequence;Fitness\n')
             for i in range(self.num_trajectories):
                 v_records_str = str(v_records[i])[1:-1].replace("'", "")
```

### Comparing `pypef-0.2.4/pypef/utils/learning_test_sets.py` & `pypef-0.3/pypef/utils/learning_test_sets.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,32 +41,14 @@
 
 import numpy as np
 import random
 import pandas as pd
 import re
 
 
-def get_wt_sequence(sequence_fasta):
-    """
-    Gets wild-type sequence from defined input file (can be pure sequence or fasta style)
-    """
-    wild_type_sequence = ""
-    try:
-        with open(sequence_fasta, 'r') as sf:
-            for lines in sf.readlines():
-                if lines.startswith(">"):
-                    continue
-                lines = ''.join(lines.split())
-                wild_type_sequence += lines
-    except FileNotFoundError:
-        raise FileNotFoundError("Did not find FASTA file. Check/specify input FASTA "
-                                "sequence file for getting the wild-type sequence.")
-    return wild_type_sequence
-
-
 def csv_input(csv_file):
     """
     Gets input data from defined .csv file (that contains variant names and fitness labels)
     """
     if csv_file is None:
         raise FileNotFoundError(
             f'Did not find (specified) csv file! '
@@ -74,30 +56,32 @@
         )
     return csv_file
 
 
 def drop_rows(
         csv_file,
         amino_acids,
-        threshold_drop
+        threshold_drop,
+        csv_sep: str = ';',
+        mutation_sep: str = '/'
 ):
     """
     Drops rows from .csv data if below defined fitness threshold or if
     amino acid/variant name is unknown or if fitness label is not a digit.
     """
     separator = ';'
     try:
         df_raw = pd.read_csv(csv_file, sep=separator, usecols=[0, 1])
     except ValueError:
         separator = ','
         df_raw = pd.read_csv(csv_file, sep=separator, usecols=[0, 1])
     except FileNotFoundError:
         raise FileNotFoundError(
-            "Specify the input CSV file containing the variant-fitness data. "
-            "Required CSV format: variant;fitness.")
+            f"Specify the input CSV file containing the variant-fitness data. "
+            f"Required CSV format: variant{csv_sep}fitness.")
 
     label = df_raw.iloc[:, 1]
     sequence = df_raw.iloc[:, 0]
 
     dropping_rows = []
 
     for i, row in enumerate(label):
@@ -106,30 +90,32 @@
             if row < threshold_drop:
                 dropping_rows.append(i)
         except ValueError:
             dropping_rows.append(i)
 
     for i, variant in enumerate(sequence):
         try:
-            if '/' in variant:
-                m = re.split(r'/', variant)
+            if mutation_sep in variant:
+                m = re.split(rf'{mutation_sep}', variant)
                 for a, splits in enumerate(m):
                     if splits[0].isdigit() and variant[-1] in amino_acids:
                         continue
                     elif splits[0] not in amino_acids or splits[-1] not in amino_acids:
                         if i not in dropping_rows:
                             dropping_rows.append(i)
-                            # print('Does not know this definition of amino acid substitution: Variant:', variant)
             else:
+                if ',' in variant or ';' in variant or '\t' in variant:
+                    raise SystemError("Found invalid characters (';', ',', or tabulator) in variants. "
+                                      "Check the --mutation_sep flag and try specifying it, e.g. --mutation_sep \',\'.")
                 if variant[0].isdigit() and variant[-1] in amino_acids:
                     continue
                 elif variant not in ['wt', 'wild_type']:
                     if variant[0] not in amino_acids or variant[-1] not in amino_acids:
                         dropping_rows.append(i)
-                        # print('Does not know this definition of amino acid substitution: Variant:', variant)
+
         except TypeError:
             raise TypeError('You might consider checking the input .csv for empty first two columns,'
                             ' e.g. in the last row.')
 
     logger.info(f'No. of dropped rows: {len(dropping_rows)}. '
                 f'Total given variants (if provided plus WT): {len(df_raw)}')
 
@@ -139,15 +125,16 @@
 
     return df
 
 
 def get_variants(
         df,
         amino_acids,
-        wild_type_sequence
+        wild_type_sequence,
+        mutation_sep: str = '/'
 ):
     """
     Gets variants and divides and counts the variant data for single substituted
     and higher substituted variants. Raises NameError if variant naming is not
     matching the given wild-type sequence, e.g. if variant A17C would define
     a substitution at residue Ala-17 to Cys but the wild-type sequence has no Ala
     at position 17.
@@ -156,16 +143,16 @@
     y = df.iloc[:, 1]
     wt_position = None
     single_variants, higher_variants, index_higher, index_lower, \
         higher_values, single_values = [], [], [], [], [], []
     single, double, triple, quadruple, quintuple, sextuple, septuple,\
         octuple, nonuple, decuple, higher = 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
     for i, variant in enumerate(x):
-        if '/' in variant:
-            count = variant.count('/')
+        if mutation_sep in variant:
+            count = variant.count(mutation_sep)
             if count == 1:
                 double += 1
             elif count == 2:
                 triple += 1
             elif count == 3:
                 quadruple += 1
             elif count == 4:
@@ -178,15 +165,15 @@
                 octuple += 1
             elif count == 8:
                 nonuple += 1
             elif count == 9:
                 decuple += 1
             else:
                 higher += 1
-            m = re.split(r'/', variant)
+            m = re.split(rf'{mutation_sep}', variant)
             for a, splits in enumerate(m):
                 if splits[0].isdigit() or splits[0] in amino_acids and splits[-1] in amino_acids:
                     new = int(re.findall(r'\d+', splits)[0])
                     if splits[0] in amino_acids:
                         if splits[0] != wild_type_sequence[new - 1]:
                             raise NameError(
                                 'Position of amino acids in given sequence does not match the given '
@@ -411,50 +398,7 @@
                     name += '/' + single_var
                 separation += 1
         print(f'>{name}', file=myfile)
         print(f';{fitness_values[i]}', file=myfile)
         print(''.join(temp), file=myfile)
         # print(name+';'+str(val[i])+';'+''.join(temp), file=myfile)  # uncomment output: CSV format
     myfile.close()
-
-
-def get_seqs_from_var_name(
-        wt_seq,
-        substitutions,
-        fitness_values
-) -> tuple[list, list, list]:
-    """
-    Similar to function above but just returns sequences
-
-    wt: str
-        Wild-type sequence as string
-    substitutions: list
-        List of substiutuions of a single variant of the format:
-            - Single substitution variant, e.g. variant A123C: ['A123C']
-            - Higher variants, e.g. variant A123C/D234E/F345G: ['A123C', 'D234E, 'F345G']
-            --> Full substitutions list, e.g.: [['A123C'], ['A123C', 'D234E, 'F345G']]
-    fitness_values: list
-        List of ints/floats of the variant fitness values, e.g. for two variants: [1.4, 0.8]
-    """
-    variant, values, sequences = [], [], []
-    for i, var in enumerate(substitutions):  # var are lists of (single or multiple) substitutions
-        temp = list(wt_seq)
-        name = ''
-        separation = 0
-        if var == ['WT']:
-            name = 'WT'
-        else:
-            for single_var in var:  # single entries of substitution list
-                position_index = int(str(single_var)[1:-1]) - 1
-                new_amino_acid = str(single_var)[-1]
-                temp[position_index] = new_amino_acid
-                # checking if multiple entries are inside list
-                if separation == 0:
-                    name += single_var
-                else:
-                    name += '/' + single_var
-                separation += 1
-        variant.append(name)
-        values.append(fitness_values[i])
-        sequences.append(''.join(temp))
-
-    return variant, values, sequences
```

### Comparing `pypef-0.2.4/pypef/utils/low_n_mutation_extrapolation.py` & `pypef-0.3/pypef/utils/low_n_mutation_extrapolation.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # https://doi.org/10.1021/acs.jcim.1c00099
 # Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
 # 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
 # 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
 # *Corresponding author
 # §Equal contribution
 
-
 import os
 import random
 import logging
 logger = logging.getLogger('pypef.utils.low_n_mutation_extrapolation')
 
 import pandas as pd
 import numpy as np
@@ -122,19 +121,19 @@
                     test_idxs.append(n)
             X_train, y_train = X[train_idxs], y[train_idxs]
             X_test, y_test = X[test_idxs], y[test_idxs]
 
             if hybrid_modeling:
                 x_wt = X[0]  # WT should be first CSV variant entry
                 hybrid_model = DCAHybridModel(
-                    X_train=X_train,
+                    x_train=X_train,
                     y_train=y_train,
-                    X_test=X_test,  # only used for adjusting +/- sign of y_dca, can also be None
+                    x_test=X_test,  # only used for adjusting +/- sign of y_dca, can also be None
                     y_test=y_test,  # only used for adjusting +/- sign of y_dca, can also be None
-                    X_wt=x_wt
+                    x_wt=x_wt
                 )
                 beta_1, beta_2, reg = hybrid_model.settings(
                     X_train, y_train, train_size_fit=train_size_train
                 )
                 spearmanr_nruns.append(
                     hybrid_model.spearmanr(
                         y_test,
@@ -267,19 +266,19 @@
         train_df = df_mut_lvl[train_idx]
         train_variants, X_train, y_train = process_df_encoding(train_df)
         all_higher_df = df_mut_lvl[-1]  # only used for adjusting +/- of y_dca
         all_higher_variants, X_all_higher, y_all_higher = process_df_encoding(all_higher_df)
         if hybrid_modeling:
             x_wt = X_train[0]
             hybrid_model = DCAHybridModel(
-                X_train=X_train,
+                x_train=X_train,
                 y_train=y_train,
-                X_test=X_all_higher,  # only used for adjusting +/- of y_dca, can also be None but
+                x_test=X_all_higher,  # only used for adjusting +/- of y_dca, can also be None but
                 y_test=y_all_higher,  # higher risk of wrong sign assignment of beta_1 (y_dca)
-                X_wt=x_wt
+                x_wt=x_wt
             )
             beta_1, beta_2, reg = hybrid_model.settings(
                 X_train, y_train, train_size_fit=train_size)
             pickle.dump(
                 {'hybrid_model': hybrid_model, 'beta_1': beta_1, 'beta_2': beta_2,
                  'spearman_rho': float('nan'), 'regressor': reg},
                 open(os.path.join('Pickles', 'HYBRID_LVL_1'), 'wb')
@@ -424,9 +423,10 @@
     )
     if conc:
         name += '_train_concat_lvls'
     else:
         name += '_train_lvl_1'
     plt.xticks(test_lvls, label_infos, fontsize=5)
     plt.ylabel(r"Spearman's $\rho$")
-    plt.savefig(name + '_extrapolation.png', dpi=500)
+    name = name.replace("\\", "").replace(".", "") + '_extrapolation.png'
+    plt.savefig(name, dpi=500)
     plt.clf()
```

### Comparing `pypef-0.2.4/pypef/utils/prediction_sets.py` & `pypef-0.3/pypef/utils/prediction_sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,22 +39,22 @@
 import numpy as np
 from tqdm import tqdm
 
 
 def make_fasta_ps(
         filename,
         wt,
-        substitution
+        substitutions
 ):
     """
     Creates prediction sets (.fasta style files, i.e. without fitness values)
     """
     myfile = open(filename, 'w')
     count = 0
-    for i, var in enumerate(substitution):
+    for i, var in enumerate(substitutions):
         temporary = list(wt)
         name = ''
         separation = 0
         for single_var in var:
             position_index = int(str(single_var)[1:-1]) - 1
             new_amino_acid = str(single_var)[-1]
             temporary[position_index] = new_amino_acid
@@ -236,15 +236,15 @@
         array,
         single_variants,
         wt_sequence,
         name,
         no
 ):
     """
-    Creates split files from given variants for yielded recombined or diverse variants
+    Creates split files from given variants for yielded recombined or diverse variants.
     """
     if len(array) > 0:
         number_of_split_files = len(array) / (len(single_variants) * 20 ** 3)
         number_of_split_files = round(number_of_split_files)
         if number_of_split_files == 0:
             number_of_split_files += 1
         split = np.array_split(array, number_of_split_files)
@@ -254,14 +254,27 @@
             make_fasta_ps(name_, wt_sequence, i)
 
         os.chdir(pwd)
 
         return ()
 
 
+def make_ssm_singles(wt_seq, aminoacids):
+    """
+    Making diverse single-saturation mutagenesis dataset, i.e., all
+    19 amino acid substitutions at each wild-type sequence position.
+    """
+    ssm_singles = []
+    for i, aa_wt in enumerate(wt_seq):
+        for aa in aminoacids:
+            if aa_wt != aa:
+                ssm_singles.append([f'{aa_wt}{i+1}{aa}'])
+    return ssm_singles
+
+
 def make_combinations_double_all_diverse(arr, aminoacids):
     """
     Make double substituted naturally diverse variants
 
     :parameter arr: List of single substitutions in tuple, e.g.,
     (['L215F'], ['A217N'], ['R219S'], ['L249Y'])
     :parameter aminoacids: List of amino acids to combine, e.g., all 20 naturally occuring:
```

### Comparing `pypef-0.2.4/pypef/utils/run.py` & `pypef-0.3/pypef/utils/utils_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,65 +13,65 @@
 # Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
 # 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
 # 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
 # *Corresponding author
 # §Equal contribution
 
 import os
+
 import logging
-logger = logging.getLogger('pypef.utils.run')
+logger = logging.getLogger('pypef.utils.utils_run')
 
 import numpy as np
 import re
-import copy
-import ray
 
 from pypef.utils.variant_data import (
     amino_acids, generate_dataframe_and_save_csv,
-    remove_nan_encoded_positions, get_basename,
-    read_csv_and_shift_pos_ints
+    get_basename, read_csv_and_shift_pos_ints,
+    get_seqs_from_var_name, get_wt_sequence
 )
 
 from pypef.utils.learning_test_sets import (
-    get_wt_sequence, csv_input, drop_rows, get_variants, make_sub_ls_ts,
-    make_sub_ls_ts_randomly, make_fasta_ls_ts, get_seqs_from_var_name
+    csv_input, drop_rows, get_variants, make_sub_ls_ts,
+    make_sub_ls_ts_randomly, make_fasta_ls_ts
 )
 from pypef.utils.prediction_sets import (
     make_fasta_ps, make_recombinations_double, make_recombinations_triple,
     make_recombinations_quadruple, make_recombinations_quintuple,
     create_split_files, make_combinations_double_all_diverse,
-    make_combinations_triple_all_diverse, make_combinations_quadruple_all_diverse
+    make_combinations_triple_all_diverse, make_combinations_quadruple_all_diverse,
+    make_ssm_singles
 )   # not yet implemented: make_combinations_double_all_diverse_and_all_positions
 
 from pypef.utils.directed_evolution import DirectedEvolution
-from pypef.dca.encoding import DCAEncoding
 from pypef.utils.sto2a2m import convert_sto2a2m
 
-from pypef.dca.encoding import get_dca_data_parallel, get_encoded_sequence
 from pypef.ml.regression import OneHotEncoding, AAIndexEncoding, full_aaidx_txt_path
+from pypef.dca.hybrid_model import plmc_or_gremlin_encoding
 
 
 def run_pypef_utils(arguments):
     if arguments['mklsts']:
         wt_sequence = get_wt_sequence(arguments['--wt'])
         t_drop = float(arguments['--drop'])
 
         logger.info(f'Length of provided sequence: {len(wt_sequence)} amino acids.')
-        df = drop_rows(arguments['--input'], amino_acids, t_drop)
+        df = drop_rows(arguments['--input'], amino_acids, t_drop, arguments['--sep'], arguments['--mutation_sep'])
         no_rnd = arguments['--numrnd']
 
         single_variants, single_values, higher_variants, higher_values = get_variants(
-            df, amino_acids, wt_sequence)
+            df, amino_acids, wt_sequence, arguments['--mutation_sep']
+        )
         logger.info(f'Number of single variants: {len(single_variants)}.')
         if len(single_variants) == 0:
             logger.info('Found NO single substitution variants for possible recombination!')
         sub_ls, val_ls, sub_ts, val_ts = make_sub_ls_ts(
             single_variants, single_values, higher_variants, higher_values)
         logger.info('Tip: You can edit your LS and TS datasets just by '
-              'cutting/pasting between the LS and TS fasta datasets.')
+                    'cutting/pasting between the LS and TS fasta datasets.')
 
         logger.info('Creating LS dataset...')
         make_fasta_ls_ts('LS.fasl', wt_sequence, sub_ls, val_ls)
         logger.info('Creating TS dataset...')
         make_fasta_ls_ts('TS.fasl', wt_sequence, sub_ts, val_ts)
 
         try:
@@ -88,31 +88,36 @@
                 )
                 make_fasta_ls_ts('LS_random_' + str(random_set_counter) + '.fasl', wt_sequence, sub_ls, val_ls)
                 make_fasta_ls_ts('TS_random_' + str(random_set_counter) + '.fasl', wt_sequence, sub_ts, val_ts)
                 random_set_counter += 1
 
     elif arguments['mkps']:
         wt_sequence = get_wt_sequence(arguments['--wt'])
-        csv_file = csv_input(arguments['--input'])
-        t_drop = float(arguments['--drop'])
-        df = drop_rows(csv_file, amino_acids, t_drop)
-        drop_wt = []
-        for i in range(len(df)):
-            if df.iloc[i, 0] == 'WT':
-                logger.info('Dropping wild-type (WT) from DataFrame as it cannot be used for (re-)combination.')
-                drop_wt.append(i)
-        df = df.drop(drop_wt).reset_index(drop=True)
+        if not arguments['--ssm']:
+            try:
+                csv_file = csv_input(arguments['--input'])
+            except FileNotFoundError:
+                raise SystemError("If creating prediction sets ('mkps') a CSV input is "
+                                  "required (if not running 'mkps --ssm').")
+            t_drop = float(arguments['--drop'])
+            df = drop_rows(csv_file, amino_acids, t_drop)
+            drop_wt = []
+            for i in range(len(df)):
+                if df.iloc[i, 0] == 'WT':
+                    logger.info('Dropping wild-type (WT) from DataFrame as it cannot be used for (re-)combination.')
+                    drop_wt.append(i)
+            df = df.drop(drop_wt).reset_index(drop=True)
 
-        logger.info(f'Length of provided sequence: {len(wt_sequence)} amino acids.')
-        single_variants, _, higher_variants, _ = get_variants(df, amino_acids, wt_sequence)
-        logger.info(f'Using single substitution variants for (re-)combination. '
-                    f'Number of single variants: {len(single_variants)}.')
-        if len(single_variants) == 0:
-            logger.info('Found NO single substitution variants for possible recombination! '
-                        'No prediction files can be created!')
+            logger.info(f'Length of provided sequence: {len(wt_sequence)} amino acids.')
+            single_variants, _, higher_variants, _ = get_variants(df, amino_acids, wt_sequence)
+            logger.info(f'Using single substitution variants for (re-)combination. '
+                        f'Number of single variants: {len(single_variants)}.')
+            if len(single_variants) == 0:
+                logger.info('Found NO single substitution variants for possible recombination! '
+                            'No prediction files can be created!')
 
         if arguments['--drecomb']:
             logger.info('Creating Recomb_Double_Split...')
             for no, files in enumerate(make_recombinations_double(single_variants)):
                 double_mutants = np.array(files)
                 create_split_files(double_mutants, single_variants, wt_sequence, 'Recomb_Double', no)
 
@@ -155,35 +160,36 @@
         if arguments['--qdiverse']:
             logger.info('Beware that this step might require much disk space as PyPEF is '
                        'creating prediction files in plain text format. Creating Diverse_Quadruple_Split...')
             for no, files in enumerate(make_combinations_quadruple_all_diverse(single_variants, amino_acids)):
                 quadruples = np.array(files)
                 create_split_files(quadruples, single_variants, wt_sequence, 'Diverse_Quadruple', no + 1)
 
-        if arguments['--drecomb'] is False and arguments['--trecomb'] is False \
-                and arguments['--qarecomb'] is False and arguments['--qirecomb'] is False \
-                and arguments['--ddiverse'] is False and arguments['--tdiverse'] is False \
-                and arguments['--qdiverse'] is False:
+        if arguments['--ssm']:
+            singles = make_ssm_singles(wt_sequence, amino_acids)
+            make_fasta_ps('ssm_singles.fasta', wt_sequence, np.array(singles))
+
+        if True not in [
+            arguments['--drecomb'], arguments['--trecomb'], arguments['--qarecomb'],
+            arguments['--qirecomb'], arguments['--ddiverse'], arguments['--tdiverse'],
+            arguments['--qdiverse'], arguments['--ssm']
+        ]:
             logger.info(f'\nMaking prediction set fasta file from {csv_file}...\n')
             make_fasta_ps(
                 filename=f'{get_basename(csv_file)}_prediction_set.fasta',
                 wt=wt_sequence,
-                substitution=tuple(list(single_variants)+list(higher_variants))
+                substitutions=tuple(list(single_variants) + list(higher_variants))
             )
 
     # Metropolis-Hastings-driven directed evolution, similar to Biswas et al.:
     # Low-N protein engineering with data-efficient deep learning,
     # see https://github.com/ivanjayapurna/low-n-protein-engineering/tree/master/directed-evo
     elif arguments['directevo']:
         if arguments['hybrid'] or arguments['--encoding'] == 'dca':
-            dca_encoder = DCAEncoding(
-                params_file=arguments['--params'],
-                separator=arguments['--sep'],
-                verbose=False
-            )
+            dca_encoder = arguments['--params']
             if arguments['ml']:
                 ml_or_hybrid = 'ml'
             else:
                 ml_or_hybrid = 'hybrid'
         else:
             dca_encoder = None
             ml_or_hybrid = 'ml'
@@ -225,15 +231,15 @@
                 logger.info('Found NO single substitution variants for possible recombination!')
             single_vars, single_ys = list(single_variants), list(single_values)  # only tuples to lists
 
         else:
             single_vars = None  # What happens now? (Full diverse?)
         # Metropolis-Hastings-driven directed evolution on single mutant .csv amino acid substitution data
         csvaa = arguments['--csvaa']  # only use identified substitutions --> taken from CSV file
-        logger.info('Running evolution trajectories and plotting...\n')
+        logger.info('Running evolution trajectories and plotting...')
         DirectedEvolution(
             ml_or_hybrid=ml_or_hybrid,
             encoding=arguments['--encoding'],
             s_wt=s_wt,
             y_wt=y_wt,
             single_vars=single_vars,
             num_iterations=num_iterations,
@@ -253,88 +259,94 @@
     elif arguments['sto2a2m']:
         convert_sto2a2m(
             sto_file=arguments['--sto'],
             inter_gap=arguments['--inter_gap'],
             intra_gap=arguments['--intra_gap']
         )
 
+    elif arguments['reformat_csv']:
+        read_csv_and_shift_pos_ints(
+            infile=arguments['--input'],
+            offset=0,
+            col_sep=arguments['--sep'],
+            substitution_sep=arguments['--mutation_sep']
+        )
+
     elif arguments['shift_pos']:
         read_csv_and_shift_pos_ints(
             infile=arguments['--input'],
             offset=arguments['--offset'],
+            col_sep=arguments['--sep'],
             substitution_sep=arguments['--mutation_sep']
         )
 
     elif arguments['encode']:  # sole parallelized task for utils for DCA encoding
-        encoded_sequences = None
         df = drop_rows(arguments['--input'], amino_acids, arguments['--drop'])
         wt_sequence = get_wt_sequence(arguments['--wt'])
         logger.info(f'Length of provided sequence: {len(wt_sequence)} amino acids.')
         single_variants, single_values, higher_variants, higher_values = get_variants(
             df, amino_acids, wt_sequence)
         variants = list(single_variants) + list(higher_variants)
-        fitnesses = list(single_values) + list(higher_values)
-        variants, fitnesses, sequences = get_seqs_from_var_name(wt_sequence, variants, fitnesses)
-        assert len(variants) == len(fitnesses) == len(sequences)
+        ys_true = list(single_values) + list(higher_values)
+        variants, ys_true, sequences = get_seqs_from_var_name(wt_sequence, variants, ys_true)
+        assert len(variants) == len(ys_true) == len(sequences)
         logger.info('Encoding variant sequences...')
 
         if arguments['--encoding'] == 'dca':
             threads = abs(arguments['--threads']) if arguments['--threads'] is not None else 1
             threads = threads + 1 if threads == 0 else threads
             logger.info(f'Using {threads} thread(s) for running...')
-            dca_encode = DCAEncoding(
+            xs, variants, sequences, ys_true, x_wt, model, model_type = plmc_or_gremlin_encoding(
+                variants=variants,
+                sequences=sequences,
+                ys_true=ys_true,
                 params_file=arguments['--params'],
-                separator=arguments['--mutation_sep'],
-                verbose=False
+                substitution_sep=arguments['--mutation_sep'],
+                threads=threads,
+                verbose=True
             )
-            if threads > 1:
-                ray.init()
-                variants, encoded_sequences, fitnesses = get_dca_data_parallel(
-                    variants=variants,
-                    fitnesses=fitnesses,
-                    dca_encode=dca_encode,
-                    threads=threads,
-                )
-            else:
-                x_ = dca_encode.collect_encoded_sequences(variants)
-                encoded_sequences, variants = remove_nan_encoded_positions(copy.copy(x_), variants)
-                encoded_sequences, fitnesses = remove_nan_encoded_positions(copy.copy(x_), fitnesses)
-                assert len(encoded_sequences) == len(variants) == len(fitnesses)
+            assert len(xs) == len(variants) == len(ys_true)
 
             if variants[0][0] != variants[0][-1]:  # WT is required for DCA-based hybrid modeling
                 if arguments['--y_wt'] is not None:
                     y_wt = arguments['--y_wt']
                 else:
                     y_wt = 1
                 # better using re then: wt = variants[0][0] + str(variants[0][1:-1] + variants[0][0])
                 wt = variants[0][0] + re.findall(r"\d+", variants[0])[0] + variants[0][0]
-                x_wt = get_encoded_sequence(variant=wt, dca_encode=dca_encode)
+                variants = list(variants)
                 variants.insert(0, wt)  # inserting WT at pos. 0
-                encoded_sequences.insert(0, x_wt)
-                fitnesses.insert(0, y_wt)  # set WT fitness to 1 or use arguments y_wt?
+                xs = list(xs)
+                xs.insert(0, list(x_wt.flatten()))
+                ys_true = list(ys_true)
+                ys_true.insert(0, y_wt)  # set WT fitness to 1 or use arguments y_wt?
 
         elif arguments['--encoding'] == 'onehot':
             onehot_encoder = OneHotEncoding(sequences)
-            encoded_sequences = onehot_encoder.collect_encoded_sequences()
+            xs = onehot_encoder.collect_encoded_sequences()
 
         elif arguments['--encoding'] == 'aaidx':
             if arguments['--model'] is None:
                 raise SystemError(
                     "Define the AAindex to use for encoding with the "
                     "flag --model AAINDEX, e.g.: --model CORJ870104."
                 )
             aa_index_encoder = AAIndexEncoding(
                 full_aaidx_txt_path(arguments['--model'] + '.txt'), sequences
             )
             x_fft, x_raw = aa_index_encoder.collect_encoded_sequences()
             if arguments['--nofft']:
-                encoded_sequences = x_raw
+                xs = x_raw
             else:
-                encoded_sequences = x_fft
+                xs = x_fft
 
+        else:
+            raise SystemError("Unknown encoding option.")
+        logger.info(f'{len(variants)} variants (plus inserted WT) remained after encoding. '
+                    f'Saving to encoding CSV file...')
         generate_dataframe_and_save_csv(  # put WT at pos. 0 for hybrid low_N or extrapolation
             variants=variants,
-            sequence_encodings=encoded_sequences,
-            fitnesses=fitnesses,
+            sequence_encodings=xs,
+            fitnesses=ys_true,
             csv_file=arguments['--input'],
             encoding_type=arguments['--encoding']
         )
```

### Comparing `pypef-0.2.4/pypef/utils/sto2a2m.py` & `pypef-0.3/pypef/utils/sto2a2m.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,28 +14,32 @@
 # 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
 # 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
 # *Corresponding author
 # §Equal contribution
 
 import logging
 logger = logging.getLogger('pypef.utils.sto2a2m')
+
 import numpy as np
 from tqdm import tqdm
 from Bio import AlignIO
 
 
 def convert_sto2a2m(
         sto_file: str,
         inter_gap: float,
         intra_gap: float
 ):
     """
     Converts alignment in format STO to A2M format.
     Removes specific sequences with inter and/or intra gaps
-    over specific thresholds.
+    over specific thresholds. More alignment type transferring
+    options can be performed using the reformat.pl script of the
+    HH-suite; (c) Johannes Soeding, 2012:
+    https://github.com/soedinglab/hh-suite/blob/master/scripts/reformat.pl
     """
     # Generate the a2m output filename
     a2m_file = f"{sto_file.split('.sto')[0]}.a2m"
 
     # Load the stockholm alignment
     logger.info('Loading MSA in stockholm format...')
     sto_alignment = AlignIO.read(sto_file, 'stockholm')
```

### Comparing `pypef-0.2.4/pypef/utils/variant_data.py` & `pypef-0.3/pypef/utils/variant_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,27 +14,46 @@
 # 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
 # 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
 # *Corresponding author
 # §Equal contribution
 
 from __future__ import annotations
 import os
-
 import numpy as np
 import pandas as pd
 
 
 amino_acids = [
     'A', 'C', 'D', 'E', 'F',
     'G', 'H', 'I', 'K', 'L',
     'M', 'N', 'P', 'Q', 'R',
     'S', 'T', 'V', 'W', 'Y'
 ]
 
 
+def get_wt_sequence(sequence_fasta):
+    """
+    Gets wild-type sequence from defined input file (can be pure sequence or fasta style)
+    """
+    if sequence_fasta is None:
+        return None
+    wild_type_sequence = ""
+    try:
+        with open(sequence_fasta, 'r') as sf:
+            for lines in sf.readlines():
+                if lines.startswith(">"):
+                    continue
+                lines = ''.join(lines.split())
+                wild_type_sequence += lines
+    except FileNotFoundError:
+        raise FileNotFoundError("Did not find FASTA file. Check/specify input FASTA "
+                                "sequence file for getting the wild-type sequence.")
+    return wild_type_sequence
+
+
 def read_models(number):
     """
     reads the models found in the file Model_Results.txt.
     If no model was trained, the .txt file does not exist.
     """
     try:
         ls = ""
@@ -132,34 +151,38 @@
 def remove_nan_encoded_positions(
         xs: np.ndarray | list,
         *yss
 ):
     """
     Removes encoded sequence (x) of sequence list xs when NaNs occur in x.
     Also removes the corresponding fitness value y (f(x) --> y) at position i.
-    ys can als be any type of list, e.g. variants or sequences.
+    ys can also be any type of list, e.g. variants or sequences.
     """
-    if type(xs) == np.ndarray:
-        xs = list(xs)
+    xs = list(xs)
     temp = []
     for ys in yss:
         try:
+            ys = list(np.atleast_1d(ys))
             if isinstance(ys, pd.Series):
                 temp.append(list(ys))
             elif ys is None:
                 if len(yss) == 1:
                     temp = (None,)
                 else:
                     temp.append([None])
             else:
-                temp.append(list(ys))
+                if type(ys) == np.ndarray:
+                    if np.array(ys).ndim == 0:
+                        temp.append([list(np.atleast_1d(ys).tolist())])
+                    else:
+                        temp.append(list(np.atleast_1d(ys).tolist()))
+                else:
+                    temp.append(list(ys))
         except ValueError:
             temp.append(list(ys))
-        except TypeError:
-            temp = (None,)
     if temp:
         yss = temp
     if not yss == () and not yss == (None,):
         for i, ys in enumerate(yss):
             assert len(xs) == len(ys), "Number of input sequences to be compared unequal."
             try:
                 for j, x in enumerate(xs):
@@ -203,14 +226,67 @@
     -------
     str
         os.path.basename (filename) string without filename extension
     """
     return os.path.basename(filename).split('.')[0]
 
 
+def get_seqs_from_var_name(
+        wt_seq,
+        substitutions,
+        fitness_values
+) -> tuple[list, list, list]:
+    """
+    Similar to function above but just returns sequences
+
+    wt: str
+        Wild-type sequence as string
+    substitutions: list
+        List of substiutuions of a single variant of the format:
+            - Single substitution variant, e.g. variant A123C: ['A123C']
+            - Higher variants, e.g. variant A123C/D234E/F345G: ['A123C', 'D234E, 'F345G']
+            --> Full substitutions list, e.g.: [['A123C'], ['A123C', 'D234E, 'F345G']]
+    fitness_values: list
+        List of ints/floats of the variant fitness values, e.g. for two variants: [1.4, 0.8]
+    """
+    variant, values, sequences = [], [], []
+    for i, var in enumerate(substitutions):  # var are lists of (single or multiple) substitutions
+        temp = list(wt_seq)
+        name = ''
+        separation = 0
+        if var == ['WT']:
+            name = 'WT'
+        else:
+            for single_var in var:  # single entries of substitution list
+                position_index = int(str(single_var)[1:-1]) - 1
+                new_amino_acid = str(single_var)[-1]
+                temp[position_index] = new_amino_acid
+                # checking if multiple entries are inside list
+                if separation == 0:
+                    name += single_var
+                else:
+                    name += '/' + single_var
+                separation += 1
+        variant.append(name)
+        values.append(fitness_values[i])
+        sequences.append(''.join(temp))
+
+    return variant, values, sequences
+
+
+def split_variants(variants, sep='/'):
+    """
+    Splits variants according to mutation separator.
+    """
+    variants_splitted = []
+    for variant in variants:
+        variants_splitted.append(variant.split(sep))
+    return variants_splitted
+
+
 def read_csv(
         file_name: str,
         fitness_key: str = None
 ) -> tuple[list, list, list]:
     """
     Description
     -----------
@@ -281,18 +357,18 @@
 
     Returns
     -------
     df_dca: pandas.DataFrame
         Dataframe with variant names, fitness values, and features (encoded sequences).
         If save_df_as_csv is True also writes DF to CSV.
     """
-    X = np.stack(sequence_encodings)
+    x = np.stack(sequence_encodings)
     feature_dict = {}            # Collecting features for each MSA position i
-    for i in range(X.shape[1]):  # (encoding at pos. i) in a dict
-        feature_dict[f'X{i + 1:d}'] = X[:, i]
+    for i in range(x.shape[1]):  # (encoding at pos. i) in a dict
+        feature_dict[f'X{i + 1:d}'] = x[:, i]
 
     df_dca = pd.DataFrame()
     df_dca.insert(0, 'variant', variants)
     df_dca.insert(1, 'y', fitnesses)
     df_dca = pd.concat([df_dca, pd.DataFrame(feature_dict)], axis=1)
 
     if save_df_as_csv:
@@ -321,28 +397,34 @@
         df_encoding.iloc[:, 1].to_numpy()
     )
 
 
 def read_csv_and_shift_pos_ints(
         infile: str,
         offset: int = 0,
+        col_sep: str = ';',
         substitution_sep: str = '/',
         target_column: int = 1
 ):
     """
     Shifts position of substitutions of variants for all variants in the provided
     CSV file and saves the position-shifted variants with the corresponding fitness
     values to a new CSV file.
     """
-    df = pd.read_csv(infile, sep=';', comment='#')
+    df = pd.read_csv(infile, sep=col_sep, comment='#')
     if df.shape[1] == 1:
         df = pd.read_csv(infile, sep=',', comment='#')
     if df.shape[1] == 1:
         df = pd.read_csv(infile, sep='\t', comment='#')
-    df = df.dropna(subset=df.columns[[target_column]])  # if specific column has a NaN drop entire row
+    try:
+        df = df.dropna(subset=df.columns[[target_column]])  # if specific column has a NaN drop entire row
+    except IndexError:
+        raise IndexError("Did only detect a single column which might indicate a missing "
+                         "target value column / a wrong specification of the CSV column "
+                         "spearator character (e.g., --sep \';\').")
 
     column_1 = df.iloc[:, 0]
     column_2 = df.iloc[:, target_column].to_numpy()
 
     new_col = []
 
     for variant in column_1:
@@ -352,19 +434,19 @@
             for s_var in splitted_var:
                 new_var_int = int(s_var[1:-1]) - offset
                 new_variant = s_var[0] + str(new_var_int) + s_var[-1]
                 split_vars_list.append(new_variant)
             new_variant = ''
             for i, v in enumerate(split_vars_list):
                 if i != len(split_vars_list) - 1:
-                    new_variant += f'{v}{substitution_sep}'
+                    new_variant += f'{v}/'  # substitution_sep replaced by '/'
                 else:
                     new_variant += v
             new_col.append(new_variant)
         else:
             new_var_int = int(variant[1:-1]) - offset
             new_variant = variant[0] + str(new_var_int) + variant[-1]
             new_col.append(new_variant)
 
     data = np.array([new_col, column_2]).T
     new_df = pd.DataFrame(data, columns=['variant', 'fitness'])
-    new_df.to_csv(infile[:-4] + '_' + df.columns[target_column] + infile[-4:], sep=';', index=False)
+    new_df.to_csv(infile[:-4] + '_new' + infile[-4:], sep=';', index=False)
```

### Comparing `pypef-0.2.4/pypef.egg-info/PKG-INFO` & `pypef-0.3/pypef.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypef
-Version: 0.2.4
+Version: 0.3
 Summary: A command-line interface (CLI) tool for performing data-driven protein engineering by building machine learning (ML)-trained regression models from sequence variant fitness data (in CSV format) based on different techniques for protein sequence encoding. Next to building pure ML models, 'hybrid modeling' is also possible using a blended model optimized for predictive contributions of a statistical and an ML-based prediction.
 Home-page: https://github.com/niklases/PyPEF
 Author: Niklas Siedhoff & Alexander-Maurice Illig
 Author-email: n.siedhoff@biotec.rwth-aachen.de
 License: CC BY-NC-SA 4.0
 Keywords: Pythonic Protein Engineering Framework
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pypef-0.2.4/pypef.egg-info/SOURCES.txt` & `pypef-0.3/pypef.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 pypef.egg-info/PKG-INFO
 pypef.egg-info/SOURCES.txt
 pypef.egg-info/dependency_links.txt
 pypef.egg-info/entry_points.txt
 pypef.egg-info/requires.txt
 pypef.egg-info/top_level.txt
 pypef/dca/__init__.py
-pypef/dca/encoding.py
+pypef/dca/dca_run.py
+pypef/dca/gremlin_inference.py
 pypef/dca/hybrid_model.py
-pypef/dca/run.py
+pypef/dca/plmc_encoding.py
 pypef/ml/__init__.py
+pypef/ml/ml_run.py
 pypef/ml/parallelization.py
 pypef/ml/regression.py
-pypef/ml/run.py
 pypef/ml/AAindex/ANDN920101.txt
 pypef/ml/AAindex/ARGP820101.txt
 pypef/ml/AAindex/ARGP820102.txt
 pypef/ml/AAindex/ARGP820103.txt
 pypef/ml/AAindex/AURR980101.txt
 pypef/ml/AAindex/AURR980102.txt
 pypef/ml/AAindex/AURR980103.txt
@@ -617,11 +618,14 @@
 pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_1_4.txt
 pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_2_2.txt
 pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_3_2.txt
 pypef/utils/__init__.py
 pypef/utils/directed_evolution.py
 pypef/utils/learning_test_sets.py
 pypef/utils/low_n_mutation_extrapolation.py
+pypef/utils/performance.py
+pypef/utils/plot.py
 pypef/utils/prediction_sets.py
-pypef/utils/run.py
 pypef/utils/sto2a2m.py
+pypef/utils/to_file.py
+pypef/utils/utils_run.py
 pypef/utils/variant_data.py
```

### Comparing `pypef-0.2.4/setup.py` & `pypef-0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/env python3
-# for installation run me with: pip install . --use-feature=in-tree-build
+# for installation run me with: pip install .
+#                      or with: pip install -e .
 
 
 from setuptools import setup, find_packages
 
 
 with open("requirements.txt", "r", encoding="utf-8") as install_requirements:
     requirements = install_requirements.read()
 
 setup(
     name='pypef',
-    version='0.2.4',
+    version='0.3',
     author='Niklas Siedhoff & Alexander-Maurice Illig',
     author_email='n.siedhoff@biotec.rwth-aachen.de',
     license='CC BY-NC-SA 4.0',
     description='A command-line interface (CLI) tool for performing data-driven protein engineering '
                 'by building machine learning (ML)-trained regression models from sequence variant '
                 'fitness data (in CSV format) based on different techniques for protein sequence encoding. '
                 'Next to building pure ML models, \'hybrid modeling\' is also possible using a blended '
```

