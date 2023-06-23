# Comparing `tmp/MACS3-3.0.0b1.tar.gz` & `tmp/MACS3-3.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MACS3-3.0.0b1.tar", last modified: Wed Oct  5 17:55:13 2022, max compression
+gzip compressed data, was "MACS3-3.0.0b2.tar", last modified: Fri Jun 23 21:35:58 2023, max compression
```

## Comparing `MACS3-3.0.0b1.tar` & `MACS3-3.0.0b2.tar`

### file list

```diff
@@ -1,362 +1,363 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 17:55:13.513366 MACS3-3.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (121)    82133 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 17:55:13.481366 MACS3-3.0.0b1/MACS3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 17:55:13.481366 MACS3-3.0.0b1/MACS3/Commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/bdgbroadcall_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     3681 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/bdgcmp_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     4324 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/bdgdiff_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     2383 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/bdgopt_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     2696 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/bdgpeakcall_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)    17848 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/callpeak_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)    18065 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/callvar_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1911 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/cmbreps_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     9949 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/diffpeak_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     4578 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/filterdup_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)    27867 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/hmmratac_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     3770 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/pileup_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     4107 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/predictd_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     3888 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/randsample_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Commands/refinepeak_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 17:55:13.481366 MACS3-3.0.0b1/MACS3/IO/
--rw-r--r--   0 runner    (1001) docker     (121)    25650 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/IO/BAM.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     2538 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/IO/BedGraphIO.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    10309 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/IO/OutputWriter.py
--rw-r--r--   0 runner    (1001) docker     (121)    52434 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/IO/Parser.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    54269 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/IO/PeakIO.pyx
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/IO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 17:55:13.485366 MACS3-3.0.0b1/MACS3/Signal/
--rw-r--r--   0 runner    (1001) docker     (121)    45819 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/BedGraph.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    76355 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/CallPeakUnit.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    21795 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/FixWidthTrack.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    11143 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/HMMR_EM.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     4270 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/HMMR_HMM.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     7730 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/HMMR_Signal_Processing.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    21950 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/PairedEndTrack.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    17522 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/PeakDetect.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    16813 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/PeakModel.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    12726 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/PeakVariants.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    23810 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/Pileup.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     7898 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/PileupV2.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    27685 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/PosReadsInfo.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    24866 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/Prob.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    35761 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/RACollection.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    19506 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/ReadAlignment.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    10155 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/Region.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    58556 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/ScoreTrack.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    13210 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/SignalProcessing.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    12281 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/UnitigRACollection.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    13764 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/VariantStat.pyx
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13930 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/cPosValCalculation.c
--rw-r--r--   0 runner    (1001) docker     (121)     1786 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/cPosValCalculation.h
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/cPosValCalculation.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     9826 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/swalign.c
--rw-r--r--   0 runner    (1001) docker     (121)     2358 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Signal/swalign.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 17:55:13.485366 MACS3-3.0.0b1/MACS3/Utilities/
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Utilities/Constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    34929 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Utilities/OptValidator.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 17:55:13.489366 MACS3-3.0.0b1/MACS3/fermi-lite/
--rw-r--r--   0 runner    (1001) docker     (121)    19571 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/bfc.c
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/bseq.c
--rw-r--r--   0 runner    (1001) docker     (121)    12235 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/bubble.c
--rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/example.c
--rw-r--r--   0 runner    (1001) docker     (121)     5083 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/fml.h
--rw-r--r--   0 runner    (1001) docker     (121)     3085 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/htab.c
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/htab.h
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/internal.h
--rw-r--r--   0 runner    (1001) docker     (121)    21102 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/khash.h
--rw-r--r--   0 runner    (1001) docker     (121)     2880 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/kmer.h
--rw-r--r--   0 runner    (1001) docker     (121)     8739 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/kseq.h
--rw-r--r--   0 runner    (1001) docker     (121)    10635 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/ksort.h
--rw-r--r--   0 runner    (1001) docker     (121)     4437 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/kstring.h
--rw-r--r--   0 runner    (1001) docker     (121)    12337 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/ksw.c
--rw-r--r--   0 runner    (1001) docker     (121)     2485 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/ksw.h
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/kthread.c
--rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/kvec.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 17:55:13.489366 MACS3-3.0.0b1/MACS3/fermi-lite/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 17:55:13.489366 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 17:55:13.501366 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/
--rw-r--r--   0 runner    (1001) docker     (121)     6276 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/aba.h
--rw-r--r--   0 runner    (1001) docker     (121)    10687 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/abd.h
--rw-r--r--   0 runner    (1001) docker     (121)     4266 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/abdl.h
--rw-r--r--   0 runner    (1001) docker     (121)    12280 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/abs.h
--rw-r--r--   0 runner    (1001) docker     (121)    18439 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/add.h
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/addl.h
--rw-r--r--   0 runner    (1001) docker     (121)     4141 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/addl_high.h
--rw-r--r--   0 runner    (1001) docker     (121)     8399 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/addlv.h
--rw-r--r--   0 runner    (1001) docker     (121)    10476 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/addv.h
--rw-r--r--   0 runner    (1001) docker     (121)     7501 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/addw.h
--rw-r--r--   0 runner    (1001) docker     (121)     6724 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/addw_high.h
--rw-r--r--   0 runner    (1001) docker     (121)    15830 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/and.h
--rw-r--r--   0 runner    (1001) docker     (121)    13752 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/bic.h
--rw-r--r--   0 runner    (1001) docker     (121)    14767 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/bsl.h
--rw-r--r--   0 runner    (1001) docker     (121)     4665 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cagt.h
--rw-r--r--   0 runner    (1001) docker     (121)    21370 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/ceq.h
--rw-r--r--   0 runner    (1001) docker     (121)     9095 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/ceqz.h
--rw-r--r--   0 runner    (1001) docker     (121)    22658 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cge.h
--rw-r--r--   0 runner    (1001) docker     (121)    11884 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cgez.h
--rw-r--r--   0 runner    (1001) docker     (121)    22278 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cgt.h
--rw-r--r--   0 runner    (1001) docker     (121)    11902 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cgtz.h
--rw-r--r--   0 runner    (1001) docker     (121)    22658 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cle.h
--rw-r--r--   0 runner    (1001) docker     (121)    11884 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/clez.h
--rw-r--r--   0 runner    (1001) docker     (121)     4854 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cls.h
--rw-r--r--   0 runner    (1001) docker     (121)    22158 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/clt.h
--rw-r--r--   0 runner    (1001) docker     (121)     7771 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cltz.h
--rw-r--r--   0 runner    (1001) docker     (121)    12387 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/clz.h
--rw-r--r--   0 runner    (1001) docker     (121)     4376 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cnt.h
--rw-r--r--   0 runner    (1001) docker     (121)    11610 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/combine.h
--rw-r--r--   0 runner    (1001) docker     (121)     5174 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/create.h
--rw-r--r--   0 runner    (1001) docker     (121)    15180 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cvt.h
--rw-r--r--   0 runner    (1001) docker     (121)     6420 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/dot.h
--rw-r--r--   0 runner    (1001) docker     (121)     7781 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/dot_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)    21506 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/dup_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)    15175 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/dup_n.h
--rw-r--r--   0 runner    (1001) docker     (121)    15830 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/eor.h
--rw-r--r--   0 runner    (1001) docker     (121)    39152 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/ext.h
--rw-r--r--   0 runner    (1001) docker     (121)     7901 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/get_high.h
--rw-r--r--   0 runner    (1001) docker     (121)    14459 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/get_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)     8238 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/get_low.h
--rw-r--r--   0 runner    (1001) docker     (121)     9710 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/hadd.h
--rw-r--r--   0 runner    (1001) docker     (121)     9710 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/hsub.h
--rw-r--r--   0 runner    (1001) docker     (121)    11789 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/ld1.h
--rw-r--r--   0 runner    (1001) docker     (121)    16633 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/ld3.h
--rw-r--r--   0 runner    (1001) docker     (121)    15320 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/ld4.h
--rw-r--r--   0 runner    (1001) docker     (121)    19022 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/max.h
--rw-r--r--   0 runner    (1001) docker     (121)     6916 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/maxnm.h
--rw-r--r--   0 runner    (1001) docker     (121)     9895 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/maxv.h
--rw-r--r--   0 runner    (1001) docker     (121)    20487 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/min.h
--rw-r--r--   0 runner    (1001) docker     (121)     6916 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/minnm.h
--rw-r--r--   0 runner    (1001) docker     (121)    10751 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/minv.h
--rw-r--r--   0 runner    (1001) docker     (121)    16338 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mla.h
--rw-r--r--   0 runner    (1001) docker     (121)    10252 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mla_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     5025 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mlal.h
--rw-r--r--   0 runner    (1001) docker     (121)     5259 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mlal_high.h
--rw-r--r--   0 runner    (1001) docker     (121)     4149 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mlal_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     7922 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mls.h
--rw-r--r--   0 runner    (1001) docker     (121)     3888 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mlsl.h
--rw-r--r--   0 runner    (1001) docker     (121)     4092 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mlsl_high.h
--rw-r--r--   0 runner    (1001) docker     (121)     3110 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mlsl_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     6302 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/movl.h
--rw-r--r--   0 runner    (1001) docker     (121)     3784 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/movl_high.h
--rw-r--r--   0 runner    (1001) docker     (121)     5749 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/movn.h
--rw-r--r--   0 runner    (1001) docker     (121)     3905 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/movn_high.h
--rw-r--r--   0 runner    (1001) docker     (121)    16534 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mul.h
--rw-r--r--   0 runner    (1001) docker     (121)    15323 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mul_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)    10970 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mul_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     7854 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mull.h
--rw-r--r--   0 runner    (1001) docker     (121)     4044 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mull_high.h
--rw-r--r--   0 runner    (1001) docker     (121)     5266 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mull_n.h
--rw-r--r--   0 runner    (1001) docker     (121)    11934 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mvn.h
--rw-r--r--   0 runner    (1001) docker     (121)    10654 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/neg.h
--rw-r--r--   0 runner    (1001) docker     (121)    14551 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/orn.h
--rw-r--r--   0 runner    (1001) docker     (121)    15798 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/orr.h
--rw-r--r--   0 runner    (1001) docker     (121)     6129 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/padal.h
--rw-r--r--   0 runner    (1001) docker     (121)     8877 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/padd.h
--rw-r--r--   0 runner    (1001) docker     (121)     7552 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/paddl.h
--rw-r--r--   0 runner    (1001) docker     (121)     7572 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/pmax.h
--rw-r--r--   0 runner    (1001) docker     (121)     7826 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/pmin.h
--rw-r--r--   0 runner    (1001) docker     (121)     7366 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qabs.h
--rw-r--r--   0 runner    (1001) docker     (121)    15857 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qadd.h
--rw-r--r--   0 runner    (1001) docker     (121)     4074 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qdmulh.h
--rw-r--r--   0 runner    (1001) docker     (121)     4152 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qdmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     8266 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qmovn.h
--rw-r--r--   0 runner    (1001) docker     (121)     4029 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qmovn_high.h
--rw-r--r--   0 runner    (1001) docker     (121)     5196 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qmovun.h
--rw-r--r--   0 runner    (1001) docker     (121)     8600 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qneg.h
--rw-r--r--   0 runner    (1001) docker     (121)     5260 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qrdmulh.h
--rw-r--r--   0 runner    (1001) docker     (121)     4088 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qrdmulh_n.h
--rw-r--r--   0 runner    (1001) docker     (121)    19189 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qshl.h
--rw-r--r--   0 runner    (1001) docker     (121)    15571 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qsub.h
--rw-r--r--   0 runner    (1001) docker     (121)    17511 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qtbl.h
--rw-r--r--   0 runner    (1001) docker     (121)    19270 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qtbx.h
--rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rbit.h
--rw-r--r--   0 runner    (1001) docker     (121)    95760 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/reinterpret.h
--rw-r--r--   0 runner    (1001) docker     (121)     4773 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rev16.h
--rw-r--r--   0 runner    (1001) docker     (121)     8072 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rev32.h
--rw-r--r--   0 runner    (1001) docker     (121)    11898 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rev64.h
--rw-r--r--   0 runner    (1001) docker     (121)    16270 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rhadd.h
--rw-r--r--   0 runner    (1001) docker     (121)     4269 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rnd.h
--rw-r--r--   0 runner    (1001) docker     (121)    43945 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rshl.h
--rw-r--r--   0 runner    (1001) docker     (121)    16744 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rshr_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     7379 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rsra_n.h
--rw-r--r--   0 runner    (1001) docker     (121)    13789 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/set_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)    35543 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/shl.h
--rw-r--r--   0 runner    (1001) docker     (121)    18134 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/shl_n.h
--rw-r--r--   0 runner    (1001) docker     (121)    19435 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/shr_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     7090 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/sra_n.h
--rw-r--r--   0 runner    (1001) docker     (121)    10700 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/st1.h
--rw-r--r--   0 runner    (1001) docker     (121)    12450 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/st1_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)    14527 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/st3.h
--rw-r--r--   0 runner    (1001) docker     (121)    16018 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/st4.h
--rw-r--r--   0 runner    (1001) docker     (121)    18645 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/sub.h
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/subl.h
--rw-r--r--   0 runner    (1001) docker     (121)     7418 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/subw.h
--rw-r--r--   0 runner    (1001) docker     (121)     8041 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/subw_high.h
--rw-r--r--   0 runner    (1001) docker     (121)     7749 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/tbl.h
--rw-r--r--   0 runner    (1001) docker     (121)     9121 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/tbx.h
--rw-r--r--   0 runner    (1001) docker     (121)     7435 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/trn.h
--rw-r--r--   0 runner    (1001) docker     (121)    14460 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/trn1.h
--rw-r--r--   0 runner    (1001) docker     (121)    14595 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/trn2.h
--rw-r--r--   0 runner    (1001) docker     (121)    17552 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/tst.h
--rw-r--r--   0 runner    (1001) docker     (121)    26581 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/types.h
--rw-r--r--   0 runner    (1001) docker     (121)     9465 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/uqadd.h
--rw-r--r--   0 runner    (1001) docker     (121)     7435 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/uzp.h
--rw-r--r--   0 runner    (1001) docker     (121)    20856 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/uzp1.h
--rw-r--r--   0 runner    (1001) docker     (121)    21036 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/uzp2.h
--rw-r--r--   0 runner    (1001) docker     (121)     7435 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/zip.h
--rw-r--r--   0 runner    (1001) docker     (121)    19744 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/zip1.h
--rw-r--r--   0 runner    (1001) docker     (121)    20392 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/zip2.h
--rw-r--r--   0 runner    (1001) docker     (121)     4351 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon.h
--rw-r--r--   0 runner    (1001) docker     (121)     9846 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/check.h
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/debug-trap.h
--rw-r--r--   0 runner    (1001) docker     (121)    74181 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/hedley.h
--rw-r--r--   0 runner    (1001) docker     (121)    17805 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-align.h
--rw-r--r--   0 runner    (1001) docker     (121)    16472 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-arch.h
--rw-r--r--   0 runner    (1001) docker     (121)    32588 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-common.h
--rw-r--r--   0 runner    (1001) docker     (121)    18585 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-constify.h
--rw-r--r--   0 runner    (1001) docker     (121)     5065 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-detect-clang.h
--rw-r--r--   0 runner    (1001) docker     (121)    18236 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-diagnostic.h
--rw-r--r--   0 runner    (1001) docker     (121)    17861 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-features.h
--rw-r--r--   0 runner    (1001) docker     (121)    57737 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-math.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 17:55:13.505366 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/
--rw-r--r--   0 runner    (1001) docker     (121)   195250 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx.h
--rw-r--r--   0 runner    (1001) docker     (121)   194448 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx2.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 17:55:13.513366 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/
--rw-r--r--   0 runner    (1001) docker     (121)     8026 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/2intersect.h
--rw-r--r--   0 runner    (1001) docker     (121)    17914 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/abs.h
--rw-r--r--   0 runner    (1001) docker     (121)    21097 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/add.h
--rw-r--r--   0 runner    (1001) docker     (121)    13194 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/adds.h
--rw-r--r--   0 runner    (1001) docker     (121)     9570 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/and.h
--rw-r--r--   0 runner    (1001) docker     (121)     7564 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/andnot.h
--rw-r--r--   0 runner    (1001) docker     (121)     8799 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/avg.h
--rw-r--r--   0 runner    (1001) docker     (121)     9480 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/blend.h
--rw-r--r--   0 runner    (1001) docker     (121)    29208 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/broadcast.h
--rw-r--r--   0 runner    (1001) docker     (121)     9094 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cast.h
--rw-r--r--   0 runner    (1001) docker     (121)    23105 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cmp.h
--rw-r--r--   0 runner    (1001) docker     (121)     5959 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cmpeq.h
--rw-r--r--   0 runner    (1001) docker     (121)     3401 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cmpge.h
--rw-r--r--   0 runner    (1001) docker     (121)     6256 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cmpgt.h
--rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cmple.h
--rw-r--r--   0 runner    (1001) docker     (121)     4012 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cmplt.h
--rw-r--r--   0 runner    (1001) docker     (121)     3008 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/copysign.h
--rw-r--r--   0 runner    (1001) docker     (121)     3959 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cvt.h
--rw-r--r--   0 runner    (1001) docker     (121)    23453 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cvts.h
--rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/div.h
--rw-r--r--   0 runner    (1001) docker     (121)     8810 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/extract.h
--rw-r--r--   0 runner    (1001) docker     (121)     4563 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/fmadd.h
--rw-r--r--   0 runner    (1001) docker     (121)     3601 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/fmsub.h
--rw-r--r--   0 runner    (1001) docker     (121)     3620 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/fnmadd.h
--rw-r--r--   0 runner    (1001) docker     (121)     3620 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/fnmsub.h
--rw-r--r--   0 runner    (1001) docker     (121)     7801 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/insert.h
--rw-r--r--   0 runner    (1001) docker     (121)     5919 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/kshift.h
--rw-r--r--   0 runner    (1001) docker     (121)     2556 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/load.h
--rw-r--r--   0 runner    (1001) docker     (121)     7347 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/loadu.h
--rw-r--r--   0 runner    (1001) docker     (121)     7454 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/lzcnt.h
--rw-r--r--   0 runner    (1001) docker     (121)     5652 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/madd.h
--rw-r--r--   0 runner    (1001) docker     (121)     6089 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/maddubs.h
--rw-r--r--   0 runner    (1001) docker     (121)    18597 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/max.h
--rw-r--r--   0 runner    (1001) docker     (121)    18599 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/min.h
--rw-r--r--   0 runner    (1001) docker     (121)    30273 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/mov.h
--rw-r--r--   0 runner    (1001) docker     (121)    11926 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/mov_mask.h
--rw-r--r--   0 runner    (1001) docker     (121)    15715 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/movm.h
--rw-r--r--   0 runner    (1001) docker     (121)     9151 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/mul.h
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/mulhi.h
--rw-r--r--   0 runner    (1001) docker     (121)     2272 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/mulhrs.h
--rw-r--r--   0 runner    (1001) docker     (121)     3842 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/mullo.h
--rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/negate.h
--rw-r--r--   0 runner    (1001) docker     (121)     7993 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/or.h
--rw-r--r--   0 runner    (1001) docker     (121)     6819 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/packs.h
--rw-r--r--   0 runner    (1001) docker     (121)     6833 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/packus.h
--rw-r--r--   0 runner    (1001) docker     (121)    69829 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/permutex2var.h
--rw-r--r--   0 runner    (1001) docker     (121)    49807 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/permutexvar.h
--rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/sad.h
--rw-r--r--   0 runner    (1001) docker     (121)    15045 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/set.h
--rw-r--r--   0 runner    (1001) docker     (121)     9209 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/set1.h
--rw-r--r--   0 runner    (1001) docker     (121)     3705 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/set4.h
--rw-r--r--   0 runner    (1001) docker     (121)     2104 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/setone.h
--rw-r--r--   0 runner    (1001) docker     (121)     4723 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/setr.h
--rw-r--r--   0 runner    (1001) docker     (121)     3735 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/setr4.h
--rw-r--r--   0 runner    (1001) docker     (121)     2924 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/setzero.h
--rw-r--r--   0 runner    (1001) docker     (121)     7868 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/shuffle.h
--rw-r--r--   0 runner    (1001) docker     (121)     8169 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/sll.h
--rw-r--r--   0 runner    (1001) docker     (121)     6812 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/slli.h
--rw-r--r--   0 runner    (1001) docker     (121)     2360 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/sllv.h
--rw-r--r--   0 runner    (1001) docker     (121)     3977 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/sqrt.h
--rw-r--r--   0 runner    (1001) docker     (121)     2684 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/sra.h
--rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/srai.h
--rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/srav.h
--rw-r--r--   0 runner    (1001) docker     (121)     6928 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/srl.h
--rw-r--r--   0 runner    (1001) docker     (121)     6593 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/srli.h
--rw-r--r--   0 runner    (1001) docker     (121)     9460 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/srlv.h
--rw-r--r--   0 runner    (1001) docker     (121)     3507 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/store.h
--rw-r--r--   0 runner    (1001) docker     (121)     3429 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/storeu.h
--rw-r--r--   0 runner    (1001) docker     (121)    10888 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/sub.h
--rw-r--r--   0 runner    (1001) docker     (121)     7107 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/subs.h
--rw-r--r--   0 runner    (1001) docker     (121)     6297 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/test.h
--rw-r--r--   0 runner    (1001) docker     (121)    17809 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/types.h
--rw-r--r--   0 runner    (1001) docker     (121)    13394 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/unpackhi.h
--rw-r--r--   0 runner    (1001) docker     (121)     3886 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/unpacklo.h
--rw-r--r--   0 runner    (1001) docker     (121)     8662 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/xor.h
--rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/xorsign.h
--rw-r--r--   0 runner    (1001) docker     (121)     3227 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512.h
--rw-r--r--   0 runner    (1001) docker     (121)    15656 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/clmul.h
--rw-r--r--   0 runner    (1001) docker     (121)    21337 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/fma.h
--rw-r--r--   0 runner    (1001) docker     (121)    31945 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/gfni.h
--rw-r--r--   0 runner    (1001) docker     (121)    76602 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/mmx.h
--rw-r--r--   0 runner    (1001) docker     (121)   144373 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/sse.h
--rw-r--r--   0 runner    (1001) docker     (121)   241454 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/sse2.h
--rw-r--r--   0 runner    (1001) docker     (121)    16133 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/sse3.h
--rw-r--r--   0 runner    (1001) docker     (121)    75653 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/sse4.1.h
--rw-r--r--   0 runner    (1001) docker     (121)    12626 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/sse4.2.h
--rw-r--r--   0 runner    (1001) docker     (121)    35506 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/ssse3.h
--rw-r--r--   0 runner    (1001) docker     (121)   398077 2022-10-05 17:53:48.000000 MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/svml.h
--rw-r--r--   0 runner    (1001) docker     (121)    17555 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/mag.c
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/mag.h
--rw-r--r--   0 runner    (1001) docker     (121)     7850 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/misc.c
--rw-r--r--   0 runner    (1001) docker     (121)     8554 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/mrope.c
--rw-r--r--   0 runner    (1001) docker     (121)     2694 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/mrope.h
--rw-r--r--   0 runner    (1001) docker     (121)    13226 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/rld0.c
--rw-r--r--   0 runner    (1001) docker     (121)     4296 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/rld0.h
--rw-r--r--   0 runner    (1001) docker     (121)     4821 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/rle.c
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/rle.h
--rw-r--r--   0 runner    (1001) docker     (121)     6965 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/rope.c
--rw-r--r--   0 runner    (1001) docker     (121)     1428 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/rope.h
--rw-r--r--   0 runner    (1001) docker     (121)    15372 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MACS3/fermi-lite/unitig.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 17:55:13.481366 MACS3-3.0.0b1/MACS3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7973 2022-10-05 17:55:13.000000 MACS3-3.0.0b1/MACS3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11577 2022-10-05 17:55:13.000000 MACS3-3.0.0b1/MACS3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 17:55:13.000000 MACS3-3.0.0b1/MACS3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-05 17:55:13.000000 MACS3-3.0.0b1/MACS3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-05 17:55:13.000000 MACS3-3.0.0b1/MACS3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7973 2022-10-05 17:55:13.513366 MACS3-3.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7081 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 17:55:13.513366 MACS3-3.0.0b1/bin/
--rw-r--r--   0 runner    (1001) docker     (121)    87479 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/bin/macs3
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 17:55:13.513366 MACS3-3.0.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6096 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/bdgbroadcall.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/bdgcmp.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/bdgdiff.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/bdgopt.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/bdgpeakcall.md
--rw-r--r--   0 runner    (1001) docker     (121)    16724 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/callpeak.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/filterdup.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/hmmratac.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/main.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/pileup.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/predictd.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/qa.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/randsample.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/refinepeak.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/testing_in_docker.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (121)     1942 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/make_docker_base.sh
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-05 17:55:13.513366 MACS3-3.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     9105 2022-10-05 17:53:44.000000 MACS3-3.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.180009 MACS3-3.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    82248 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.128005 MACS3-3.0.0b2/MACS3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.128005 MACS3-3.0.0b2/MACS3/Commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/bdgbroadcall_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/bdgcmp_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/bdgdiff_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/bdgopt_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/bdgpeakcall_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17848 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/callpeak_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18078 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/callvar_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/cmbreps_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/diffpeak_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/filterdup_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28259 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/hmmratac_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/pileup_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/predictd_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/randsample_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Commands/refinepeak_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.132005 MACS3-3.0.0b2/MACS3/IO/
+-rw-r--r--   0 runner    (1001) docker     (123)    25603 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/IO/BAM.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/IO/BedGraphIO.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/IO/OutputWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52515 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/IO/Parser.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    54269 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/IO/PeakIO.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/IO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.136006 MACS3-3.0.0b2/MACS3/Signal/
+-rw-r--r--   0 runner    (1001) docker     (123)    48049 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/BedGraph.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    76301 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/CallPeakUnit.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    21780 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/FixWidthTrack.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/HMMR_EM.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/HMMR_HMM.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/HMMR_Signal_Processing.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    22046 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/PairedEndTrack.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/PeakDetect.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    16813 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/PeakModel.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/PeakVariants.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    23810 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/Pileup.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/PileupV2.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/PosReadsInfo.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    24866 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/Prob.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    35761 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/RACollection.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    19506 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/ReadAlignment.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/Region.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    58541 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/ScoreTrack.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/SignalProcessing.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/UnitigRACollection.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    13764 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/VariantStat.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13930 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/cPosValCalculation.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/cPosValCalculation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/cPosValCalculation.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/swalign.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Signal/swalign.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.136006 MACS3-3.0.0b2/MACS3/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Utilities/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Utilities/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31761 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Utilities/OptValidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.140006 MACS3-3.0.0b2/MACS3/fermi-lite/
+-rw-r--r--   0 runner    (1001) docker     (123)    19571 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/bfc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/bseq.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/bubble.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/example.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/fml.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/htab.c
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/htab.h
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21102 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/khash.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/kmer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/kseq.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/ksort.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/kstring.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/ksw.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/ksw.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/kthread.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/kvec.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.140006 MACS3-3.0.0b2/MACS3/fermi-lite/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.144006 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.164008 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/aba.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/abd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/abdl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/abs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/add.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addl_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addlv.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addw.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addw_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/bic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/bsl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cagt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21370 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ceq.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ceqz.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cge.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cgez.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22278 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cgt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11902 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cgtz.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cle.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/clez.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cls.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22158 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/clt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cltz.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/clz.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cnt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/combine.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/create.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cvt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dot_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21506 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dup_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dup_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/eor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    39152 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ext.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/get_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14459 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/get_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/get_low.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/hadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/hsub.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ld1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ld3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15320 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ld4.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19022 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/max.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/maxnm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/maxv.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/min.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/minnm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/minv.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16338 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mla.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mla_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlal_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlal_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mls.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlsl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlsl_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlsl_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movl_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movn.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movn_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mul.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mul_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mul_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mull_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mull_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mvn.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10654 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/neg.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/orn.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15798 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/orr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/padal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/padd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/paddl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/pmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/pmin.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qabs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qdmulh.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qdmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qmovn.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qmovn_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qmovun.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qneg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qrdmulh.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qrdmulh_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qshl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qsub.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17511 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qtbl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qtbx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rbit.h
+-rw-r--r--   0 runner    (1001) docker     (123)    95760 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/reinterpret.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rev16.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rev32.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rev64.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16270 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rhadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rnd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    43945 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rshl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rshr_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rsra_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/set_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35543 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/shl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/shl_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19435 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/shr_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/sra_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st1_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st4.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/sub.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/subl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/subw.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/subw_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/tbl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/tbx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/trn.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14460 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/trn1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/trn2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/tst.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26581 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uqadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uzp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20856 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uzp1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21036 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uzp2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/zip.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/zip1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/zip2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/check.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/debug-trap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    74181 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/hedley.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-align.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-arch.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18585 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-constify.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-detect-clang.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-diagnostic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-features.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57737 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-math.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.168008 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/
+-rw-r--r--   0 runner    (1001) docker     (123)   195250 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx.h
+-rw-r--r--   0 runner    (1001) docker     (123)   194448 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx2.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.180009 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/2intersect.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17914 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/abs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21097 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/add.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/adds.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/andnot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/avg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/blend.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29208 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/broadcast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23105 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmpeq.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmpge.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmpgt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmple.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmplt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/copysign.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cvt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23453 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cvts.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/div.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/extract.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fmadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fmsub.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fnmadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fnmsub.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/insert.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/kshift.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/load.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/loadu.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/lzcnt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/madd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/maddubs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18597 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/max.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/min.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30273 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mov.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mov_mask.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15715 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/movm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mul.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mulhi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mulhrs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mullo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/negate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/or.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/packs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/packus.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69829 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/permutex2var.h
+-rw-r--r--   0 runner    (1001) docker     (123)    49807 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/permutexvar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sad.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/set.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/set1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/set4.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setone.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setr4.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setzero.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/shuffle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sll.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/slli.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sllv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sqrt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sra.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srai.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srav.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srli.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srlv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/store.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/storeu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sub.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/subs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/test.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/unpackhi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/unpacklo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/xor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/xorsign.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15656 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/clmul.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/fma.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31945 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/gfni.h
+-rw-r--r--   0 runner    (1001) docker     (123)    76602 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/mmx.h
+-rw-r--r--   0 runner    (1001) docker     (123)   144373 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse.h
+-rw-r--r--   0 runner    (1001) docker     (123)   241454 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    75653 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse4.1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse4.2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35506 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/ssse3.h
+-rw-r--r--   0 runner    (1001) docker     (123)   398077 2023-06-23 21:34:02.000000 MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/svml.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/mag.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/mag.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/misc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/mrope.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/mrope.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/rld0.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/rld0.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/rle.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/rle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/rope.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/rope.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15372 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MACS3/fermi-lite/unitig.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.128005 MACS3-3.0.0b2/MACS3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-23 21:35:58.000000 MACS3-3.0.0b2/MACS3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-06-23 21:35:58.000000 MACS3-3.0.0b2/MACS3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:35:58.000000 MACS3-3.0.0b2/MACS3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 21:35:58.000000 MACS3-3.0.0b2/MACS3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 21:35:58.000000 MACS3-3.0.0b2/MACS3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-23 21:35:58.180009 MACS3-3.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.180009 MACS3-3.0.0b2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    98279 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/bin/macs3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:58.180009 MACS3-3.0.0b2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/bdgbroadcall.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/bdgcmp.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/bdgdiff.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/bdgopt.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/bdgpeakcall.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/callpeak.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/filterdup.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/hmmratac.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/main.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/pileup.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/predictd.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/qa.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/randsample.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/refinepeak.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/testing_in_docker.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/make_docker_base.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 21:35:58.180009 MACS3-3.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-06-23 21:33:58.000000 MACS3-3.0.0b2/setup.py
```

### Comparing `MACS3-3.0.0b1/ChangeLog` & `MACS3-3.0.0b2/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-2022-06-07  Tao Liu  <vladimir.liu@gmail.com>
-	MACS 3.0.0b1
+2023-06-23  Tao Liu  <vladimir.liu@gmail.com>
+	MACS 3.0.0b2
 	* New features in MACS3:
 
-	1) Speed/memory optimization.  Use the cykhash to replace python 
-	dictionary. Use buffer (10MB) to read and parse input file (not 
-	available for BAM file parser). And many optimization tweaks. 
+	1) Speed/memory optimization.  Use the cykhash to replace python
+	dictionary. Use buffer (10MB) to read and parse input file (not
+	available for BAM file parser). And many optimization tweaks. We
+	added memory monitoring to the runtime messages.
 
 	2) Code cleanup. Reorganize source codes. 
 
 	3) Unit testing. 
 
 	4) R wrappers for MACS -- MACSr
 
@@ -43,16 +44,18 @@
 	in JAVA, by Evan Tarbell. We implemented it in Python/Cython and
 	optimize the whole process using existing MACS functions and
 	hmmlearn. Now it can run much faster than the original JAVA
 	version. Note: evaluation of the peak calling results is underway.
 
 	11) The effective genome size parameters have been updated
 	according to deeptools. #508
+
+	12) Memory usage now will be displayed in the runtime message.
 	
-	12) Multiple updates regarding dependencies, anaconda built, CI/CD
+	13) Multiple updates regarding dependencies, anaconda built, CI/CD
 	process.
 	
 	* Other:
 	1) Missing header line while no peaks can be called #501 #502
 
 2020-04-11  Tao Liu  <vladimir.liu@gmail.com>
 	MACS version 2.2.7.1
```

### Comparing `MACS3-3.0.0b1/LICENSE` & `MACS3-3.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Commands/bdgbroadcall_cmd.py` & `MACS3-3.0.0b2/MACS3/Commands/bdgbroadcall_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,33 +11,30 @@
 
 # ------------------------------------
 # python modules
 # ------------------------------------
 
 import sys
 import os
-import logging
 from MACS3.IO import BedGraphIO
 # ------------------------------------
 # constants
 # ------------------------------------
-logging.basicConfig(level=20,
-                    format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                    datefmt='%a, %d %b %Y %H:%M:%S',
-                    stream=sys.stderr,
-                    filemode="w"
-                    )
 
 # ------------------------------------
 # Misc functions
 # ------------------------------------
-error   = logging.critical		# function alias
-warn    = logging.warning
-debug   = logging.debug
-info    = logging.info
+import logging
+import MACS3.Utilities.Logger
+
+logger = logging.getLogger(__name__)
+debug   = logger.debug
+info    = logger.info
+error   = logger.critical
+warn    = logger.warning
 # ------------------------------------
 # Classes
 # ------------------------------------
 
 # ------------------------------------
 # Main function
 # ------------------------------------
```

### Comparing `MACS3-3.0.0b1/MACS3/Commands/bdgcmp_cmd.py` & `MACS3-3.0.0b2/MACS3/Commands/bdgcmp_cmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,44 +5,39 @@
 This code is free software; you can redistribute it and/or modify it
 under the terms of the BSD License (see the file LICENSE included with
 the distribution).
 """
 
 import sys
 import os
-import logging
 
 from MACS3.IO import BedGraphIO
 from MACS3.Utilities.OptValidator import opt_validate_bdgcmp
 
 from math import log as mlog
 
 # ------------------------------------
 # constants
 # ------------------------------------
-logging.basicConfig(level=20,
-                    format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                    datefmt='%a, %d %b %Y %H:%M:%S',
-                    stream=sys.stderr,
-                    filemode="w"
-                    )
 
 # ------------------------------------
 # Misc functions
 # ------------------------------------
-error   = logging.critical		# function alias
-warn    = logging.warning
-debug   = logging.debug
-info    = logging.info
+
 # ------------------------------------
 # Main function
 # ------------------------------------
 
 def run( options ):
     options = opt_validate_bdgcmp( options )
+    info = options.info
+    warn = options.warn
+    debug = options.debug
+    error = options.error
+    
     scaling_factor = options.sfactor
     pseudo_depth = 1.0/scaling_factor   # not an actual depth, but its reciprocal, a trick to override SPMR while necessary.
 
     info("Read and build treatment bedGraph...")
     tbio = BedGraphIO.bedGraphIO(options.tfile)
     tbtrack = tbio.build_bdgtrack()
```

### Comparing `MACS3-3.0.0b1/MACS3/Commands/bdgdiff_cmd.py` & `MACS3-3.0.0b2/MACS3/Commands/bdgdiff_cmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,36 +9,32 @@
 
 # ------------------------------------
 # python modules
 # ------------------------------------
 
 import sys
 import os
-import logging
-
 from MACS3.IO import BedGraphIO
 from MACS3.Signal import ScoreTrack
 
 # ------------------------------------
 # constants
 # ------------------------------------
-logging.basicConfig(level=20,
-                    format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                    datefmt='%a, %d %b %Y %H:%M:%S',
-                    stream=sys.stderr,
-                    filemode="w"
-                    )
 
 # ------------------------------------
 # Misc functions
 # ------------------------------------
-error   = logging.critical		# function alias
-warn    = logging.warning
-debug   = logging.debug
-info    = logging.info
+import logging
+import MACS3.Utilities.Logger
+
+logger = logging.getLogger(__name__)
+debug   = logger.debug
+info    = logger.info
+error   = logger.critical
+warn    = logger.warning
 # ------------------------------------
 # Classes
 # ------------------------------------
 
 # ------------------------------------
 # Main function
 # ------------------------------------
```

### Comparing `MACS3-3.0.0b1/MACS3/Commands/bdgopt_cmd.py` & `MACS3-3.0.0b2/MACS3/Commands/bdgopt_cmd.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,45 +8,40 @@
 """
 
 # ------------------------------------
 # python modules
 # ------------------------------------
 import sys
 import os
-import logging
 
 from MACS3.IO import BedGraphIO
 from MACS3.Utilities.OptValidator import opt_validate_bdgopt
 
 # ------------------------------------
 # constants
 # ------------------------------------
-logging.basicConfig(level=20,
-                    format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                    datefmt='%a, %d %b %Y %H:%M:%S',
-                    stream=sys.stderr,
-                    filemode="w"
-                    )
 
 # ------------------------------------
 # Misc functions
 # ------------------------------------
-error   = logging.critical		# function alias
-warn    = logging.warning
-debug   = logging.debug
-info    = logging.info
+
 # ------------------------------------
 # Classes
 # ------------------------------------
 
 # ------------------------------------
 # Main function
 # ------------------------------------
 def run( options ):
     options = opt_validate_bdgopt( options )
+    info = options.info
+    warn = options.warn
+    debug = options.debug
+    error = options.error
+    
     info("Read and build bedGraph...")
     bio = BedGraphIO.bedGraphIO(options.ifile)
     btrack = bio.build_bdgtrack(baseline_value=0)
 
     info("Modify bedGraph...")
     if options.method.lower() == "p2q":
         btrack.p2q()
```

### Comparing `MACS3-3.0.0b1/MACS3/Commands/bdgpeakcall_cmd.py` & `MACS3-3.0.0b2/MACS3/Commands/bdgpeakcall_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,33 +9,30 @@
 """
 
 # ------------------------------------
 # python modules
 # ------------------------------------
 import sys
 import os
-import logging
 from MACS3.IO import BedGraphIO
 # ------------------------------------
 # constants
 # ------------------------------------
-logging.basicConfig(level=20,
-                    format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                    datefmt='%a, %d %b %Y %H:%M:%S',
-                    stream=sys.stderr,
-                    filemode="w"
-                    )
 
 # ------------------------------------
 # Misc functions
 # ------------------------------------
-error   = logging.critical		# function alias
-warn    = logging.warning
-debug   = logging.debug
-info    = logging.info
+import logging
+import MACS3.Utilities.Logger
+
+logger = logging.getLogger(__name__)
+debug   = logger.debug
+info    = logger.info
+error   = logger.critical
+warn    = logger.warning
 # ------------------------------------
 # Classes
 # ------------------------------------
 
 # ------------------------------------
 # Main function
 # ------------------------------------
```

### Comparing `MACS3-3.0.0b1/MACS3/Commands/callpeak_cmd.py` & `MACS3-3.0.0b2/MACS3/Commands/callpeak_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # Time-stamp: <2020-11-28 17:06:30 Tao Liu>
 
-"""Description: MACS 2 main executable
+"""Description: MACS 3 call peak main executable
 
 This code is free software; you can redistribute it and/or modify it
 under the terms of the BSD License (see the file LICENSE included with
 the distribution).
 """
 
 # ------------------------------------
 # python modules
 # ------------------------------------
 
 import os
 import sys
-import logging
 from time import strftime
 import tempfile
 
 # ------------------------------------
 # MACS3 python modules
 # ------------------------------------
 from MACS3.Utilities.Constants import *
@@ -48,14 +47,15 @@
     # Parse options...
     options = opt_validate_callpeak( args )
     # end of parsing commandline options
     info = options.info
     warn = options.warn
     debug = options.debug
     error = options.error
+    
     #0 output arguments
     info("\n"+options.argtxt)
     options.PE_MODE = options.format in ('BAMPE','BEDPE')
     if options.PE_MODE:
         tag = 'fragment' # call things fragments not tags
     else:
         tag = 'tag'
```

### Comparing `MACS3-3.0.0b1/MACS3/Commands/callvar_cmd.py` & `MACS3-3.0.0b2/MACS3/Commands/callvar_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # Time-stamp: <2022-09-15 17:25:49 Tao Liu>
 
-"""Description: macs call
+"""Description: Call variants directly
 
-Copyright (c) 2017 Tao Liu <tliu4@buffalo.edu>
+Copyright (c) 2017-2023 Tao Liu <vladimir.liu@gmail.com>
 
 This code is free software; you can redistribute it and/or modify it
 under the terms of the BSD License (see the file COPYING included
 with the distribution).
 
 @status: release candidate
 @version: $Id$
 @author:  Tao Liu
-@contact: tliu4@buffalo.edu
+@contact: vladimir.liu@gmail.com
 """
 
 # ------------------------------------
 # python modules
 # ------------------------------------
 
-import logging
 import datetime
 import sys
 from functools import partial
 import multiprocessing as mp
 
 from time import time
 from math import ceil
```

### Comparing `MACS3-3.0.0b1/MACS3/Commands/diffpeak_cmd.py` & `MACS3-3.0.0b2/MACS3/Commands/diffpeak_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 # ------------------------------------
 # python modules
 # ------------------------------------
 
 import os
 import sys
-import logging
 from time import strftime
 
 # ------------------------------------
 # own python modules
 # ------------------------------------
 # from MACS3.IO import cBedGraphIO
 # from MACS3.IO.cDiffScore import DiffScoreTrackI
@@ -26,28 +25,24 @@
 # from MACS3.Prob import binomial_cdf_inv
 # from MACS3.PeakModel import PeakModel,NotEnoughPairsException
 # from MACS3.PeakDetect import PeakDetect
 # from MACS3.Constants import *
 # ------------------------------------
 # constants
 # ------------------------------------
-logging.basicConfig(level=20,
-                    format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                    datefmt='%a, %d %b %Y %H:%M:%S',
-                    stream=sys.stderr,
-                    filemode="w"
-                    )
 
 # ------------------------------------
 # Misc functions
 # ------------------------------------
-error   = logging.critical		# function alias
-warn    = logging.warning
-debug   = logging.debug
-info    = logging.info
+import logging
+import MACS3.Utilities.Logger
+
+logger = logging.getLogger(__name__)
+debug   = logger.debug
+info    = logger.info
 # ------------------------------------
 # Main function
 # ------------------------------------
 def run( args ):
     """The Differential function/pipeline for MACS.
 
     """
```

### Comparing `MACS3-3.0.0b1/MACS3/Commands/filterdup_cmd.py` & `MACS3-3.0.0b2/MACS3/Commands/filterdup_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 # ------------------------------------
 # python modules
 # ------------------------------------
 
 import os
 import sys
-import logging
 
 # ------------------------------------
 # own python modules
 # ------------------------------------
 from MACS3.Utilities.Constants import *
 from MACS3.Utilities.OptValidator import opt_validate_filterdup
 from MACS3.Signal.Prob import binomial_cdf_inv
```

### Comparing `MACS3-3.0.0b1/MACS3/Commands/hmmratac_cmd.py` & `MACS3-3.0.0b2/MACS3/Commands/hmmratac_cmd.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-# Time-stamp: <2022-10-04 16:58:30 Tao Liu>
+# Time-stamp: <2023-06-08 11:03:46 Tao Liu>
 
 """Description: Main HMMR command
 
 This code is free software; you can redistribute it and/or modify it
-under the terms of the BSD License (see thefile LICENSE included with
+under the terms of the BSD License (see the file LICENSE included with
 the distribution).
 """
 
 # ------------------------------------
 # python modules
 # ------------------------------------
 
-from logging.handlers import RotatingFileHandler
 import os
 import sys
-import logging
+import gc
 import numpy as np
 import json
 from hmmlearn import hmm
 #from typing import Sized
 
 # ------------------------------------
 # own python modules
@@ -65,19 +64,22 @@
     training_datalengthfile = os.path.join( options.outdir, options.name+"_training_lengths.txt" )
     hmm_modelfile = os.path.join( options.outdir, options.name+"_model.json" )
     open_state_bdgfile = os.path.join( options.outdir, options.name+"_open.bdg" )
     nuc_state_bdgfile = os.path.join( options.outdir, options.name+"_nuc.bdg" )
     bg_state_bdgfile = os.path.join( options.outdir, options.name+"_bg.bdg" )
     states_file = os.path.join( options.outdir, options.name+"_states.bed" )
     accessible_file = os.path.join( options.outdir, options.name+"_accessible_regions.gappedPeak" )
+    cutoffanalysis_file = os.path.join( options.outdir, options.name+"_cutoff_analysis.tsv" )
     
     #############################################
     # 1. Read the input BAM files
     #############################################
-    options.info("\n" + options.argtxt)    
+    options.info("\n" + options.argtxt)
+    #options.info("Some important parameters for this run")
+    #options.info(f" binsize for HMM: {options.binsize} ()")
     options.info("#1 Read fragments from BAM file...")
 
     bam = BAMPEParser(options.bam_file[0], buffer_size=options.buffer_size)
     petrack = bam.build_petrack()
     if len( options.bam_file ) > 1:
         # multiple input
         for bamfile in options.bam_file[1:]:
@@ -129,48 +131,73 @@
             em_stddevs[ i ] = round(em_stddevs[ i ], 1)
         options.info( f"#  The means and stddevs after EM:")
 
     options.info(  "#                    {0[0]:>10s} {0[1]:>10s} {0[2]:>10s} {0[3]:>10s}".format( ["short", "mono", "di", "tri"] ) )
     options.info(  "#             means: {0[0]:>10.4g} {0[1]:>10.4g} {0[2]:>10.4g} {0[3]:>10.4g}".format( em_means ) )
     options.info(  "#           stddevs: {0[0]:>10.4g} {0[1]:>10.4g} {0[2]:>10.4g} {0[3]:>10.4g}".format( em_stddevs ) )    
 
-    options.info( f"#  Pile up all fragments" )
-    minlen = int(petrack.average_template_length)
-    fc_bdg = petrack.pileup_bdg( [1.0,], baseline_value = 0 )
-    (sum_v, n_v, max_v, min_v, mean_v, std_v) = fc_bdg.summary()
-    options.info( f"#  Convert pileup to fold-change over average signal" )
-    fc_bdg.apply_func(lambda x: x/mean_v)
-
     # to finalize the EM training, we will decompose ATAC-seq into four signal tracks
     options.info( f"#  Compute the weights for each fragment length for each of the four signal types")
     fl_dict = petrack.count_fraglengths()
     fl_list = list(fl_dict.keys())
     fl_list.sort()
 
     # now we will prepare the weights for each fragment length for
     # each of the four distributions based on the EM results
     weight_mapping = generate_weight_mapping( fl_list, em_means, em_stddevs )
     
     options.info( f"#  Generate short, mono-, di-, and tri-nucleosomal signals")
     digested_atac_signals = generate_digested_signals( petrack, weight_mapping )
 
+    # save three types of signals if needed
     if options.save_digested:
         fhd = open(short_bdgfile,"w")
         digested_atac_signals[ 0 ].write_bedGraph(fhd, "short","short")
         fhd.close()
         fhd = open(mono_bdgfile,"w")
         digested_atac_signals[ 0 ].write_bedGraph(fhd, "mono","mono")
         fhd.close()
         fhd = open(di_bdgfile,"w")
         digested_atac_signals[ 0 ].write_bedGraph(fhd, "di","di")
         fhd.close()
         fhd = open(tri_bdgfile,"w")
         digested_atac_signals[ 0 ].write_bedGraph(fhd, "tri","tri")
         fhd.close()        
 
+    minlen = int(petrack.average_template_length)
+    # if options.pileup_short is on, we pile up only the short fragments to identify training 
+    #  regions and to prescan for candidate regions for decoding.
+    if options.pileup_short:
+        options.info( f"#  Pile up ONLY short fragments" )
+        fc_bdg = digested_atac_signals[ 0 ]
+        (sum_v, n_v, max_v, min_v, mean_v, std_v) = fc_bdg.summary()
+        print(sum_v, n_v, max_v, min_v, mean_v, std_v)
+        options.info( f"#  Convert pileup to fold-change over average signal" )
+        fc_bdg.apply_func(lambda x: x/mean_v)
+    else:
+        options.info( f"#  Pile up all fragments" )
+        fc_bdg = petrack.pileup_bdg( [1.0,], baseline_value = 0 )
+        (sum_v, n_v, max_v, min_v, mean_v, std_v) = fc_bdg.summary()
+        options.info( f"#  Convert pileup to fold-change over average signal" )
+        fc_bdg.apply_func(lambda x: x/mean_v)
+       
+        
+    # if cutoff_analysis only, generate and save the report and quit
+    if options.cutoff_analysis_only:
+        # we will run cutoff analysis only and quit
+        options.info( f"#3 Generate cutoff analysis report from {petrack.total} fragments")
+        options.info( f"#   Please review the cutoff analysis result in {cutoffanalysis_file}" )
+
+        # Let MACS3 do the cutoff analysis to help decide the lower and upper cutoffs
+        with open(cutoffanalysis_file, "w") as ofhd_cutoff:
+            ofhd_cutoff.write( fc_bdg.cutoff_analysis( min_length=minlen, max_gap=options.hmm_training_flanking ) )
+        #raise Exception("Cutoff analysis only.")
+        sys.exit(1)
+        
+        
     #############################################
     # 3. Define training set by peak calling
     #############################################
 
     if options.hmm_file:
         # skip this step if hmm_file is given
         options.info( f"#3 Skip this step of looking for training set since a Hidden Markov Model file has been provided!")
@@ -179,22 +206,37 @@
         # Find regions with zscore values above certain cutoff to exclude from viterbi.
         # 
         options.info( f"#3 Look for training set from {petrack.total} fragments" )
         options.info( f"#  Call peak above within fold-change range of {options.hmm_lower} and {options.hmm_upper}." )
         options.info( f"#   The minimum length of the region is set as the average template/fragment length in the dataset: {minlen}" )
         options.info( f"#   The maximum gap to merge nearby significant regions is set as the flanking size to extend training regions: {options.hmm_training_flanking}" )    
         peaks = fc_bdg.call_peaks (cutoff=options.hmm_lower, min_length=minlen, max_gap=options.hmm_training_flanking, call_summits=False)
-        options.info( f"#  Total training regions called: {peaks.total}" )
+        options.info( f"#  Total training regions called after applying the lower cutoff {options.hmm_lower}: {peaks.total}" )
         peaks.filter_score( options.hmm_lower, options.hmm_upper )
-        options.info( f"#  Total training regions after filtering with lower and upper cutoff: {peaks.total}" )
+        options.info( f"#  Total training regions after filtering with upper cutoff {options.hmm_upper}: {peaks.total}" )
+
+        options.info( f"#  **IMPORTANT**")
+        options.info( f"#  Please review the cutoff analysis result in {cutoffanalysis_file} to verify" )
+        options.info( f"#   if the choices of lower, upper and prescanning cutoff are appropriate." )
+        options.info( f"#   Please read the message in the section 'Choices of cutoff values' by running" )
+        options.info( f"#   `macs3 hmmratac -h` for detail." )
+        options.info( f"#  ****" )
         
+        # Let MACS3 do the cutoff analysis to help decide the lower and upper cutoffs
+        with open(cutoffanalysis_file, "w") as ofhd_cutoff:
+            ofhd_cutoff.write( fc_bdg.cutoff_analysis( min_length=minlen, max_gap=options.hmm_training_flanking ) )
+            
+        # we will check if anything left after filtering
         if peaks.total > options.hmm_maxTrain:
             peaks = peaks.randomly_pick( options.hmm_maxTrain, seed = options.hmm_randomSeed )
             options.info( f"#  We randomly pick {options.hmm_maxTrain} regions for training" )
-
+        elif peaks.total == 0:
+            options.error( f"# No training regions found. Please adjust the lower or upper cutoff." )
+            raise Exception("Not enough training regions!")
+        
         # Now we convert PeakIO to Regions and filter blacklisted regions
         training_regions = Regions()
         training_regions.init_from_PeakIO( peaks )
         # We will expand the regions to both directions and merge overlap
         options.info( f"#  We expand the training regions with {options.hmm_training_flanking} basepairs and merge overlap" )
         training_regions.expand( options.hmm_training_flanking )
         training_regions.merge_overlap()
@@ -315,19 +357,24 @@
     options.info( f"#  Use HMM to predict states")
     n = 0
     predicted_proba = []
     candidate_bins = []
     while candidate_regions.total != 0:
         n += 1
         cr = candidate_regions.pop( options.decoding_steps )
+        options.info( "#    decoding %d..." % ( n*options.decoding_steps ) )        
         [ cr_bins, cr_data, cr_data_lengths ] = extract_signals_from_regions( digested_atac_signals, cr, binsize = options.hmm_binsize )
-        options.info( "#    decoding %d..." % ( n*options.decoding_steps ) )
+        #options.info( "#     extracted signals in the candidate regions")
         candidate_bins.extend( cr_bins )
+        #options.info( "#     saving information regarding the candidate regions")        
         predicted_proba.extend( hmm_predict( cr_data, cr_data_lengths, hmm_model ) )
+        #options.info( "#     prediction done")
+        gc.collect()
 
+        
 #############################################
 # 6. Output - add to OutputWriter
 #############################################
     options.info( f"# Write the output...")
     # Now taken the candidate_bins and predicted_proba, we can generate various
     # outputs
     
@@ -405,87 +452,73 @@
 def save_states_bed( states_path, states_bedfile ):
     # we do not need to output background state. 
     for l in range( len( states_path ) ):
         if states_path[l][3] != "bg":
             states_bedfile.write( "%s\t%s\t%s\t%s\n" % states_path[l] )
     return
 
-def generate_states_path( candidate_bins, predicted_proba, binsize, i_open_region, i_nucleosomal_region, i_background_region ):
+def generate_states_path(candidate_bins, predicted_proba, binsize, i_open_region, i_nucleosomal_region, i_background_region):
     ret_states_path = []
-    labels_list = ["open","nuc","bg"]
-    start_pos = candidate_bins[0][1]-binsize
+    labels_list = ["open", "nuc", "bg"]
+    start_pos = candidate_bins[0][1] - binsize
     for l in range(1, len(predicted_proba)):
-        proba_prev = np.array([ predicted_proba[l-1][ i_open_region ], predicted_proba[l-1][ i_nucleosomal_region ], predicted_proba[l-1][ i_background_region ] ])
-        label_prev = labels_list[ np.argmax(proba_prev) ]
-        proba_curr = np.array([ predicted_proba[l][ i_open_region ], predicted_proba[l][ i_nucleosomal_region ], predicted_proba[l][ i_background_region ] ])
-        label_curr = labels_list[ np.argmax(proba_curr) ]
-        if candidate_bins[l-1][0] == candidate_bins[l][0]: #if we are looking at the same chromosome ...
+        chromosome = candidate_bins[l][0].decode()
+        prev_open, prev_nuc, prev_bg = predicted_proba[l-1][i_open_region], predicted_proba[l-1][i_nucleosomal_region], predicted_proba[l-1][i_background_region]
+        curr_open, curr_nuc, curr_bg = predicted_proba[l][i_open_region], predicted_proba[l][i_nucleosomal_region], predicted_proba[l][i_background_region]
+        
+        label_prev = labels_list[max((prev_open, 0), (prev_nuc, 1), (prev_bg, 2), key=lambda x: x[0])[1]]
+        label_curr = labels_list[max((curr_open, 0), (curr_nuc, 1), (curr_bg, 2), key=lambda x: x[0])[1]]
+
+        if candidate_bins[l-1][0] == candidate_bins[l][0]:  # if we are looking at the same chromosome ...
             if label_prev != label_curr:
                 end_pos = candidate_bins[l-1][1]
-                ret_states_path.append( (candidate_bins[l][0].decode(), start_pos, end_pos, label_prev) )
-                start_pos = candidate_bins[l][1]-binsize
-            
-            elif l == len(predicted_proba)-1:
+                ret_states_path.append((chromosome, start_pos, end_pos, label_prev))
+                start_pos = candidate_bins[l][1] - binsize
+            elif l == len(predicted_proba) - 1:
                 end_pos = candidate_bins[l][1]
-                ret_states_path.append( (candidate_bins[l][0].decode(), start_pos, end_pos, label_prev) )
+                ret_states_path.append((chromosome, start_pos, end_pos, label_prev))
         else:
-            start_pos = candidate_bins[l][1]-binsize
-
+            start_pos = candidate_bins[l][1] - binsize
     return ret_states_path
 
-def save_accessible_regions( states_path, accessible_region_file, openregion_minlen ):
-    # select only accessible regions from _states.bed, look for nuc-open-nuc pattern
+def save_accessible_regions(states_path, accessible_region_file, openregion_minlen):
+    # Function to add regions to the list
+    def add_regions(i, regions):
+        for j in range(i, i+3):
+            if not regions or states_path[j][2] != regions[-1][2]:
+                regions.append((states_path[j][0], int(states_path[j][1]), int(states_path[j][2]), states_path[j][3]))
+        return regions
+
+    # Select only accessible regions from _states.bed, look for nuc-open-nuc pattern
     # This by default is the only final output from HMMRATAC
     accessible_regions = []
     for i in range(len(states_path)-2):
-        #if region has pattern nuc-open-nuc (are the same chromosome and are consecutive bins) AND the open region size > minlen
-        if states_path[i][3] == 'nuc' and states_path[i+1][3] == 'open' and states_path[i+2][3] == 'nuc' and states_path[i][2] == states_path[i+1][1] and states_path[i+1][2] == states_path[i+2][1] and states_path[i+1][2] - states_path[i+1][1] > openregion_minlen:
-        # if states_path[i][3] == 'nuc' and states_path[i+1][3] == 'open' and states_path[i+2][3] == 'nuc' and states_path[i][0] == states_path[i+1][0] and states_path[i+1][0] == states_path[i+2][0] and states_path[i][2] == states_path[i+1][1] and states_path[i+1][2] == states_path[i+2][1]:
-            if len(accessible_regions) > 0:  
-                if int(states_path[i][2]) == int(accessible_regions[-1][2]): #if element already in list, don't repeat
-                    accessible_regions.append((states_path[i+1][0], int(states_path[i+1][1]), int(states_path[i+1][2]), states_path[i+1][3]))
-                    accessible_regions.append((states_path[i+2][0], int(states_path[i+2][1]), int(states_path[i+2][2]), states_path[i+2][3]))
-                else:
-                    accessible_regions.append((states_path[i][0], int(states_path[i][1]), int(states_path[i][2]), states_path[i][3]))
-                    accessible_regions.append((states_path[i+1][0], int(states_path[i+1][1]), int(states_path[i+1][2]), states_path[i+1][3]))
-                    accessible_regions.append((states_path[i+2][0], int(states_path[i+2][1]), int(states_path[i+2][2]), states_path[i+2][3]))
-            elif len(accessible_regions) == 0:
-                accessible_regions.append((states_path[i][0], int(states_path[i][1]), int(states_path[i][2]), states_path[i][3]))
-                accessible_regions.append((states_path[i+1][0], int(states_path[i+1][1]), int(states_path[i+1][2]), states_path[i+1][3]))
-                accessible_regions.append((states_path[i+2][0], int(states_path[i+2][1]), int(states_path[i+2][2]), states_path[i+2][3]))
-    
-    # group states by region
+        if (states_path[i][3] == 'nuc' and states_path[i+1][3] == 'open' and states_path[i+2][3] == 'nuc' and 
+            states_path[i][2] == states_path[i+1][1] and states_path[i+1][2] == states_path[i+2][1] and 
+            states_path[i+1][2] - states_path[i+1][1] > openregion_minlen):
+            accessible_regions = add_regions(i, accessible_regions)
+
+    # Group states by region
     list_of_groups = []
-    one_group = []
-    one_group.append(accessible_regions[0])
+    one_group = [accessible_regions[0]]
     for j in range(1, len(accessible_regions)):
-        # future: add gap here ... if accessible_regions[j][1] == accessible_regions[j-1][2]+options.hmm_binsize or +options.gap 
-        # (this will need to be addressed in how _states.bed and the nuc-open-nuc pattern is selected)
         if accessible_regions[j][1] == accessible_regions[j-1][2]:
             one_group.append(accessible_regions[j])
-        elif accessible_regions[j][1] != accessible_regions[j-1][2]:
-            # if one_group[-2][2] - one_group[1][1] > openregion_minlen: #check: if distance between first open region start_pos and last open region end_pos is above threshold ... then add to list
+        else:
             list_of_groups.append(one_group)
-            one_group = []
-            one_group.append(accessible_regions[j])
+            one_group = [accessible_regions[j]]
     accessible_regions = list_of_groups
-    #print(len(accessible_regions))
-    # generate broadpeak object
+
+    # Generate broadpeak object
     broadpeak = BroadPeakIO()
-    for i in range(len(accessible_regions)-1):
-        block_num = sum('open' in tup for tup in accessible_regions[i]) #number of open states in the region
-        block_sizes = ''
-        block_starts = ''
-        for j in range(1, len(accessible_regions[i])-1, 2):
-            block_sizes = block_sizes + str(accessible_regions[i][j][2] - accessible_regions[i][j][1]) + ',' #distance between start_pos and end_pos in each open state
-            block_starts = block_starts + str(accessible_regions[i][j][1] - accessible_regions[i][0][1] ) + ',' #start_pos for each open state, it's relative position to the start_pos of the whole broad region
-        broadpeak.add(bytes(accessible_regions[i][1][0], encoding="raw_unicode_escape"), #chromosome
-            accessible_regions[i][0][1], #start_pos of first nuc state in the region
-            accessible_regions[i][-1][2], #end_pos of the last nuc state in the region
-            thickStart=bytes(str(accessible_regions[i][1][1]), encoding="raw_unicode_escape"), #start_pos of the first open state
-            thickEnd=bytes(str(accessible_regions[i][-2][2]), encoding="raw_unicode_escape"), #end_pos of the last open state
-            blockNum=block_num,
-            blockSizes=bytes(str(block_sizes[0:-1]), encoding="raw_unicode_escape"),
-            blockStarts=bytes(str(block_starts[0:-1]), encoding="raw_unicode_escape"))
+    for region in accessible_regions[:-1]:
+        block_num = sum('open' in tup for tup in region)
+        block_sizes = ','.join(str(region[j][2] - region[j][1]) for j in range(1, len(region) - 1, 2))
+        block_starts = ','.join(str(region[j][1] - region[0][1]) for j in range(1, len(region) - 1, 2))
+        broadpeak.add(bytes(region[1][0], encoding="raw_unicode_escape"), region[0][1], region[-1][2],
+                      thickStart=bytes(str(region[1][1]), encoding="raw_unicode_escape"),
+                      thickEnd=bytes(str(region[-2][2]), encoding="raw_unicode_escape"),
+                      blockNum=block_num,
+                      blockSizes=bytes(block_sizes, encoding="raw_unicode_escape"),
+                      blockStarts=bytes(block_starts, encoding="raw_unicode_escape"))
     broadpeak.write_to_gappedPeak(accessible_region_file)
     return
-
```

### Comparing `MACS3-3.0.0b1/MACS3/Commands/pileup_cmd.py` & `MACS3-3.0.0b2/MACS3/Commands/pileup_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # Time-stamp: <2020-11-24 16:50:16 Tao Liu>
 # ------------------------------------
 # python modules
 # ------------------------------------
 
 import os
 import sys
-import logging
 
 # ------------------------------------
 # own python modules
 # ------------------------------------
 from MACS3.Utilities.Constants import *
 from MACS3.Utilities.OptValidator import opt_validate_pileup
 from MACS3.Signal.Pileup import pileup_and_write_se, pileup_and_write_pe
```

### Comparing `MACS3-3.0.0b1/MACS3/Commands/predictd_cmd.py` & `MACS3-3.0.0b2/MACS3/Commands/predictd_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 # ------------------------------------
 # python modules
 # ------------------------------------
 
 import os
 import sys
-import logging
 
 # ------------------------------------
 # own python modules
 # ------------------------------------
 from MACS3.Utilities.Constants import *
 from MACS3.Utilities.OptValidator import opt_validate_predictd
 from MACS3.Signal.PeakModel import PeakModel,NotEnoughPairsException
```

### Comparing `MACS3-3.0.0b1/MACS3/Commands/randsample_cmd.py` & `MACS3-3.0.0b2/MACS3/Commands/randsample_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 # ------------------------------------
 # python modules
 # ------------------------------------
 
 import os
 import sys
-import logging
 
 # ------------------------------------
 # own python modules
 # ------------------------------------
 from MACS3.Utilities.Constants import *
 from MACS3.Utilities.OptValidator import opt_validate_randsample
```

### Comparing `MACS3-3.0.0b1/MACS3/Commands/refinepeak_cmd.py` & `MACS3-3.0.0b2/MACS3/Commands/refinepeak_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 # ------------------------------------
 # python modules
 # ------------------------------------
 
 import os
 import sys
-import logging
 from collections import Counter
 
 # ------------------------------------
 # own python modules
 # ------------------------------------
 from MACS3.Utilities.Constants import *
 from MACS3.Utilities.OptValidator import opt_validate_refinepeak
```

### Comparing `MACS3-3.0.0b1/MACS3/IO/BAM.pyx` & `MACS3-3.0.0b2/MACS3/IO/BAM.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 under the terms of the BSD License (see the file LICENSE included with
 the distribution).
 """
 
 # ------------------------------------
 # python modules
 # ------------------------------------
-import logging
-from logging import info, debug
 import struct
 from struct import unpack
 import gzip
 import io
 import os
 import sys
 from zlib import decompress, MAX_WBITS
```

### Comparing `MACS3-3.0.0b1/MACS3/IO/BedGraphIO.pyx` & `MACS3-3.0.0b2/MACS3/IO/BedGraphIO.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/IO/OutputWriter.py` & `MACS3-3.0.0b2/MACS3/IO/OutputWriter.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,50 +15,53 @@
 from array import array as pyarray
 
 from MACS3.Utilities.Constants import MACS_VERSION
 
 # ------------------------------------
 # constants
 # ------------------------------------
+import logging
+import MACS3.Utilities.Logger
 
+logger = logging.getLogger(__name__)
+debug   = logger.debug
+info    = logger.info
 # ------------------------------------
 # Misc functions
 # ------------------------------------
 def zwig_write (trackI, subdir, fileprefix, d, log=None,space=10, single=False):
     """Write shifted tags information in wiggle file in a given
     step. Then compress it using 'gzip' program.
 
     trackI: shifted tags from PeakDetect object
     subdir: directory where to put the wiggle file
     fileprefix: wiggle file prefix
     d     : d length
     log   : logging function, default is sys.stderr.write
     space : space to write tag number on spots, default 10
     """
-    if not log:
-        log = lambda x: sys.stderr.write(x+"\n")
     chrs = trackI.get_chr_names()
     os.makedirs (subdir)
     step = 10000000 + 2*d
 
     if single:
-        log("write to a wiggle file")
+        info("write to a wiggle file")
         f = os.path.join(subdir,fileprefix+"_all"+".wig")
         wigfhd = open(f,"w")
         wigfhd.write("track type=wiggle_0 name=\"%s_all\" description=\"Extended tag pileup from MACS version %s for every %d bp\"\n" % (fileprefix.replace('_afterfiting',''), MACS_VERSION, space)) # data type line
 
     for chrom in sorted(chrs):
         if not single:
             f = os.path.join(subdir,fileprefix+"_"+chrom+".wig")
-            log("write to "+f+" for chromosome "+chrom)
+            info("write to "+f+" for chromosome "+chrom)
             wigfhd = open(f,"w")
             # suggested by dawe
             wigfhd.write("track type=wiggle_0 name=\"%s_%s\" description=\"Extended tag pileup from MACS version %s for every %d bp\"\n" % ( fileprefix.replace('_afterfiting',''), chrom, MACS_VERSION, space)) # data type line
         else:
-            log("write data for chromosome "+chrom)
+            info("write data for chromosome "+chrom)
 
         wigfhd.write("variableStep chrom=%s span=%d\n" % (chrom,space))
         tags = trackI.get_locations_by_chr(chrom)[0]
         l = len(tags)
         window_counts = pyarray('L',[0]*step)
         startp = -1*d
         endp   = startp+step
@@ -95,19 +98,19 @@
         for i in range(d,step-d,space):
             if window_counts[i] == 0:
                 pass
             else:
                 wigfhd.write("%d\t%d\n" % (i+startp+1,window_counts[i]))
         if not single:
             wigfhd.close()
-            log("compress the wiggle file using gzip...")
+            info("compress the wiggle file using gzip...")
             os.system("gzip "+f)
     if single:
         wigfhd.close()
-        log("compress the wiggle file using gzip...")
+        info("compress the wiggle file using gzip...")
         os.system("gzip "+f)
 
 
 def zbdg_write (trackI, subdir, fileprefix, d, log=None, single=False):
     """Write shifted tags information in wiggle file in a given
     step. Then compress it using 'gzip' program.
 
@@ -121,27 +124,27 @@
     if not log:
         log = lambda x: sys.stderr.write(x+"\n")
     chrs = trackI.get_chr_names()
     os.makedirs (subdir)
     step = 10000000 + 2*d
 
     if single:
-        log("write to a bedGraph file")
+        info("write to a bedGraph file")
         f = os.path.join(subdir,fileprefix+"_all"+".bdg")
         bdgfhd = open(f,"w")
         bdgfhd.write("track type=bedGraph name=\"%s_all\" description=\"Extended tag pileup from MACS version %s\"\n" % (fileprefix.replace('_afterfiting',''), MACS_VERSION)) # data type line
 
     for chrom in sorted(chrs):
         if not single:
             f = os.path.join(subdir,fileprefix+"_"+chrom+".bdg")
-            log("write to "+f+" for chromosome "+chrom)
+            info("write to "+f+" for chromosome "+chrom)
             bdgfhd = open(f,"w")
             bdgfhd.write("track type=bedGraph name=\"%s_%s\" description=\"Extended tag pileup from MACS version %s\"\n" % (fileprefix.replace('_afterfiting',''), chrom, MACS_VERSION)) # data type line
         else:
-            log("write data for chromosome "+chrom)
+            info("write data for chromosome "+chrom)
 
         tags = trackI.get_locations_by_chr(chrom)[0]
         l = len(tags)
         window_counts = pyarray('L',[0]*step)
         startp = -1*d
         endp   = startp+step
         index_tag = 0
@@ -203,19 +206,19 @@
                 right = left + 1
         # last bin
         if prev != 0:
             bdgfhd.write("%s\t%d\t%d\t%d\n" % (chrom,left,right,prev))
 
         if not single:
             bdgfhd.close()
-            log("compress the bedGraph file using gzip...")
+            info("compress the bedGraph file using gzip...")
             os.system("gzip "+f)
     if single:
         bdgfhd.close()
-        log("compress the bedGraph file using gzip...")
+        info("compress the bedGraph file using gzip...")
         os.system("gzip "+f)
 
 
 def model2r_script(model,filename,name):
     rfhd = open(filename,"w")
     p = model.plus_line
     m = model.minus_line
```

### Comparing `MACS3-3.0.0b1/MACS3/IO/Parser.pyx` & `MACS3-3.0.0b2/MACS3/IO/Parser.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -11,23 +11,27 @@
 the distribution).
 
 """
 
 # ------------------------------------
 # python modules
 # ------------------------------------
-import logging
-from logging import info, debug
 import struct
 from struct import unpack
 from re import findall
 import gzip
 import io
 import sys
 
+import logging
+import MACS3.Utilities.Logger
+
+logger = logging.getLogger(__name__)
+debug   = logger.debug
+info    = logger.info
 # ------------------------------------
 # MACS3 modules
 # ------------------------------------
 
 from MACS3.Utilities.Constants import *
 from MACS3.Signal.FixWidthTrack import FWTrack
 from MACS3.Signal.PairedEndTrack import PETrackI
```

### Comparing `MACS3-3.0.0b1/MACS3/IO/PeakIO.pyx` & `MACS3-3.0.0b2/MACS3/IO/PeakIO.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/BedGraph.pyx` & `MACS3-3.0.0b2/MACS3/Signal/BedGraph.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # cython: language_level=3
 # cython: profile=True
-# Time-stamp: <2022-10-04 15:46:00 Tao Liu>
+# Time-stamp: <2023-06-08 10:52:59 Tao Liu>
 
 """Module for BedGraph data class.
 
 This code is free software; you can redistribute it and/or modify it
 under the terms of the BSD License (see the file LICENSE included with
 the distribution).
 """
 
 # ------------------------------------
 # python modules
 # ------------------------------------
-import logging
 #from array import array
 from cpython cimport array
 from array import array as pyarray
 from math import prod
 # ------------------------------------
 # MACS3 modules
 # ------------------------------------
@@ -398,16 +397,17 @@
                     new_value.append(value)
                 new_pre_pos = new_pos[-1]
                 new_pre_value = new_value[-1]
             self.__data[chrom]=[new_pos,new_value]
         return True
 
     cpdef tuple summary (self):
-        """Calculate the sum, total_length, max, min, mean, and std. Return a tuple for (sum, max, min, mean, std).
+        """Calculate the sum, total_length, max, min, mean, and std. 
 
+        Return a tuple for (sum, total_length, max, min, mean, std).
         """
         cdef:
             int64_tn_v
             float32_t sum_v, max_v, min_v, mean_v, variance, tmp, std_v
             int32_t pre_p, l, i
 
         pre_p = 0
@@ -1128,41 +1128,71 @@
                 pass
 
         ret.finalize()
         #ret.merge_regions()
         return ret
 
     cpdef str cutoff_analysis ( self, int32_t max_gap, int32_t min_length, int32_t steps = 100 ):
+        """
+        Cutoff analysis function for bedGraphTrackI object.
+    
+        This function will try all possible cutoff values on the score column to call peaks. Then 
+        will give a report of a number of metrics (number of peaks, total length of peaks, average
+        length of peak) at varying score cutoffs. For each score cutoff, the function finds the 
+        positions where the score exceeds the cutoff, then groups those positions into "peaks" 
+        based on the maximum allowed gap (max_gap) between consecutive positions. If a peak's length
+        exceeds the minimum length (min_length), the peak is counted.
+
+        Parameters
+        ----------
+        max_gap : int32_t
+        Maximum allowed gap between consecutive positions above cutoff
+        
+        min_length : int32_t
+        Minimum length of peak
+        
+        steps: int32_t
+
+        Returns
+        -------
+        Cutoff analysis report in 'str'
+        
+        """
         cdef:
             set chrs
-            list tmplist, peak_content
+            list peak_content, ret_list, cutoff_list, cutoff_npeaks, cutoff_lpeaks
             bytes  chrom
             str ret
             float32_t cutoff
             int64_t total_l, total_p, i, n, ts, te, lastp, tl, peak_length
-            dict cutoff_npeaks, cutoff_lpeaks
+            #dict cutoff_npeaks, cutoff_lpeaks
             float32_t s, midvalue
 
         chrs = self.get_chr_names()
 
-        midvalue = self.minvalue/2 + self.maxvalue/2
-        s = float(self.minvalue - midvalue)/steps
+        #midvalue = self.minvalue/2 + self.maxvalue/2
+        #s = float(self.minvalue - midvalue)/steps
+        minv = self.minvalue
+        maxv = self.maxvalue
 
-        tmplist = list( np.arange( midvalue, self.minvalue - s, s ) )
+        s = float(maxv - minv)/steps
 
-        cutoff_npeaks = {}
-        cutoff_lpeaks = {}
+        # a list of possible cutoff values from minv to maxv with step of s
+        cutoff_list = [round(value, 3) for value in np.arange(minv, maxv, s)]
+
+        cutoff_npeaks = [0] * len( cutoff_list )
+        cutoff_lpeaks = [0] * len( cutoff_list )
 
         for chrom in sorted(chrs):
             ( pos_array, score_array ) = self.__data[ chrom ]
             pos_array = np.array( self.__data[ chrom ][ 0 ] )
             score_array = np.array( self.__data[ chrom ][ 1 ] )
 
-            for n in range( len( tmplist ) ):
-                cutoff = round( tmplist[ n ], 3 )
+            for n in range( len( cutoff_list ) ):
+                cutoff = cutoff_list[ n ]
                 total_l = 0           # total length of peaks
                 total_p = 0           # total number of peaks
 
                 # get the regions with scores above cutoffs
                 above_cutoff = np.nonzero( score_array > cutoff )[0]# this is not an optimized method. It would be better to store score array in a 2-D ndarray?
                 above_cutoff_endpos = pos_array[above_cutoff] # end positions of regions where score is above cutoff
                 above_cutoff_startpos = pos_array[above_cutoff-1] # start positions of regions where score is above cutoff
@@ -1194,17 +1224,45 @@
                     lastp = te
 
                 if peak_content:
                     peak_length = peak_content[ -1 ][ 1 ] - peak_content[ 0 ][ 0 ]
                     if peak_length >= min_length: # if the peak is too small, reject it
                         total_l +=  peak_length
                         total_p += 1
-                cutoff_lpeaks[ cutoff ] = cutoff_lpeaks.get( cutoff, 0 ) + total_l
-                cutoff_npeaks[ cutoff ] = cutoff_npeaks.get( cutoff, 0 ) + total_p
-
-        # write pvalue and total length of predicted peaks
-        ret = "pscore\tnpeaks\tlpeaks\tavelpeak\n"
-        for cutoff in sorted(cutoff_lpeaks.keys(), reverse=True):
-            if cutoff_npeaks[ cutoff ] > 0:
-                ret += "%.2f\t%d\t%d\t%.2f\n" % ( cutoff, cutoff_npeaks[ cutoff ], cutoff_lpeaks[ cutoff ], cutoff_lpeaks[ cutoff ]/cutoff_npeaks[ cutoff ] )
+                cutoff_lpeaks[ n ] += total_l
+                cutoff_npeaks[ n ] += total_p
+                
+        # prepare the returnning text
+        ret_list = ["score\tnpeaks\tlpeaks\tavelpeak\n"]
+        for n in range( len( cutoff_list )-1, -1, -1 ):
+            cutoff = cutoff_list[ n ]
+            if cutoff_npeaks[ n ] > 0:
+                ret_list.append("%.2f\t%d\t%d\t%.2f\n" % ( cutoff, cutoff_npeaks[ n ], \
+                                                          cutoff_lpeaks[ n ], \
+                                                          cutoff_lpeaks[ n ]/cutoff_npeaks[ n ] ))
+        ret = ''.join(ret_list)
         return ret
 
+
+cdef np.ndarray calculate_elbows( np.ndarray values, float32_t threshold=0.01):
+    # although this function is supposed to find elbow pts for cutoff analysis, 
+    # however, in reality, it barely works...
+    cdef: 
+        np.ndarray deltas, slopes, delta_slopes, elbows
+        np.float32_t avg_delta_slope
+        
+    # Calculate the difference between each point and the first point
+    deltas = values - values[0]
+    
+    # Calculate the slope between each point and the last point
+    slopes = deltas / (values[-1] - values[0])
+    
+    # Calculate the change in slope
+    delta_slopes = np.diff(slopes)
+    
+    # Calculate the average change in slope
+    avg_delta_slope = np.mean(delta_slopes)
+    
+    # Find all points where the change in slope is significantly larger than the average
+    elbows = np.where(delta_slopes > avg_delta_slope + threshold)[0]
+    
+    return elbows
```

### Comparing `MACS3-3.0.0b1/MACS3/Signal/CallPeakUnit.pyx` & `MACS3-3.0.0b2/MACS3/Signal/CallPeakUnit.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,25 @@
 
 # ------------------------------------
 # python modules
 # ------------------------------------
 
 from collections import Counter
 from copy import copy
-import logging
 from time import time as ttime
 import _pickle as cPickle
 from tempfile import mkstemp
 import os
+
+import logging
+import MACS3.Utilities.Logger
+
+logger = logging.getLogger(__name__)
+debug   = logger.debug
+info    = logger.info
 # ------------------------------------
 # Other modules
 # ------------------------------------
 import numpy as np
 cimport numpy as np
 from numpy cimport uint8_t, uint16_t, uint32_t, uint64_t, int8_t, int16_t, int32_t, int64_t, float32_t, float64_t
 from cpython cimport bool
@@ -623,15 +629,15 @@
             int64_t N, k, this_l
             float32_t f
             list unique_values
             int32_t * pos_ptr
             float32_t * treat_value_ptr
             float32_t * ctrl_value_ptr
 
-        logging.debug ( "Start to calculate pvalue stat..." )
+        debug ( "Start to calculate pvalue stat..." )
 
         pscore_stat = {} #dict()
         for i in range( len( self.chromosomes ) ):
             chrom = self.chromosomes[ i ]
             pre_p = 0
 
             self.__pileup_treat_ctrl_a_chromosome( chrom )
@@ -705,15 +711,15 @@
             list tmplist
 
             int32_t * acs_ptr   # above cutoff start position pointer
             int32_t * ace_ptr   # above cutoff end position pointer
             int32_t * pos_array_ptr # position array pointer
             float32_t * score_array_ptr # score array pointer
 
-        logging.debug ( "Start to calculate pvalue stat..." )
+        debug ( "Start to calculate pvalue stat..." )
 
         # tmplist contains a list of log pvalue cutoffs from 0.3 to 10
         tmplist = [round(x,5) for x in sorted( list(np.arange(0.3, 10.0, 0.3)), reverse = True )]
 
         pscore_stat = {} #dict()
         #print (list(pscore_stat.keys()))
         #print (list(self.pvalue_length.keys()))
@@ -781,15 +787,15 @@
                     pscore_stat[ this_v ] += this_l
                 else:
                     pscore_stat[ this_v ] = this_l
                 pre_p = this_p #pos_array[ i ]
                 pos_array_ptr += 1
                 score_array_ptr += 1
 
-        #logging.debug ( "make pscore_stat cost %.5f seconds" % t )
+        #debug ( "make pscore_stat cost %.5f seconds" % t )
 
         # add all pvalue cutoffs from cutoff-analysis part. So that we
         # can get the corresponding qvalues for them.
         for cutoff in tmplist:
             if cutoff not in pscore_stat:
                 pscore_stat[ cutoff ] = 0
 
@@ -830,18 +836,18 @@
         y = []
         for cutoff in tmplist:
             if self.pvalue_npeaks[ cutoff ] > 0:
                 fhd.write( "%.2f\t%.2f\t%d\t%d\t%.2f\n" % ( cutoff, self.pqtable[ cutoff ], self.pvalue_npeaks[ cutoff ], self.pvalue_length[ cutoff ], self.pvalue_length[ cutoff ]/self.pvalue_npeaks[ cutoff ] ) )
                 x.append( cutoff )
                 y.append( self.pvalue_length[ cutoff ] )
         fhd.close()
-        logging.info( "#3 Analysis of cutoff vs num of peaks or total length has been saved in %s" % self.cutoff_analysis_filename )
-        #logging.info( "#3 Suggest a cutoff..." )
+        info( "#3 Analysis of cutoff vs num of peaks or total length has been saved in %s" % self.cutoff_analysis_filename )
+        #info( "#3 Suggest a cutoff..." )
         #optimal_cutoff, optimal_length = find_optimal_cutoff( x, y )
-        #logging.info( "#3 -10log10pvalue cutoff %.2f will call approximately %.0f bps regions as significant regions" % ( optimal_cutoff, optimal_length ) )
+        #info( "#3 -10log10pvalue cutoff %.2f will call approximately %.0f bps regions as significant regions" % ( optimal_cutoff, optimal_length ) )
         #print (list(pqtable.keys()))
         #print (list(self.pvalue_length.keys()))
         #print (list(self.pvalue_npeaks.keys()))
         return
 
     cpdef call_peaks ( self, list scoring_function_symbols, list score_cutoff_s, int32_t min_length = 200,
                        int32_t max_gap = 50, bool call_summits = False, bool cutoff_analysis = False ):
@@ -858,46 +864,46 @@
             bytes chrom
             bytes tmp_bytes
 
         peaks = PeakIO()
 
         # prepare p-q table
         if len( self.pqtable ) == 0:
-            logging.info("#3 Pre-compute pvalue-qvalue table...")
+            info("#3 Pre-compute pvalue-qvalue table...")
             if cutoff_analysis:
-                logging.info("#3 Cutoff vs peaks called will be analyzed!")
+                info("#3 Cutoff vs peaks called will be analyzed!")
                 self.__pre_computes( max_gap = max_gap, min_length = min_length )
             else:
                 self.__cal_pvalue_qvalue_table()
 
 
         # prepare bedGraph file
         if self.save_bedGraph:
             self.bedGraph_treat_f = fopen( self.bedGraph_treat_filename, "w" )
             self.bedGraph_ctrl_f = fopen( self.bedGraph_control_filename, "w" )
 
-            logging.info ("#3 In the peak calling step, the following will be performed simultaneously:")
-            logging.info ("#3   Write bedGraph files for treatment pileup (after scaling if necessary)... %s" % self.bedGraph_filename_prefix.decode() + "_treat_pileup.bdg")
-            logging.info ("#3   Write bedGraph files for control lambda (after scaling if necessary)... %s" % self.bedGraph_filename_prefix.decode() + "_control_lambda.bdg")
+            info ("#3 In the peak calling step, the following will be performed simultaneously:")
+            info ("#3   Write bedGraph files for treatment pileup (after scaling if necessary)... %s" % self.bedGraph_filename_prefix.decode() + "_treat_pileup.bdg")
+            info ("#3   Write bedGraph files for control lambda (after scaling if necessary)... %s" % self.bedGraph_filename_prefix.decode() + "_control_lambda.bdg")
 
             if self.save_SPMR:
-                logging.info ( "#3   --SPMR is requested, so pileup will be normalized by sequencing depth in million reads." )
+                info ( "#3   --SPMR is requested, so pileup will be normalized by sequencing depth in million reads." )
             elif self.treat_scaling_factor == 1:
-                logging.info ( "#3   Pileup will be based on sequencing depth in treatment." )
+                info ( "#3   Pileup will be based on sequencing depth in treatment." )
             else:
-                logging.info ( "#3   Pileup will be based on sequencing depth in control." )
+                info ( "#3   Pileup will be based on sequencing depth in control." )
 
             if self.trackline:
                 # this line is REQUIRED by the wiggle format for UCSC browser
                 tmp_bytes = ("track type=bedGraph name=\"treatment pileup\" description=\"treatment pileup after possible scaling for \'%s\'\"\n" % self.bedGraph_filename_prefix).encode()
                 fprintf( self.bedGraph_treat_f, tmp_bytes )
                 tmp_bytes = ("track type=bedGraph name=\"control lambda\" description=\"control lambda after possible scaling for \'%s\'\"\n" % self.bedGraph_filename_prefix).encode()
                 fprintf( self.bedGraph_ctrl_f, tmp_bytes )
 
-        logging.info("#3 Call peaks for each chromosome...")
+        info("#3 Call peaks for each chromosome...")
         for chrom in self.chromosomes:
             # treat/control bedGraph will be saved if requested by user.
             self.__chrom_call_peak_using_certain_criteria ( peaks, chrom, scoring_function_symbols, score_cutoff_s, min_length, max_gap, call_summits, self.save_bedGraph )
 
         # close bedGraph file
         if self.save_bedGraph:
             fclose(self.bedGraph_treat_f)
@@ -1423,39 +1429,39 @@
             list tmppeakset
 
         lvl1peaks = PeakIO()
         lvl2peaks = PeakIO()
 
         # prepare p-q table
         if len( self.pqtable ) == 0:
-            logging.info("#3 Pre-compute pvalue-qvalue table...")
+            info("#3 Pre-compute pvalue-qvalue table...")
             if cutoff_analysis:
-                logging.info("#3 Cutoff value vs broad region calls will be analyzed!")
+                info("#3 Cutoff value vs broad region calls will be analyzed!")
                 self.__pre_computes( max_gap = lvl2_max_gap, min_length = min_length )
             else:
                 self.__cal_pvalue_qvalue_table()
 
         # prepare bedGraph file
         if self.save_bedGraph:
 
             self.bedGraph_treat_f = fopen( self.bedGraph_treat_filename, "w" )
             self.bedGraph_ctrl_f = fopen( self.bedGraph_control_filename, "w" )
-            logging.info ("#3 In the peak calling step, the following will be performed simultaneously:")
-            logging.info ("#3   Write bedGraph files for treatment pileup (after scaling if necessary)... %s" % self.bedGraph_filename_prefix.decode() + "_treat_pileup.bdg")
-            logging.info ("#3   Write bedGraph files for control lambda (after scaling if necessary)... %s" % self.bedGraph_filename_prefix.decode() + "_control_lambda.bdg")
+            info ("#3 In the peak calling step, the following will be performed simultaneously:")
+            info ("#3   Write bedGraph files for treatment pileup (after scaling if necessary)... %s" % self.bedGraph_filename_prefix.decode() + "_treat_pileup.bdg")
+            info ("#3   Write bedGraph files for control lambda (after scaling if necessary)... %s" % self.bedGraph_filename_prefix.decode() + "_control_lambda.bdg")
 
             if self.trackline:
                 # this line is REQUIRED by the wiggle format for UCSC browser
                 tmp_bytes = ("track type=bedGraph name=\"treatment pileup\" description=\"treatment pileup after possible scaling for \'%s\'\"\n" % self.bedGraph_filename_prefix).encode()
                 fprintf( self.bedGraph_treat_f, tmp_bytes )
                 tmp_bytes = ("track type=bedGraph name=\"control lambda\" description=\"control lambda after possible scaling for \'%s\'\"\n" % self.bedGraph_filename_prefix).encode()
                 fprintf( self.bedGraph_ctrl_f, tmp_bytes )
 
 
-        logging.info("#3 Call peaks for each chromosome...")
+        info("#3 Call peaks for each chromosome...")
         for chrom in self.chromosomes:
             self.__chrom_call_broadpeak_using_certain_criteria ( lvl1peaks, lvl2peaks, chrom, scoring_function_symbols, lvl1_cutoff_s, lvl2_cutoff_s, min_length, lvl1_max_gap, lvl2_max_gap, self.save_bedGraph )
 
         # close bedGraph file
         if self.save_bedGraph:
             fclose( self.bedGraph_treat_f )
             fclose( self.bedGraph_ctrl_f )
```

### Comparing `MACS3-3.0.0b1/MACS3/Signal/FixWidthTrack.pyx` & `MACS3-3.0.0b2/MACS3/Signal/FixWidthTrack.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 under the terms of the BSD License (see the file LICENSE included with
 the distribution).
 """
 
 # ------------------------------------
 # python modules
 # ------------------------------------
-import logging
 import sys
 import io
 from copy import copy
 from collections import Counter
 
 # ------------------------------------
 # MACS3 modules
```

### Comparing `MACS3-3.0.0b1/MACS3/Signal/HMMR_EM.pyx` & `MACS3-3.0.0b2/MACS3/Signal/HMMR_EM.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 the distribution).
 """
 # ------------------------------------
 # python modules
 # ------------------------------------
 from math import sqrt
 import logging
-debug   = logging.debug
-info    = logging.info
+import MACS3.Utilities.Logger
+
+logger = logging.getLogger(__name__)
+debug   = logger.debug
+info    = logger.info
 # ------------------------------------
 # Other modules
 # ------------------------------------
 
 import numpy as np
 cimport numpy as np
 from cpython cimport bool
```

### Comparing `MACS3-3.0.0b1/MACS3/Signal/HMMR_HMM.pyx` & `MACS3-3.0.0b2/MACS3/Signal/HMMR_HMM.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 under the terms of the BSD License (see the file LICENSE included with
 the distribution).
 """
 # ------------------------------------
 # python modules
 # ------------------------------------
 from math import sqrt
-import logging
-debug   = logging.debug
-info    = logging.info
+
 # ------------------------------------
 # Other modules
 # ------------------------------------
 
 import numpy as np
 cimport numpy as np
 from cpython cimport bool
```

### Comparing `MACS3-3.0.0b1/MACS3/Signal/HMMR_Signal_Processing.pyx` & `MACS3-3.0.0b2/MACS3/Signal/HMMR_Signal_Processing.pyx`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # cython: language_level=3
 # cython: profile=True
-# Time-stamp: <2022-10-04 16:14:23 Tao Liu>
+# Time-stamp: <2023-06-08 00:28:40 Tao Liu>
 
 """Module description:
 
 This code is free software; you can redistribute it and/or modify it
 under the terms of the BSD License (see the file LICENSE included with
 the distribution).
 """
 # ------------------------------------
 # python modules
 # ------------------------------------
 from math import sqrt
 import logging
-debug   = logging.debug
-info    = logging.info
+
+logger = logging.getLogger(__name__)
+debug   = logger.debug
+info    = logger.info
 # ------------------------------------
 # Other modules
 # ------------------------------------
 
 import numpy as np
 cimport numpy as np
 from cpython cimport bool
@@ -120,27 +122,27 @@
             bdg.add_chrom_data_hmmr_PV( chrom, certain_signals[ chrom ] )
         ret_bedgraphs.append( bdg )
     return ret_bedgraphs
 
 cpdef list extract_signals_from_regions( list signals, object regions, int binsize = 10  ):
     # we will take regions in peaks, create a bedGraphTrackI with
     # binned regions in peaks, then let them overlap with signals to
-    # create a list (4) of value arrays. 
+    # create a list (4) of value arrays.
+    # 
     cdef:
         list extracted_data, extracted_len, extracted_positions
         object signaltrack
         object regionsbdg
         bytes chrom
         int i, s, e, tmp_s, tmp_e, tmp_n, n, c, counter, prev_c
         list ps
         object p
         list ret_training_data, ret_training_lengths, ret_training_bins
 
     regionsbdg = _make_bdg_of_bins_from_regions( regions, binsize )
-
     # now, let's overlap
     extracted_positions = []
     extracted_data = []
     extracted_len = []
     for signaltrack in signals: # four signal tracks
         # signaltrack is bedGraphTrackI object
         [ positions, values, lengths ] = signaltrack.extract_value_hmmr( regionsbdg )
@@ -148,17 +150,18 @@
         extracted_data.append( values )
         extracted_len.append( lengths )
     ret_training_bins = []
     ret_training_data = []
     ret_training_lengths = []
     c = 0
     nn = len( extracted_data[0] )
-    assert len( extracted_data[0] ) == len( extracted_data[1] )
-    assert len( extracted_data[0] ) == len( extracted_data[2] )
-    assert len( extracted_data[0] ) == len( extracted_data[3] )
+    assert nn > 0
+    assert nn == len( extracted_data[1] )
+    assert nn == len( extracted_data[2] )
+    assert nn == len( extracted_data[3] )
     counter = 0
     prev_c = extracted_len[0][0]
     c = 0
     for i in range( nn ):
         ret_training_bins.append( extracted_positions[0][i] )
         ret_training_data.append(
             [ max( 0.0001, extracted_data[0][i] ),
@@ -174,14 +177,15 @@
     # last region
     ret_training_lengths.append( counter )
     assert sum(ret_training_lengths) == len(ret_training_data)
     assert len(ret_training_bins) == len(ret_training_data)
     return [ ret_training_bins, ret_training_data, ret_training_lengths ]
 
 cdef _make_bdg_of_bins_from_regions ( object regions, int binsize ):
+    # this function will return a BedGraphTrackI object
     cdef:
         object regionsbdg
         long n
         bytes chrom
         list ps
         int s, e, tmp_p, mark_bin, i, r
```

### Comparing `MACS3-3.0.0b1/MACS3/Signal/PairedEndTrack.pyx` & `MACS3-3.0.0b2/MACS3/Signal/PairedEndTrack.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,24 @@
 """
 
 # ------------------------------------
 # Python modules
 # ------------------------------------
 import io
 import sys
-from logging import debug, info
 from copy import copy
 from array import array as pyarray
 from collections import Counter
 
+import logging
+import MACS3.Utilities.Logger
+
+logger = logging.getLogger(__name__)
+debug   = logger.debug
+info    = logger.info
 # ------------------------------------
 # MACS3 modules
 # ------------------------------------
 from MACS3.Utilities.Constants import *
 from MACS3.Signal.Pileup import quick_pileup, over_two_pv_array, se_all_in_one_pileup
 from MACS3.Signal.BedGraph import bedGraphTrackI
 from MACS3.Signal.PileupV2 import pileup_from_LR_hmmratac
```

### Comparing `MACS3-3.0.0b1/MACS3/Signal/PeakDetect.pyx` & `MACS3-3.0.0b2/MACS3/Signal/PeakDetect.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/PeakModel.pyx` & `MACS3-3.0.0b2/MACS3/Signal/PeakModel.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/PeakVariants.pyx` & `MACS3-3.0.0b2/MACS3/Signal/PeakVariants.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/Pileup.pyx` & `MACS3-3.0.0b2/MACS3/Signal/Pileup.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/PileupV2.pyx` & `MACS3-3.0.0b2/MACS3/Signal/PileupV2.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/PosReadsInfo.pyx` & `MACS3-3.0.0b2/MACS3/Signal/PosReadsInfo.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/Prob.pyx` & `MACS3-3.0.0b2/MACS3/Signal/Prob.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/RACollection.pyx` & `MACS3-3.0.0b2/MACS3/Signal/RACollection.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/ReadAlignment.pyx` & `MACS3-3.0.0b2/MACS3/Signal/ReadAlignment.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/Region.pyx` & `MACS3-3.0.0b2/MACS3/Signal/Region.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/ScoreTrack.pyx` & `MACS3-3.0.0b2/MACS3/Signal/ScoreTrack.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 """
 
 # ------------------------------------
 # python modules
 # ------------------------------------
 from copy import copy
 from functools import reduce
-import logging
 
 # ------------------------------------
 # MACS3 modules
 # ------------------------------------
 from MACS3.Signal.SignalProcessing import maxima, enforce_valleys, enforce_peakyness
 from MACS3.Signal.Prob import poisson_cdf
 from MACS3.IO.PeakIO import PeakIO, BroadPeakIO, parse_peakname
```

### Comparing `MACS3-3.0.0b1/MACS3/Signal/SignalProcessing.pyx` & `MACS3-3.0.0b2/MACS3/Signal/SignalProcessing.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/UnitigRACollection.pyx` & `MACS3-3.0.0b2/MACS3/Signal/UnitigRACollection.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/VariantStat.pyx` & `MACS3-3.0.0b2/MACS3/Signal/VariantStat.pyx`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/cPosValCalculation.c` & `MACS3-3.0.0b2/MACS3/Signal/cPosValCalculation.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/cPosValCalculation.h` & `MACS3-3.0.0b2/MACS3/Signal/cPosValCalculation.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/cPosValCalculation.pxd` & `MACS3-3.0.0b2/MACS3/Signal/cPosValCalculation.pxd`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/swalign.c` & `MACS3-3.0.0b2/MACS3/Signal/swalign.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Signal/swalign.h` & `MACS3-3.0.0b2/MACS3/Signal/swalign.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/Utilities/Constants.py` & `MACS3-3.0.0b2/MACS3/Utilities/Constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MACS_VERSION = "3.0.0b1"
+MACS_VERSION = "3.0.0b2"
 MAX_PAIRNUM = 1000
 MAX_LAMBDA  = 100000
 FESTEP      = 20
 BUFFER_SIZE = 100000                   # np array will increase at step of 1 million items
 READ_BUFFER_SIZE = 10000000            # 10M bytes for read buffer size
 N_MP = 2                               # Number of processers
```

### Comparing `MACS3-3.0.0b1/MACS3/Utilities/OptValidator.py` & `MACS3-3.0.0b2/MACS3/Utilities/OptValidator.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # ------------------------------------
 # python modules
 # ------------------------------------
 import sys
 import os
 import re
-import logging
+import resource # we turn on memory monitoring inside of logging
 from argparse import ArgumentError
 from subprocess import Popen, PIPE
 from math import log
 
 # ------------------------------------
 # MACS3 modules
 # ------------------------------------
@@ -26,31 +26,46 @@
     BEDPEParser, BowtieParser,  guess_parser
 
 from MACS3.Utilities.Constants import EFFECTIVEGS as efgsize
 # ------------------------------------
 # constants
 # ------------------------------------
 
+import logging
+import MACS3.Utilities.Logger
+logger = logging.getLogger(__name__)
+
 # ------------------------------------
 # Misc functions
 # ------------------------------------
+
+logger = logging.getLogger(__name__)
+
 def opt_validate_callpeak ( options ):
     """Validate options from a OptParser object.
 
     Ret: Validated options object.
     """
+    # logging object
+    logger.setLevel((4-options.verbose)*10)
+
+    options.error   = logger.critical        # function alias
+    options.warn    = logger.warning
+    options.debug   = logger.debug
+    options.info    = logger.info
+    
     # gsize
     try:
         options.gsize = efgsize[options.gsize]
     except:
         try:
             options.gsize = float(options.gsize)
         except:
-            logging.error("Error when interpreting --gsize option: %s" % options.gsize)
-            logging.error("Available shortcuts of effective genome sizes are %s" % ",".join(list(efgsize.keys())))
+            logger.error("Error when interpreting --gsize option: %s" % options.gsize)
+            logger.error("Available shortcuts of effective genome sizes are %s" % ",".join(list(efgsize.keys())))
             sys.exit(1)
 
     # format
     options.gzip_flag = False           # if the input is gzip file
 
     options.format = options.format.upper()
     if options.format == "ELAND":
@@ -74,39 +89,39 @@
         options.parser = BEDPEParser
         options.nomodel = True
     elif options.format == "BOWTIE":
         options.parser = BowtieParser
     elif options.format == "AUTO":
         options.parser = guess_parser
     else:
-        logging.error("Format \"%s\" cannot be recognized!" % (options.format))
+        logger.error("Format \"%s\" cannot be recognized!" % (options.format))
         sys.exit(1)
 
     # duplicate reads
     if options.keepduplicates != "auto" and options.keepduplicates != "all":
         if not options.keepduplicates.isdigit():
-            logging.error("--keep-dup should be 'auto', 'all' or an integer!")
+            logger.error("--keep-dup should be 'auto', 'all' or an integer!")
             sys.exit(1)
 
     # shiftsize>0
     #if options.shiftsize:               # only if --shiftsize is set, it's true
     #    options.extsize = 2 * options.shiftsize
     #else:                               # if --shiftsize is not set
     #    options.shiftsize = options.extsize / 2
     if options.extsize < 1 :
-        logging.error("--extsize must >= 1!")
+        logger.error("--extsize must >= 1!")
         sys.exit(1)
 
     # refine_peaks, call_summits can't be combined with --broad
     #if options.broad and (options.refine_peaks or options.call_summits):
-    #    logging.error("--broad can't be combined with --refine-peaks or --call-summits!")
+    #    logger.error("--broad can't be combined with --refine-peaks or --call-summits!")
     #    sys.exit(1)
 
     if options.broad and options.call_summits:
-        logging.error("--broad can't be combined with --call-summits!")
+        logger.error("--broad can't be combined with --call-summits!")
         sys.exit(1)
 
     if options.pvalue:
         # if set, ignore qvalue cutoff
         options.log_qvalue = None
         options.log_pvalue = log(options.pvalue,10)*-1
     else:
@@ -116,22 +131,22 @@
         options.log_broadcutoff = log(options.broadcutoff,10)*-1
 
     # uppercase the format string
     options.format = options.format.upper()
 
     # d_min is non-negative
     if options.d_min < 0:
-        logging.error("Minimum fragment size shouldn't be negative!" % options.d_min)
+        logger.error("Minimum fragment size shouldn't be negative!" % options.d_min)
         sys.exit(1)
 
     # upper and lower mfold
     options.lmfold = options.mfold[0]
     options.umfold = options.mfold[1]
     if options.lmfold > options.umfold:
-        logging.error("Upper limit of mfold should be greater than lower limit!" % options.mfold)
+        logger.error("Upper limit of mfold should be greater than lower limit!" % options.mfold)
         sys.exit(1)
 
     # output filenames
     options.peakxls = os.path.join( options.outdir, options.name+"_peaks.xls" )
     options.peakbed = os.path.join( options.outdir, options.name+"_peaks.bed" )
     options.peakNarrowPeak = os.path.join( options.outdir, options.name+"_peaks.narrowPeak" )
     options.peakBroadPeak = os.path.join( options.outdir, options.name+"_peaks.broadPeak" )
@@ -144,27 +159,14 @@
     else:
         options.cutoff_analysis_file = "None"
     #options.negxls  = os.path.join( options.name+"_negative_peaks.xls" )
     #options.diagxls = os.path.join( options.name+"_diag.xls" )
     options.modelR  = os.path.join( options.outdir, options.name+"_model.r" )
     #options.pqtable  = os.path.join( options.outdir, options.name+"_pq_table.txt" )
 
-    # logging object
-    logging.basicConfig(level=(4-options.verbose)*10,
-                        format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                        datefmt='%a, %d %b %Y %H:%M:%S',
-                        stream=sys.stderr,
-                        filemode="w"
-                        )
-
-    options.error   = logging.critical        # function alias
-    options.warn    = logging.warning
-    options.debug   = logging.debug
-    options.info    = logging.info
-
     options.argtxt = "\n".join((
         "# Command line: %s" % " ".join(sys.argv[1:]),\
         "# ARGUMENTS LIST:",\
         "# name = %s" % (options.name),\
         "# format = %s" % (options.format),\
         "# ChIP-seq file = %s" % (options.tfile),\
         "# control file = %s" % (options.cfile),\
@@ -242,24 +244,32 @@
     return options
 
 def opt_validate_diffpeak ( options ):
     """Validate options from a OptParser object.
 
     Ret: Validated options object.
     """
+    # logging object
+    logger.setLevel((4-options.verbose)*10)
+
+    options.error   = logger.critical        # function alias
+    options.warn    = logger.warning
+    options.debug   = logger.debug
+    options.info    = logger.info
+    
     # format
     options.gzip_flag = False           # if the input is gzip file
 
 #    options.format = options.format.upper()
     # fox this stuff
 #    if True: pass
 #    elif options.format == "AUTO":
 #        options.parser = guess_parser
 #    else:
-#        logging.error("Format \"%s\" cannot be recognized!" % (options.format))
+#        logger.error("Format \"%s\" cannot be recognized!" % (options.format))
 #        sys.exit(1)
 
     if options.peaks_pvalue:
         # if set, ignore qvalue cutoff
         options.peaks_log_qvalue = None
         options.peaks_log_pvalue = log(options.peaks_pvalue,10)*-1
         options.track_score_method = 'p'
@@ -326,43 +336,38 @@
 
     if options.diff_pvalue:
         options.argtxt +=  "# differential pvalue cutoff = %.2e\n" % (options.log_pvalue)
         options.argtxt +=  "# differential qvalue will not be calculated and reported as -1 in the final output.\n"
     else:
         options.argtxt +=  "# differential qvalue cutoff = %.2e\n" % (options.log_qvalue)
 
-    # logging object
-    logging.basicConfig(level=(4-options.verbose)*10,
-                        format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                        datefmt='%a, %d %b %Y %H:%M:%S',
-                        stream=sys.stderr,
-                        filemode="w"
-                        )
-
-    options.error   = logging.critical        # function alias
-    options.warn    = logging.warning
-    options.debug   = logging.debug
-    options.info    = logging.info
-
     return options
 
 def opt_validate_filterdup ( options ):
     """Validate options from a OptParser object.
 
     Ret: Validated options object.
     """
+    # logging object
+    logger.setLevel((4-options.verbose)*10)
+
+    options.error   = logger.critical        # function alias
+    options.warn    = logger.warning
+    options.debug   = logger.debug
+    options.info    = logger.info
+    
     # gsize
     try:
         options.gsize = efgsize[options.gsize]
     except:
         try:
             options.gsize = float(options.gsize)
         except:
-            logging.error("Error when interpreting --gsize option: %s" % options.gsize)
-            logging.error("Available shortcuts of effective genome sizes are %s" % ",".join(list(efgsize.keys())))
+            logger.error("Error when interpreting --gsize option: %s" % options.gsize)
+            logger.error("Available shortcuts of effective genome sizes are %s" % ",".join(list(efgsize.keys())))
             sys.exit(1)
 
     # format
 
     options.gzip_flag = False           # if the input is gzip file
 
     options.format = options.format.upper()
@@ -387,46 +392,41 @@
         options.parser = BAMPEParser
         options.gzip_flag = True
     elif options.format == "BEDPE":
         options.parser = BEDPEParser
     elif options.format == "AUTO":
         options.parser = guess_parser
     else:
-        logging.error("Format \"%s\" cannot be recognized!" % (options.format))
+        logger.error("Format \"%s\" cannot be recognized!" % (options.format))
         sys.exit(1)
 
     # duplicate reads
     if options.keepduplicates != "auto" and options.keepduplicates != "all":
         if not options.keepduplicates.isdigit():
-            logging.error("--keep-dup should be 'auto', 'all' or an integer!")
+            logger.error("--keep-dup should be 'auto', 'all' or an integer!")
             sys.exit(1)
 
     # uppercase the format string
     options.format = options.format.upper()
 
-    # logging object
-    logging.basicConfig(level=(4-options.verbose)*10,
-                        format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                        datefmt='%a, %d %b %Y %H:%M:%S',
-                        stream=sys.stderr,
-                        filemode="w"
-                        )
-
-    options.error   = logging.critical        # function alias
-    options.warn    = logging.warning
-    options.debug   = logging.debug
-    options.info    = logging.info
-
     return options
 
 def opt_validate_randsample ( options ):
     """Validate options from a OptParser object.
 
     Ret: Validated options object.
     """
+    # logging object
+    logger.setLevel((4-options.verbose)*10)
+
+    options.error   = logger.critical        # function alias
+    options.warn    = logger.warning
+    options.debug   = logger.debug
+    options.info    = logger.info
+    
     # format
 
     options.gzip_flag = False           # if the input is gzip file
 
     options.format = options.format.upper()
     if options.format == "ELAND":
         options.parser = ELANDResultParser
@@ -447,50 +447,45 @@
         options.parser = BAMPEParser
         options.gzip_flag = True
     elif options.format == "BEDPE":
         options.parser = BEDPEParser
     elif options.format == "AUTO":
         options.parser = guess_parser
     else:
-        logging.error("Format \"%s\" cannot be recognized!" % (options.format))
+        logger.error("Format \"%s\" cannot be recognized!" % (options.format))
         sys.exit(1)
 
     # uppercase the format string
     options.format = options.format.upper()
 
     # percentage or number
     if options.percentage:
         if options.percentage > 100.0:
-            logging.error("Percentage can't be bigger than 100.0. Please check your options and retry!")
+            logger.error("Percentage can't be bigger than 100.0. Please check your options and retry!")
             sys.exit(1)
     elif options.number:
         if options.number <= 0:
-            logging.error("Number of tags can't be smaller than or equal to 0. Please check your options and retry!")
+            logger.error("Number of tags can't be smaller than or equal to 0. Please check your options and retry!")
             sys.exit(1)
 
-    # logging object
-    logging.basicConfig(level=(4-options.verbose)*10,
-                        format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                        datefmt='%a, %d %b %Y %H:%M:%S',
-                        stream=sys.stderr,
-                        filemode="w"
-                        )
-
-    options.error   = logging.critical        # function alias
-    options.warn    = logging.warning
-    options.debug   = logging.debug
-    options.info    = logging.info
-
     return options
 
 def opt_validate_refinepeak ( options ):
     """Validate options from a OptParser object.
 
     Ret: Validated options object.
     """
+    # logging object
+    logger.setLevel((4-options.verbose)*10)
+
+    options.error   = logger.critical        # function alias
+    options.warn    = logger.warning
+    options.debug   = logger.debug
+    options.info    = logger.info
+    
     # format
 
     options.gzip_flag = False           # if the input is gzip file
 
     options.format = options.format.upper()
     if options.format == "ELAND":
         options.parser = ELANDResultParser
@@ -506,49 +501,44 @@
         options.parser = BAMParser
         options.gzip_flag = True
     elif options.format == "BOWTIE":
         options.parser = BowtieParser
     elif options.format == "AUTO":
         options.parser = guess_parser
     else:
-        logging.error("Format \"%s\" cannot be recognized!" % (options.format))
+        logger.error("Format \"%s\" cannot be recognized!" % (options.format))
         sys.exit(1)
 
     # uppercase the format string
     options.format = options.format.upper()
 
-    # logging object
-    logging.basicConfig(level=(4-options.verbose)*10,
-                        format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                        datefmt='%a, %d %b %Y %H:%M:%S',
-                        stream=sys.stderr,
-                        filemode="w"
-                        )
-
-    options.error   = logging.critical        # function alias
-    options.warn    = logging.warning
-    options.debug   = logging.debug
-    options.info    = logging.info
-
     return options
 
 def opt_validate_predictd ( options ):
     """Validate options from a OptParser object.
 
     Ret: Validated options object.
     """
+    # logging object
+    logger.setLevel((4-options.verbose)*10)
+
+    options.error   = logger.critical        # function alias
+    options.warn    = logger.warning
+    options.debug   = logger.debug
+    options.info    = logger.info
+    
     # gsize
     try:
         options.gsize = efgsize[options.gsize]
     except:
         try:
             options.gsize = float(options.gsize)
         except:
-            logging.error("Error when interpreting --gsize option: %s" % options.gsize)
-            logging.error("Available shortcuts of effective genome sizes are %s" % ",".join(list(efgsize.keys())))
+            logger.error("Error when interpreting --gsize option: %s" % options.gsize)
+            logger.error("Available shortcuts of effective genome sizes are %s" % ",".join(list(efgsize.keys())))
             sys.exit(1)
 
     # format
     options.gzip_flag = False           # if the input is gzip file
 
     options.format = options.format.upper()
     if options.format == "ELAND":
@@ -572,55 +562,50 @@
         options.parser = BEDPEParser
         options.nomodel = True
     elif options.format == "BOWTIE":
         options.parser = BowtieParser
     elif options.format == "AUTO":
         options.parser = guess_parser
     else:
-        logging.error("Format \"%s\" cannot be recognized!" % (options.format))
+        logger.error("Format \"%s\" cannot be recognized!" % (options.format))
         sys.exit(1)
 
     # uppercase the format string
     options.format = options.format.upper()
 
     # d_min is non-negative
     if options.d_min < 0:
-        logging.error("Minimum fragment size shouldn't be negative!" % options.d_min)
+        logger.error("Minimum fragment size shouldn't be negative!" % options.d_min)
         sys.exit(1)
 
     # upper and lower mfold
     options.lmfold = options.mfold[0]
     options.umfold = options.mfold[1]
     if options.lmfold > options.umfold:
-        logging.error("Upper limit of mfold should be greater than lower limit!" % options.mfold)
+        logger.error("Upper limit of mfold should be greater than lower limit!" % options.mfold)
         sys.exit(1)
 
     options.modelR  = os.path.join( options.outdir, options.rfile )
 
-    # logging object
-    logging.basicConfig(level=(4-options.verbose)*10,
-                        format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                        datefmt='%a, %d %b %Y %H:%M:%S',
-                        stream=sys.stderr,
-                        filemode="w"
-                        )
-
-    options.error   = logging.critical        # function alias
-    options.warn    = logging.warning
-    options.debug   = logging.debug
-    options.info    = logging.info
-
     return options
 
 
 def opt_validate_pileup ( options ):
     """Validate options from a OptParser object.
 
     Ret: Validated options object.
     """
+    # logging object
+    logger.setLevel((4-options.verbose)*10)
+
+    options.error   = logger.critical        # function alias
+    options.warn    = logger.warning
+    options.debug   = logger.debug
+    options.info    = logger.info
+    
     # format
 
     options.gzip_flag = False           # if the input is gzip file
 
     options.format = options.format.upper()
     if options.format == "ELAND":
         options.parser = ELANDResultParser
@@ -639,193 +624,154 @@
         options.parser = BowtieParser
     elif options.format == "BAMPE":
         options.parser = BAMPEParser
         options.gzip_flag = True
     elif options.format == "BEDPE":
         options.parser = BEDPEParser
     else:
-        logging.error("Format \"%s\" cannot be recognized!" % (options.format))
+        logger.error("Format \"%s\" cannot be recognized!" % (options.format))
         sys.exit(1)
 
     # uppercase the format string
     options.format = options.format.upper()
 
-    # logging object
-    logging.basicConfig(level=(4-options.verbose)*10,
-                        format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                        datefmt='%a, %d %b %Y %H:%M:%S',
-                        stream=sys.stderr,
-                        filemode="w"
-                        )
-
-    options.error   = logging.critical        # function alias
-    options.warn    = logging.warning
-    options.debug   = logging.debug
-    options.info    = logging.info
-
     # extsize
     if options.extsize <= 0 :
-        logging.error("--extsize must > 0!")
+        logger.error("--extsize must > 0!")
         sys.exit(1)
 
     return options
 
 def opt_validate_bdgcmp ( options ):
     """Validate options from a OptParser object.
 
     Ret: Validated options object.
     """
     # logging object
-    logging.basicConfig(level=20,
-                        format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                        datefmt='%a, %d %b %Y %H:%M:%S',
-                        stream=sys.stderr,
-                        filemode="w"
-                        )
-
-    options.error   = logging.critical        # function alias
-    options.warn    = logging.warning
-    options.debug   = logging.debug
-    options.info    = logging.info
+    logger.setLevel((4-options.verbose)*10)
+
+    options.error   = logger.critical        # function alias
+    options.warn    = logger.warning
+    options.debug   = logger.debug
+    options.info    = logger.info
 
     # methods should be valid:
 
     for method in set(options.method):
         if method not in [ 'ppois', 'qpois', 'subtract', 'logFE', 'FE', 'logLR', 'slogLR', 'max' ]:
-            logging.error( "Invalid method: %s" % method )
+            logger.error( "Invalid method: %s" % method )
             sys.exit( 1 )
 
     # # of --ofile must == # of -m
 
     if options.ofile:
         if len(options.method) != len(options.ofile):
-            logging.error("The number and the order of arguments for --ofile must be the same as for -m.")
+            logger.error("The number and the order of arguments for --ofile must be the same as for -m.")
             sys.exit(1)
 
     return options
 
 
 def opt_validate_cmbreps ( options ):
     """Validate options from a OptParser object.
 
     Ret: Validated options object.
     """
     # logging object
-    logging.basicConfig(level=20,
-                        format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                        datefmt='%a, %d %b %Y %H:%M:%S',
-                        stream=sys.stderr,
-                        filemode="w"
-                        )
-
-    options.error   = logging.critical        # function alias
-    options.warn    = logging.warning
-    options.debug   = logging.debug
-    options.info    = logging.info
+    logger.setLevel((4-options.verbose)*10)
+
+    options.error   = logger.critical        # function alias
+    options.warn    = logger.warning
+    options.debug   = logger.debug
+    options.info    = logger.info
 
     # methods should be valid:
 
 
     if options.method not in [ 'fisher', 'max', 'mean']:
-        logging.error( "Invalid method: %s" % options.method )
+        logger.error( "Invalid method: %s" % options.method )
         sys.exit( 1 )
 
     if len( options.ifile ) < 2:
-        logging.error("Combining replicates needs at least two replicates!")
+        logger.error("Combining replicates needs at least two replicates!")
         sys.exit( 1 )
 
     # # of -i must == # of -w
 
     # if not options.weights:
     #     options.weights = [ 1.0 ] * len( options.ifile )
 
     # if len( options.ifile ) != len( options.weights ):
-    #     logging.error("Must provide same number of weights as number of input files.")
+    #     logger.error("Must provide same number of weights as number of input files.")
     #     sys.exit( 1 )
 
     # if options.method == "fisher" and len( options.ifile ) > 3:
-    #     logging.error("NOT IMPLEMENTED! Can't combine more than 3 replicates using Fisher's method.")
+    #     logger.error("NOT IMPLEMENTED! Can't combine more than 3 replicates using Fisher's method.")
     #     sys.exit( 1 )
 
     return options
 
 
 def opt_validate_bdgopt ( options ):
     """Validate options from a OptParser object.
 
     Ret: Validated options object.
     """
     # logging object
-    logging.basicConfig(level=20,
-                        format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                        datefmt='%a, %d %b %Y %H:%M:%S',
-                        stream=sys.stderr,
-                        filemode="w"
-                        )
-
-    options.error   = logging.critical        # function alias
-    options.warn    = logging.warning
-    options.debug   = logging.debug
-    options.info    = logging.info
+    logger.setLevel((4-options.verbose)*10)
+
+    options.error   = logger.critical        # function alias
+    options.warn    = logger.warning
+    options.debug   = logger.debug
+    options.info    = logger.info
 
     # methods should be valid:
 
     if options.method.lower() not in [ 'multiply', 'add', 'p2q', 'max', 'min']:
-        logging.error( "Invalid method: %s" % options.method )
+        logger.error( "Invalid method: %s" % options.method )
         sys.exit( 1 )
 
     if options.method.lower() in [ 'multiply', 'add' ] and not options.extraparam:
-        logging.error( "Need EXTRAPARAM for method multiply or add!")
+        logger.error( "Need EXTRAPARAM for method multiply or add!")
         sys.exit( 1 )
 
     return options
 
 def opt_validate_callvar ( options ):
     """Validate options from a OptParser object.
 
     Ret: Validated options object.
     """
     # logging object
-    logging.basicConfig(level=20,
-                        format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                        datefmt='%a, %d %b %Y %H:%M:%S',
-                        stream=sys.stderr,
-                        filemode="w"
-                        )
-
-    options.error   = logging.critical        # function alias
-    options.warn    = logging.warning
-    options.debug   = logging.debug
-    options.info    = logging.info
+    logger.setLevel((4-options.verbose)*10)
+
+    options.error   = logger.critical        # function alias
+    options.warn    = logger.warning
+    options.debug   = logger.debug
+    options.info    = logger.info
 
     # methods should be valid:
 
     if options.np <= 0:
         options.np = 1
     return options
 
 
 def opt_validate_hmmratac ( options ):
     """Validate options from a OptParser object.
 
     Ret: Validated options object.
     """
     # logging object
-    logging.basicConfig(level=(4-options.verbose)*10,
-                        format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                        datefmt='%a, %d %b %Y %H:%M:%S',
-                        stream=sys.stderr,
-                        filemode="w"
-                        )
-
-    options.error   = logging.critical        # function alias
-    options.warn    = logging.warning
-    options.debug   = logging.debug
-    options.info    = logging.info
+    logger.setLevel((4-options.verbose)*10)
 
+    options.error   = logger.critical        # function alias
+    options.warn    = logger.warning
+    options.debug   = logger.debug
+    options.info    = logger.info
    
     # input options.argtxt for hmmratac
     options.argtxt = "# Command line: %s\n" % " ".join(sys.argv[1:])
     #        "# ARGUMENTS LIST:",\
     #        "# outfile = %s" % (options.ofile),\
     #        "# input file = %s\n" % (options.bam_file),\
     # ... add additional
@@ -853,123 +799,114 @@
 
     # EM
     # em_skip
     if options.em_skip:
         options.argtxt += "# EM training not performed on fragment distribution. \n"
     # em_means non-negative
     if sum( [ x < 0 for x in options.em_means ] ):
-        logging.error(" --means should not be negative! ")
+        logger.error(" --means should not be negative! ")
         sys.exit( 1 )
     # em_stddev non-negative
     if sum( [ x < 0 for x in options.em_stddevs ] ):
-        logging.error(" --stddev should not be negative! ")
+        logger.error(" --stddev should not be negative! ")
         sys.exit( 1 )
 
 
     # HMM
     # hmm_states non-negative int, warn if not k=3
     #if options.hmm_states <=0:
-    #    logging.error(" -s, --states must be an integer >= 0.")
+    #    logger.error(" -s, --states must be an integer >= 0.")
     #    sys.exit( 1 )
     #elif options.hmm_states != 3 and options.hmm_states > 0 and options.store_peaks == False:
-    #    logging.warn(" If -s, --states not k=3, recommend NOT calling peaks, use bedgraph.")
+    #    logger.warn(" If -s, --states not k=3, recommend NOT calling peaks, use bedgraph.")
 
     # hmm_binsize > 0
     if options.hmm_binsize <=0:
-        logging.error(" --binsize must be larger than 0.")
+        logger.error(" --binsize must be larger than 0.")
         sys.exit( 1 )
 
     # hmm_lower less than hmm_upper, non-negative 
     if options.hmm_lower <0:
-        logging.error(" -l, --lower should not be negative! ")
+        logger.error(" -l, --lower should not be negative! ")
         sys.exit( 1 )
     if options.hmm_upper <0:
-        logging.error(" -u, --upper should not be negative! ")
+        logger.error(" -u, --upper should not be negative! ")
         sys.exit( 1 )
     if options.hmm_lower > options.hmm_upper:
-        logging.error("Upper limit of fold change range should be greater than lower limit!" % options.mfold)
+        logger.error("Upper limit of fold change range should be greater than lower limit!" % options.mfold)
         sys.exit(1)
     
     # hmm_maxTrain non-negative
     if options.hmm_maxTrain <= 0:
-        logging.error(" --maxTrain should be larger than 0!")
+        logger.error(" --maxTrain should be larger than 0!")
         sys.exit( 1 )
     
     # hmm_training_regions
     #if options.hmm_training_regions:
     #    options.argtxt += "# Using -t, --training input to train HMM instead of using fold change settings to select. \n"
     
     # hmm_zscore non-negative
     #if options.hmm_zscore <0:
-    #    logging.error(" -z, --zscore should not be negative!")
+    #    logger.error(" -z, --zscore should not be negative!")
     #    sys.exit( 1 )
     
     # hmm_randomSeed
     if options.hmm_randomSeed:
         options.argtxt += "# Random seed selected as: %d\n" % options.hmm_randomSeed
     
     # hmm_window non-negative
     #if options.hmm_window <0:
-    #    logging.error(" --window should not be negative! ")
+    #    logger.error(" --window should not be negative! ")
     #    sys.exit( 1 )
 
     # hmm_file
     #if options.hmm_file:
     #    options.argtxt += "# HMM training will be skipped, --model input used instead. \n"
 
     # hmm_modelonly
     #if options.hmm_modelonly:
     #    options.argtxt += "# Program will stop after generating model, which can be later applied with '--model'. \n"
 
 
     # Peak Calling
     if options.prescan_cutoff <= 1:
-        logging.error(" In order to use -c or --prescan-cutoff, the cutoff must be larger than 1.")
+        logger.error(" In order to use -c or --prescan-cutoff, the cutoff must be larger than 1.")
         sys.exit( 1 )
     
     if options.openregion_minlen < 0: # and options.store_peaks == True:
-        logging.error(" In order to use --minlen, the length should not be negative.")
+        logger.error(" In order to use --minlen, the length should not be negative.")
         sys.exit( 1 )
 
     #if options.call_score.lower() not in [ 'max', 'ave', 'med', 'fc', 'zscore', 'all']:
-    #    logging.error( " Invalid method: %s" % options.call_score )
+    #    logger.error( " Invalid method: %s" % options.call_score )
     #    sys.exit( 1 )
 
     # call_threshold non-negative
     #if options.call_threshold <0:
-    #    logging.error(" --threshold should not be negative! ")
+    #    logger.error(" --threshold should not be negative! ")
     #    sys.exit( 1 )
     
 
     # Misc
     # misc_blacklist 
     #if options.misc_keep_duplicates:
     #    options.argtxt += "# Duplicate reads from analysis will be stored. \n"
 
     # misc_trim non-negative
     #if options.misc_trim <0:
-    #    logging.error(" --trim should not be negative! ")
+    #    logger.error(" --trim should not be negative! ")
     #    sys.exit( 1 )
 
     # np # should this be mp? non-negative
     #if options.np <0:
-    #    logging.error(" -m, --multiple-processing should not be negative! ")
+    #    logger.error(" -m, --multiple-processing should not be negative! ")
     #    sys.exit( 1 )
     
-    # verbose 
-    # logging object
-    logging.basicConfig(level=(4-options.verbose)*10,
-                        format='%(levelname)-5s @ %(asctime)s: %(message)s ',
-                        datefmt='%a, %d %b %Y %H:%M:%S',
-                        stream=sys.stderr,
-                        filemode="w"
-                        )
-    
     # min_map_quality non-negative
     #if options.min_map_quality <0:
-    #    logging.error(" -q, --minmapq should not be negative! ")
+    #    logger.error(" -q, --minmapq should not be negative! ")
     #    sys.exit( 1 )
 
     
     return options
```

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/bfc.c` & `MACS3-3.0.0b2/MACS3/fermi-lite/bfc.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/bseq.c` & `MACS3-3.0.0b2/MACS3/fermi-lite/bseq.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/bubble.c` & `MACS3-3.0.0b2/MACS3/fermi-lite/bubble.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/example.c` & `MACS3-3.0.0b2/MACS3/fermi-lite/example.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/fml.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/fml.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/htab.c` & `MACS3-3.0.0b2/MACS3/fermi-lite/htab.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/htab.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/htab.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/khash.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/khash.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/kmer.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/kmer.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/kseq.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/kseq.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/ksort.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/ksort.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/kstring.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/kstring.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/ksw.c` & `MACS3-3.0.0b2/MACS3/fermi-lite/ksw.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/ksw.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/ksw.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/kthread.c` & `MACS3-3.0.0b2/MACS3/fermi-lite/kthread.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/kvec.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/kvec.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/aba.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/aba.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/abd.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/abd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/abdl.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/abdl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/abs.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/abs.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/add.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/add.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/addl.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/addl_high.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addl_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/addlv.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addlv.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/addv.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addv.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/addw.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addw.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/addw_high.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/addw_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/and.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/and.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/bic.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/bic.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/bsl.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/bsl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cagt.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cagt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/ceq.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ceq.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/ceqz.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ceqz.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cge.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cge.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cgez.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cgez.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cgt.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cgt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cgtz.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cgtz.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cle.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cle.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/clez.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/clez.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cls.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cls.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/clt.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/clt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cltz.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cltz.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/clz.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/clz.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cnt.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cnt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/combine.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/combine.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/create.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/create.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/cvt.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/cvt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/dot.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dot.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/dot_lane.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dot_lane.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/dup_lane.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dup_lane.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/dup_n.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/dup_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/eor.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/eor.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/ext.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ext.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/get_high.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/get_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/get_lane.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/get_lane.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/get_low.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/get_low.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/hadd.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/hadd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/hsub.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/hsub.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/ld1.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ld1.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/ld3.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ld3.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/ld4.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/ld4.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/max.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/max.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/maxnm.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/maxnm.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/maxv.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/maxv.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/min.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/min.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/minnm.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/minnm.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/minv.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/minv.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mla.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mla.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mla_n.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mla_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mlal.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlal.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mlal_high.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlal_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mlal_n.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlal_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mls.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mls.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mlsl.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlsl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mlsl_high.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlsl_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mlsl_n.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mlsl_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/movl.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/movl_high.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movl_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/movn.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movn.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/movn_high.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/movn_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mul.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mul.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mul_lane.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mul_lane.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mul_n.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mul_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mull.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mull.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mull_high.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mull_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mull_n.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mull_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/mvn.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/mvn.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/neg.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/neg.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/orn.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/orn.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/orr.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/orr.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/padal.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/padal.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/padd.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/padd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/paddl.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/paddl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/pmax.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/pmax.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/pmin.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/pmin.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qabs.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qabs.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qadd.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qadd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qdmulh.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qdmulh.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qdmull.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qdmull.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qmovn.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qmovn.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qmovn_high.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qmovn_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qmovun.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qmovun.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qneg.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qneg.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qrdmulh.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qrdmulh.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qrdmulh_n.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qrdmulh_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qshl.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qshl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qsub.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qsub.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qtbl.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qtbl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/qtbx.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/qtbx.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rbit.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rbit.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/reinterpret.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/reinterpret.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rev16.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rev16.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rev32.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rev32.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rev64.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rev64.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rhadd.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rhadd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rnd.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rnd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rshl.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rshl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rshr_n.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rshr_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/rsra_n.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/rsra_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/set_lane.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/set_lane.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/shl.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/shl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/shl_n.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/shl_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/shr_n.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/shr_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/sra_n.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/sra_n.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/st1.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st1.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/st1_lane.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st1_lane.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/st3.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st3.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/st4.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/st4.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/sub.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/sub.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/subl.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/subl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/subw.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/subw.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/subw_high.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/subw_high.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/tbl.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/tbl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/tbx.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/tbx.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/trn.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/trn.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/trn1.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/trn1.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/trn2.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/trn2.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/tst.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/tst.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/types.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/types.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/uqadd.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uqadd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/uzp.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uzp.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/uzp1.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uzp1.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/uzp2.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/uzp2.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/zip.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/zip.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/zip1.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/zip1.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon/zip2.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon/zip2.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/arm/neon.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/arm/neon.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/check.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/check.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/debug-trap.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/debug-trap.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/hedley.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/hedley.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-align.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-align.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-arch.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-arch.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-common.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-common.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-constify.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-constify.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-detect-clang.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-detect-clang.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-diagnostic.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-diagnostic.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-features.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-features.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/simde-math.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/simde-math.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx2.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx2.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/2intersect.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/2intersect.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/abs.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/abs.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/add.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/add.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/adds.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/adds.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/and.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/and.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/andnot.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/andnot.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/avg.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/avg.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/blend.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/blend.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/broadcast.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/broadcast.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cast.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cast.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cmp.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmp.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cmpeq.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmpeq.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cmpge.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmpge.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cmpgt.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmpgt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cmple.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmple.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cmplt.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cmplt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/copysign.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/copysign.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cvt.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cvt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/cvts.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/cvts.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/div.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/div.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/extract.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/extract.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/fmadd.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fmadd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/fmsub.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fmsub.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/fnmadd.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fnmadd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/fnmsub.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/fnmsub.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/insert.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/insert.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/kshift.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/kshift.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/load.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/load.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/loadu.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/loadu.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/lzcnt.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/lzcnt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/madd.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/madd.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/maddubs.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/maddubs.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/max.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/max.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/min.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/min.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/mov.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mov.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/mov_mask.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mov_mask.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/movm.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/movm.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/mul.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mul.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/mulhi.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mulhi.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/mulhrs.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mulhrs.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/mullo.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/mullo.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/negate.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/negate.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/or.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/or.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/packs.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/packs.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/packus.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/packus.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/permutex2var.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/permutex2var.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/permutexvar.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/permutexvar.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/sad.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sad.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/set.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/set.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/set1.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/set1.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/set4.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/set4.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/setone.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setone.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/setr.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setr.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/setr4.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setr4.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/setzero.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/setzero.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/shuffle.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/shuffle.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/sll.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sll.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/slli.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/slli.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/sllv.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sllv.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/sqrt.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sqrt.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/sra.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sra.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/srai.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srai.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/srav.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srav.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/srl.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srl.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/srli.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srli.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/srlv.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/srlv.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/store.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/store.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/storeu.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/storeu.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/sub.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/sub.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/subs.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/subs.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/test.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/test.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/types.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/types.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/unpackhi.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/unpackhi.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/unpacklo.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/unpacklo.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/xor.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/xor.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512/xorsign.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512/xorsign.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/avx512.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/avx512.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/clmul.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/clmul.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/fma.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/fma.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/gfni.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/gfni.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/mmx.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/mmx.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/sse.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/sse2.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse2.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/sse3.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse3.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/sse4.1.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse4.1.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/sse4.2.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/sse4.2.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/ssse3.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/ssse3.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/lib/x86/svml.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/lib/x86/svml.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/mag.c` & `MACS3-3.0.0b2/MACS3/fermi-lite/mag.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/mag.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/mag.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/misc.c` & `MACS3-3.0.0b2/MACS3/fermi-lite/misc.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/mrope.c` & `MACS3-3.0.0b2/MACS3/fermi-lite/mrope.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/mrope.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/mrope.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/rld0.c` & `MACS3-3.0.0b2/MACS3/fermi-lite/rld0.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/rld0.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/rld0.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/rle.c` & `MACS3-3.0.0b2/MACS3/fermi-lite/rle.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/rle.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/rle.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/rope.c` & `MACS3-3.0.0b2/MACS3/fermi-lite/rope.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/rope.h` & `MACS3-3.0.0b2/MACS3/fermi-lite/rope.h`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3/fermi-lite/unitig.c` & `MACS3-3.0.0b2/MACS3/fermi-lite/unitig.c`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/MACS3.egg-info/PKG-INFO` & `MACS3-3.0.0b2/MACS3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: MACS3
-Version: 3.0.0b1
+Version: 3.0.0b2
 Summary: Model Based Analysis for ChIP-Seq data
 Home-page: http://github.com/macs3-project/MACS/
 Author: Tao Liu
 Author-email: vladimir.liu@gmail.com
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Cython
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MACS: Model-based Analysis for ChIP-Seq
 
 ![Status](https://img.shields.io/pypi/status/macs3.svg) ![License](https://img.shields.io/github/license/macs3-project/MACS) ![Programming languages](https://img.shields.io/github/languages/top/macs3-project/MACS) ![CI x64](https://github.com/macs3-project/MACS/workflows/CI%20x64/badge.svg) ![CI non x64](https://github.com/macs3-project/MACS/workflows/CI%20non%20x64,%20python%203.7/badge.svg)
 
@@ -48,44 +48,36 @@
 position and orientation. MACS can be easily used for ChIP-Seq data
 alone, or with a control sample with the increase of
 specificity. Moreover, as a general peak-caller, MACS can also be
 applied to any "DNA enrichment assays" if the question to be asked is
 simply: *where we can find significant reads coverage than the random
 background*.
 
-**Please note that current MACS3 is still in alpha stage. However, we
+**Please note that current MACS3 is still in beta stage. However, we
 utilize Github Action to implement the CI (Continous Integration) to
 make sure that the main branch passes unit testing on certain
 functions and subcommands to reproduce the correct outputs. We will
 add more new features in the future.**
 
-## Recent Changes for MACS (3.0.0b1)
+## Recent Changes for MACS (3.0.0b2)
 
-### 3.0.0b1
-        The first beta version of MACS3, with HMMRATAC feature recently added.
+### 3.0.0b2
+    The second beta version of MACS3, with HMMRATAC feature refined.
 	   
-	* New features from alpha7:
-
-	1) HMMRATAC module is added
-	HMMRATAC is a dedicated software to analyze ATAC-seq data. The
-	basic idea behind HMMRATAC is to digest ATAC-seq data according to
-	the fragment length of read pairs into four signal tracks: short
-	fragments, mononucleosomal fragments, di-nucleosomal fragments and
-	tri-nucleosomal fragments. Then integrate the four tracks again
-	using Hidden Markov Model to consider three hidden states: open
-	region, nucleosomal region, and background region. The orginal
-	paper was published in 2019 written in JAVA, by Evan Tarbell. We
-	implemented it in Python/Cython and optimize the whole process
-	using existing MACS functions and hmmlearn. Now it can run much
-	faster than the original JAVA version. Note: evaluation of the
-	peak calling results is underway.
-	
-	2) Multiple updates regarding dependencies, anaconda built, CI/CD
-	process.
+	* New features from beta1:
 
+	1) HMMRATAC module fixes
+    
+       Cutoff analysis function added
+       Description regarding it has been added
+    
+    2) Memory monitoring in the runtime message
+    
+    3) testing for s390x, armv7 and power64le is back. However, we turned off the function to check if the `hmmratac` results from non-x86 architectures are the same as the standard results, because in order to let the testing run, we need to use old python libraries (scipy and sklearn) through the distribution of Debian/Linux bullseye.
+    
 ## Install
 
 The common way to install MACS is through
 [PYPI](https://pypi.org/project/macs3/)) or
 [conda](https://anaconda.org/bioconda/macs3). Please check the
 [INSTALL](./docs/INSTALL.md) document for detail.
 
@@ -108,15 +100,15 @@
 
 `macs3 callpeak -t ChIP.bam -c Control.bam --broad -g hs --broad-cutoff 0.1`
 
 Example for peak calling on ATAC-seq (paired-end mode):
 
 `macs3 callpeak -f BAMPE -t ATAC.bam -g hs -n test -B -q 0.01`
 
-There are currently twelve functions available in MAC3 serving as
+There are currently 14 functions available in MACS3 serving as
 sub-commands. Please click on the link to see the detail description
 of the subcommands.
 
 Subcommand | Description
 -----------|----------
 [`callpeak`](./docs/callpeak.md) | Main MACS3 Function to call peaks from alignment results.
 [`bdgpeakcall`](./docs/bdgpeakcall.md) | Call peaks from bedGraph output.
```

### Comparing `MACS3-3.0.0b1/MACS3.egg-info/SOURCES.txt` & `MACS3-3.0.0b2/MACS3.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 MACS3/Signal/__init__.py
 MACS3/Signal/cPosValCalculation.c
 MACS3/Signal/cPosValCalculation.h
 MACS3/Signal/cPosValCalculation.pxd
 MACS3/Signal/swalign.c
 MACS3/Signal/swalign.h
 MACS3/Utilities/Constants.py
+MACS3/Utilities/Logger.py
 MACS3/Utilities/OptValidator.py
 MACS3/Utilities/__init__.py
 MACS3/fermi-lite/bfc.c
 MACS3/fermi-lite/bseq.c
 MACS3/fermi-lite/bubble.c
 MACS3/fermi-lite/example.c
 MACS3/fermi-lite/fml.h
```

### Comparing `MACS3-3.0.0b1/PKG-INFO` & `MACS3-3.0.0b2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: MACS3
-Version: 3.0.0b1
+Version: 3.0.0b2
 Summary: Model Based Analysis for ChIP-Seq data
 Home-page: http://github.com/macs3-project/MACS/
 Author: Tao Liu
 Author-email: vladimir.liu@gmail.com
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Cython
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MACS: Model-based Analysis for ChIP-Seq
 
 ![Status](https://img.shields.io/pypi/status/macs3.svg) ![License](https://img.shields.io/github/license/macs3-project/MACS) ![Programming languages](https://img.shields.io/github/languages/top/macs3-project/MACS) ![CI x64](https://github.com/macs3-project/MACS/workflows/CI%20x64/badge.svg) ![CI non x64](https://github.com/macs3-project/MACS/workflows/CI%20non%20x64,%20python%203.7/badge.svg)
 
@@ -48,44 +48,36 @@
 position and orientation. MACS can be easily used for ChIP-Seq data
 alone, or with a control sample with the increase of
 specificity. Moreover, as a general peak-caller, MACS can also be
 applied to any "DNA enrichment assays" if the question to be asked is
 simply: *where we can find significant reads coverage than the random
 background*.
 
-**Please note that current MACS3 is still in alpha stage. However, we
+**Please note that current MACS3 is still in beta stage. However, we
 utilize Github Action to implement the CI (Continous Integration) to
 make sure that the main branch passes unit testing on certain
 functions and subcommands to reproduce the correct outputs. We will
 add more new features in the future.**
 
-## Recent Changes for MACS (3.0.0b1)
+## Recent Changes for MACS (3.0.0b2)
 
-### 3.0.0b1
-        The first beta version of MACS3, with HMMRATAC feature recently added.
+### 3.0.0b2
+    The second beta version of MACS3, with HMMRATAC feature refined.
 	   
-	* New features from alpha7:
-
-	1) HMMRATAC module is added
-	HMMRATAC is a dedicated software to analyze ATAC-seq data. The
-	basic idea behind HMMRATAC is to digest ATAC-seq data according to
-	the fragment length of read pairs into four signal tracks: short
-	fragments, mononucleosomal fragments, di-nucleosomal fragments and
-	tri-nucleosomal fragments. Then integrate the four tracks again
-	using Hidden Markov Model to consider three hidden states: open
-	region, nucleosomal region, and background region. The orginal
-	paper was published in 2019 written in JAVA, by Evan Tarbell. We
-	implemented it in Python/Cython and optimize the whole process
-	using existing MACS functions and hmmlearn. Now it can run much
-	faster than the original JAVA version. Note: evaluation of the
-	peak calling results is underway.
-	
-	2) Multiple updates regarding dependencies, anaconda built, CI/CD
-	process.
+	* New features from beta1:
 
+	1) HMMRATAC module fixes
+    
+       Cutoff analysis function added
+       Description regarding it has been added
+    
+    2) Memory monitoring in the runtime message
+    
+    3) testing for s390x, armv7 and power64le is back. However, we turned off the function to check if the `hmmratac` results from non-x86 architectures are the same as the standard results, because in order to let the testing run, we need to use old python libraries (scipy and sklearn) through the distribution of Debian/Linux bullseye.
+    
 ## Install
 
 The common way to install MACS is through
 [PYPI](https://pypi.org/project/macs3/)) or
 [conda](https://anaconda.org/bioconda/macs3). Please check the
 [INSTALL](./docs/INSTALL.md) document for detail.
 
@@ -108,15 +100,15 @@
 
 `macs3 callpeak -t ChIP.bam -c Control.bam --broad -g hs --broad-cutoff 0.1`
 
 Example for peak calling on ATAC-seq (paired-end mode):
 
 `macs3 callpeak -f BAMPE -t ATAC.bam -g hs -n test -B -q 0.01`
 
-There are currently twelve functions available in MAC3 serving as
+There are currently 14 functions available in MACS3 serving as
 sub-commands. Please click on the link to see the detail description
 of the subcommands.
 
 Subcommand | Description
 -----------|----------
 [`callpeak`](./docs/callpeak.md) | Main MACS3 Function to call peaks from alignment results.
 [`bdgpeakcall`](./docs/bdgpeakcall.md) | Call peaks from bedGraph output.
```

### Comparing `MACS3-3.0.0b1/README.md` & `MACS3-3.0.0b2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,44 +24,36 @@
 position and orientation. MACS can be easily used for ChIP-Seq data
 alone, or with a control sample with the increase of
 specificity. Moreover, as a general peak-caller, MACS can also be
 applied to any "DNA enrichment assays" if the question to be asked is
 simply: *where we can find significant reads coverage than the random
 background*.
 
-**Please note that current MACS3 is still in alpha stage. However, we
+**Please note that current MACS3 is still in beta stage. However, we
 utilize Github Action to implement the CI (Continous Integration) to
 make sure that the main branch passes unit testing on certain
 functions and subcommands to reproduce the correct outputs. We will
 add more new features in the future.**
 
-## Recent Changes for MACS (3.0.0b1)
+## Recent Changes for MACS (3.0.0b2)
 
-### 3.0.0b1
-        The first beta version of MACS3, with HMMRATAC feature recently added.
+### 3.0.0b2
+    The second beta version of MACS3, with HMMRATAC feature refined.
 	   
-	* New features from alpha7:
-
-	1) HMMRATAC module is added
-	HMMRATAC is a dedicated software to analyze ATAC-seq data. The
-	basic idea behind HMMRATAC is to digest ATAC-seq data according to
-	the fragment length of read pairs into four signal tracks: short
-	fragments, mononucleosomal fragments, di-nucleosomal fragments and
-	tri-nucleosomal fragments. Then integrate the four tracks again
-	using Hidden Markov Model to consider three hidden states: open
-	region, nucleosomal region, and background region. The orginal
-	paper was published in 2019 written in JAVA, by Evan Tarbell. We
-	implemented it in Python/Cython and optimize the whole process
-	using existing MACS functions and hmmlearn. Now it can run much
-	faster than the original JAVA version. Note: evaluation of the
-	peak calling results is underway.
-	
-	2) Multiple updates regarding dependencies, anaconda built, CI/CD
-	process.
+	* New features from beta1:
 
+	1) HMMRATAC module fixes
+    
+       Cutoff analysis function added
+       Description regarding it has been added
+    
+    2) Memory monitoring in the runtime message
+    
+    3) testing for s390x, armv7 and power64le is back. However, we turned off the function to check if the `hmmratac` results from non-x86 architectures are the same as the standard results, because in order to let the testing run, we need to use old python libraries (scipy and sklearn) through the distribution of Debian/Linux bullseye.
+    
 ## Install
 
 The common way to install MACS is through
 [PYPI](https://pypi.org/project/macs3/)) or
 [conda](https://anaconda.org/bioconda/macs3). Please check the
 [INSTALL](./docs/INSTALL.md) document for detail.
 
@@ -84,15 +76,15 @@
 
 `macs3 callpeak -t ChIP.bam -c Control.bam --broad -g hs --broad-cutoff 0.1`
 
 Example for peak calling on ATAC-seq (paired-end mode):
 
 `macs3 callpeak -f BAMPE -t ATAC.bam -g hs -n test -B -q 0.01`
 
-There are currently twelve functions available in MAC3 serving as
+There are currently 14 functions available in MACS3 serving as
 sub-commands. Please click on the link to see the detail description
 of the subcommands.
 
 Subcommand | Description
 -----------|----------
 [`callpeak`](./docs/callpeak.md) | Main MACS3 Function to call peaks from alignment results.
 [`bdgpeakcall`](./docs/bdgpeakcall.md) | Call peaks from bedGraph output.
```

### Comparing `MACS3-3.0.0b1/bin/macs3` & `MACS3-3.0.0b2/bin/macs3`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Time-stamp: <2022-10-04 13:48:15 Tao Liu>
+# Time-stamp: <2023-06-23 12:59:17 Tao Liu>
 
 """Description: MACS v3 main executable.
 
 This code is free software; you can redistribute it and/or modify it
 under the terms of the BSD License (see the file LICENSE included with
 the distribution).
 """
@@ -115,15 +115,15 @@
 
     """
     description = "%(prog)s -- Model-based Analysis for ChIP-Sequencing"
     epilog = "For command line options of each command, type: %(prog)s COMMAND -h"
     # top-level parser
     argparser = ap.ArgumentParser( description = description, epilog = epilog ) #, usage = usage )
     argparser.add_argument("--version", action="version", version="%(prog)s "+MACS_VERSION)
-    subparsers = argparser.add_subparsers( dest = 'subcommand' ) #help="sub-command help")
+    subparsers = argparser.add_subparsers( dest = 'subcommand' )
     subparsers.required = True
 
     # command for 'callpeak'
     add_callpeak_parser( subparsers )
 
     # # command for 'diffpeak'
     # add_diffpeak_parser( subparsers )
@@ -293,25 +293,26 @@
     postprocess_group = group_postprocessing.add_mutually_exclusive_group()
 
     postprocess_group.add_argument( "--call-summits", dest="call_summits", action="store_true",
                                     help="If set, MACS will use a more sophisticated signal processing approach to find subpeak summits in each enriched peak region. DEFAULT: False",default=False)
     group_postprocessing.add_argument( "--fe-cutoff", dest="fecutoff", type=float, default = 1.0,
                                        help = "When set, the value will be used as the minimum requirement to filter out peaks with low fold-enrichment. Note, MACS3 adds one as pseudocount while calculating fold-enrichment. By default, it is set as 1 so there is no filtering. DEFAULT: 1.0")
 
+    # obsolete options
+    group_obsolete = argparser_callpeak.add_argument_group( "Obsolete options" )
+    group_obsolete.add_argument( "--to-large", dest = "tolarge", action = "store_true", default = False,
+                                 help = "Obsolete option. Please use '--scale-to large' instead." )
+    group_obsolete.add_argument( "--ratio", dest = "ratio", type = float, default = 1.0,
+                                 help = "Obsolete option. Originally designed to normalize treatment and control with customized ratio, now it won't have any effect." )
+
     # other options
     group_other = argparser_callpeak.add_argument_group( "Other options" )
     group_other.add_argument( "--buffer-size", dest = "buffer_size", type = int, default = "100000",
                                   help = "Buffer size for incrementally increasing internal array size to store reads alignment information. In most cases, you don't have to change this parameter. However, if there are large number of chromosomes/contigs/scaffolds in your alignment, it's recommended to specify a smaller buffer size in order to decrease memory usage (but it will take longer time to read alignment files). Minimum memory requested for reading an alignment file is about # of CHROMOSOME * BUFFER_SIZE * 8 Bytes. DEFAULT: 100000 " )
 
-    # obsolete options
-    group_obsolete = argparser_callpeak.add_argument_group( "Obsolete options" )
-    group_obsolete.add_argument( "--to-large", dest = "tolarge", action = "store_true", default = False,
-                                     help = "Obsolete option. Please use '--scale-to large' instead." )
-    group_obsolete.add_argument( "--ratio", dest = "ratio", type = float, default = 1.0,
-                                     help = "Obsolete option. Originally designed to normalize treatment and control with customized ratio, now it won't have any effect." )
     return
 
 def add_diffpeak_parser( subparsers ):
     """Add main function 'peak calling' argument parsers.
     """
     argparser_diffpeak = subparsers.add_parser("diffpeak", help="MACS3 Differential Peak Function: Call peaks from bedgraphs (or use optional peak regions) and determine peaks of differential occupancy")
 
@@ -416,14 +417,16 @@
                                        help = "maximum gap between significant points in a peak, better to set it as tag size. DEFAULT: 30", default = 30 )
     argparser_bdgpeakcall.add_argument( "--call-summits", dest="call_summits", action="store_true", help=ap.SUPPRESS, default=False)
 #                         help="If set, MACS will use a more sophisticated approach to find all summits in each enriched peak region. DEFAULT: False",default=False)
     argparser_bdgpeakcall.add_argument( "--cutoff-analysis", dest="cutoff_analysis", action="store_true",
                                         help = "While set, bdgpeakcall will analyze number or total length of peaks that can be called by different cutoff then output a summary table to help user decide a better cutoff. Note, minlen and maxgap may affect the results. DEFAULT: False", default = False )
     argparser_bdgpeakcall.add_argument("--no-trackline", dest="trackline", action="store_false", default=True,
                          help="Tells MACS not to include trackline with bedGraph files. The trackline is required by UCSC.")
+    argparser_bdgpeakcall.add_argument( "--verbose", dest = "verbose", type = int, default = 2,
+                                        help = "Set verbose level of runtime message. 0: only show critical message, 1: show additional warning message, 2: show process information, 3: show debug messages. DEFAULT:2" )
 
     add_outdir_option( argparser_bdgpeakcall )
     add_output_group( argparser_bdgpeakcall )
 
     return
 
 def add_bdgbroadcall_parser( subparsers ):
@@ -442,14 +445,16 @@
                                          help = "minimum length of peak, better to set it as d value. DEFAULT: 200", default = 200 )
     argparser_bdgbroadcall.add_argument( "-g", "--lvl1-max-gap", dest = "lvl1maxgap", type = int,
                                          help = "maximum gap between significant peaks, better to set it as tag size. DEFAULT: 30", default = 30 )
     argparser_bdgbroadcall.add_argument( "-G", "--lvl2-max-gap", dest = "lvl2maxgap", type = int,
                                          help = "maximum linking between significant peaks, better to set it as 4 times of d value. DEFAULT: 800", default = 800)
     argparser_bdgbroadcall.add_argument("--no-trackline", dest="trackline", action="store_false", default=True,
                                          help="Tells MACS not to include trackline with bedGraph files. The trackline is required by UCSC.")
+    argparser_bdgbroadcall.add_argument( "--verbose", dest = "verbose", type = int, default = 2,
+                                         help = "Set verbose level of runtime message. 0: only show critical message, 1: show additional warning message, 2: show process information, 3: show debug messages. DEFAULT:2" )
     add_outdir_option( argparser_bdgbroadcall )
     add_output_group( argparser_bdgbroadcall )
     return
 
 def add_bdgcmp_parser( subparsers ):
     """Add function 'peak calling on bedGraph' argument parsers.
     """
@@ -463,14 +468,16 @@
                                    help = "Scaling factor for treatment and control track. Keep it as 1.0 or default in most cases. Set it ONLY while you have SPMR output from MACS3 callpeak, and plan to calculate scores as MACS3 callpeak module. If you want to simulate 'callpeak' w/o '--to-large', calculate effective smaller sample size after filtering redudant reads in million (e.g., put 31.415926 if effective reads are 31,415,926) and input it for '-S'; for 'callpeak --to-large', calculate effective reads in larger sample. DEFAULT: 1.0")
     argparser_bdgcmp.add_argument( "-p", "--pseudocount", dest = "pseudocount", type = float, default = 0.0,
                                    help = "The pseudocount used for calculating logLR, logFE or FE. The count will be applied after normalization of sequencing depth. DEFAULT: 0.0, no pseudocount is applied.")
 
     argparser_bdgcmp.add_argument( "-m", "--method", dest = "method", type = str, nargs = "+",
                                    choices = ( "ppois", "qpois", "subtract", "logFE", "FE", "logLR", "slogLR", "max" ),
                                    help = "Method to use while calculating a score in any bin by comparing treatment value and control value. Available choices are: ppois, qpois, subtract, logFE, logLR, and slogLR. They represent Poisson Pvalue (-log10(pvalue) form) using control as lambda and treatment as observation, q-value through a BH process for poisson pvalues, subtraction from treatment, linear scale fold enrichment, log10 fold enrichment(need to set pseudocount), log10 likelihood between ChIP-enriched model and open chromatin model(need to set pseudocount), symmetric log10 likelihood between two ChIP-enrichment models, or maximum value between the two tracks. Default option is ppois.",default="ppois")
+    argparser_bdgcmp.add_argument( "--verbose", dest = "verbose", type = int, default = 2,
+                                   help = "Set verbose level of runtime message. 0: only show critical message, 1: show additional warning message, 2: show process information, 3: show debug messages. DEFAULT:2" )
 
     add_outdir_option( argparser_bdgcmp )
     output_group = argparser_bdgcmp.add_mutually_exclusive_group( required = True )
     output_group.add_argument( "--o-prefix", dest = "oprefix", type = str,
                                help = "The PREFIX of output bedGraph file to write scores. If it is given as A, and method is 'ppois', output file will be A_ppois.bdg. Mutually exclusive with -o/--ofile." )
     output_group.add_argument( "-o", "--ofile", dest = "ofile", type = str, nargs = "+",
                                help = "Output filename. Mutually exclusive with --o-prefix. The number and the order of arguments for --ofile must be the same as for -m." )
@@ -487,14 +494,16 @@
                                    choices = ( "multiply", "add", "p2q", "max", "min" ),
                                    help = "Method to modify the score column of bedGraph file. Available choices are: multiply, add, max, min, or p2q. 1) multiply, the EXTRAPARAM is required and will be multiplied to the score column. If you intend to divide the score column by X, use value of 1/X as EXTRAPARAM. 2) add, the EXTRAPARAM is required and will be added to the score column. If you intend to subtract the score column by X, use value of -X as EXTRAPARAM. 3) max, the EXTRAPARAM is required and will take the maximum value between score and the EXTRAPARAM. 4) min, the EXTRAPARAM is required and will take the minimum value between score and the EXTRAPARAM. 5) p2q, this will convert p-value scores to q-value scores using Benjamini-Hochberg process. The EXTRAPARAM is not required. This method assumes the scores are -log10 p-value from MACS3. Any other types of score will cause unexpected errors.", default="p2q")
     argparser_bdgopt.add_argument( "-p", "--extra-param", dest = "extraparam", type = float, nargs = "*",
                                    help = "The extra parameter for METHOD. Check the detail of -m option.")
     add_outdir_option( argparser_bdgopt )
     argparser_bdgopt.add_argument( "-o", "--ofile", dest = "ofile", type = str,
                                    help = "Output BEDGraph filename.", required = True )
+    argparser_bdgopt.add_argument( "--verbose", dest = "verbose", type = int, default = 2,
+                                   help = "Set verbose level of runtime message. 0: only show critical message, 1: show additional warning message, 2: show process information, 3: show debug messages. DEFAULT:2" )
     return
 
 def add_cmbreps_parser( subparsers ):
     """Add function 'combine replicates' argument parsers.
     """
     argparser_cmbreps = subparsers.add_parser( "cmbreps",
                                                help = "Combine BEDGraphs of scores from replicates. Note: All regions on the same chromosome in the bedGraph file should be continuous so only bedGraph files from MACS3 are accpetable." )
@@ -504,14 +513,16 @@
     #                                 help = "Weight for each replicate. Default is 1.0 for each. When given, require same number of parameters as IFILE." )
     argparser_cmbreps.add_argument( "-m", "--method", dest = "method", type = str,
                                     choices = ( "fisher", "max", "mean" ),
                                     help = "Method to use while combining scores from replicates. 1) fisher: Fisher's combined probability test. It requires scores in ppois form (-log10 pvalues) from bdgcmp. Other types of scores for this method may cause cmbreps unexpected errors. 2) max: take the maximum value from replicates for each genomic position. 3) mean: take the average value. Note, except for Fisher's method, max or mean will take scores AS IS which means they won't convert scores from log scale to linear scale or vice versa.", default="fisher")
     add_outdir_option( argparser_cmbreps )
     argparser_cmbreps.add_argument( "-o", "--ofile", dest = "ofile", type = str, required = True,
                                     help = "Output BEDGraph filename for combined scores." )
+    argparser_cmbreps.add_argument( "--verbose", dest = "verbose", type = int, default = 2,
+                                    help = "Set verbose level of runtime message. 0: only show critical message, 1: show additional warning message, 2: show process information, 3: show debug messages. DEFAULT:2" )
     return
 
 def add_randsample_parser( subparsers ):
     argparser_randsample = subparsers.add_parser( "randsample",
                                                   help = "Randomly sample number/percentage of total reads." )
     argparser_randsample.add_argument( "-i", "--ifile", dest = "ifile", type = str, required = True, nargs = "+",
                                       help = "Alignment file. If multiple files are given as '-t A B C', then they will all be read and combined. Note that pair-end data is not supposed to work with this command. REQUIRED." )
@@ -557,15 +568,17 @@
                                     help = "Minimum length of differential region. Try bigger value to remove small regions. DEFAULT: 200", default = 200 )
     argparser_bdgdiff.add_argument( "-g", "--max-gap", dest = "maxgap", type = int,
                                     help = "Maximum gap to merge nearby differential regions. Consider a wider gap for broad marks. Maximum gap should be smaller than minimum length (-g). DEFAULT: 100", default = 100 )
     argparser_bdgdiff.add_argument( "--d1", "--depth1", dest = "depth1", type = float, default = 1.0,
                                     help = "Sequencing depth (# of non-redundant reads in million) for condition 1. It will be used together with --d2. See description for --d2 below for how to assign them. Default: 1" )
     argparser_bdgdiff.add_argument( "--d2", "--depth2", dest = "depth2", type = float, default = 1.0,
                                     help = "Sequencing depth (# of non-redundant reads in million) for condition 2. It will be used together with --d1. DEPTH1 and DEPTH2 will be used to calculate scaling factor for each sample, to down-scale larger sample to the level of smaller one. For example, while comparing 10 million condition 1 and 20 million condition 2, use --d1 10 --d2 20, then pileup value in bedGraph for condition 2 will be divided by 2. Default: 1" )
-
+    argparser_bdgdiff.add_argument( "--verbose", dest = "verbose", type = int, default = 2,
+                                    help = "Set verbose level of runtime message. 0: only show critical message, 1: show additional warning message, 2: show process information, 3: show debug messages. DEFAULT:2" )
+    
     add_outdir_option( argparser_bdgdiff )
     output_group = argparser_bdgdiff.add_mutually_exclusive_group( required = True )
     output_group.add_argument( "--o-prefix", dest = "oprefix", type = str,
                                help = "Output file prefix. Actual files will be named as PREFIX_cond1.bed, PREFIX_cond2.bed and PREFIX_common.bed. Mutually exclusive with -o/--ofile." )
     output_group.add_argument( "-o", "--ofile", dest = "ofile", type = str, nargs = 3,
                                help = "Output filenames. Must give three arguments in order: 1. file for unique regions in condition 1; 2. file for unique regions in condition 2; 3. file for common regions in both conditions. Note: mutually exclusive with --o-prefix." )
 
@@ -650,15 +663,15 @@
 
     argparser_pileup.add_argument( "--extsize", dest = "extsize", type = int, default = 200,
                                    help = "The extension size in bps. Each alignment read will become a EXTSIZE of fragment, then be piled up. Check description for -B for detail. It's twice the `shiftsize` in old MACSv1 language. This option will be ignored when the format is set as BAMPE or BEDPE. DEFAULT: 200 " )
     argparser_pileup.add_argument( "--buffer-size", dest = "buffer_size", type = int, default = "100000",
                                    help = "Buffer size for incrementally increasing internal array size to store reads alignment information. In most cases, you don't have to change this parameter. However, if there are large number of chromosomes/contigs/scaffolds in your alignment, it's recommended to specify a smaller buffer size in order to decrease memory usage (but it will take longer time to read alignment files). Minimum memory requested for reading an alignment file is about # of CHROMOSOME * BUFFER_SIZE * 8 Bytes. DEFAULT: 100000 " )
 
     argparser_pileup.add_argument( "--verbose", dest = "verbose", type = int, default = 2,
-                                      help = "Set verbose level. 0: only show critical message, 1: show additional warning message, 2: show process information, 3: show debug messages. If you want to know where are the duplicate reads, use 3. DEFAULT:2" )
+                                   help = "Set verbose level. 0: only show critical message, 1: show additional warning message, 2: show process information, 3: show debug messages. If you want to know where are the duplicate reads, use 3. DEFAULT:2" )
     return
 
 def add_callvar_parser( subparsers ):
     """Add function 'variant calling' argument parsers. From SAPPER package
     """
     argparser_callvar = subparsers.add_parser("callvar",
                                               formatter_class = ap.RawDescriptionHelpFormatter,
@@ -729,27 +742,158 @@
 
 def add_hmmratac_parser( subparsers ):
     """Add function 'HMMRATAC' argument parsers. From SAPPER package
     """
     argparser_hmmratac = subparsers.add_parser("hmmratac",
                                                 formatter_class = ap.RawDescriptionHelpFormatter,
                                                 help="Dedicated peak calling based on Hidden Markov Model for ATAC-seq data.",
-                                                epilog = "TBA...")
+                                                epilog = """HMMRATAC is a dedicated tool for processing ATAC-seq data
+
+HMMRATAC, first released as a JAVA program in 2019, is a dedicated
+tool specifically designed for processing ATAC-seq data. In MACS3, it
+has been integrated as a subcommand (`hmmratac`). Reimagined and
+rewritten in Python and Cython, this tool's functionality might vary
+from its JAVA version. The core principle of HMMRATAC involves
+utilizing the Hidden Markov Model to learn the nucleosome structure
+around open chromatin regions.
+
+Here's an example of how to run the `hmmratac` command:
+
+```
+$ macs3 hmmratac -b test/yeast_500k_SRR1822137.bam -n hmmratac_yeast500k
+```
+
+Before proceeding, it's essential to carefully read the help messages
+concerning each option and the default parameters. There are several
+crucial parameters we usually need to specify:
+
+1. Lower cutoff to select training regions through `-l`.
+2. Upper cutoff to select training regions through `-u`.
+3. Pre-scanning cutoff to select candidate regions for
+   decoding/predicting the states, including open, nucleosome, and
+   background states, through `-c`.
+
+These three parameters can significantly influence the
+results. Therefore, it's highly recommended to run `macs3 hmmratac
+--cutoff-analysis-only -b your.bam` first, which will help you decide
+the parameters for `-l`, `-u`, and `-c`. Since there isn't an
+automatic way to determine these parameters, your judgement will be
+vital. Please read the output from `macs3 hmmratac
+--cutoff-analysis-only -b your.bam` and the following section `Choices
+of cutoff values` for guidance.
+
+* Choices of cutoff values *
+
+Before you proceed, it's highly recommended to run with
+`--cutoff-analysis-only` for the initial attempt. When this option is
+activated, `hmmratac` will use EM to estimate the best parameters for
+fragment sizes of short fragments, mono-, di-, and tri-nucleosomes,
+pileup fragments, convert the pileup values into fold-change, and
+analyze each possible cutoff. This analysis includes the number of
+peaks that can be called, their average peak length, and their total
+length. After the report is generated, you can review its contents and
+decide on the optimal `-l`, `-u`, and `-c`.
+
+The report consists of four columns:
+
+1. score: the possible fold change cutoff value.
+2. npeaks: the number of peaks under this cutoff.
+3. lpeaks: the total length of all peaks.
+4. avelpeak: the average length of peaks.
+
+While there's no universal rule, here are a few suggestions:
+
+- The lower cutoff should be the cutoff in the report that captures a
+  moderate number (about 10k-30k) of peaks with a normal width (average
+  length 500-1000bps long).
+- The upper cutoff should capture some (typically hundreds of)
+  extremely high enrichment and unusually wide peaks in the
+  report. The aim here is to exclude abnormal enrichment caused by
+  artifacts such as repetitive regions.
+- The pre-scanning cutoff should be the cutoff close to the BOTTOM of
+  the report that can capture a large number of potential peaks with a
+  normal length (average length 500-1000bps). However, it's
+  recommended not to use the lowest cutoff value in the report as this
+  may include too much noise from the genome.
+  
+* Tune the HMM model *
+
+It's highly recommended to check the runtime message of the HMM model
+after training. An example is like this:
+
+```
+#4 Train Hidden Markov Model with Multivariate Gaussian Emission
+#  Extract signals in training regions with bin size of 10
+#  Use Baum-Welch algorithm to train the HMM
+#   HMM converged: True
+#  Write HMM parameters into JSON: test_model.json
+#  The Hidden Markov Model for signals of binsize of 10 basepairs:
+#   open state index: state2
+#   nucleosomal state index: state1
+#   background state index: state0
+#   Starting probabilities of states:
+#                            bg        nuc       open
+#                        0.7994     0.1312    0.06942
+#   HMM Transition probabilities:
+#                            bg        nuc       open
+#               bg->     0.9842    0.01202   0.003759
+#              nuc->    0.03093     0.9562    0.01287
+#             open->   0.007891    0.01038     0.9817
+#   HMM Emissions (mean):
+#                         short       mono         di        tri
+#               bg:      0.2551      1.526     0.4646    0.07071
+#              nuc:       6.538      17.94      3.422    0.05819
+#             open:       5.016      17.47      6.897      2.121
+```
+
+We will 'guess' which hidden state is for the open region, which is
+the nucleosomal region, and which is the background. We compute from
+the HMM Emission matrix to pick the state with the highest sum of mean
+signals as the open state, the lowest as the backgound state, then the
+rest is the nucleosomal state. However it may not work in every
+case. In the above example, it may be tricky to call the second row as
+'nuc' and the third as 'open'. If the users want to exchange the state
+assignments of the 'nuc' and 'open', they can modify the state
+assignment in the HMM model file (e.g. test_model.json). For the above
+example, the model.json looks like this (we skipped some detail):
+
+```
+{"startprob": [...], "transmat": [...], "means": [...], "covars": [...], 
+"covariance_type": "full", "n_features": 4, 
+"i_open_region": 2, "i_background_region": 0, "i_nucleosomal_region": 1,
+"hmm_binsize": 10}
+```
+
+We can modify the assignment of: `"i_open_region": 2,
+"i_background_region": 0, "i_nucleosomal_region": 1,` by assigning `1`
+to open, and `2` to nucleosomal as: `"i_open_region": 1,
+"i_background_region": 0, "i_nucleosomal_region": 2,` Then save the
+HMM in a new model file such as `new_model.json`.
+
+Then next, we can re-run `macs3 hmmratac` with the same parameters
+plus an extra option for the HMM model file like `macs3 hmmratac
+--model new_model.json`
+
+""")
+    
     # group for input files
     group_input = argparser_hmmratac.add_argument_group( "Input files arguments" )
     group_input.add_argument( "-b", "--bam", dest = "bam_file", type = str, required = True, nargs = "+",
-                              help = "Sorted BAM files containing the ATAC-seq reads. If multiple files are given as '-t A B C', then they will all be read and pooled together. REQUIRED." )
+                              help = "BAM files containing the aligment results for ATAC-seq paired end reads. If multiple files are given as '-t A B C', then they will all be read and pooled together. The file should be in BAMPE format (aligned in paired end mode). REQUIRED." )
     
     # group for output files
     group_output = argparser_hmmratac.add_argument_group( "Output arguments" )
 
     add_outdir_option( group_output )
     group_output.add_argument( "-n", "--name", dest = "name", type = str,
                                help = "Name for this experiment, which will be used as a prefix to generate output file names. DEFAULT: \"NA\"",
                                default = "NA" )
+    group_output.add_argument( "--cutoff-analysis-only", dest = "cutoff_analysis_only", action = "store_true",
+                                help = "Only run the cutoff analysis and output a report. After generating the report, the process will stop. The report will help user decide the three crucial parameters for `-l`, `-u`, and `-c`. So it's highly recommanded to run this first! Please read the report and instructions in `Choices of cutoff values` on how to decide the three crucial parameters",
+                                default = False )
     group_output.add_argument( "--save-digested", dest = "save_digested", action = "store_true",
                                help = "Save the digested ATAC signals of short-, mono-, di-, and tri- signals in three BedGraph files with the names NAME_short.bdg, NAME_mono.bdg, NAME_di.bdg, and NAME_tri.bdg. DEFAULT: False",
                                default = False )    
     group_output.add_argument( "--save-states", dest = "save_states", action = "store_true",
                                help = "Save all open and nucleosomal state annotations into a BED file with the name NAME_states.bed. DEFAULT: False",
                                default = False )
     group_output.add_argument( "--save-likelihoods", dest = "save_likelihoods", action = "store_true",
@@ -781,55 +925,58 @@
     #group_hmm.add_argument( "-s", "--states", dest = "hmm_states", type = int,
     #                        help = "Number of States in the model. Default = 3. If not k=3, recommend NOT calling peaks, use bedgraph. This option is named as `--kmeans` in HMMRATAC since it will also control the number of clusters in the k-means clustering process to decide the initial emissions for HMM training.",
     #                        default = 3 )
     group_hmm.add_argument( "--binsize", dest = "hmm_binsize", type = int,
                             help = "Size of the bins to split the pileup signals for training and decoding with Hidden Markov Model. Must >= 1. Smaller the binsize, higher the resolution of the results, slower the process. Default = 10",
                             default = 10 )    
     group_hmm.add_argument( "-u", "--upper", dest = "hmm_upper", type = int,
-                            help = "Upper limit on fold change range for choosing training sites. Default: 20",
+                            help = "Upper limit on fold change range for choosing training sites. This is an important parameter for training so please read. The purpose of this parameter is to EXCLUDE those unusually highly enriched chromatin regions so we can get training samples in 'ordinary' regions instead. It's highly recommended to run the `--cutoff-analysis-only` first to decide the lower cutoff `-l`, the upper cutoff `-u`, and the pre-scanning cutoff `-c`. The upper cutoff should be the cutoff in the cutoff analysis result that can capture some (typically hundreds of) extremely high enrichment and unusually wide peaks. Default: 20",
                             default = 20 )
     group_hmm.add_argument( "-l", "--lower", dest = "hmm_lower", type = int,
-                            help = "Lower limit on fold change range for choosing training sites. Default: 10",
+                            help = "Lower limit on fold change range for choosing training sites. This is an important parameter for training so please read. The purpose of this parameter is to ONLY INCLUDE those chromatin regions having ordinary enrichment so we can get training samples to learn the common features through HMM. It's highly recommended to run the `--cutoff-analysis-only` first to decide the lower cutoff `-l`, the upper cutoff `-u`, and the pre-scanning cutoff `-c`. The lower cutoff should be the cutoff in the cutoff analysis result that can capture moderate number ( about 10k ) of peaks with normal width ( average length 500-1000bps long). Default: 10",
                             default = 10 )
     group_hmm.add_argument( "--maxTrain", dest = "hmm_maxTrain", type = int,
-                            help = "Maximum number of training regions to use. Default: 1000",
+                            help = "Maximum number of training regions to use. After we identify the training regions between `-l` and `-u`, the lower and upper cutoffs, we will randomly pick this number of regions for training. Default: 1000",
                             default = 1000 )
     group_hmm.add_argument( "--training-flanking", dest = "hmm_training_flanking", type = int, required = False,
                             help = "Training regions will be expanded to both side with this number of basepairs. The purpose is to include more background regions. Default: 1000",
                             default = 1000 )
     #group_hmm.add_argument( "-t", "--training", dest = "hmm_training_regions", type = str, required = False, 
-    #                        help = "Filename of training regions (previously was BED_file) to use for training HMM, instead of using foldchange settings to select. Default: NA" )    
+    #                        help = "Filename of training regions (previously was BED_file) to use for training HMM, instead of using foldchange settings to select. Default: NA" )
     #group_hmm.add_argument( "-z", "--zscore", dest = "hmm_zscore", type = int,
     #                        help = "Zscored read depth to mask during Viterbi decoding. Default: 100",
     #                        default = 100 )
     #group_hmm.add_argument( "--window", dest = "hmm_window", type = int,
     #                        help = "Size of the bins to split the genome into for Viterbi decoding. To save memory, the genome is split into WINDOW long bins and viterbi decoding occurs across each bin. Default = 25000000. Note: For machines with limited memory, it is recommended to reduce the size of the bins.",
     #                        default = 25000000 )
     group_hmm.add_argument( "--model", dest = "hmm_file", type = str, required = False, 
                             help = "A JSON file generated from previous HMMRATAC run to use instead of creating new one. When provided, HMM training will be skipped. Default: NA" )
     #group_hmm.add_argument( "--modelonly", dest = "hmm_modelonly", action = "store_true", default = False,
     #                        help = "Stop the program after generating model. Use this option to generate HMM model ONLY, which can be later applied with `--model`. Default: False")
 
     # group for peak calling arguments
-    group_call = argparser_hmmratac.add_argument_group( "Peak calling arguments" )
+    group_call = argparser_hmmratac.add_argument_group( "Peak calling/HMM decoding arguments" )
     group_call.add_argument( "-c", "--prescan-cutoff", dest = "prescan_cutoff", type = float,
-                             help = "The fold change cutoff for prescanning candidate regions in the whole dataset. Then we will use HMM to predict states on these candidate regions. Higher the prescan cutoff, fewer regions will be considered. Must > 1. Default: 1.2",
+                             help = "The fold change cutoff for prescanning candidate regions in the whole dataset. Then we will use HMM to predict/decode states on these candidate regions. Higher the prescan cutoff, fewer regions will be considered. Must > 1. This is an important parameter for decoding so please read. The purpose of this parameter is to EXCLUDE those chromatin regions having noises/random enrichment so we can have a large number of possible regions to predict the HMM states. It's highly recommended to run the `--cutoff-analysis-only` first to decide the lower cutoff `-l`, the upper cutoff `-u`, and the pre-scanning cutoff `-c`. The pre-scanning cutoff should be the cutoff close to the BOTTOM of the cutoff analysis result that can capture large number of possible peaks with normal length (average length 500-1000bps). In most cases, please do not pick a cutoff too low that capture almost all the background noises from the data. Default: 1.2",
                              default = 1.2 )
     
     group_call.add_argument( "--minlen", dest = "openregion_minlen", type = int,
                              help = "Minimum length of open region to call accessible regions. Must be larger than 0. If it is set as 0, it means no filtering on the length of the open regions called. Please note that, when bin size is small, setting a too small OPENREGION_MINLEN will bring a lot of false positives. Default: 100",
                              default = 100 )
     #group_call.add_argument( "--score", dest = "call_score", type = str, choices = ("max", "ave", "med", "fc", "zscore", "all"),
     #                         help = "What type of score system to use for peaks. Can be used for ranking peaks. Default: max",
     #                         default = "max" )
     #group_call.add_argument( "--threshold", dest = "call_threshold", type = float,
     #                         help = "Threshold for reporting peaks. Only peaks who's score is >= this value will be reported. Default: 100",
     #                         default = 100 )
     # group for misc
     group_misc = argparser_hmmratac.add_argument_group( "Misc arguments" )
+    group_misc.add_argument( "--pileup-short", dest = "pileup_short", action = "store_true",
+                             help = "By default, HMMRATAC will pileup all fragments in order to identify regions for training and candidate regions for decoding. When this option is on, it will pileup only the short fragments to do so. Although it sounds a good idea since we assume that open region should have a lot of short fragments, it may be possible that the overall short fragments are too few to be useful. Default: False",
+                             default = False )
     group_misc.add_argument( "--randomSeed", dest = "hmm_randomSeed", type = int,
                              help = "Seed to set for random sampling of training regions. Default: 10151",
                              default = 10151 )
     group_misc.add_argument( "--decoding-steps", dest = "decoding_steps", type = int, default = 1000, 
                              help = "Number of candidate regions to be decoded at a time. The HMM model will be applied with Viterbi to find the optimal state path in each region. bigger the number, 'possibly' faster the decoding process, 'definitely' larger the memory usage. Default: 1000.")
     group_misc.add_argument( "-e", "--blacklist", dest = "blacklist", type = str, required = False, 
                              help = "Filename of blacklisted regions to exclude (previously was BED_file). Examples are those from ENCODE. Default: NA" )
@@ -850,15 +997,14 @@
     #                           default = 30 )
     group_misc.add_argument( "--buffer-size", dest = "buffer_size", type = int, default = "100000",
                                help = "Buffer size for incrementally increasing internal array size to store reads alignment information. In most cases, you don't have to change this parameter. However, if there are large number of chromosomes/contigs/scaffolds in your alignment, it's recommended to specify a smaller buffer size in order to decrease memory usage (but it will take longer time to read alignment files). Minimum memory requested for reading an alignment file is about # of CHROMOSOME * BUFFER_SIZE * 8 Bytes. DEFAULT: 100000 " )
     
     return
 
 
-
 if __name__ == '__main__':
     __spec__ = None
     try:
         main()
     except KeyboardInterrupt:
         sys.stderr.write("User interrupted me! ;-) Bye!\n")
     except MemoryError:
```

### Comparing `MACS3-3.0.0b1/docs/INSTALL.md` & `MACS3-3.0.0b2/docs/INSTALL.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # INSTALL Guide For MACS3
-Time-stamp: <2020-12-05 16:35:26 Tao Liu>
+Time-stamp: <2023-06-16 11:46:32 Tao Liu>
 
 Please check the following instructions to complete your installation.
 
 ## Prerequisites
 
+Here we list some prerequisites for installing and running MACS3. But
+if you are using conda or pip to install, the installer will check the
+dependencies and install them if necessary.
+
 ### Python3
 
-MACS v3.x.x requires Python3. We have tested MACS in Python3.6, 3.7 and 3.8. 
+MACS v3.x.x requires Python3. We have tested MACS in Python3.8 to 3.11. 
 
-### NumPy
+### NumPy, hmmlearn
 
-MACS also requires [Numpy](http://www.scipy.org/Download) (>=1.17).
+MACS requires NumPy>=1.19 (>=1.24 recommended) and hmmlearn>=0.3 during installation. Note that hmmlearn further requires SciPy and sklearn (aka scikit-learn). 
 
 ### Cython
 
 [Cython](http://cython.org/) is required to translate .pyx codes to .c
 code. The version of Cython has to be >=0.29.
 
 ### cykhash
@@ -57,64 +61,49 @@
 
 `$ python3 -m venv MyPythonEnv/`
 
 Then activate it by
 
 `$ source MyPythonEnv/bin/activate`
 
+If you use 'conda', it will also provide virtual environment. Please 
+read: [conda](https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html) or [miniconda](https://docs.conda.io/en/latest/miniconda.html)
+
 ## Install through PyPI
 
 The easiest way to install MACS is through PyPI system. Get `pip` if
 it's not available in your system. If you create a virtual environment
 as described before, your `pip` command will install everything under
-the folder you specified previously through `python3 -m env` command.
+the folder you specified previously through `python3 -m env` command,
+or to your active conda environment. 
 
 Then under the command line, type `pip install macs3`. PyPI will
-install Numpy automatically if it is absent.
+install dependencies automatically if it is absent.
 
 To upgrade MACS3, type `pip install --upgrade macs3`. It will check
 currently installed MACS3, compare the version with the one on PyPI
 repository, download and install a newer version while necessary.
 
-If you plan to install MACS in your own user directory, use `pip
-install macs3 --user`.
-
 ## Install from source
 
-MACS uses Python's [setuptools](https://setuptools.readthedocs.io) for
-source code installations. To install a source distribution of MACS,
-unpack the distribution tarball, or clone Git repository with `git
-clone --recurse-submodules git@github.com:taoliu/MACS.git`. Go to the directory where you
-unpacked MACS, and simply run the install script:
+MACS uses `pip` for source code installations. To install a source 
+distribution of MACS, unpack the distribution tarball, or clone Git 
+repository with `git clone --recurse-submodules git@github.com:taoliu/MACS.git`. 
+Go to the directory where you cloned MACS from github, and simply
+run the install command:
 
- `$ python setup.py install`
+ `$ pip install .`
 
 By default, the script will install python library and executable
 codes according to the environment. When you run the command under
-virtualenv, the script will install to the virtual environment
-instead. When you run it without virtual environment, you may need to
-be root or administrator of the machine so as to complete the
-installation. Please contact the system administrator if you want
-their help. If you need to provide a nonstandard install prefix, or
-any other nonstandard options, you can provide many command line
-options to the install script. Use the `--help` option to see a brief
-list of available options:
-
- `$ python setup.py --help`
-
-For example, if I want to install everything under my own HOME
-directory, use this command:
-
- `$ python setup.py install --prefix /home/myaccount/`
-
-As mentioned in *Prerequisites*, you don't need to install Cython in
-order to install MACS. When Cython is available, this setup script
-will regenerate C codes from Pyx codes when necessary. When Cython is
-not available, this setup script will just use the C codes included in
-the release package (or your Github clone) for installation.
+virtualenv or conda environment, the script will install to the virtual
+environment instead. When you run the command without virtual environment, 
+you may need to be root or administrator of the machine so as to 
+complete the installation. Please contact the system administrator
+if you want their help. 
 
 ## Configure environment variables
 
 *Note*, if you are using a virtual environment, you should skip this
 section since all the corresponding environment variables have been
 correctly set while you `activate` the environment.
```

### Comparing `MACS3-3.0.0b1/docs/callpeak.md` & `MACS3-3.0.0b2/docs/callpeak.md`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/make_docker_base.sh` & `MACS3-3.0.0b2/make_docker_base.sh`

 * *Files identical despite different names*

### Comparing `MACS3-3.0.0b1/setup.py` & `MACS3-3.0.0b2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 the distribution).
 """
 
 import sys
 import os
 import re
 from setuptools import setup, Extension
+from Cython.Build import cythonize
 import subprocess
 import sysconfig
 import numpy
 
 # get MACS version
 exec(open("MACS3/Utilities/Constants.py").read())
 
 # classifiers
 classifiers =[\
-              'Development Status :: 3 - Alpha',
+              'Development Status :: 4 - Beta',
               'Environment :: Console',
               'Intended Audience :: Developers',
               'Intended Audience :: Science/Research',
               'License :: OSI Approved :: BSD License',
               'Operating System :: MacOS :: MacOS X',
               'Operating System :: POSIX',
               'Operating System :: Unix',
               'Topic :: Scientific/Engineering :: Bio-Informatics',
-              'Programming Language :: Python :: 3.8',
               'Programming Language :: Python :: 3.9',
               'Programming Language :: Python :: 3.10',
+              'Programming Language :: Python :: 3.11',
               'Programming Language :: Cython', ]
 
-install_requires = [ "numpy>=1.23",
-                     "hmmlearn>=0.2.8",
+install_requires = [ "numpy>=1.19",
+                     "hmmlearn>=0.3",
                      "cykhash>=2.0",
                      "Cython>=0.29" ]
 
 tests_requires = [ 'pytest' ]
 
 
 def main():
@@ -89,17 +90,16 @@
 
     extra_c_args_for_fermi = ["-std=gnu99","-DUSE_SIMDE", "-DSIMDE_ENABLE_NATIVE_ALIASES"]
     if icc or sysconfig.get_config_vars()['CC'] == 'icc':
         extra_c_args_for_fermi.extend(['-qopenmp-simd', '-DSIMDE_ENABLE_OPENMP'])
     elif new_gcc or clang or sysconfig.get_config_vars()['CC'] == 'clang':
         extra_c_args_for_fermi.extend(['-fopenmp-simd', '-DSIMDE_ENABLE_OPENMP'])
 
-    # extensions, those has to be processed by Cython
+    # extensions, those have to be processed by Cython
     ext_modules = [ \
-                    # Signal
                     Extension("MACS3.Signal.HMMR_EM", ["MACS3/Signal/HMMR_EM.pyx"], libraries=["m"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args ),
                     Extension("MACS3.Signal.HMMR_Signal_Processing", ["MACS3/Signal/HMMR_Signal_Processing.pyx"], libraries=["m"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args ),
                     Extension("MACS3.Signal.HMMR_HMM", ["MACS3/Signal/HMMR_HMM.pyx"], libraries=["m"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args ),
                     Extension("MACS3.Signal.Prob", ["MACS3/Signal/Prob.pyx"], libraries=["m"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args ),
                     Extension("MACS3.Signal.Region", ["MACS3/Signal/Region.pyx"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args ),
                     Extension("MACS3.Signal.Pileup", ["MACS3/Signal/Pileup.pyx","MACS3/Signal/cPosValCalculation.c"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args ),
                     Extension("MACS3.Signal.PileupV2", ["MACS3/Signal/PileupV2.pyx"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args ),                    
@@ -144,12 +144,13 @@
            packages = ['MACS3', 'MACS3.IO', 'MACS3.Signal', 'MACS3.Commands','MACS3.Utilities'],
            package_data = {'MACS3':['*.pxd']},
            scripts = ['bin/macs3', ],
            classifiers = classifiers,
            install_requires = install_requires,
            setup_requires = install_requires,
            tests_require = tests_requires,
-           python_requires = '>=3.8',
-           ext_modules = ext_modules )
+           python_requires = '>=3.9',
+           ext_modules=cythonize( ext_modules ) ),
+#                                  compiler_directives={'linetrace': True, 'binding': True}) )
 
 if __name__ == '__main__':
     main()
```

