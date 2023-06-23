# Comparing `tmp/eugene-tools-0.0.6.tar.gz` & `tmp/eugene_tools-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eugene-tools-0.0.6.tar", max compression
+gzip compressed data, was "eugene_tools-0.1.0.tar", max compression
```

## Comparing `eugene-tools-0.0.6.tar` & `eugene_tools-0.1.0.tar`

### file list

```diff
@@ -1,175 +1,72 @@
--rw-r--r--   0        0        0     1066 2022-07-27 17:31:19.000000 eugene-tools-0.0.6/LICENSE
--rw-r--r--   0        0        0     1690 2022-10-25 16:30:37.000000 eugene-tools-0.0.6/README.md
--rw-r--r--   0        0        0      966 2022-09-19 00:55:15.000000 eugene-tools-0.0.6/eugene/__init__.py
--rw-r--r--   0        0        0      439 2022-07-01 15:26:51.000000 eugene-tools-0.0.6/eugene/_compat.py
--rw-r--r--   0        0        0      396 2022-07-01 15:26:51.000000 eugene-tools-0.0.6/eugene/_constants.py
--rw-r--r--   0        0        0      226 2022-09-13 15:31:12.000000 eugene-tools-0.0.6/eugene/_eugene.py
--rw-r--r--   0        0        0     9226 2022-09-29 17:51:38.000000 eugene-tools-0.0.6/eugene/_settings.py
--rw-r--r--   0        0        0     3517 2022-07-30 20:45:31.000000 eugene-tools-0.0.6/eugene/cli/generate_model_config.py
--rw-r--r--   0        0        0     1453 2022-08-07 18:25:16.000000 eugene-tools-0.0.6/eugene/conftest.py
--rw-r--r--   0        0        0      368 2022-09-18 22:23:10.000000 eugene-tools-0.0.6/eugene/dataload/__init__.py
--rw-r--r--   0        0        0    26710 2022-10-03 17:38:35.000000 eugene-tools-0.0.6/eugene/dataload/_io.py
--rw-r--r--   0        0        0     1456 2022-09-21 18:00:43.000000 eugene-tools-0.0.6/eugene/dataload/_transforms.py
--rw-r--r--   0        0        0     3693 2022-09-21 18:01:24.000000 eugene-tools-0.0.6/eugene/dataload/_utils.py
--rw-r--r--   0        0        0    14466 2022-09-21 17:59:56.000000 eugene-tools-0.0.6/eugene/dataload/dataloaders/_SeqData.py
--rw-r--r--   0        0        0     4632 2022-09-13 15:31:12.000000 eugene-tools-0.0.6/eugene/dataload/dataloaders/_SeqDataModule.py
--rw-r--r--   0        0        0     3938 2022-10-10 16:00:37.000000 eugene-tools-0.0.6/eugene/dataload/dataloaders/_SeqDataset.py
--rw-r--r--   0        0        0       66 2022-09-18 22:23:10.000000 eugene-tools-0.0.6/eugene/dataload/dataloaders/__init__.py
--rw-r--r--   0        0        0        0 2022-09-13 15:31:12.000000 eugene-tools-0.0.6/eugene/dataload/dataloaders/_utlis.py
--rw-r--r--   0        0        0      189 2022-09-13 18:23:49.000000 eugene-tools-0.0.6/eugene/dataload/motif/__init__.py
--rw-r--r--   0        0        0     7229 2022-09-21 17:57:41.000000 eugene-tools-0.0.6/eugene/dataload/motif/_fimo.py
--rw-r--r--   0        0        0    12122 2022-09-20 02:50:05.000000 eugene-tools-0.0.6/eugene/dataload/motif/_motif.py
--rw-r--r--   0        0        0      152 2022-09-18 22:23:10.000000 eugene-tools-0.0.6/eugene/datasets/__init__.py
--rw-r--r--   0        0        0    11892 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/_datasets.py
--rw-r--r--   0        0        0     3718 2022-09-21 18:09:07.000000 eugene-tools-0.0.6/eugene/datasets/_utils.py
--rw-r--r--   0        0        0     3554 2022-10-25 15:52:19.000000 eugene-tools-0.0.6/eugene/datasets/datasets.csv
--rw-r--r--   0        0        0       14 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/10regions.bed
--rw-r--r--   0        0        0       16 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/bed_test.bed
--rw-r--r--   0        0        0      375 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/positive.bed
--rw-r--r--   0        0        0       95 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/positive.bedgraph
--rw-r--r--   0        0        0       30 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/positive_gap.bed
--rw-r--r--   0        0        0       15 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/positive_shift.bed
--rw-r--r--   0        0        0  1626119 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/pseudo_genome.fa
--rw-r--r--   0        0        0     1688 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/pseudo_snps.vcf
--rw-r--r--   0        0        0       66 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/region_w_strand.bed
--rw-r--r--   0        0        0       34 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/roi.bed
--rw-r--r--   0        0        0       16 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/roi_test.bed
--rw-r--r--   0        0        0       18 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/roi_train.bed
--rw-r--r--   0        0        0      229 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sacCer3.chrom.sizes
--rw-r--r--   0        0        0     2948 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample.bam
--rw-r--r--   0        0        0      240 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample.bam.bai
--rw-r--r--   0        0        0       46 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample.bed
--rw-r--r--   0        0        0       81 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample.bedgraph
--rw-r--r--   0        0        0     1200 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample.bw
--rw-r--r--   0        0        0       22 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample.chrom.sizes
--rw-r--r--   0        0        0      200 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample.csv
--rw-r--r--   0        0        0   880417 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample.fa
--rw-r--r--   0        0        0      147 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample.gtf
--rw-r--r--   0        0        0     2130 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample.vcf
--rw-r--r--   0        0        0      287 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample2.bam
--rw-r--r--   0        0        0      176 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample2.bam.bai
--rw-r--r--   0        0        0   881158 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample2.fa
--rw-r--r--   0        0        0    22590 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample2_test.fa
--rw-r--r--   0        0        0       68 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample_equalsize.bed
--rw-r--r--   0        0        0       26 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample_fulltile.bed
--rw-r--r--   0        0        0       57 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample_fulltile2.bed
--rw-r--r--   0        0        0    61012 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample_genome.fa
--rw-r--r--   0        0        0     1409 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample_protein.fa
--rw-r--r--   0        0        0    22576 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/sample_test.fa
--rw-r--r--   0        0        0      104 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/scored_sample.bed
--rw-r--r--   0        0        0       33 2022-10-02 18:48:23.000000 eugene-tools-0.0.6/eugene/datasets/janggu_resources/scores.bed
--rw-r--r--   0        0        0  1082384 2022-10-20 23:39:00.000000 eugene-tools-0.0.6/eugene/datasets/random1000/random1000.h5sd
--rw-r--r--   0        0        0    80128 2022-09-18 22:23:10.000000 eugene-tools-0.0.6/eugene/datasets/random1000/random1000_activities.npy
--rw-r--r--   0        0        0    24128 2022-07-19 22:36:44.000000 eugene-tools-0.0.6/eugene/datasets/random1000/random1000_ids.npy
--rw-r--r--   0        0        0    80128 2022-09-18 22:23:10.000000 eugene-tools-0.0.6/eugene/datasets/random1000/random1000_labels.npy
--rw-r--r--   0        0        0   400128 2022-09-18 22:23:10.000000 eugene-tools-0.0.6/eugene/datasets/random1000/random1000_ohe_rev_seqs.npy
--rw-r--r--   0        0        0   400128 2022-09-18 22:23:10.000000 eugene-tools-0.0.6/eugene/datasets/random1000/random1000_ohe_seqs.npy
--rw-r--r--   0        0        0   400128 2022-09-18 22:23:10.000000 eugene-tools-0.0.6/eugene/datasets/random1000/random1000_rev_seqs.npy
--rw-r--r--   0        0        0   109000 2022-09-18 22:23:10.000000 eugene-tools-0.0.6/eugene/datasets/random1000/random1000_seqs.fa
--rw-r--r--   0        0        0   400128 2022-09-18 22:23:10.000000 eugene-tools-0.0.6/eugene/datasets/random1000/random1000_seqs.npy
--rw-r--r--   0        0        0   320826 2022-09-18 22:23:10.000000 eugene-tools-0.0.6/eugene/datasets/random1000/random1000_seqs.tsv
--rw-r--r--   0        0        0      245 2022-09-13 15:31:13.000000 eugene-tools-0.0.6/eugene/evaluate/__init__.py
--rw-r--r--   0        0        0     2746 2022-09-29 17:51:38.000000 eugene-tools-0.0.6/eugene/evaluate/_metrics.py
--rw-r--r--   0        0        0     8867 2022-10-16 00:10:48.000000 eugene-tools-0.0.6/eugene/evaluate/_predict.py
--rw-r--r--   0        0        0     9465 2022-09-29 17:51:38.000000 eugene-tools-0.0.6/eugene/evaluate/_rnacomplete_metrics.py
--rw-r--r--   0        0        0      534 2022-09-21 18:11:01.000000 eugene-tools-0.0.6/eugene/evaluate/utils.py
--rw-r--r--   0        0        0       62 2022-09-13 15:31:13.000000 eugene-tools-0.0.6/eugene/external/__init__.py
--rw-r--r--   0        0        0       33 2022-07-01 15:26:52.000000 eugene-tools-0.0.6/eugene/external/gkm_svm/__init__.py
--rw-r--r--   0        0        0     1220 2022-07-16 15:14:24.000000 eugene-tools-0.0.6/eugene/external/gkm_svm/_gkm_svm.py
--rw-r--r--   0        0        0        0 2022-09-18 22:23:10.000000 eugene-tools-0.0.6/eugene/external/janggu/__init__.py
--rw-r--r--   0        0        0     6453 2022-10-10 21:23:26.000000 eugene-tools-0.0.6/eugene/external/janggu/data/__init__.py
--rw-r--r--   0        0        0    65505 2022-08-16 16:22:42.000000 eugene-tools-0.0.6/eugene/external/janggu/data/coverage.py
--rw-r--r--   0        0        0     6650 2022-08-16 16:22:42.000000 eugene-tools-0.0.6/eugene/external/janggu/data/data.py
--rw-r--r--   0        0        0    33560 2022-08-16 16:22:42.000000 eugene-tools-0.0.6/eugene/external/janggu/data/dna.py
--rw-r--r--   0        0        0    15761 2022-08-16 16:22:42.000000 eugene-tools-0.0.6/eugene/external/janggu/data/genomic_indexer.py
--rw-r--r--   0        0        0    46782 2022-08-16 16:22:42.000000 eugene-tools-0.0.6/eugene/external/janggu/data/genomicarray.py
--rw-r--r--   0        0        0    11716 2022-08-16 16:22:42.000000 eugene-tools-0.0.6/eugene/external/janggu/data/nparr.py
--rw-r--r--   0        0        0    10917 2022-08-16 16:22:42.000000 eugene-tools-0.0.6/eugene/external/janggu/data/visualization.py
--rw-r--r--   0        0        0       14 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/10regions.bed
--rw-r--r--   0        0        0       16 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/bed_test.bed
--rw-r--r--   0        0        0      375 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/positive.bed
--rw-r--r--   0        0        0       95 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/positive.bedgraph
--rw-r--r--   0        0        0       30 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/positive_gap.bed
--rw-r--r--   0        0        0       15 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/positive_shift.bed
--rw-r--r--   0        0        0  1626119 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/pseudo_genome.fa
--rw-r--r--   0        0        0     1688 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/pseudo_snps.vcf
--rw-r--r--   0        0        0       66 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/region_w_strand.bed
--rw-r--r--   0        0        0       34 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/roi.bed
--rw-r--r--   0        0        0       16 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/roi_test.bed
--rw-r--r--   0        0        0       18 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/roi_train.bed
--rw-r--r--   0        0        0      229 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sacCer3.chrom.sizes
--rw-r--r--   0        0        0     2948 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample.bam
--rw-r--r--   0        0        0      240 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample.bam.bai
--rw-r--r--   0        0        0       46 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample.bed
--rw-r--r--   0        0        0       81 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample.bedgraph
--rw-r--r--   0        0        0     1200 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample.bw
--rw-r--r--   0        0        0       22 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample.chrom.sizes
--rw-r--r--   0        0        0      200 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample.csv
--rw-r--r--   0        0        0   880417 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample.fa
--rw-r--r--   0        0        0      147 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample.gtf
--rw-r--r--   0        0        0     2130 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample.vcf
--rw-r--r--   0        0        0      287 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample2.bam
--rw-r--r--   0        0        0      176 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample2.bam.bai
--rw-r--r--   0        0        0   881158 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample2.fa
--rw-r--r--   0        0        0    22590 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample2_test.fa
--rw-r--r--   0        0        0       68 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample_equalsize.bed
--rw-r--r--   0        0        0       26 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample_fulltile.bed
--rw-r--r--   0        0        0       57 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample_fulltile2.bed
--rw-r--r--   0        0        0    61012 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample_genome.fa
--rw-r--r--   0        0        0     1409 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample_protein.fa
--rw-r--r--   0        0        0    22576 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/sample_test.fa
--rw-r--r--   0        0        0      104 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/scored_sample.bed
--rw-r--r--   0        0        0       33 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/resources/scores.bed
--rw-r--r--   0        0        0    29096 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/utils.py
--rw-r--r--   0        0        0       19 2022-08-07 19:55:25.000000 eugene-tools-0.0.6/eugene/external/janggu/version.py
--rw-r--r--   0        0        0      223 2022-09-13 15:31:13.000000 eugene-tools-0.0.6/eugene/external/kipoi/__init__.py
--rw-r--r--   0        0        0      658 2022-09-13 15:31:13.000000 eugene-tools-0.0.6/eugene/external/kipoi/_wrappers.py
--rw-r--r--   0        0        0        0 2022-09-13 15:31:13.000000 eugene-tools-0.0.6/eugene/external/kipoi/kipoi_veff/__init__.py
--rw-r--r--   0        0        0     8117 2022-09-13 15:31:13.000000 eugene-tools-0.0.6/eugene/external/kipoi/kipoi_veff/plot.py
--rw-r--r--   0        0        0    15507 2022-09-13 15:31:13.000000 eugene-tools-0.0.6/eugene/external/kipoi/kipoi_veff/seqplotting_deps.py
--rw-r--r--   0        0        0    15805 2022-09-13 15:31:13.000000 eugene-tools-0.0.6/eugene/external/kipoi/kipoi_veff/seqplotting_letters.py
--rw-r--r--   0        0        0        0 2022-09-12 23:30:44.000000 eugene-tools-0.0.6/eugene/external/sklearn/__init__.py
--rw-r--r--   0        0        0      342 2022-09-13 20:00:01.000000 eugene-tools-0.0.6/eugene/interpret/__init__.py
--rw-r--r--   0        0        0     2239 2022-09-29 17:51:39.000000 eugene-tools-0.0.6/eugene/interpret/_dim_reduction.py
--rw-r--r--   0        0        0    20454 2022-10-10 16:00:37.000000 eugene-tools-0.0.6/eugene/interpret/_feature_attribution.py
--rw-r--r--   0        0        0    11626 2022-09-29 17:51:39.000000 eugene-tools-0.0.6/eugene/interpret/_filter_viz.py
--rw-r--r--   0        0        0    12413 2022-10-10 16:00:37.000000 eugene-tools-0.0.6/eugene/interpret/_in_silico.py
--rw-r--r--   0        0        0     4780 2022-10-10 16:00:37.000000 eugene-tools-0.0.6/eugene/interpret/_utils.py
--rw-r--r--   0        0        0      273 2022-10-10 21:45:40.000000 eugene-tools-0.0.6/eugene/models/__init__.py
--rw-r--r--   0        0        0    26009 2022-10-20 23:39:00.000000 eugene-tools-0.0.6/eugene/models/_base_models.py
--rw-r--r--   0        0        0     7754 2022-10-20 23:39:00.000000 eugene-tools-0.0.6/eugene/models/_custom_models.py
--rw-r--r--   0        0        0     4614 2022-10-10 16:00:38.000000 eugene-tools-0.0.6/eugene/models/_initialize.py
--rw-r--r--   0        0        0    10361 2022-10-03 18:21:33.000000 eugene-tools-0.0.6/eugene/models/_sota_models.py
--rw-r--r--   0        0        0      452 2022-09-13 15:31:13.000000 eugene-tools-0.0.6/eugene/models/_utils.py
--rw-r--r--   0        0        0      161 2022-09-13 15:31:13.000000 eugene-tools-0.0.6/eugene/models/base/__init__.py
--rw-r--r--   0        0        0     8438 2022-10-10 16:00:38.000000 eugene-tools-0.0.6/eugene/models/base/_base_model.py
--rw-r--r--   0        0        0     5877 2022-10-03 18:29:04.000000 eugene-tools-0.0.6/eugene/models/base/_base_modules.py
--rw-r--r--   0        0        0     3595 2022-09-29 17:51:39.000000 eugene-tools-0.0.6/eugene/models/base/_custom_conv_modules.py
--rw-r--r--   0        0        0     1845 2022-09-29 17:51:39.000000 eugene-tools-0.0.6/eugene/models/base/_utils.py
--rw-r--r--   0        0        0      579 2022-10-20 23:58:52.000000 eugene-tools-0.0.6/eugene/plot/__init__.py
--rw-r--r--   0        0        0     6836 2022-09-29 17:51:39.000000 eugene-tools-0.0.6/eugene/plot/_catplot.py
--rw-r--r--   0        0        0     8018 2022-09-29 17:51:39.000000 eugene-tools-0.0.6/eugene/plot/_classification.py
--rw-r--r--   0        0        0     3322 2022-09-13 15:31:13.000000 eugene-tools-0.0.6/eugene/plot/_dim_reduce.py
--rw-r--r--   0        0        0     5652 2022-10-10 16:00:38.000000 eugene-tools-0.0.6/eugene/plot/_regression.py
--rw-r--r--   0        0        0    25675 2022-10-15 21:45:41.000000 eugene-tools-0.0.6/eugene/plot/_seq.py
--rw-r--r--   0        0        0    10157 2022-09-29 17:51:39.000000 eugene-tools-0.0.6/eugene/plot/_summary.py
--rw-r--r--   0        0        0     3932 2022-10-10 16:00:38.000000 eugene-tools-0.0.6/eugene/plot/_training.py
--rw-r--r--   0        0        0     9368 2022-09-29 17:51:39.000000 eugene-tools-0.0.6/eugene/plot/_utils.py
--rw-r--r--   0        0        0     1189 2022-10-11 02:26:41.000000 eugene-tools-0.0.6/eugene/preprocess/__init__.py
--rw-r--r--   0        0        0     3129 2022-10-10 16:00:38.000000 eugene-tools-0.0.6/eugene/preprocess/_dataset_preprocess.py
--rw-r--r--   0        0        0    13712 2022-10-20 23:39:00.000000 eugene-tools-0.0.6/eugene/preprocess/_preprocessing.py
--rw-r--r--   0        0        0    13486 2022-10-10 16:00:38.000000 eugene-tools-0.0.6/eugene/preprocess/_seq_preprocess.py
--rw-r--r--   0        0        0     9319 2022-09-13 15:31:13.000000 eugene-tools-0.0.6/eugene/preprocess/_utils.py
--rw-r--r--   0        0        0       22 2022-08-01 23:00:33.000000 eugene-tools-0.0.6/eugene/train/__init__.py
--rw-r--r--   0        0        0        0 2022-07-01 15:26:53.000000 eugene-tools-0.0.6/eugene/train/_crossfold.py
--rw-r--r--   0        0        0     6472 2022-09-29 17:51:39.000000 eugene-tools-0.0.6/eugene/train/_fit.py
--rw-r--r--   0        0        0     5679 2022-09-13 15:31:13.000000 eugene-tools-0.0.6/eugene/train/_hyperopt.py
--rw-r--r--   0        0        0      315 2022-09-20 02:00:39.000000 eugene-tools-0.0.6/eugene/utils/__init__.py
--rw-r--r--   0        0        0     1147 2022-09-29 17:51:39.000000 eugene-tools-0.0.6/eugene/utils/_custom_callbacks.py
--rw-r--r--   0        0        0     3802 2022-10-10 16:00:38.000000 eugene-tools-0.0.6/eugene/utils/_decorators.py
--rw-r--r--   0        0        0     4062 2022-09-29 17:51:39.000000 eugene-tools-0.0.6/eugene/utils/_hpc.py
--rw-r--r--   0        0        0     3467 2022-09-29 17:51:39.000000 eugene-tools-0.0.6/eugene/utils/_random_data.py
--rw-r--r--   0        0        0      281 2022-07-23 19:03:48.000000 eugene-tools-0.0.6/eugene/utils/_utils.py
--rw-r--r--   0        0        0     2857 2022-10-26 16:56:39.000000 eugene-tools-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5158 2022-10-26 16:58:28.897886 eugene-tools-0.0.6/setup.py
--rw-r--r--   0        0        0     5059 2022-10-26 16:58:28.898386 eugene-tools-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-01-26 02:27:24.000000 eugene_tools-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1840 2023-03-21 15:05:35.000000 eugene_tools-0.1.0/README.md
+-rw-r--r--   0        0        0      578 2023-06-19 16:37:09.000000 eugene_tools-0.1.0/eugene/__init__.py
+-rw-r--r--   0        0        0     6279 2023-06-19 16:37:09.000000 eugene_tools-0.1.0/eugene/_settings.py
+-rw-r--r--   0        0        0     1455 2023-06-19 16:37:09.000000 eugene_tools-0.1.0/eugene/conftest.py
+-rw-r--r--   0        0        0       45 2023-06-19 16:37:09.000000 eugene_tools-0.1.0/eugene/dataload/__init__.py
+-rw-r--r--   0        0        0    15141 2023-06-21 23:18:28.000000 eugene_tools-0.1.0/eugene/dataload/_augment.py
+-rw-r--r--   0        0        0     1244 2023-06-19 16:37:09.000000 eugene_tools-0.1.0/eugene/dataload/_utils.py
+-rw-r--r--   0        0        0      258 2023-06-04 23:20:15.000000 eugene_tools-0.1.0/eugene/evaluate/__init__.py
+-rw-r--r--   0        0        0     1259 2023-06-19 16:37:09.000000 eugene_tools-0.1.0/eugene/evaluate/_evaluate.py
+-rw-r--r--   0        0        0     8522 2023-06-19 16:37:09.000000 eugene_tools-0.1.0/eugene/evaluate/_predict.py
+-rw-r--r--   0        0        0      991 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/evaluate/_utils.py
+-rw-r--r--   0        0        0        0 2023-06-04 23:18:14.000000 eugene_tools-0.1.0/eugene/evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0     2741 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/evaluate/metrics/_binary_classification.py
+-rw-r--r--   0        0        0      541 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/evaluate/metrics/_multiclass_classification.py
+-rw-r--r--   0        0        0    13629 2023-06-22 01:19:28.000000 eugene_tools-0.1.0/eugene/evaluate/metrics/_profile_prediction.py
+-rw-r--r--   0        0        0      745 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/evaluate/metrics/_regression.py
+-rw-r--r--   0        0        0     3049 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/experimental/_AdverserialModule.py
+-rw-r--r--   0        0        0     8244 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/experimental/_AugmentModule.py
+-rw-r--r--   0        0        0     7013 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/experimental/_GenerativeModule.py
+-rw-r--r--   0        0        0        0 2023-06-02 01:31:03.000000 eugene_tools-0.1.0/eugene/experimental/_LanguageModule.py
+-rw-r--r--   0        0        0     1204 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/experimental/_hyperopt_wandb.py
+-rw-r--r--   0        0        0     7154 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/experimental/_language_models.py
+-rw-r--r--   0        0        0     1905 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/experimental/_preprocess.py
+-rw-r--r--   0        0        0      218 2023-06-22 19:12:07.000000 eugene_tools-0.1.0/eugene/interpret/__init__.py
+-rw-r--r--   0        0        0     1981 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/interpret/_attribute.py
+-rw-r--r--   0        0        0     5085 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/interpret/_filters.py
+-rw-r--r--   0        0        0     2804 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/interpret/_generative.py
+-rw-r--r--   0        0        0     4390 2023-06-22 19:11:28.000000 eugene_tools-0.1.0/eugene/interpret/_gia.py
+-rw-r--r--   0        0        0     8268 2023-06-22 01:39:46.000000 eugene_tools-0.1.0/eugene/models/_ProfileModule.py
+-rw-r--r--   0        0        0    11056 2023-06-21 19:34:53.000000 eugene_tools-0.1.0/eugene/models/_SequenceModule.py
+-rw-r--r--   0        0        0      255 2023-06-22 22:48:25.000000 eugene_tools-0.1.0/eugene/models/__init__.py
+-rw-r--r--   0        0        0     1778 2023-06-22 23:12:56.000000 eugene_tools-0.1.0/eugene/models/_utils.py
+-rw-r--r--   0        0        0        0 2023-06-02 01:31:03.000000 eugene_tools-0.1.0/eugene/models/base/__init__.py
+-rw-r--r--   0        0        0     8986 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_blocks.py
+-rw-r--r--   0        0        0     4566 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_initializers.py
+-rw-r--r--   0        0        0    11661 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_layers.py
+-rw-r--r--   0        0        0     3654 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_losses.py
+-rw-r--r--   0        0        0     1642 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_metrics.py
+-rw-r--r--   0        0        0    10447 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_module.py
+-rw-r--r--   0        0        0      625 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_optimizers.py
+-rw-r--r--   0        0        0     3311 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_regularizers.py
+-rw-r--r--   0        0        0      121 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_schedulers.py
+-rw-r--r--   0        0        0    12485 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_towers.py
+-rw-r--r--   0        0        0     1731 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_utils.py
+-rw-r--r--   0        0        0      347 2023-06-22 22:46:51.000000 eugene_tools-0.1.0/eugene/models/zoo/__init__.py
+-rw-r--r--   0        0        0    21129 2023-06-19 16:39:57.000000 eugene_tools-0.1.0/eugene/models/zoo/_basic_models.py
+-rw-r--r--   0        0        0     4964 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/zoo/_cre_activity_predictors.py
+-rw-r--r--   0        0        0     6353 2023-06-21 19:28:04.000000 eugene_tools-0.1.0/eugene/models/zoo/_profile_predictors.py
+-rw-r--r--   0        0        0    13340 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/zoo/_regulatory_classifiers.py
+-rw-r--r--   0        0        0     3291 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/zoo/_single_cell_predictors.py
+-rw-r--r--   0        0        0    10772 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/zoo/_tf_binding_predictors.py
+-rw-r--r--   0        0        0      578 2023-06-22 19:12:32.000000 eugene_tools-0.1.0/eugene/plot/__init__.py
+-rw-r--r--   0        0        0     7390 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/plot/_catplot.py
+-rw-r--r--   0        0        0     7922 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/plot/_classification.py
+-rw-r--r--   0        0        0     3601 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/plot/_dim_reduce.py
+-rw-r--r--   0        0        0     3450 2023-06-22 19:07:58.000000 eugene_tools-0.1.0/eugene/plot/_gia.py
+-rw-r--r--   0        0        0     6217 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/plot/_regression.py
+-rw-r--r--   0        0        0    20681 2023-06-23 20:45:02.000000 eugene_tools-0.1.0/eugene/plot/_seq.py
+-rw-r--r--   0        0        0    11115 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/plot/_summary.py
+-rw-r--r--   0        0        0     3868 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/plot/_training.py
+-rw-r--r--   0        0        0     9721 2023-06-23 20:43:47.000000 eugene_tools-0.1.0/eugene/plot/_utils.py
+-rw-r--r--   0        0        0      281 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/preprocess/__init__.py
+-rw-r--r--   0        0        0     8699 2023-06-23 20:21:46.000000 eugene_tools-0.1.0/eugene/preprocess/_seqdata.py
+-rw-r--r--   0        0        0     1084 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/preprocess/_utils.py
+-rw-r--r--   0        0        0       78 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/train/__init__.py
+-rw-r--r--   0        0        0     8499 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/train/_fit.py
+-rw-r--r--   0        0        0     7183 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/train/_hyperopt.py
+-rw-r--r--   0        0        0       30 2023-06-04 01:53:27.000000 eugene_tools-0.1.0/eugene/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/utils/_utils.py
+-rw-r--r--   0        0        0      679 2023-06-23 20:48:37.000000 eugene_tools-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 eugene_tools-0.1.0/PKG-INFO
```

### Comparing `eugene-tools-0.0.6/LICENSE` & `eugene_tools-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eugene-tools-0.0.6/README.md` & `eugene_tools-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,8 +5,10 @@
 
 <img src="docs/_static/EugeneLogoText.png" alt="EUGENe Logo" width=350>
 
 # **E**lucidating the **U**tility of **G**enomic **E**lements with **Ne**ural Nets
 
 EUGENe represents a computational framework for machine learning based modeling of regulatory sequences. It is designed after the [Scanpy](https://scanpy.readthedocs.io/en/stable/) package for single cell analysis in Python and is meant to make the development of deep learning workflows in the genomics field more findable, accessible, interoperitable and reproducible (FAIR). EUGENe consists of several modules for handling data and for building, training, evaluating and interpreting deep learners that predict annotations of biological sequences. EUGENe is primarily designed to be used through its Python API and we feel that users will get the most out of it by using a notebook interface (i.e. Jupyter).
 
-EUGENe is a package that is still under construction, so there's a good chance you'll run into an error or two to if you use EUGENe before its first stable release. However, catching these errors is incredbily valuable for us! If you run into such errors or have any questions, please open an issue! You can read the [current documentation](https://eugene-tools.readthedocs.io/en/latest/index.html) here for getting started.
+EUGENe is a package that is still under construction, so there's a chance you'll run into an error or two in the current release. However, catching these errors is incredbily valuable for us! If you run into such errors, have enhancement suggestions, or have any questions, please open an issue! You can read the [current documentation](https://eugene-tools.readthedocs.io/en/latest/index.html) here for getting started.
+
+If you use EUGENe for your research, please cite our preprint: [Klie *et al.* bioRxiv 2022](https://www.biorxiv.org/content/10.1101/2022.10.24.513593v1)
```

### Comparing `eugene-tools-0.0.6/eugene/_settings.py` & `eugene_tools-0.1.0/eugene/models/base/_module.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,286 +1,337 @@
-import logging
-from pathlib import Path
-from typing import Any, Union
-from typing import Tuple
-import pytorch_lightning as pl
 import torch
-from rich.console import Console
-from rich.logging import RichHandler
-from ._compat import Literal
-
-if torch.cuda.is_available():
-    print(f"GPU is available: {torch.cuda.is_available()}")
-    print(f"Number of GPUs: {torch.cuda.device_count()}")
-    print(f"Current GPU: {torch.cuda.current_device()}")
-    print(f"GPUs: {torch.cuda.get_device_name(torch.cuda.current_device())}")
-
-
-eugene_logger = logging.getLogger("eugene")
-
-
-def _type_check(var: Any, varname: str, types: Union[type, Tuple[type, ...]]):
-    if isinstance(var, types):
-        return
-    if isinstance(types, type):
-        possible_types_str = types.__name__
-    else:
-        type_names = [t.__name__ for t in types]
-        possible_types_str = "{} or {}".format(
-            ", ".join(type_names[:-1]), type_names[-1]
-        )
-    raise TypeError(f"{varname} must be of type {possible_types_str}")
+import numpy as np
+from tqdm.auto import tqdm
+from typing import Union, Callable, Optional, Tuple
+from pytorch_lightning import seed_everything
+from pytorch_lightning.core import LightningModule
+from pytorch_lightning.utilities.model_summary import ModelSummary
+from base._losses import LOSS_REGISTRY
+from base._optimizers import OPTIMIZER_REGISTRY
+from base._schedulers import SCHEDULER_REGISTRY
+from base._metrics import METRIC_REGISTRY, DEFAULT_TASK_METRICS, DEFAULT_METRIC_KWARGS
 
 
-class EugeneConfig:
+class BaseModule(LightningModule):
     """
-    Config manager for eugene.
-    Examples
-    --------
-    To set the seed
-    >>> eugene.settings.seed = 13
-    To set the default batch size for all functions
-    >>> eugene.settings.batch_size = 1024
-    To set the progress bar style, choose one of "rich", "tqdm"
-    >>> eugene.settings.progress_bar_style = "rich"
-    To set the verbosity
-    >>> import logging
-    >>> eugene.settings.verbosity = logging.INFO
-    To set pin memory for GPU training
-    >>> eugene.settings.dl_pin_memory_gpu_training = True
+    TODO: Make this a protocol with expectations for multiple child class modules
     """
 
     def __init__(
         self,
-        verbosity: int = logging.INFO,
-        seed: int = 13,
-        progress_bar_style: Literal["rich", "tqdm"] = "tqdm",
-        rc_context: dict = None,
-        dpi: int = 300,
-        batch_size: int = 128,
-        gpus: int = None,
-        dl_num_workers: int = 0,
-        dl_pin_memory_gpu_training: bool = False,
-        dataset_dir="./eugene_data/",
-        logging_dir: str = "./eugene_logs/",
-        output_dir: str = "./eugene_output/",
-        config_dir: str = "./eugene_configs/",
-        figure_dir: str = "./eugene_figures/",
+        model: torch.nn.Module,
+        task: str = "regression",
+        loss_fxn: Union[str, Callable] = "mse",
+        optimizer: str = "adam",
+        optimizer_lr: float = 1e-3,
+        optimizer_kwargs: dict = {},
+        scheduler: str = None,
+        scheduler_monitor: str = "val_loss_epoch",
+        scheduler_kwargs: dict = {},
+        metric: str = None,
+        metric_kwargs: dict = None,
+        seed: int = None,
+        save_hyperparams: bool = True,
+        arch: str = None,  # TODO: this should be a class attribute
+        name: str = None,
     ):
+        super().__init__()
 
-        self.verbosity = verbosity
-        self.seed = seed
-        if progress_bar_style not in ["rich", "tqdm"]:
-            raise ValueError("Progress bar style must be in ['rich', 'tqdm']")
-        self.progress_bar_style = progress_bar_style
-        self.rc_context = rc_context
-        self.dpi = dpi
-        self.batch_size = batch_size
-        self.gpus = 1 if torch.cuda.is_available() else 0 if gpus is None else gpus
-        self.dl_num_workers = dl_num_workers
-        self.dl_pin_memory_gpu_training = dl_pin_memory_gpu_training
-        self.dataset_dir = dataset_dir
-        self.logging_dir = logging_dir
-        self.output_dir = output_dir
-        self.config_dir = config_dir
-        self.figure_dir = figure_dir
+        # Set the base attributes of a Sequence model
+        self.input_len = model.input_len
+        self.output_dim = model.output_dim
+        self.task = task
+
+        # Set the loss function
+        self.loss_fxn = (
+            LOSS_REGISTRY[loss_fxn] if isinstance(loss_fxn, str) else loss_fxn
+        )
 
-    @property
-    def verbosity(self) -> int:
-        """Verbosity level (default `logging.INFO`)."""
-        return self._verbosity
+        # Set the optimizer
+        self.optimizer = OPTIMIZER_REGISTRY[optimizer]
+        self.optimizer_lr = optimizer_lr if optimizer_lr is not None else 1e-3
+        self.optimizer_kwargs = optimizer_kwargs
+
+        # Set the scheduler
+        self.scheduler = (
+            SCHEDULER_REGISTRY[scheduler] if scheduler is not None else None
+        )
+        self.scheduler_monitor = scheduler_monitor
+        self.scheduler_kwargs = scheduler_kwargs
 
-    @verbosity.setter
-    def verbosity(self, level: Union[str, int]):
-        """
-        Sets logging configuration for eugene based on chosen level of verbosity.
-        If "eugene" logger has no StreamHandler, add one.
-        Else, set its level to `level`.
-        Parameters
-        ----------
-        level
-            Sets "eugene" logging level to `level`
-        force_terminal
-            Rich logging option, set to False if piping to file output.
-        """
-        self._verbosity = level
-        eugene_logger.setLevel(level)
-        logging.getLogger('tensorflow').disabled = True
-        if len(eugene_logger.handlers) == 0:
-            console = Console(force_terminal=True)
-            if console.is_jupyter is True:
-                console.is_jupyter = False
-            ch = RichHandler(
-                level=level, show_path=False, console=console, show_time=False
-            )
-            formatter = logging.Formatter("%(message)s")
-            ch.setFormatter(formatter)
-            eugene_logger.addHandler(ch)
+        # Set the metric
+        (
+            self.train_metric,
+            self.metric_kwargs,
+            self.metric_name,
+        ) = self.configure_metrics(metric=metric, metric_kwargs=metric_kwargs)
+        self.val_metric = self.train_metric.clone()
+        self.test_metric = self.train_metric.clone()
+
+        # Set the seed
+        if seed is not None:
+            self.seed = seed
+            seed_everything(self.seed)
         else:
-            eugene_logger.setLevel(level)
+            self.seed = None
 
-    def reset_logging_handler(self):
-        """
-        Resets "eugene" log handler to a basic RichHandler().
-        This is useful if piping outputs to a file.
-        """
-        eugene_logger.removeHandler(eugene_logger.handlers[0])
-        ch = RichHandler(level=self._verbosity, show_path=False, show_time=False)
-        formatter = logging.Formatter("%(message)s")
-        ch.setFormatter(formatter)
-        eugene_logger.addHandler(ch)
+        # Set the hyperparameters if passed in
+        if save_hyperparams:
+            self.save_hyperparameters()
 
-    @property
-    def seed(self) -> int:
-        """Random seed for torch and numpy."""
-        return self._seed
+        # Set the architecture
+        self.arch = arch if arch is not None else self.model.__class__.__name__
 
-    @seed.setter
-    def seed(self, seed: int):
-        """Random seed for torch and numpy."""
-        torch.backends.cudnn.deterministic = True
-        torch.backends.cudnn.benchmark = False
-        pl.utilities.seed.seed_everything(seed)
-        self._seed = seed
+        # Set the model name
+        self.name = name if name is not None else "model"
 
-    @property
-    def progress_bar_style(self) -> str:
-        """Library to use for progress bar."""
-        return self._pbar_style
-
-    @progress_bar_style.setter
-    def progress_bar_style(self, pbar_style: Literal["tqdm", "rich"]):
-        """Library to use for progress bar."""
-        self._pbar_style = pbar_style
-
-    @property
-    def rc_context(self) -> dict:
-        """Matplotlib rc_context."""
-        return self._rc_context
-
-    default_rc_context = {
-        "axes.titlesize": 16,
-        "axes.labelsize": 14,
-        "xtick.labelsize": 12,
-        "ytick.labelsize": 12,
-        "legend.fontsize": 12,
-        "pdf.fonttype": 42,
-        "ps.fonttype": 42,
-    }
-    @rc_context.setter
-    def rc_context(self, rc_context: dict):
-        """Matplotlib rc_context."""
-        if rc_context is None:
-            self._rc_context = self.default_rc_context
-        else:
-            self._rc_context = rc_context
-
-    @property
-    def dpi(self) -> int:
-        """Matplotlib dpi."""
-        return self._dpi
-
-    @dpi.setter
-    def dpi(self, dpi: int):
-        """Matplotlib dpi."""
-        self._dpi = dpi
-
-    @property
-    def batch_size(self) -> int:
+    def forward(self, x) -> torch.Tensor:
         """
-        Minibatch size for loading data into the model.
-        This is only used after a model is trained. Trainers have specific
-        `batch_size` parameters.
-        """
-        return self._batch_size
-
-    @batch_size.setter
-    def batch_size(self, batch_size: int):
-        """
-        Minibatch size for loading data into the model.
-        This is only used after a model is trained. Trainers have specific
-        `batch_size` parameters.
-        """
-        self._batch_size = batch_size
+        Forward pass of the model. This method must be implemented by the child class.
 
-    @property
-    def gpus(self) -> int:
-        """
-        Number of GPUs to use.
+        Parameters:
+        ----------
+        x (torch.Tensor):
+            input sequence
         """
-        return self._gpus
+        self.model(x)
 
-    @gpus.setter
-    def gpus(self, gpus: int):
+    def predict(self, x, batch_size=128):
         """
-        Number of GPUs to use.
+        Predict the output of the model in batches
         """
-        self._gpus = gpus
+        with torch.no_grad():
+            device = self.model.device
+            self.model.eval()
+            if isinstance(x, np.ndarray):
+                x = torch.from_numpy(x.astype(np.float32))
+            outs = []
+            for _, i in tqdm(
+                enumerate(range(0, len(x), batch_size)),
+                desc="Predicting on batches",
+                total=len(x) // batch_size,
+            ):
+                batch = x[i : i + batch_size].to(device)
+                outs.append(self.model(batch))
+            return torch.cat(outs)
 
-    @property
-    def dl_num_workers(self) -> int:
-        """Number of workers for PyTorch data loaders (Default is 0)."""
-        return self._dl_num_workers
-
-    @dl_num_workers.setter
-    def dl_num_workers(self, dl_num_workers: int):
-        """Number of workers for PyTorch data loaders (Default is 0)."""
-        self._dl_num_workers = dl_num_workers
+    def _common_step(self, batch, batch_idx, stage: str):
+        """Common step for training, validation and test
 
-    @property
-    def dl_pin_memory_gpu_training(self) -> int:
-        """Set `pin_memory` in data loaders when using a GPU for training."""
-        return self._dl_pin_memory_gpu_training
-
-    @dl_pin_memory_gpu_training.setter
-    def dl_pin_memory_gpu_training(self, dl_pin_memory_gpu_training: int):
-        """Set `pin_memory` in data loaders when using a GPU for training."""
-        self._dl_pin_memory_gpu_training = dl_pin_memory_gpu_training
+        Parameters:
+        ----------
+        batch (tuple):
+            batch of data
+        batch_idx (int):
+            index of the batch
+        stage (str):
+            stage of the training
 
-    @property
-    def logging_dir(self) -> Path:
-        """Directory for training logs (default `'./eugene_log/'`)."""
-        return self._logging_dir
-
-    @logging_dir.setter
-    def logging_dir(self, logging_dir: Union[str, Path]):
-        self._logging_dir = Path(logging_dir).resolve()
+        Returns:
+        ----------
+        dict:
+            dictionary of metrics
+        """
+        # Get and log loss
+        X, y = batch["seq"], batch["target"]
+        outs = self.model(X).squeeze(dim=1)
+        loss = self.loss_fxn(outs, y.float())  # train
+        return {"loss": loss, "outs": outs.detach(), "y": y.detach()}
+
+    def training_step(self, batch, batch_idx):
+        """Training step"""
+        step_dict = self._common_step(batch, batch_idx, "train")
+        self.log("train_loss", step_dict["loss"], on_step=True, on_epoch=False)
+        self.log("train_loss_epoch", step_dict["loss"], on_step=False, on_epoch=True)
+        self.train_metric(step_dict["outs"], step_dict["y"])
+        self.log(
+            f"train_{self.metric_name}_epoch",
+            self.train_metric,
+            on_step=False,
+            on_epoch=True,
+        )
+        return step_dict
 
-    @property
-    def dataset_dir(self) -> Path:
-        """Directory for example (default `'./data/'`)."""
-        return self._dataset_dir
-
-    @dataset_dir.setter
-    def dataset_dir(self, dataset_dir: Union[str, Path]):
-        _type_check(dataset_dir, "dataset_dir", (str, Path))
-        self._dataset_dir = Path(dataset_dir).resolve()
+    def validation_step(self, batch, batch_idx):
+        """Validation step"""
+        step_dict = self._common_step(batch, batch_idx, "val")
+        self.log("val_loss_epoch", step_dict["loss"], on_step=False, on_epoch=True)
+        self.val_metric(step_dict["outs"], step_dict["y"])
+        self.log(
+            f"val_{self.metric_name}_epoch",
+            self.val_metric,
+            on_step=False,
+            on_epoch=True,
+        )
 
-    @property
-    def output_dir(self) -> Path:
-        """Directory for saving output (default `'./eugene_output/'`)."""
-        return self._output_dir
-
-    @output_dir.setter
-    def output_dir(self, output_dir: Union[str, Path]):
-        self._output_dir = Path(output_dir).resolve()
+    def test_step(self, batch, batch_idx):
+        """Test step"""
+        step_dict = self._common_step(batch, batch_idx, "test")
+        self.log("test_loss", step_dict["loss"], on_step=False, on_epoch=True)
+        self.test_metric(step_dict["outs"], step_dict["y"])
+        self.log(
+            f"test_{self.metric_name}", self.test_metric, on_step=False, on_epoch=True
+        )
 
-    @property
-    def config_dir(self) -> Path:
-        """Directory for config files (default `'./eugene_config/'`)."""
-        return self._config_dir
-
-    @config_dir.setter
-    def config_dir(self, config_dir: Union[str, Path]):
-        self._config_dir = Path(config_dir).resolve()
+    def configure_metrics(self, metric, metric_kwargs):
+        """Configure metrics
+        Keeping this a function allows for the metric to be reconfigured
+        in inherited classes
+        TODO: add support for multiple metrics
+        Returns:
+        ----------
+        torchmetrics.Metric:
+            metric
+        """
+        metric_name = DEFAULT_TASK_METRICS[self.task] if metric is None else metric
+        metric_kwargs = (
+            metric_kwargs
+            if metric_kwargs is not None
+            else DEFAULT_METRIC_KWARGS[self.task]
+        )
+        metric = METRIC_REGISTRY[metric_name](
+            num_outputs=self.output_dim, **metric_kwargs
+        )
+        return metric, metric_kwargs, metric_name
 
-    @property
-    def figure_dir(self) -> Path:
-        """Directory for saving figures (default `'./eugene_figures/'`)."""
-        return self._figure_dir
+    def configure_optimizers(self):
+        """Configure optimizers
 
-    @figure_dir.setter
-    def figure_dir(self, figure_dir: Union[str, Path]):
-        self._figure_dir = Path(figure_dir).resolve()
+        Returns:
+        ----------
+        torch.optim.Optimizer:
+            optimizer
+        torch.optim.lr_scheduler._LRScheduler:
+            learning rate scheduler
+        """
+        optimizer = self.optimizer(
+            self.parameters(), lr=self.optimizer_lr, **self.optimizer_kwargs
+        )
+        if self.scheduler is None:
+            return optimizer
+        else:
+            scheduler = self.scheduler(optimizer, **self.scheduler_kwargs)
+            return {
+                "optimizer": optimizer,
+                "lr_scheduler": scheduler,
+                "monitor": self.scheduler_monitor,
+            }
+
+    def summary(self):
+        """Print a summary of the model"""
+        print(f"Model: {self.model.__class__.__name__}")
+        print(f"Sequence length: {self.input_len}")
+        print(f"Output dimension: {self.output_dim}")
+        print(f"Task: {self.task}")
+        print(f"Loss function: {self.loss_fxn.__name__}")
+        print(f"Optimizer: {self.optimizer.__name__}")
+        print(f"\tOptimizer parameters: {self.optimizer_kwargs}")
+        print(f"\tOptimizer starting learning rate: {self.optimizer_lr}")
+        print(
+            f"Scheduler: {self.scheduler.__name__}"
+        ) if self.scheduler is not None else print("Scheduler: None")
+        print(f"\tScheduler parameters: {self.scheduler_kwargs}")
+        print(f"Metric: {self.metric_name}")
+        print(f"\tMetric parameters: {self.metric_kwargs}")
+        print(f"Seed: {self.seed}")
+        print(f"Parameters summary:")
+        return ModelSummary(self.model)
+
+    @property
+    def model(self) -> nn.Module:
+        """Model"""
+        return self._model
+
+    @model.setter
+    def model(self, value: nn.Module):
+        """Set model"""
+        self._model = value
+
+    @property
+    def input_len(self) -> int:
+        """Input length"""
+        return self._input_len
+
+    @input_len.setter
+    def input_len(self, value: int):
+        """Set input length"""
+        self._input_len = value
+
+    @property
+    def output_dim(self) -> int:
+        """Output dimension"""
+        return self._output_dim
+
+    @output_dim.setter
+    def output_dim(self, value: int):
+        """Set output dimension"""
+        self._output_dim = value
+
+    @property
+    def task(self) -> str:
+        """Task"""
+        return self._task
+
+    @task.setter
+    def task(self, value: str):
+        """Set task"""
+        self._task = value
+
+    @property
+    def loss_fxn(self) -> Callable:
+        """Loss function"""
+        return self._loss_fxn
+
+    @loss_fxn.setter
+    def loss_fxn(self, value: Callable):
+        """Set loss function"""
+        self._loss_fxn = value
+
+    @property
+    def optimizer(self) -> Callable:
+        """Optimizer"""
+        return self._optimizer
+
+    @optimizer.setter
+    def optimizer(self, value: Callable):
+        """Set optimizer"""
+        self._optimizer = value
+
+    @property
+    def optimizer_lr(self) -> float:
+        """Optimizer starting learning rate"""
+        return self._optimizer_lr
+
+    @optimizer_lr.setter
+    def optimizer_lr(self, value: float):
+        """Set optimizer starting learning rate"""
+        self._optimizer_lr = value
+
+    @property
+    def scheduler(self) -> Callable:
+        """Scheduler"""
+        return self._scheduler
+
+    @scheduler.setter
+    def scheduler(self, value: Callable):
+        """Set scheduler"""
+        self._scheduler = value
+
+    @property
+    def train_metric(self) -> str:
+        """Train metric"""
+        return self._train_metric
+
+    @train_metric.setter
+    def train_metric(self, value: str):
+        """Set train metric"""
+        self._train_metric = value
 
+    @property
+    def seed(self) -> int:
+        """Seed"""
+        return self._seed
 
-settings = EugeneConfig()
+    @seed.setter
+    def seed(self, value: int):
+        """Set seed"""
+        self._seed = value
```

### Comparing `eugene-tools-0.0.6/eugene/conftest.py` & `eugene_tools-0.1.0/eugene/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,12 +36,14 @@
 
 # These fixtures provide a per test new copy of pbmc3k with some preprocessing run on it,
 # without having to hit the disk or recompute normalization.
 # The private fixture creates the object while the public one returns a deep copy.
 @pytest.fixture(scope="session")
 def _random1000():
     import eugene as eu
+
     return eu.datasets.random1000()
 
+
 @pytest.fixture
 def random1000(_random1000):
     return _random1000.copy()
```

### Comparing `eugene-tools-0.0.6/eugene/dataload/motif/_motif.py` & `eugene_tools-0.1.0/eugene/models/base/_towers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,330 +1,345 @@
-import numpy as np
-import pandas as pd
 import torch
-import re
-import os
-from dataclasses import dataclass
-from typing import Optional, Dict
-from io import TextIOBase
-from ...preprocess import decode_seq
-from ...preprocess._utils import _token2one_hot
-from ... import settings
-
-
-@dataclass
-class Motif:
-    """
-    Motif class for storing motif information.
-
-    Adapted from https://github.com/tobjores/Synthetic-Promoter-Designs-Enabled-by-a-Comprehensive-Analysis-of-Plant-Core-Promoters/blob/main/CNN/CNN_train%2Bevaluate.ipynb
-    """
-
-    identifier: str
-    pfm: np.ndarray
-    consensus: str
-    alphabet_length: int
-    length: int
-    name: Optional[str] = None
-    source_sites: Optional[int] = None
-    source_evalue: Optional[float] = None
-
-    def __len__(self) -> int:
-        return self.length
-
-
-class MinimalMEME:
-    """
-    Minimal MEME parser for MEME files.
-
-    Adapted from https://github.com/tobjores/Synthetic-Promoter-Designs-Enabled-by-a-Comprehensive-Analysis-of-Plant-Core-Promoters/blob/main/CNN/CNN_train%2Bevaluate.ipynb
-    MEME format: http://meme-suite.org/doc/meme-format.html
-    """
-
-    __version_regex = re.compile("^MEME version ([0-9]+)$")
-    __background_regex = re.compile(
-        "^Background letter frequencies(?: \(from (.+)\))?$"
-    )
-    __background_sum_error = 0.00001
-    __pfm_header_regex = re.compile(
-        "^letter-probability matrix:(?: alength= ([0-9]+))?(?: w= ([0-9]+))?(?: nsites= ([0-9]+))?(?: E= ([0-9.e-]+))?$"
-    )
-    version = None
-    alphabet = None
-    strands = None
-    background = None
-    background_source = None
-    motifs = None
-    consensus = None
-
-    def __init__(self, path):
-        self.motifs = {}
-
-        # parse the minimal MEME file
-        with open(path) as minimal_meme_file:
-            line = minimal_meme_file.readline()
-            # first line must be version
-            self.version = self._parse_version(line)
-
-            line = minimal_meme_file.readline()
-            while line:
-                if line.startswith("ALPHABET"):
-                    if self.alphabet is None:
-                        self.alphabet = self._parse_alphabet(line)
-                        line = minimal_meme_file.readline()
-                    else:
-                        raise RuntimeError(
-                            "Multiple alphabet definitions encountered in MEME file"
-                        )
-                elif line.startswith("strands: "):
-                    if self.strands is None:
-                        self.strands = self._parse_strands(line)
-                        line = minimal_meme_file.readline()
-                    else:
-                        raise RuntimeError(
-                            "Multiple strand definitions encountered in MEME file"
-                        )
-                elif line.startswith("Background letter frequencies"):
-                    if self.background is None:
-                        line = self._parse_background(line, minimal_meme_file)
-                    else:
-                        raise RuntimeError(
-                            "Multiple background frequency definitions encountered in MEME file"
-                        )
-                elif line.startswith("MOTIF"):
-                    line = self._parse_motif(line, minimal_meme_file)
-                else:
-                    line = minimal_meme_file.readline()
-
-    def _parse_version(self, line: str) -> str:
-        match = re.match(self.__version_regex, line)
-        if match:
-            return match.group(1)
-        else:
-            raise RuntimeError("Minimal MEME file missing version string on first line")
-
-    def _parse_alphabet(self, line: str) -> str:
-        if line.startswith("ALPHABET "):
-            raise NotImplementedError("Alphabet definitions not supported")
-        elif line.startswith("ALPHABET= "):
-            return line.rstrip()[10:]
-        else:
-            raise RuntimeError("Unable to parse alphabet line")
-
-    def _parse_strands(self, line: str) -> str:
-        strands = line.rstrip()[9:]
-        if not ((strands == "+") or (strands == "+ -")):
-            raise RuntimeError("Invalid strand specification")
-        else:
-            return strands
-
-    def _parse_background(self, line: str, handle: TextIOBase) -> str:
-        match = re.match(self.__background_regex, line)
-        if match:
-            if match.group(1) is not None:
-                self.background_source = match.group(1)
-        else:
-            raise RuntimeError("Unable to parse background frequency line")
-
-        self.background = {}
-        # start parsing possibly multiple lines of background frequencies
-        line = handle.readline()
-        while line:
-            if (not line.rstrip()) or line.startswith("MOTIF"):
-                if (
-                    abs(1 - sum(self.background.values()))
-                    <= self.__background_sum_error
-                ):
-                    return line
-                else:
-                    raise RuntimeError("Background frequencies do not sum to 1")
-            else:
-                line_freqs = line.rstrip().split(" ")
-                if len(line_freqs) % 2 != 0:
-                    raise RuntimeError("Invalid background frequency definition")
-                for residue, freq in zip(line_freqs[0::2], line_freqs[1::2]):
-                    self.background[residue] = float(freq)
-            line = handle.readline()
-
-    def _parse_motif(self, line: str, handle: TextIOBase) -> str:
-        # parse motif identifier
-        line_split = line.rstrip().split(" ")
-        if (len(line_split) < 2) or (len(line_split) > 3):
-            raise RuntimeError("Invalid motif name line")
-        motif_identifier = line_split[1]
-        motif_name = line_split[2] if len(line_split) == 3 else None
-
-        line = handle.readline()
-        # parse letter probability matrix header
-        if not line.startswith("letter-probability matrix:"):
-            raise RuntimeError(
-                "No letter-probability matrix header line in motif entry"
+from torch import nn
+import torch.nn.functional as F
+from inspect import signature
+from typing import Type, Dict, Union, Callable, List, Any
+from ._utils import get_output_size, get_conv1dblock_output_len
+from . import _layers as layers
+
+
+class Tower(nn.Module):
+    def __init__(
+        self,
+        block: Type[nn.Module],
+        repeats: int,
+        input_size: tuple,
+        static_block_args: Dict[str, Any] = None,
+        dynamic_block_args: Dict[str, Any] = None,
+        mults: Dict[str, float] = None,
+        name: str = "tower",
+    ):
+        """A tower of blocks.
+
+        Parameters
+        ----------
+        block : Type[nn.Module]
+        repeats : int
+        static_block_args : Dict[str, Any]
+            Arguments to initialize blocks that are static across repeats.
+        dynamic_block_args : Dict[str, Any]
+            Arguments to initialize blocks that change across repeats.
+        mults : Dict[str, float]
+            Multipliers for dynamic block arguments.
+        """
+        super().__init__()
+        self.input_size = input_size
+        self.repeats = repeats
+        self.block_name = block.__name__.lower()
+        self.name = name
+
+        blocks = nn.ModuleList()
+        if static_block_args is None:
+            static_block_args = {}
+        if dynamic_block_args is None:
+            dynamic_block_args = {}
+        if mults is None:
+            mults = {}
+
+        for arg, mult in mults.items():
+            # replace initial value with geometric progression
+            init_val = dynamic_block_args.get(
+                arg, signature(block).parameters[arg].default
             )
-        match = re.match(self.__pfm_header_regex, line)
-        if match:
-            motif_alphabet_length = (
-                int(match.group(1)) if match.group(1) is not None else None
-            )
-            motif_length = int(match.group(2)) if match.group(2) is not None else None
-            motif_source_sites = (
-                int(match.group(3)) if match.group(3) is not None else None
-            )
-            motif_source_evalue = (
-                float(match.group(4)) if match.group(4) is not None else None
+            dynamic_block_args[arg] = (
+                (
+                    init_val
+                    * torch.logspace(start=0, end=repeats - 1, steps=repeats, base=mult)
+                )
+                .to(dtype=signature(block).parameters[arg].annotation)
+                .tolist()
             )
+
+        self.blocks = nn.Sequential()
+        for i in range(repeats):
+            args = {arg: vals[i] for arg, vals in dynamic_block_args.items()}
+            args.update(static_block_args)
+            self.blocks.add_module(f"{self.block_name}_{i}", block(**args))
+
+        self.output_size = get_output_size(self.blocks, self.input_size)
+
+    def forward(self, x):
+        return self.blocks(x)
+
+
+class Conv1DTower(nn.Module):
+    def __init__(
+        self,
+        input_len: int,
+        input_channels: int,
+        conv_channels: list,
+        conv_kernels: list,
+        conv_strides: list = None,
+        conv_dilations: list = None,
+        conv_padding: Union[str, list] = "valid",
+        conv_biases: bool = True,
+        activations: Union[str, Callable, List[Union[str, Callable]]] = "relu",
+        pool_types: Union[str, Callable, List[Union[str, Callable]]] = "max",
+        pool_kernels: list = None,
+        pool_strides: list = None,
+        pool_dilations: list = None,
+        pool_padding: list = None,
+        dropout_rates: float = 0.0,
+        batchnorm: bool = False,
+        batchnorm_first: bool = False,
+    ):
+        super(Conv1DTower, self).__init__()
+
+        # Define input parameters
+        self.input_len = input_len
+        self.input_channels = input_channels
+
+        # Define convolutional layers
+        self.conv_channels = conv_channels
+        self.conv_kernels = conv_kernels
+        self.conv_strides = (
+            conv_strides if conv_strides is not None else [1] * len(conv_channels)
+        )
+        self.conv_dilations = (
+            conv_dilations if conv_dilations is not None else [1] * len(conv_channels)
+        )
+        self.conv_padding = (
+            conv_padding
+            if type(conv_padding) == list
+            else [conv_padding] * len(conv_channels)
+        )
+        self.conv_biases = (
+            conv_biases
+            if type(conv_biases) == list
+            else [conv_biases] * len(conv_channels)
+        )
+        assert (
+            len(self.conv_channels)
+            == len(self.conv_kernels)
+            == len(self.conv_strides)
+            == len(self.conv_dilations)
+            == len(self.conv_padding)
+            == len(self.conv_biases)
+        ), "Convolutional parameters must be of the same length"
+
+        # Define activation layers
+        activations = (
+            activations
+            if type(activations) == list
+            else [activations] * len(conv_channels)
+        )
+        self.activations = [
+            layers.ACTIVATION_REGISTRY[activation](inplace=False)
+            if isinstance(activation, str)
+            else activation
+            for activation in activations
+        ]
+
+        # Define pooling layers
+        pool_types = (
+            pool_types
+            if type(pool_types) == list
+            else [pool_types] * len(conv_channels)
+        )
+        self.pool_types = [
+            layers.POOLING_REGISTRY[pool_type]
+            if isinstance(pool_type, str)
+            else pool_type
+            for pool_type in pool_types
+        ]
+        self.pool_kernels = (
+            pool_kernels if pool_kernels is not None else [1] * len(self.pool_types)
+        )
+        self.pool_strides = (
+            pool_strides if pool_strides is not None else [1] * len(self.pool_types)
+        )
+        self.pool_padding = (
+            pool_padding if pool_padding is not None else [0] * len(self.pool_types)
+        )
+        self.pool_dilations = (
+            pool_dilations if pool_dilations is not None else [1] * len(self.pool_types)
+        )
+        assert (
+            len(self.pool_types)
+            == len(self.pool_kernels)
+            == len(self.pool_strides)
+            == len(self.pool_padding)
+            == len(self.pool_dilations)
+        ), "Pooling parameters must be of equal length"
+
+        # Define dropout layers
+        if dropout_rates != 0.0 and dropout_rates is not None:
+            if type(dropout_rates) == float:
+                self.dropout_rates = [dropout_rates] * len(conv_channels)
+            elif type(dropout_rates) == list:
+                self.dropout_rates = dropout_rates
         else:
-            raise RuntimeError("Unable to parse letter-probability matrix header")
+            self.dropout_rates = []
 
-        # parse letter probability matrix
-        line = handle.readline()
-        pfm_rows = []
-        while line:
-            if (not line.rstrip()) or line.startswith("MOTIF"):
-                if motif_identifier in self.motifs:
-                    raise RuntimeError("Motif identifiers not unique within file")
-                pfm = np.stack(pfm_rows)
-                if motif_length is None:
-                    motif_length = pfm.shape[0]
-                elif motif_length != pfm.shape[0]:
-                    raise RuntimeError(
-                        "Provided motif length is not consistent with the letter-probability matrix shape"
+        # Define batchnorm layers
+        self.batchnorm = batchnorm
+        self.batchnorm_first = batchnorm_first
+
+        # Build block
+        self.layers = nn.Sequential()
+        for i in range(len(conv_channels)):
+            # Add a convolutional layer
+            if i == 0:
+                self.layers.append(
+                    nn.Conv1d(
+                        self.input_channels,
+                        self.conv_channels[0],
+                        self.conv_kernels[0],
+                        stride=self.conv_strides[0],
+                        dilation=self.conv_dilations[0],
+                        padding=self.conv_padding[0],
                     )
-                consensus = decode_seq(_token2one_hot(pfm.argmax(axis=1)))
-                self.motifs[motif_identifier] = Motif(
-                    identifier=motif_identifier,
-                    pfm=pfm,
-                    consensus=consensus,
-                    alphabet_length=motif_alphabet_length,
-                    length=motif_length,
-                    name=motif_name,
-                    source_sites=motif_source_sites,
-                    source_evalue=motif_source_evalue,
                 )
-                return line
             else:
-                line_split = line.rstrip().split()
-                if motif_alphabet_length is None:
-                    motif_alphabet_length = len(line_split)
-                elif motif_alphabet_length != len(line_split):
-                    raise RuntimeError(
-                        "Letter-probability matrix row length doesn't equal alphabet length"
+                self.layers.append(
+                    nn.Conv1d(
+                        self.conv_channels[i - 1],
+                        self.conv_channels[i],
+                        self.conv_kernels[i],
+                        stride=self.conv_strides[i],
+                        dilation=self.conv_dilations[i],
+                        padding=self.conv_padding[i],
                     )
-                pfm_row = np.array([float(s) for s in line_split])
-                pfm_rows.append(pfm_row)
-                line = handle.readline()
-
-
-def _create_kernel_matrix(
-    size: tuple, motifs: Dict[str, Motif], convert_to_pwm=True
-) -> np.ndarray:
-    if len(size) != 3:
-        raise RuntimeError("Kernel matrix size must be a tuple of length 3")
-    kernel = torch.zeros(size)
-    torch.nn.init.xavier_uniform_(kernel)
-    for i, motif_id in enumerate(motifs):
-        motif = motifs[motif_id]
-        if convert_to_pwm:
-            new_weight = torch.tensor(
-                motif.pfm[: min(len(motif), kernel.shape[2]), :] / 0.25
-            ).transpose(0, 1)
-        else:
-            new_weight = torch.tensor(
-                motif.pfm[: min(len(motif), kernel.shape[2]), :]
-            ).transpose(0, 1)
-        kernel[i, :, : min(len(motif), kernel.shape[2])] = new_weight
-    return kernel
+                )
 
+            # Add a batchnorm layer if specified
+            if batchnorm and batchnorm_first:
+                self.layers.append(nn.BatchNorm1d(self.conv_channels[i]))
+
+            # Add an activation layer if specified
+            if i < len(self.activations):
+                if self.activations[i] is not None:
+                    self.layers.append(self.activations[i])
+
+            # Add a pooling layer if specified
+            if i < len(self.pool_types):
+                if self.pool_types[i] is not None:
+                    self.layers.append(
+                        self.pool_types[i](
+                            kernel_size=self.pool_kernels[i],
+                            stride=self.pool_strides[i],
+                            padding=self.pool_padding[i],
+                        )
+                    )
 
-def pwm_to_meme(pwm, output_file_path, vocab="DNA"):
-    """
-    Function to convert pwm as ndarray to meme file
-    Adapted from:: nnexplain GitHub:
+            # Add a dropout layer if specified
+            if i < len(self.dropout_rates):
+                if self.dropout_rates[i] is not None:
+                    self.layers.append(nn.Dropout(self.dropout_rates[i]))
+
+            # Add a batchnorm layer if specified
+            if self.batchnorm and not self.batchnorm_first:
+                self.layers.append(nn.BatchNorm1d(conv_channels[i]))
+
+        # Define output parameters
+        self.out_channels = self.conv_channels[-1]
+        self.output_len = get_conv1dblock_output_len(
+            self.layers, input_len=self.input_len
+        )
+        self.flatten_dim = self.output_len * self.out_channels
+
+    def forward(self, x):
+        return self.layers(x)
+
+
+class BiConv1DTower(nn.Module):
+    """Generates a PyTorch module with the convolutional architecture described in:
+    TODO: Add paper reference
+    Will be deprecated in favor of Conv1D blocks wrapped by a Tower in the future
 
     Parameters
     ----------
-    pwm:
-        numpy.array, pwm matrices, shape (U, 4, filter_size), where U - number of units
-    output_file_path:
-        string, the name of the output meme file
+    input_len : int
+        Length of the input sequence
+    filters : int
+        Number of filters in the convolutional layers. Applies the same number to all layers
+    kernel_size : int
+        Size of the kernel in the convolutional layers. Applies the same size to all layers
+    layers : int
+        Number of convolutional layers
+    stride : int
+        Stride of the convolutional layers. Applies the same stride to all layers
+    dropout_rate : float
+        Dropout rate of the convolutional layers. Applies the same rate to all layers
+
+    Returns
+    -------
+    torch.nn.Module
+        TODO: Add description
     """
-    from ...preprocess._utils import _get_vocab
 
-    vocab = "".join(_get_vocab(vocab))
-    n_filters = pwm.shape[0]
-    filter_size = pwm.shape[2]
-    meme_file = open(output_file_path, "w")
-    meme_file.write("MEME version 4\n\n")
-    meme_file.write(f"ALPHABET= {vocab}\n\n")
-    meme_file.write("strands: + -\n\n")
-    meme_file.write("Background letter frequencies\n")
-    meme_file.write(
-        f"{vocab[0]} 0.25 {vocab[1]} 0.25 {vocab[2]} 0.25 {vocab[3]} 0.25\n"
-    )
-
-    print("Saved PWM File as : {}".format(output_file_path))
-
-    for i in range(0, n_filters):
-        if np.sum(pwm[i, :, :]) > 0:
-            meme_file.write("\n")
-            meme_file.write("MOTIF filter%s\n" % i)
-            meme_file.write(
-                "letter-probability matrix: alength= 4 w= %d \n"
-                % np.count_nonzero(np.sum(pwm[i, :, :], axis=0))
+    def __init__(
+        self,
+        filters: int,
+        kernel_size: int,
+        input_size: int = 4,
+        layers: int = 1,
+        stride: int = 1,
+        dropout_rate: float = 0.15,
+    ):
+        super().__init__()
+        self.filters = filters
+        self.kernel_size = kernel_size
+        self.input_size = input_size
+        if layers < 1:
+            raise ValueError("At least one layer needed")
+        self.layers = layers
+        if (dropout_rate < 0) or (dropout_rate > 1):
+            raise ValueError("Dropout rate must be a float between 0 and 1")
+        self.dropout_rate = dropout_rate
+        self.stride = stride
+
+        self.kernels = nn.ParameterList()
+        self.biases = nn.ParameterList()
+        kernel = nn.Parameter(torch.zeros(self.filters, self.input_size, kernel_size))
+        nn.init.xavier_uniform_(kernel)
+        self.kernels.append(kernel)
+        bias = nn.Parameter(torch.zeros(filters))
+        nn.init.zeros_(bias)
+        self.biases.append(bias)
+        for layer in range(1, self.layers):
+            kernel = nn.Parameter(
+                torch.empty((self.filters, self.filters, self.kernel_size))
             )
-
-        for j in range(0, filter_size):
-            if np.sum(pwm[i, :, j]) > 0:
-                meme_file.write(
-                    str(pwm[i, 0, j])
-                    + "\t"
-                    + str(pwm[i, 1, j])
-                    + "\t"
-                    + str(pwm[i, 2, j])
-                    + "\t"
-                    + str(pwm[i, 3, j])
-                    + "\n"
-                )
-
-    meme_file.close()
-
-
-def filters_to_meme_sdata(
-    sdata,
-    output_dir: str = None,
-    file_name="filter.meme",
-    uns_key="pfms",
-    filter_ids: int = None,
-    vocab="DNA",
-    convert_to_pfm: bool = False,
-    change_length_axis=True,
-    return_pfms=False,
-):
-    """
-    Function to convert a single filter to a meme file
-
-    sdata:
-        SingleData, single cell data
-    filter_ids:
-        int, index of the filter to convert
-    output_file_path:
-        string, the name of the output meme file
-    convert_to_pwm:
-        bool, whether to convert the filter to a pwm
-    """
-    try:
-        pfms = sdata.uns.get(uns_key)
-    except KeyError:
-        print("No filters found in sdata.uns['{}']".format(uns_key))
-    if filter_ids is None:
-        filter_ids = list(sdata.uns[uns_key].keys())
-    if output_dir is None:
-        output_file_path = os.path.join(settings.output_dir, file_name)
-    else:
-        output_file_path = os.path.join(output_dir, file_name)
-    pwms = np.array([pfms[key].values for key in filter_ids])
-    if convert_to_pfm:
-        pwms / pwms.sum(axis=2, keepdims=True)
-    if change_length_axis:
-        pwms = pwms.transpose(0, 2, 1)
-    pwm_to_meme(pwms, output_file_path, vocab=vocab)
-    if return_pfms:
-        return pwms
+            nn.init.xavier_uniform_(kernel)
+            self.kernels.append(kernel)
+            bias = nn.Parameter(torch.empty((self.filters)))
+            nn.init.zeros_(bias)
+            self.biases.append(bias)
+
+    def forward(self, x):
+        x_fwd = F.conv1d(x, self.kernels[0], stride=self.stride, padding="same")
+        x_fwd = torch.add(x_fwd.transpose(1, 2), self.biases[0]).transpose(1, 2)
+        x_fwd = F.dropout(F.relu(x_fwd), p=self.dropout_rate, training=self.training)
+        x_rev = F.conv1d(
+            x,
+            torch.flip(self.kernels[0], dims=[0, 1]),
+            stride=self.stride,
+            padding="same",
+        )
+        x_rev = torch.add(x_rev.transpose(1, 2), self.biases[0]).transpose(1, 2)
+        x_rev = F.dropout(F.relu(x_rev), p=self.dropout_rate, training=self.training)
+        for layer in range(1, self.layers):
+            x_fwd = F.conv1d(
+                x_fwd, self.kernels[layer], stride=self.stride, padding="same"
+            )
+            x_fwd = torch.add(x_fwd.transpose(1, 2), self.biases[layer]).transpose(1, 2)
+            x_fwd = F.dropout(F.relu(x_fwd), p=self.dropout_rate, training=self.training)
+            x_rev = F.conv1d(
+                x_rev,
+                torch.flip(self.kernels[layer], dims=[0, 1]),
+                stride=self.stride,
+                padding="same",
+            )
+            x_rev = torch.add(x_rev.transpose(1, 2), self.biases[layer]).transpose(1, 2)
+            x_rev = F.dropout(F.relu(x_rev), p=self.dropout_rate, training=self.training)
+        return torch.add(x_fwd, x_rev)
```

### Comparing `eugene-tools-0.0.6/eugene/evaluate/_metrics.py` & `eugene_tools-0.1.0/eugene/evaluate/metrics/_binary_classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     Parameters
     ----------
     y_true : array-like
         The true binary labels. Assumed to be 1 for positive and 0 for negative.
     y_score : array-like
         The scores predicted by a model
-    
+
     Returns
     -------
     median : float
         The median of the scores in y_score for the positive class labels in y_true.
     """
     if isinstance(y_score, pd.Series):
         y_score = y_score.values
@@ -50,15 +50,15 @@
     y_score = y_score[nan_mask]
     return roc_auc_score(y_true, y_score)
 
 
 def escore(y_true, y_score):
     """
     Calculate the E-score for a binary y_true against scores in y_score.
-    The E-score is 
+    The E-score is
 
     Parameters
     ----------
     y_true : array-like
         The true binary labels. Assumed to be 1 for positive and 0 for negative.
     y_score : array-like
         The scores predicted by a model
```

### Comparing `eugene-tools-0.0.6/eugene/evaluate/_predict.py` & `eugene_tools-0.1.0/eugene/evaluate/_predict.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,255 +1,249 @@
 import os
 import numpy as np
 import pandas as pd
 from typing import Union, List
 from torch.utils.data import DataLoader
-from pytorch_lightning import LightningModule, Trainer, seed_everything
-from ..dataload import SeqData, SeqDataset
-from ..utils._decorators import track
-from .._settings import settings
+from pytorch_lightning import LightningModule, Trainer
+from eugene import settings
+import xarray as xr
+import seqdata as sd
+from ._utils import PredictionWriter
 
 
-@track
 def predictions(
     model: LightningModule,
-    sdata: SeqData = None,
-    target_keys: Union[str, List[str]] = None,
+    dataloader: DataLoader,
     gpus: int = None,
-    batch_size: int = None,
-    num_workers: int = None,
-    store_only: bool = False,
     out_dir: os.PathLike = None,
     name: str = None,
     version: str = "",
     file_label: str = "",
-    prefix: str = "",
-    suffix: str = "",
-    sdataset: SeqDataset = None,
-    sdataloader: DataLoader = None,
-    seq_transforms: List = None,
-    transform_kwargs: dict = {},
-    copy: bool = False,
 ):
-    """Predict the outputs of sequences in a SeqData object using a model.
-
-    Parameters
-    ----------
-
-    model: LightningModule
-       The model to predict on.
-    sdata: SeqData
-       The data to predict on.
-    target_keys: Union[str, List[str]]
-       The target_keys to predict on.
-    gpus: int
-       The number of GPUs to use.
-    batch_size: int
-       The batch size to use.
-    num_workers: int
-       The number of workers to use.
-    out_dir: os.PathLike
-       The directory to save the predictions to.
-    name: str
-       The name of the model.
-    version: str
-       The version of the model.
-    file_label: str
-       The label to add to the file name.
-    sdataset: SeqDataset
-       The dataset to predict on.
-    sdataloader: DataLoader
-       The dataloader to predict on.
-    seq_transforms: List
-       The sequence transforms to use.
-    transform_kwargs: dict
-       The transform kwargs to use.
-    copy: bool
-       Whether to copy the SeqData or not.
-
-    Returns
-    -------
-    sdata
-         The SeqData object with the predictions added if copy is True.
-    """
     gpus = gpus if gpus is not None else settings.gpus
-    batch_size = batch_size if batch_size is not None else settings.batch_size
-    num_workers = num_workers if num_workers is not None else settings.dl_num_workers
-    target_keys = [target_keys] if type(target_keys) == str else target_keys
-    out_dir = out_dir if out_dir is not None else settings.output_dir
-    model_name = model.strand + model.__class__.__name__ + "_" + model.task
+    model_name = model.model_name
     name = name if name is not None else model_name
-    out_dir = os.path.join(out_dir, name, version)
-
-    # Save the final predictions to sdata if applicable
-    if sdata is not None:
-        if sdata.names is None:
-            sdata.names = sdata.seqs_annot.index
-        sdataset = sdata.to_dataset(
-            target_keys=target_keys,
-            seq_transforms=seq_transforms,
-            transform_kwargs=transform_kwargs,
-        )
-        sdataloader = sdataset.to_dataloader(
-            batch_size=batch_size, num_workers=num_workers, shuffle=False
-        )
-    elif sdataset is not None:
-        sdataloader = sdataset.to_dataloader(
-            batch_size=batch_size, num_workers=num_workers, shuffle=False
-        )
-    else:
-        assert sdataloader is not None, "No data to predict on."
-    if not store_only:
-        from ..utils._custom_callbacks import PredictionWriter
+    if out_dir is not None:
+        out_dir = os.path.join(out_dir, name, version)
         predictor = Trainer(
             logger=False,
             callbacks=PredictionWriter(output_dir=out_dir, file_label=file_label),
-            gpus=gpus,
+            devices=gpus,
         )
     else:
-        predictor = Trainer(logger=False, gpus=gpus)
-    ps = np.concatenate(predictor.predict(model, sdataloader), axis=0)
+        predictor = Trainer(logger=False, devices=gpus)
+    ps = np.concatenate(predictor.predict(model, dataloader), axis=0)
     num_outs = model.output_dim
-    preds = pd.DataFrame(index=ps[:, 0], data=ps[:, 1 : num_outs + 1])
-    sannot_cols = [f"{prefix}{lab}_predictions{suffix}" for lab in target_keys]
-    ordered_preds = preds.loc[sdata.seqs_annot.index].astype(float)
-    sdata.seqs_annot[sannot_cols] = ordered_preds
-    return sdata if copy else None
+    preds = pd.DataFrame(data=ps[:, 0:num_outs])
+    preds.columns = [f"predictions_{i}" for i in range(num_outs)]
+    return preds
 
 
-@track
-def train_val_predictions(
+def predictions_sequence_module(
     model: LightningModule,
-    sdata: SeqData = None,
+    sdata=None,
+    seq_key: str = "ohe_seq",
     target_keys: Union[str, List[str]] = None,
-    train_key: str = "train_val",
     gpus: int = None,
     batch_size: int = None,
     num_workers: int = None,
+    transforms: List = None,
+    prefetch_factor: int = None,
+    store_only: bool = False,
+    in_memory: bool = False,
     out_dir: os.PathLike = None,
     name: str = None,
     version: str = "",
+    file_label: str = "",
     prefix: str = "",
     suffix: str = "",
-    train_dataset: SeqDataset = None,
-    val_dataset: SeqDataset = None,
-    train_dataloader: DataLoader = None,
-    val_dataloader: DataLoader = None,
-    seq_transforms: List = None,
-    transform_kwargs: dict = {},
     copy: bool = False,
 ):
-    """
-    Predict the outputs of sequences split into training and validation in a SeqData object using a model.
-    This is mostly just a helper for separating sequences based on the train_key column of seqs_annot. This operates
-    under the assumption that the train_key is True for training sequences and False for validation sequences.
-
-    Params:
-    -------
-
-    model: LightningModule
-       The model to predict on.
-    sdata: SeqData
-       The data to predict on.
-    target_keys: Union[str, List[str]]
-       The target_keys to predict on.
-    gpus: int
-       The number of GPUs to use.
-    batch_size: int
-       The batch size to use.
-    num_workers: int
-       The number of workers to use.
-    out_dir: os.PathLike
-       The directory to save the predictions to.
-    name: str
-       The name of the model.
-    version: str
-       The version of the model.
-    file_label: str
-       The label to add to the file name.
-    sdataset: SeqDataset
-       The dataset to predict on.
-    sdataloader: DataLoader
-       The dataloader to predict on.
-    seq_transforms: List
-       The sequence transforms to use.
-    transform_kwargs: dict
-       The transform kwargs to use.
-    copy: bool
-       Whether to copy the data or not.
-
-    Returns:
-    --------
-
-    """
-    gpus = gpus if gpus is not None else settings.gpus
+    sdata = sdata.copy() if copy else sdata
     batch_size = batch_size if batch_size is not None else settings.batch_size
     num_workers = num_workers if num_workers is not None else settings.dl_num_workers
     target_keys = [target_keys] if type(target_keys) == str else target_keys
-    out_dir = out_dir if out_dir is not None else settings.output_dir
-    model_name = model.strand + model.__class__.__name__ + "_" + model.task
-    name = name if name is not None else model_name
-    out_dir = os.path.join(out_dir, name, version)
-
-    # Save the final predictions to sdata if applicable
-    if train_dataloader is not None:
-        assert val_dataloader is not None
-    elif train_dataset is not None:
-        assert val_dataset is not None
-        train_dataloader = DataLoader(
-            train_dataset, batch_size=batch_size, num_workers=num_workers, shuffle=False
-        )
-        val_dataloader = DataLoader(
-            val_dataset, batch_size=batch_size, num_workers=num_workers, shuffle=False
-        )
-    elif sdata is not None:
-        train_idx = np.where(sdata.seqs_annot[train_key] == True)[0]
-        train_dataset = sdata[train_idx].to_dataset(
-            target_keys=target_keys,
-            seq_transforms=seq_transforms,
-            transform_kwargs=transform_kwargs,
-        )
-        train_dataloader = train_dataset.to_dataloader(
-            batch_size=batch_size, num_workers=num_workers, shuffle=False
-        )
-        val_idx = np.where(sdata.seqs_annot[train_key] == False)[0]
-        val_dataset = sdata[val_idx].to_dataset(
-            target_keys=target_keys,
-            seq_transforms=seq_transforms,
-            transform_kwargs=transform_kwargs,
-        )
-        val_dataloader = val_dataset.to_dataloader(
-            batch_size=batch_size, num_workers=num_workers, shuffle=False
+    if not store_only:
+        out_dir = out_dir if out_dir is not None else settings.output_dir
+    if target_keys is not None:
+        if isinstance(target_keys, str):
+            target_keys = [target_keys]
+        if len(target_keys) == 1:
+            sdata["target"] = sdata[target_keys[0]]
+        else:
+            sdata["target"] = xr.concat(
+                [sdata[target_key] for target_key in target_keys], dim="_targets"
+            ).transpose("_sequence", "_targets")
+    if in_memory:
+        print(f"Loading {seq_key} and {target_keys} into memory")
+        sdata[seq_key].load()
+        sdata["target"].load()
+    dataloader = sd.get_torch_dataloader(
+        sdata,
+        sample_dims=["_sequence"],
+        variables=[seq_key, "target"],
+        batch_size=batch_size,
+        num_workers=num_workers,
+        prefetch_factor=prefetch_factor,
+        transforms=transforms,
+        shuffle=False,
+    )
+    preds = predictions(
+        model=model,
+        dataloader=dataloader,
+        gpus=gpus,
+        out_dir=out_dir,
+        name=name,
+        version=version,
+        file_label=file_label,
+    )
+    pred_cols = preds.columns
+    for i, target_key in enumerate(target_keys):
+        # print(f"Adding {prefix}{target_key}_predictions{suffix} to sdata")
+        sdata[f"{prefix}{target_key}_predictions{suffix}"] = xr.DataArray(
+            preds[pred_cols[i]].values, dims=["_sequence"]
         )
-    else:
-        raise ValueError("No data to predict on.")
-    if out_dir is not None:
-        from ..utils._custom_callbacks import PredictionWriter
+    return sdata if copy else None
+
 
+def train_val_predictions(
+    model: LightningModule,
+    train_dataloader: DataLoader,
+    val_dataloader: DataLoader,
+    train_key="train_val",
+    gpus: int = None,
+    out_dir: os.PathLike = None,
+    name: str = None,
+    version: str = "",
+):
+    gpus = gpus if gpus is not None else settings.gpus
+    model_name = model.model_name
+    name = name if name is not None else model_name
+    if out_dir is not None:
+        out_dir = os.path.join(out_dir, name, version)
         train_predictor = Trainer(
             logger=False,
             callbacks=PredictionWriter(out_dir, file_label="train"),
-            gpus=gpus,
+            devices=gpus,
         )
         val_predictor = Trainer(
             logger=False,
             callbacks=PredictionWriter(out_dir, file_label="val"),
-            gpus=gpus,
+            devices=gpus,
         )
     else:
-        train_predictor = Trainer(logger=False, gpus=gpus)
-        val_predictor = Trainer(logger=False, gpus=gpus)
+        train_predictor = Trainer(logger=False, devices=gpus)
+        val_predictor = Trainer(logger=False, devices=gpus)
 
     t = np.concatenate(train_predictor.predict(model, train_dataloader), axis=0)
     v = np.concatenate(val_predictor.predict(model, val_dataloader), axis=0)
     num_outs = model.output_dim
     preds = pd.concat(
         [
-            pd.DataFrame(index=t[:, 0], data=t[:, 1 : num_outs + 1]),
-            pd.DataFrame(index=v[:, 0], data=v[:, 1 : num_outs + 1]),
+            pd.DataFrame(data=t[:, 0:num_outs]),
+            pd.DataFrame(data=v[:, 0:num_outs]),
         ],
         axis=0,
+    ).reset_index(drop=True)
+    preds.columns = [f"predictions_{i}" for i in range(num_outs)]
+    preds[train_key] = [True] * len(t) + [False] * len(v)
+    return preds
+
+
+def train_val_predictions_sequence_module(
+    model: LightningModule,
+    sdata=None,
+    seq_key: str = "ohe_seq",
+    target_keys: Union[str, List[str]] = None,
+    train_key="train_val",
+    gpus: int = None,
+    batch_size: int = None,
+    num_workers: int = None,
+    transforms: List = None,
+    prefetch_factor: int = None,
+    store_only: bool = False,
+    in_memory: bool = False,
+    out_dir: os.PathLike = None,
+    name: str = None,
+    version: str = "",
+    prefix: str = "",
+    suffix: str = "",
+    copy: bool = False,
+):
+    # Set-up dataloaders
+    sdata = sdata.copy() if copy else sdata
+    batch_size = batch_size if batch_size is not None else settings.batch_size
+    num_workers = num_workers if num_workers is not None else settings.dl_num_workers
+    target_keys = [target_keys] if type(target_keys) == str else target_keys
+    if not store_only:
+        out_dir = out_dir if out_dir is not None else settings.output_dir
+    if target_keys is not None:
+        if isinstance(target_keys, str):
+            target_keys = [target_keys]
+        if len(target_keys) == 1:
+            sdata["target"] = sdata[target_keys[0]]
+        else:
+            sdata["target"] = xr.concat(
+                [sdata[target_key] for target_key in target_keys], dim="_targets"
+            ).transpose("_sequence", "_targets")
+    if in_memory:
+        print(f"Loading {seq_key} and {target_keys} into memory")
+        sdata[seq_key].load()
+        sdata["target"].load()
+    sdata[train_key].load()
+    train_sdata = sdata.where(sdata[train_key] == 1, drop=True)
+    val_sdata = sdata.where(sdata[train_key] == 0, drop=True)
+    train_dataloader = sd.get_torch_dataloader(
+        train_sdata,
+        sample_dims=["_sequence"],
+        variables=[seq_key, "target"],
+        batch_size=batch_size,
+        num_workers=num_workers,
+        prefetch_factor=prefetch_factor,
+        transforms=transforms,
+        shuffle=False,
+        drop_last=False,
+    )
+    val_dataloader = sd.get_torch_dataloader(
+        val_sdata,
+        sample_dims=["_sequence"],
+        variables=[seq_key, "target"],
+        batch_size=batch_size,
+        num_workers=num_workers,
+        prefetch_factor=prefetch_factor,
+        transforms=transforms,
+        shuffle=False,
+        drop_last=False,
+    )
+
+    # Predict with train_val_predictions function
+    preds = train_val_predictions(
+        model=model,
+        train_dataloader=train_dataloader,
+        val_dataloader=val_dataloader,
+        gpus=gpus,
+        out_dir=out_dir,
+        name=name,
+        version=version,
     )
-    sdata.seqs_annot[
-        [f"{prefix}{label}_predictions{suffix}" for label in target_keys]
-    ] = preds.loc[sdata.seqs_annot.index].astype(float)
+
+    # Create an empty dataframe the same size as preds
+    ordered_preds = pd.DataFrame(index=preds.index, columns=preds.columns).drop(
+        columns=["train_val"]
+    )
+
+    # Grab the train and val predictions and put them in the right place
+    train_preds = preds[preds[train_key] == True].drop(columns=["train_val"])
+    train_pred_index = np.where(sdata[train_key].values == 1)[0]
+    val_preds = preds[preds[train_key] == False].drop(columns=["train_val"])
+    val_pred_index = np.where(sdata[train_key].values == 0)[0]
+    ordered_preds.iloc[train_pred_index] = train_preds
+    ordered_preds.iloc[val_pred_index] = val_preds
+
+    # Add the predictions to the sdata
+    pred_cols = ordered_preds.columns
+    for i, target_key in enumerate(target_keys):
+        # print(f"Adding {prefix}{target_key}_predictions{suffix} to sdata")
+        sdata[f"{prefix}{target_key}_predictions{suffix}"] = xr.DataArray(
+            ordered_preds[pred_cols[i]].values, dims=["_sequence"]
+        )
     return sdata if copy else None
```

### Comparing `eugene-tools-0.0.6/eugene/models/_sota_models.py` & `eugene_tools-0.1.0/eugene/models/zoo/_tf_binding_predictors.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,30 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from .base import BaseModel, BasicFullyConnectedModule, BasicConv1D
-from .base._utils import GetFlattenDim
+from ..base import _layers as layers
+from ..base import _blocks as blocks
+from ..base import _towers as towers
 
 
-mode_dict = {"dna": 1, "rbp": 2}
-
-
-class DeepBind(BaseModel):
+class DeepBind(nn.Module):
     """
     DeepBind model implemented from Alipanahi et al 2015 in PyTorch
 
-    DeepBind is a model that takes in a DNA or RNA sequence and outputs a probability of 
+    DeepBind is a model that takes in a DNA or RNA sequence and outputs a probability of
     binding for a given DNA transcription factor or RNA binding protein respectively.
     This is a flexible implementation of the original DeepBind architecture that allows users
     to modify the number of convolutional layers, the number of fully connected layers, and
     many more hyperparameters. If parameters for the CNN and FCN are not passed in, the model
     will be instantiated with the parameters described in Alipanahi et al 2015.
 
     Like the original DeepBind models, this model can be used for both DNA and RNA binding. For DNA,
-    we implemented the "dna" mode which only uses the max pooling of the representation generated by 
+    we implemented the "dna" mode which only uses the max pooling of the representation generated by
     the convolutional layers. For RNA, we implemented the "rbp" mode which uses both the max and average
     pooling of the representation generated by the convolutional layers.
-    - For "ss" models, we use the representation generated by the convolutional layers and pass that through a 
-        set of fully connected layer to generate the output.
-    - For "ds" models, we use the representation generated by the convolutional layers for both the forward and 
-        reverse complement strands and pass that through the same set of fully connected layers to generate the output.
-    - For "ts" models, we use the representation generated by separate sets of convolutional layers for the forward and
-        reverse complement strands and passed that through separate sets of fully connected layers to generate the output.
-    
-    aggr defines how the output for "ds" and "ts" models is generated. If "max", we take the max of the forward and reverse
-    complement outputs. If "avg", we take the average of the forward and reverse complement outputs. There is no "concat" for
-    the current implementation of DeepBind models.
 
     Parameters
     ----------
     input_len : int
         Length of input sequence
     output_dim : int
         Number of output classes
@@ -58,186 +46,249 @@
         Scheduler of model, either "lr_scheduler" or "plateau"
     scheduler_patience : int
         Scheduler patience of model
     mp_kwargs : dict
         Keyword arguments for multiprocessing
     conv_kwargs : dict
         Keyword arguments for convolutional layers
-    fc_kwargs : dict
+    dense_kwargs : dict
         Keyword arguments for fully connected layers
     """
+
     def __init__(
         self,
         input_len: int,
         output_dim: int,
-        strand: str = "ss",
-        task: str = "regression",
-        aggr: str = "max",
-        loss_fxn: str ="mse",
-        mode: str = "rbp",
         conv_kwargs: dict = {},
-        fc_kwargs: dict = {},
-        **kwargs
+        dense_kwargs: dict = {},
+        mode: str = "rbp",
     ):
-        super().__init__(
-            input_len, 
-            output_dim, 
-            strand=strand, 
-            task=task, 
-            aggr=aggr, 
-            loss_fxn=loss_fxn, 
-            **kwargs
-        )
-        self.conv_kwargs, self.fc_kwargs = self.kwarg_handler(conv_kwargs, fc_kwargs)
+        super(DeepBind, self).__init__()
+
+        # Set the attributes
+        self.input_len = input_len
+        self.output_dim = output_dim
         self.mode = mode
-        self.mode_multiplier = mode_dict[self.mode]
-        self.aggr = aggr
-        self.convnet = BasicConv1D(input_len=input_len, **self.conv_kwargs)
-        self.pool_dim = GetFlattenDim(self.convnet.module, seq_len=input_len)
+        self.mode_dict = {"dna": 1, "rbp": 2}
+        self.mode_multiplier = self.mode_dict[self.mode]
+        self.conv_kwargs, self.dense_kwargs = self.kwarg_handler(
+            conv_kwargs, dense_kwargs
+        )
+
+        # Create the blocks
+        self.conv1d_tower = towers.Conv1DTower(**self.conv_kwargs)
+        self.pool_dim = self.conv1d_tower.output_len
         self.max_pool = nn.MaxPool1d(kernel_size=self.pool_dim)
         self.avg_pool = nn.AvgPool1d(kernel_size=self.pool_dim)
-        if self.strand == "ss":
-            self.fcn = BasicFullyConnectedModule(
-                input_dim=self.convnet.out_channels * self.mode_multiplier,
-                output_dim=output_dim,
-                **self.fc_kwargs
-            )
-        elif self.strand == "ds":
-            self.fcn = BasicFullyConnectedModule(
-                input_dim=self.convnet.out_channels * self.mode_multiplier,
-                output_dim=output_dim,
-                **self.fc_kwargs
-            )
-        elif self.strand == "ts":
-            self.fcn = BasicFullyConnectedModule(
-                self.convnet.out_channels * self.mode_multiplier,
-                output_dim=output_dim,
-                **self.fc_kwargs
-            )
-            self.reverse_convnet = BasicConv1D(
-                input_len=input_len, 
-                **self.conv_kwargs
-                )
-            self.reverse_fcn = BasicFullyConnectedModule(
-                self.convnet.out_channels * self.mode_multiplier,
-                output_dim=output_dim,
-                **self.fc_kwargs
-            )
+        self.dense_block = blocks.DenseBlock(
+            input_dim=self.conv1d_tower.out_channels * self.mode_multiplier,
+            output_dim=output_dim,
+            **self.dense_kwargs
+        )
 
-    def forward(self, x, x_rev_comp=None):
-        x = self.convnet(x)
+    def forward(self, x):
+        x = self.conv1d_tower(x)
         if self.mode == "rbp":
             x = torch.cat((self.max_pool(x), self.avg_pool(x)), dim=1)
-            x = x.view(x.size(0), self.convnet.out_channels * 2)
+            x = x.view(x.size(0), self.conv1d_tower.out_channels * 2)
         elif self.mode == "dna":
             x = self.max_pool(x)
-            x = x.view(x.size(0), self.convnet.out_channels)
-        x = self.fcn(x)
-        if self.strand == "ds":
-            x_rev_comp = self.convnet(x_rev_comp)
-            if self.mode == "rbp":
-                x_rev_comp = torch.cat((self.max_pool(x_rev_comp), self.avg_pool(x_rev_comp)), dim=1)
-                x_rev_comp = x_rev_comp.view(x_rev_comp.size(0), self.convnet.out_channels * 2)
-            elif self.mode == "dna":
-                x_rev_comp = self.max_pool(x_rev_comp)
-                x_rev_comp = x_rev_comp.view(x_rev_comp.size(0), self.convnet.out_channels)
-            x_rev_comp = self.fcn(x_rev_comp)
-            if self.aggr == "max":
-                x = F.max_pool1d(torch.cat((x, x_rev_comp), dim=1), 2)
-            elif self.aggr == "avg":
-                x = torch.mean(torch.cat((x, x_rev_comp), dim=1), dim=1).unsqueeze(dim=1)
-        elif self.strand == "ts":
-            x_rev_comp = self.reverse_convnet(x_rev_comp)
-            if self.mode == "rbp":
-                x_rev_comp = torch.cat((self.max_pool(x_rev_comp), self.avg_pool(x_rev_comp)), dim=1)
-                x_rev_comp = x_rev_comp.view(x_rev_comp.size(0), self.convnet.out_channels * 2)
-            elif self.mode == "dna":
-                x_rev_comp = self.max_pool(x_rev_comp)
-                x_rev_comp = x_rev_comp.view(x_rev_comp.size(0), self.convnet.out_channels)
-            x_rev_comp = self.reverse_fcn(x_rev_comp)
-            if self.aggr == "max":
-                x = F.max_pool1d(torch.cat((x, x_rev_comp), dim=1), 2)
-            elif self.aggr == "avg":
-                x = torch.mean(torch.cat((x, x_rev_comp), dim=1), dim=1).unsqueeze(dim=1)
+            x = x.view(x.size(0), self.conv1d_tower.out_channels)
+        x = self.dense_block(x)
         return x
 
-    def kwarg_handler(self, conv_kwargs, fc_kwargs):
+    def kwarg_handler(self, conv_kwargs, dense_kwargs):
         """Sets default kwargs for conv and fc modules if not specified"""
-        conv_kwargs.setdefault("channels", [4, 16])
+        conv_kwargs.setdefault("input_len", self.input_len)
+        conv_kwargs.setdefault("input_channels", 4)
+        conv_kwargs.setdefault("conv_channels", [16])
         conv_kwargs.setdefault("conv_kernels", [16])
-        conv_kwargs.setdefault("pool_kernels", None)
-        conv_kwargs.setdefault("omit_final_pool", True)
+        conv_kwargs.setdefault("pool_types", None)
         conv_kwargs.setdefault("dropout_rates", 0.25)
         conv_kwargs.setdefault("batchnorm", False)
-        fc_kwargs.setdefault("hidden_dims", [32])
-        fc_kwargs.setdefault("dropout_rate", 0.25)
-        fc_kwargs.setdefault("batchnorm", False)
-        return conv_kwargs, fc_kwargs
+        dense_kwargs.setdefault("hidden_dims", [32])
+        dense_kwargs.setdefault("dropout_rates", 0.25)
+        dense_kwargs.setdefault("batchnorm", False)
+        return conv_kwargs, dense_kwargs
 
 
-class DeepSEA(BaseModel):
-    """DeepSEA model implementation for EUGENe
-    
-    Default parameters are those specified in the DeepSEA paper. We currently do not implement a "ds" or "ts" model
-    for DeepSEA.
+class ResidualBind(nn.Module):
+    # TODO: clean this up
+    def __init__(
+        self,
+        input_len,
+        output_dim,
+        input_chanels=4,
+        conv_channels=[96],
+        conv_kernel_size=[11],
+        conv_stride_size=[1],
+        conv_dilation_rate=[1],
+        conv_padding="valid",
+        conv_activation="relu",
+        conv_batchnorm=True,
+        conv_batchnorm_first=True,
+        conv_dropout_rates=0.1,
+        conv_biases=False,
+        residual_channels=[96, 96, 96],
+        residual_kernel_size=[3, 3, 3],
+        residual_stride_size=[1, 1, 1],
+        residual_dilation_rate=[1, 2, 4],
+        residual_padding="same",
+        residual_activation="relu",
+        residual_batchnorm=True,
+        residual_batchnorm_first=True,
+        residual_dropout_rates=0.1,
+        residual_biases=False,
+        pool_kernel_size=10,
+        pool_dropout_rate=0.2,
+        dense_hidden_dims=[256],
+        dense_activation="relu",
+        dense_batchnorm=True,
+        dense_batchnorm_first=True,
+        dense_dropout_rates=0.5,
+        dense_biases=False,
+    ):
+        super(ResidualBind, self).__init__()
+
+        # Set the attributes
+        self.input_len = input_len
+        self.output_dim = output_dim
+        if isinstance(conv_channels, int):
+            conv_channels = [conv_channels]
+
+        # Pass through normal conv
+        self.conv1d_tower = towers.Conv1DTower(
+            input_len=input_len,
+            input_channels=input_chanels,
+            conv_channels=conv_channels,
+            conv_kernels=conv_kernel_size,
+            conv_strides=conv_stride_size,
+            conv_dilations=conv_dilation_rate,
+            conv_padding=conv_padding,
+            conv_biases=conv_biases,
+            activations=conv_activation,
+            pool_types=[None],
+            dropout_rates=conv_dropout_rates,
+            batchnorm=conv_batchnorm,
+            batchnorm_first=conv_batchnorm_first,
+        )
 
+        # Pass through residual block
+        res_block_input_len = self.conv1d_tower.output_len
+        self.residual_block = layers.Residual(
+            towers.Conv1DTower(
+                input_len=res_block_input_len,
+                input_channels=self.conv1d_tower.out_channels,
+                conv_channels=residual_channels,
+                conv_kernels=residual_kernel_size,
+                conv_strides=residual_stride_size,
+                conv_dilations=residual_dilation_rate,
+                conv_padding=residual_padding,
+                conv_biases=residual_biases,
+                activations=residual_activation,
+                pool_types=None,
+                dropout_rates=residual_dropout_rates,
+                batchnorm=residual_batchnorm,
+                batchnorm_first=residual_batchnorm_first,
+            )
+        )
+        self.average_pool = nn.AvgPool1d(pool_kernel_size, stride=1)
+        self.dropout = nn.Dropout(pool_dropout_rate)
+        self.flatten = nn.Flatten()
+        self.dense_block = blocks.DenseBlock(
+            input_dim=self.residual_block.wrapped.out_channels
+            * (res_block_input_len - pool_kernel_size + 1),
+            output_dim=output_dim,
+            hidden_dims=dense_hidden_dims,
+            activations=dense_activation,
+            batchnorm=dense_batchnorm,
+            batchnorm_first=dense_batchnorm_first,
+            dropout_rates=dense_dropout_rates,
+            biases=dense_biases,
+        )
+
+    def forward(self, x):
+        x = self.conv1d_tower(x)
+        x = self.residual_block(x)
+        x = self.average_pool(x)
+        x = self.dropout(x)
+        x = self.flatten(x)
+        x = self.dense_block(x)
+        return x
+
+
+class Kopp21CNN(nn.Module):
+    """
+    Custom convolutional model used in Kopp et al. 2021 paper
+
+    PyTorch implementation of the TensorFlow model described here:
+    https://github.com/wkopp/janggu_usecases/tree/master/01_jund_prediction
+
+    This model can only be run in "ds" mode. The reverse complement must be included in the Dataloader
     Parameters
     ----------
-    input_len:
-        int, input sequence length
-    channels:
-        list-like or int, channel width for each conv layer. If int each of the three layers will be the same channel width
-    conv_kernels:
-        list-like or int, conv kernel size for each conv layer. If int will be the same for all conv layers
-    pool_kernels:
-        list-like or int, maxpooling kernel size for the first two conv layers. If int will be the same for all conv layers
-    dropout_rates:
-        list-like or float, dropout rates for each conv layer. If int will be the same for all conv layers
+    input_len : int
+        Length of the input sequence.
+    output_dim : int
+        Dimension of the output.
+    strand : str, optional
+        Strand of the input. This model is only implemented for "ds"
+    task : str, optional
+        Task for this model. By default "binary_classification" for this mode
+    aggr : str, optional
+        Aggregation method. Either "concat", "max", or "avg". By default "max" for this model.
+    filters : list, optional
+        Number of filters in the convolutional layers.
+    conv_kernel_size : list, optional
+        Kernel size of the convolutional layers.
+    maxpool_kernel_size : int, optional
+        Kernel size of the maxpooling layer.
+    stride : int, optional
+        Stride of the convolutional layers.
     """
+
     def __init__(
         self,
-        input_len: int = 1000,
-        output_dim: int = 1,
-        strand: str = "ss",
-        task: str = "regression",
-        aggr: str = None,
-        loss_fxn: str = "mse",
-        conv_kwargs: dict = {},
-        fc_kwargs: dict = {},
-        **kwargs
+        input_len: int,
+        output_dim: int,
+        aggr: str = "max",
+        filters: list = [10, 8],
+        conv_kernel_size: list = [11, 3],
+        maxpool_kernel_size: int = 30,
+        stride: int = 1,
     ):
-        super().__init__(
-            input_len, 
-            output_dim, 
-            strand=strand, 
-            task=task, 
-            aggr=aggr, 
-            loss_fxn=loss_fxn, 
-            **kwargs
-        )
-        self.conv_kwargs, self.fc_kwargs = self.kwarg_handler(conv_kwargs, fc_kwargs)
-        self.convnet = BasicConv1D(
-            input_len=input_len, 
-            **self.conv_kwargs)
-        self.fcn = BasicFullyConnectedModule(
-            input_dim=self.convnet.flatten_dim, 
-            output_dim=output_dim, 
-            **self.fc_kwargs
-        )
-
-    def forward(self, x, x_rev_comp=None):
-        x = self.convnet(x)
-        x = x.view(x.size(0), self.convnet.flatten_dim)
-        x = self.fcn(x)
-        return x
+        super(Kopp21CNN, self).__init__()
 
-    def kwarg_handler(self, conv_kwargs, fc_kwargs):
-        """Sets default kwargs for conv and fc modules if not specified"""
-        conv_kwargs.setdefault("channels", [4, 320, 480, 960])
-        conv_kwargs.setdefault("conv_kernels", [8, 8, 8])
-        conv_kwargs.setdefault("pool_kernels", [4, 4, 4])
-        conv_kwargs.setdefault("omit_final_pool", True)
-        conv_kwargs.setdefault("activation", "relu")
-        conv_kwargs.setdefault("dropout_rates", [0.2, 0.2, 0.5])
-        conv_kwargs.setdefault("batchnorm", False)
-        fc_kwargs.setdefault("hidden_dims", [925])
-        return conv_kwargs, fc_kwargs
+        # Set the attributes
+        self.input_len = input_len
+        self.output_dim = output_dim
+        self.aggr = aggr
+        self.revcomp = layers.RevComp()
+        self.conv = nn.Conv1d(4, filters[0], conv_kernel_size[0], stride=stride)
+        self.maxpool = nn.MaxPool1d(kernel_size=maxpool_kernel_size, stride=stride)
+        self.batchnorm = nn.BatchNorm1d(filters[0])
+        self.conv2 = nn.Conv1d(
+            filters[0], filters[1], conv_kernel_size[1], stride=stride
+        )
+        self.batchnorm2 = nn.BatchNorm1d(filters[1])
+        self.linear = nn.Linear(filters[1], self.output_dim)
+
+    def forward(self, x):
+        x_rev_comp = self.revcomp(x)
+        x_fwd = F.relu(self.conv(x))
+        x_rev_comp = F.relu(self.conv(x_rev_comp))
+        if self.aggr == "concat":
+            x = torch.cat((x_fwd, x_rev_comp), dim=2)
+        elif self.aggr == "max":
+            x = torch.max(x_fwd, x_rev_comp)
+        elif self.aggr == "avg":
+            x = (x_fwd + x_rev_comp) / 2
+        elif self.aggr is None:
+            x = torch.cat((x_fwd, x_rev_comp), dim=1)
+        x = self.maxpool(x)
+        x = self.conv2(x)
+        x = F.relu(x)
+        x = F.max_pool1d(x, x.shape[2])
+        x = self.batchnorm2(x)
+        x = x.view(x.shape[0], -1)
+        x = self.linear(x)
+        return x
```

### Comparing `eugene-tools-0.0.6/eugene/models/base/_base_model.py` & `eugene_tools-0.1.0/eugene/experimental/_AugmentModule.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,288 +1,242 @@
-import numpy as np
+"""
+Model (implemented in Pytorch Lightning) demonstrating how to use augmentations
+during training. Modified evoaug
+"""
+
 import torch
-import torch.nn.functional as F
-from torch.optim import Adam, SGD
-from torchmetrics import (
-    R2Score,
-    ExplainedVariance,
-    Accuracy,
-    AUROC,
-    F1Score,
-    Precision,
-    Recall,
-)
-from torch.optim.lr_scheduler import ReduceLROnPlateau
-from pytorch_lightning.core.lightning import LightningModule
-from pytorch_lightning import seed_everything
-from pytorch_lightning.utilities.model_summary import ModelSummary
-from ...preprocess import ascii_decode_seq
-from ..._settings import settings
+from pytorch_lightning import LightningModule
+import numpy as np
 
 
-class BaseModel(LightningModule):
-    """
-    Base model class to be inherited by all models in EUGENe
+class RobustModel(LightningModule):
+    """PyTorch Lightning module to specify how augmentation should be applied to a model.
 
-    Paramters:
+    Parameters
     ----------
-
-    input_len (int):
-        length of input sequence
-    output_dim (int):
-        number of output dimensions
-    strand (str):
-        strand of the input sequence
-    task (str):
-        task of the model
-    aggr (str):
-        aggregation method for the input sequence
-    loss_fxn (str):
-        loss function to use
-    hp_metric (str):
-        metric to use for hyperparameter tuning
-    kwargs (dict):
-        additional arguments to pass to the model
+    model : torch.nn.Module
+        PyTorch model.
+    criterion : callable
+        PyTorch loss function
+    optimizer : torch.optim.Optimizer or dict
+        PyTorch optimizer as a class or dictionary
+    augment_list : list
+        List of data augmentations, each a callable class from augment.py.
+        Default is empty list -- no augmentations.
+    max_augs_per_seq : int
+        Maximum number of augmentations to apply to each sequence. Value is superceded by the number of augmentations in augment_list.
+    hard_aug : bool
+        Flag to set a hard number of augmentations, otherwise the number of augmentations is set randomly up to max_augs_per_seq, default is True.
+    finetune : bool
+        Flag to turn off augmentations during training, default is False.
+    inference_aug : bool
+        Flag to turn on augmentations during inference, default is False.
     """
+
     def __init__(
         self,
-        input_len: int,
-        output_dim: int,
-        strand: str = "ss",
-        task: str = "regression",
-        aggr: str = None,
-        loss_fxn: str = "mse",
-        optimizer: str = "adam",
-        lr: float = 1e-3,
-        scheduler: str = "lr_scheduler",
-        scheduler_patience: int = 2,
-        hp_metric: str = None,
-        optimizer_kwargs: dict = {},
-        seed: int = None,
-        **kwargs,
+        model,
+        criterion,
+        optimizer,
+        augment_list=[],
+        max_augs_per_seq=0,
+        hard_aug=True,
+        finetune=False,
+        inference_aug=False,
     ):
         super().__init__()
-        self.input_len = input_len
-        self.output_dim = output_dim
-        self.strand = strand
-        self.task = task
-        self.aggr = aggr
-        self.loss_fxn = loss_fxn_dict[loss_fxn]
-        self.hp_metric_name = (
-            hp_metric if hp_metric is not None else default_hp_metric_dict[self.task]
-        )
-        self.hp_metric = _metric_handler(self.hp_metric_name, output_dim)
+        self.model = model
+        self.criterion = criterion
         self.optimizer = optimizer
-        self.lr = lr
-        self.scheduler = scheduler
-        self.scheduler_patience = scheduler_patience
-        self.optimizer_kwargs = optimizer_kwargs
-        seed_everything(seed) if seed is not None else None
-        self.kwargs = kwargs
-        self.save_hyperparameters()
-
-    def forward(self, x, x_rev_comp=None) -> torch.Tensor:
-        """
-        Forward pass of the model. This method must be implemented by the child class.
+        self.augment_list = augment_list
+        self.max_augs_per_seq = np.minimum(max_augs_per_seq, len(augment_list))
+        self.hard_aug = hard_aug
+        self.inference_aug = inference_aug
+        self.optimizer = optimizer
+        self.max_num_aug = len(augment_list)
+        self.insert_max = augment_max_len(augment_list)
+        self.finetune = finetune
+
+    def forward(self, x):
+        """Standard forward pass."""
+        y_hat = self.model(x)
+        return y_hat
 
-        Parameters:
-        ----------
-        x (torch.Tensor):
-            input sequence
-        x_rev_comp (torch.Tensor):
-            reverse complement of the input sequence
-        """
-        raise NotImplementedError()
+    def configure_optimizers(self):
+        """Standard optimizer configuration."""
+        return self.optimizer
 
     def training_step(self, batch, batch_idx):
-        """Training step"""
-        return self._common_step(batch, batch_idx, "train")
-
-    def validation_step(self, batch, batch_idx):
-        """Validation step"""
-        self._common_step(batch, batch_idx, "val")
-
-    def test_step(self, batch, batch_idx):
-        """Test step"""
-        self._common_step(batch, batch_idx, "test")
-
-    def predict_step(self, batch, batch_idx):
-        """Predict step
-
-        Parameters:
-        ----------
-        batch (tuple):
-            batch of data
-        batch_idx (int):
-            index of the batch
-
-        Returns:
-        ----------
-        np.ndarray:
-            predictions with the format ID, prediction, true value
-        """
-        ID, x, x_rev_comp, y = batch
-        ID = np.array(
-            [ascii_decode_seq(item) for item in ID.squeeze(dim=1).detach().cpu().numpy()]
-        )
-        y = y.detach().cpu().numpy()
-        outs = self(x, x_rev_comp).squeeze(dim=1).detach().cpu().numpy()
-        return np.column_stack([ID, outs, y])
-
-    def _common_step(self, batch, batch_idx, stage: str):
-        """Common step for training, validation and test
-
-        Parameters:
-        ----------
-        batch (tuple):
-            batch of data
-        batch_idx (int):
-            index of the batch
-        stage (str):
-            stage of the training
-
-        Returns:
-        ----------
-        dict:
-            dictionary of metrics
-        """
-        # Get and log loss
-        ID, x, x_rev_comp, y = batch
-        outs = self(x, x_rev_comp).squeeze(dim=1)
-        loss = self.loss_fxn(outs, y)
-        hp_metric = self._calculate_metric(outs, y)
-
-        # Get and log metrics
-        self.log(f"{stage}_loss", loss, on_epoch=True, rank_zero_only=True)
+        """Training step with augmentations."""
+        x, y = batch
+        if self.finetune:  # if finetune, no augmentations
+            if (
+                self.insert_max
+            ):  # if insert_max is larger than 0, then pad each sequence with random DNA
+                x = self._pad_end(x)
+        else:
+            x = self._apply_augment(x)
+        y_hat = self(x)
+        loss = self.criterion(y_hat, y)
         self.log(
-            f"{stage}_{self.hp_metric_name}",
-            hp_metric,
-            on_epoch=True,
-            rank_zero_only=True,
+            "train_loss", loss, on_step=False, on_epoch=True, prog_bar=True, logger=True
         )
-
-        # Get and log "hp_metric" useful for hyperopt
-        if stage == "val":
-            self.log("hp_metric", hp_metric, on_epoch=True, rank_zero_only=True)
-
         return loss
 
-    def configure_optimizers(self):
-        """Configure optimizers
+    def validation_step(self, batch, batch_idx):
+        """Validation step without (or with) augmentations."""
+        x, y = batch
+        if (
+            self.inference_aug
+        ):  # if inference_aug, then apply augmentations during inference
+            x = self._apply_augment(x)
+        else:
+            if (
+                self.insert_max
+            ):  # if insert_max is larger than 0, then pad each sequence with random DNA
+                x = self._pad_end(x)
+        y_hat = self(x)
+        loss = self.criterion(y_hat, y)
+        self.log("val_loss", loss, on_step=False, on_epoch=True, prog_bar=True)
 
-        Returns:
-        ----------
-        torch.optim.Optimizer:
-            optimizer
-        torch.optim.lr_scheduler._LRScheduler:
-            learning rate scheduler
-        """
-        optimizer = optimizer_dict[self.optimizer](
-            self.parameters(), lr=self.lr, **self.optimizer_kwargs
-        )
-        scheduler = (
-            ReduceLROnPlateau(optimizer, patience=self.scheduler_patience)
-            if self.scheduler_patience is not None
-            else None
-        )
-        return {
-            "optimizer": optimizer,
-            "lr_scheduler": scheduler,
-            "monitor": "val_loss",
-        }
-
-    def _calculate_metric(self, outs, y):
-        """Calculate metrics on set of predictions
-
-        Parameters:
-        ----------
-        outs (torch.Tensor):
-            output of the model
-        y (torch.Tensor):
-            ground truth
-
-        Returns:
-        ----------
-        torch.Tensor:
-            metric
-        """
-        if self.hp_metric_name == "r2":
-            return self.hp_metric(outs, y)
-        elif self.hp_metric_name == "auroc":
-            if self.task == "binary_classification":
-                probs = torch.sigmoid(outs)
-                return self.hp_metric(probs, y.long())
-            return self.hp_metric(outs, y.long())
-        elif self.hp_metric_name == "accuracy":
-            preds = torch.round(torch.sigmoid(outs))
-            return self.hp_metric(preds, y.long())
-
-    def summary(self):
-        """Print a summary of the model"""
-        print(f"Model: {self.__class__.__name__}")
-        print(f"Input length: {self.input_len}")
-        print(f"Output dimension: {self.output_dim}")
-        print(f"Strand: {self.strand}")
-        print(f"Task: {self.task}")
-        print(f"Aggregation: {self.aggr}")
-        print(f"Loss function: {self.loss_fxn.__name__}")
-        print(f"Optimizer: {self.optimizer}")
-        print(f"\tOptimizer parameters: {self.optimizer_kwargs}")
-        print(f"Learning rate: {self.lr}")
-        print(f"Scheduler: {self.scheduler}")
-        print(f"Scheduler patience: {self.scheduler_patience}")
-        return ModelSummary(self)
+    def test_step(self, batch, batch_idx):
+        """Test step without (or with) augmentations."""
+        x, y = batch
+        if (
+            self.inference_aug
+        ):  # if inference_aug, then apply augmentations during inference
+            x = self._apply_augment(x)
+        else:
+            if (
+                self.insert_max
+            ):  # if insert_max is larger than 0, then pad each sequence with random DNA
+                x = self._pad_end(x)
+        y_hat = self(x)
+        loss = self.criterion(y_hat, y)
+        self.log("test_loss", loss, on_step=False, on_epoch=True, prog_bar=True)
 
+    def predict_step(self, batch, batch_idx):
+        """Prediction step without (or with) augmentations."""
+        x = batch
+        if (
+            self.inference_aug
+        ):  # if inference_aug, then apply augmentations during inference
+            x = self._apply_augment(x)
+        else:
+            if (
+                self.insert_max
+            ):  # if insert_max is larger than 0, then pad each sequence with random DNA
+                x = self._pad_end(x)
+        return self(x)
+
+    def _sample_aug_combos(self, batch_size):
+        """Set the number of augmentations and randomly select augmentations to apply
+        to each sequence.
+        """
+        # determine the number of augmentations per sequence
+        if self.hard_aug:
+            batch_num_aug = self.max_augs_per_seq * np.ones((batch_size,), dtype=int)
+        else:
+            batch_num_aug = np.random.randint(
+                1, self.max_augs_per_seq + 1, (batch_size,)
+            )
+
+        # randomly choose which subset of augmentations from augment_list
+        aug_combos = [
+            list(sorted(np.random.choice(self.max_num_aug, sample, replace=False)))
+            for sample in batch_num_aug
+        ]
+        return aug_combos
+
+    def _apply_augment(self, x):
+        """Apply augmentations to each sequence in batch, x."""
+        # number of augmentations per sequence
+        aug_combos = self._sample_aug_combos(x.shape[0])
+
+        # apply augmentation combination to sequences
+        x_new = []
+        for aug_indices, seq in zip(aug_combos, x):
+            seq = torch.unsqueeze(seq, dim=0)
+            insert_status = True  # status to see if random DNA padding is needed
+            for aug_index in aug_indices:
+                seq = self.augment_list[aug_index](seq)
+                if hasattr(self.augment_list[aug_index], "insert_max"):
+                    insert_status = False
+            if insert_status:
+                if self.insert_max:
+                    seq = self._pad_end(seq)
+            x_new.append(seq)
+        return torch.cat(x_new)
+
+    def _pad_end(self, x):
+        """Add random DNA padding of length insert_max to the end of each sequence in batch."""
+        N, A, L = x.shape
+        a = torch.eye(A)
+        p = torch.tensor([1 / A for _ in range(A)])
+        padding = torch.stack(
+            [
+                a[p.multinomial(self.insert_max, replacement=True)].transpose(0, 1)
+                for _ in range(N)
+            ]
+        ).to(x.device)
+        x_padded = torch.cat([x, padding.to(x.device)], dim=2)
+        return x_padded
+
+    def finetune_mode(self, optimizer=None):
+        """Turn on finetune flag -- no augmentations during training."""
+        self.finetune = True
+        if optimizer != None:
+            self.optimizer = optimizer
 
-def _metric_handler(metric_name, num_outputs):
-    """Handler for metrics
 
-    Parameters:
-    ----------
-    metric_name (str):
-        name of the metric
-    num_outputs (int):
-        number of outputs of the model
+def load_model_from_checkpoint(model, checkpoint_path):
+    """Load PyTorch lightning model from checkpoint.
 
-    Returns:
+    Parameters
     ----------
-    torch.Tensor:
-        metric
+    model : RobustModel
+        RobustModel instance.
+    checkpoint_path : str
+        path to checkpoint of model weights
+
+    Returns
+    -------
+    RobustModel
+        Object with weights and config loaded from checkpoint.
     """
-    if metric_name == "r2":
-        return R2Score(num_outputs=num_outputs)
-    elif metric_name == "explained_variance":
-        return ExplainedVariance()
-    elif metric_name == "auroc":
-        return AUROC(num_classes=num_outputs)
-    elif metric_name == "accuracy":
-        return Accuracy(num_classes=num_outputs)
-    elif metric_name == "f1":
-        return F1Score(num_classes=num_outputs)
-    elif metric_name == "precision":
-        return Precision(num_classes=num_outputs)
-    elif metric_name == "recall":
-        return Recall(num_classes=num_outputs)
-    else:
-        raise ValueError(f"Unknown metric: {metric_name}")
-
-
-loss_fxn_dict = {
-    "mse": F.mse_loss,
-    "poisson": F.poisson_nll_loss,
-    "bce": F.binary_cross_entropy_with_logits,
-    "cross_entropy": F.cross_entropy,
-}
-
-
-default_hp_metric_dict = {
-    "regression": "r2",
-    "multitask_regression": "r2",
-    "binary_classification": "auroc",
-    "multiclass_classification": "auroc",
-}
-
-
-optimizer_dict = {"adam": Adam, "sgd": SGD}
+    return model.load_from_checkpoint(
+        checkpoint_path,
+        model=model.model,
+        criterion=model.criterion,
+        optimizer=model.optimizer,
+        augment_list=model.augment_list,
+        max_augs_per_seq=model.max_augs_per_seq,
+        hard_aug=model.hard_aug,
+        finetune=model.finetune,
+        inference_aug=model.inference_aug,
+    )
+
+
+# ------------------------------------------------------------------------
+# Helper function
+# ------------------------------------------------------------------------
+
+
+def augment_max_len(augment_list):
+    """Determine whether insertions are applied to determine the insert_max,
+    which will be applied to pad other sequences with random DNA.
 
+    Parameters
+    ----------
+    augment_list : list
+        List of augmentations.
 
-lr_scheduler_dict = {"reduce_lr_on_plateau": ReduceLROnPlateau}
+    Returns
+    -------
+    int
+        Value for insert max.
+    """
+    insert_max = 0
+    for augment in augment_list:
+        if hasattr(augment, "insert_max"):
+            insert_max = augment.insert_max
+    return insert_max
```

### Comparing `eugene-tools-0.0.6/eugene/plot/_catplot.py` & `eugene_tools-0.1.0/eugene/plot/_catplot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import seaborn as sns
+from .. import settings
 import matplotlib.pyplot as plt
-from typing import Union, Mapping 
+from typing import Union, Mapping
 from typing import Sequence, Iterable
 from ._utils import _plot_seaborn, _violin_long
-from .. import settings
 
 
 def countplot(
     sdata,
     keys: Union[str, Sequence[str]],
     groupby: str = None,
     orient: str = "h",
@@ -15,16 +15,16 @@
     return_axes: bool = False,
     **kwargs
 ) -> None:
     """
     Plots a countplot of a column(s) in seqs_annot using Seaborn.
 
     This function can be used to show the counts of observations in a single
-    or multiple columns of seqs_annot within a SeqData. If a groupby is 
-    provided then the counts are grouped by the groupby column.  
+    or multiple columns of seqs_annot within a SeqData. If a groupby is
+    provided then the counts are grouped by the groupby column.
 
     Parameters
     ----------
     sdata : SeqData
         SeqData object that contains keys in seqs_annot.
     keys : str or list of str
         Keys to plot. Will be plotted in separate adjacent subplots.
@@ -39,22 +39,22 @@
     **kwargs
         Additional keyword arguments to pass to seaborn.
 
     Returns
     -------
         None
     """
+    keys = [keys] if isinstance(keys, str) else keys
+    if groupby is None:
+        sdata_df = sdata[keys].to_dataframe()
+    else:
+        sdata_df = sdata[keys + [groupby]].to_dataframe()
     with plt.rc_context(rc_context):
         ax = _plot_seaborn(
-            sdata.seqs_annot,
-            keys,
-            func=sns.countplot,
-            groupby=groupby,
-            orient=orient,
-            **kwargs
+            sdata_df, keys, func=sns.countplot, groupby=groupby, orient=orient, **kwargs
         )
     if return_axes:
         return ax
 
 
 def histplot(
     sdata,
@@ -88,22 +88,18 @@
     **kwargs
         Additional keyword arguments to pass to seaborn.
 
     Returns
     -------
         None
     """
+    sdata_df = sdata[keys].to_dataframe()
     with plt.rc_context(rc_context):
         ax = _plot_seaborn(
-            sdata.seqs_annot,
-            keys,
-            func=sns.histplot,
-            orient=orient,
-            ylab="Frequency",
-            **kwargs
+            sdata_df, keys, func=sns.histplot, orient=orient, ylab="Frequency", **kwargs
         )
     if return_axes:
         return ax
 
 
 def boxplot(
     sdata,
@@ -114,15 +110,15 @@
     rc_context: Mapping[str, str] = settings.rc_context,
     return_axes: bool = False,
     **kwargs
 ) -> None:
     """
     Plots a boxplot of a column(s) in seqs_annot using Seaborn.
 
-    This function can be used to show the distribution of a single or multiple 
+    This function can be used to show the distribution of a single or multiple
     columns of seqs_annot within a SeqData. If a groupby is provided then the
     distribution is grouped by the groupby column.
 
     Parameters
     ----------
     sdata : SeqData
         SeqData object.
@@ -139,26 +135,26 @@
     **kwargs
         Additional keyword arguments to pass to seaborn.
 
     Returns
     -------
         None
     """
+    keys = [keys] if isinstance(keys, str) else keys
+    if groupby is None:
+        sdata_df = sdata[keys].to_dataframe()
+    else:
+        sdata_df = sdata[keys + [groupby]].to_dataframe()
     with plt.rc_context(rc_context):
         ax = _plot_seaborn(
-            sdata.seqs_annot,
-            keys,
-            func=sns.boxplot,
-            groupby=groupby,
-            orient=orient,
-            **kwargs
+            sdata_df, keys, func=sns.boxplot, groupby=groupby, orient=orient, **kwargs
         )
         if jitter == True:
             _plot_seaborn(
-                sdata.seqs_annot,
+                sdata_df,
                 keys,
                 func=sns.stripplot,
                 groupby=groupby,
                 orient=orient,
                 ax=ax,
                 **kwargs
             )
@@ -175,15 +171,15 @@
     return_axes: bool = False,
     **kwargs
 ) -> None:
     """
     Plots a violinplot of a column(s) in seqs_annot using Seaborn.
 
     This function can be used to show the distribution of a single or multiple
-    columns of seqs_annot within a SeqData as a violin plot. If a groupby is provided 
+    columns of seqs_annot within a SeqData as a violin plot. If a groupby is provided
     then the distribution is grouped by the groupby column.
 
     Parameters
      ----------
      sdata : SeqData
          SeqData object.
      keys : str or list of str
@@ -199,34 +195,41 @@
      **kwargs
          Additional keyword arguments to pass to seaborn.
 
      Returns
      -------
          None
     """
+    keys = [keys] if isinstance(keys, str) else keys
+    if groupby is None:
+        sdata_df = sdata[keys].to_dataframe()
+    elif groupby is not None and isinstance(groupby, Iterable) and keys is None:
+        sdata_df = sdata[groupby].to_dataframe()
+    else:
+        sdata_df = sdata[keys + [groupby]].to_dataframe()
     with plt.rc_context(rc_context):
         if groupby is not None and isinstance(groupby, Iterable) and keys is None:
-            _violin_long(sdata, groupby, **kwargs)
+            ax = _violin_long(sdata_df, groupby, **kwargs)
         else:
             ax = _plot_seaborn(
-                sdata.seqs_annot,
+                sdata_df,
                 keys,
                 func=sns.violinplot,
                 groupby=groupby,
                 orient=orient,
                 **kwargs
             )
     if return_axes:
         return ax
 
 
 def scatterplot(
-    sdata, 
-    x: str, 
-    y: str, 
+    sdata,
+    x: str,
+    y: str,
     seq_idx: Sequence[int] = None,
     return_axes: bool = False,
     **kwargs
 ) -> None:
     """
     Plots a scatterplot of two columns in seqs_annot using Seaborn.
 
@@ -241,25 +244,21 @@
     x : str
         Key for x-axis.
     y : str
         Key for y-axis.
     seq_idx : int or list of int
         Index of sequences to plot.
     **kwargs: dict
-        Additional keyword arguments to pass to _plot_seaborn.    
+        Additional keyword arguments to pass to _plot_seaborn.
     Returns
     -------
     None
     """
     if seq_idx is not None:
         sdata = sdata[seq_idx]
+    keys = [keys] if isinstance(keys, str) else keys
+    sdata_df = sdata[keys].to_dataframe()
     ax = _plot_seaborn(
-        sdata.seqs_annot, 
-        keys=x, 
-        func=sns.scatterplot, 
-        groupby=y, 
-        xlab=x,
-        ylab=y, 
-        **kwargs
+        sdata_df, keys=x, func=sns.scatterplot, groupby=y, xlab=x, ylab=y, **kwargs
     )
     if return_axes:
         return ax
```

### Comparing `eugene-tools-0.0.6/eugene/plot/_classification.py` & `eugene_tools-0.1.0/eugene/plot/_classification.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from os import PathLike
 import numpy as np
 import seaborn as sns
+from .. import settings
+from os import PathLike
 import matplotlib.pyplot as plt
 from sklearn.metrics import (
     confusion_matrix,
     roc_curve,
     auc,
     precision_recall_curve,
     average_precision_score,
 )
-from typing import Union, Sequence 
+from typing import Union, Sequence
 from sklearn.preprocessing import binarize
 from ._utils import _check_input, _label_plot, _save_fig
-from .. import settings
 
 
 def _plot_binary_confusion_mtx(
-    sdata, 
+    sdata,
     target_key: str,
     prediction_key: str,
-    threshold: float, 
-    title: str = None, 
+    threshold: float,
+    title: str = None,
     xlab: str = None,
     ylab: str = None,
     figsize: tuple = (6, 6),
     save: PathLike = None,
-    ax = None,
-    **kwargs
+    ax=None,
+    **kwargs,
 ) -> None:
     """
     Plot a confusion matrix for binary classification.
 
     This function plots a binary confusion matrix as a seaborn heatmap.
     Pulls a target and prediction key from seqs_annot and uses the passed in
     threshold to binarize the prediction. The confusion matrix is then plotted
@@ -54,28 +54,27 @@
     Returns
     -------
     None
     """
     if ax is None:
         _, ax = plt.subplots(1, 1, figsize=figsize)
     cf_names = ["True Neg", "False Pos", "False Neg", "True Pos"]
-    ts = sdata.seqs_annot[target_key].values.reshape(-1, 1)
-    ps = binarize(sdata.seqs_annot[prediction_key].values.reshape(-1, 1), threshold=threshold)
+    ts = sdata[target_key].values.reshape(-1, 1)
+    ps = binarize(sdata[prediction_key].values.reshape(-1, 1), threshold=threshold)
     cf_mtx = confusion_matrix(ts, ps)
-    cf_pcts = [ "{0:.2%}".format(value) for value in (cf_mtx / cf_mtx.sum(axis=1)[:, None]).flatten()]
-    labels = [f"{v1}\n{v2}\n{v3}" for v1, v2, v3 in zip(cf_mtx.flatten(), cf_pcts, cf_names)]
+    cf_pcts = [
+        "{0:.2%}".format(value)
+        for value in (cf_mtx / cf_mtx.sum(axis=1)[:, None]).flatten()
+    ]
+    labels = [
+        f"{v1}\n{v2}\n{v3}" for v1, v2, v3 in zip(cf_mtx.flatten(), cf_pcts, cf_names)
+    ]
     labels = np.asarray(labels).reshape(2, 2)
     sns.heatmap(
-        cf_mtx, 
-        annot=labels, 
-        fmt="s", 
-        cmap="Blues", 
-        cbar=False, 
-        ax=ax, 
-        **kwargs
+        cf_mtx, annot=labels, fmt="s", cmap="Blues", cbar=False, ax=ax, **kwargs
     )
     _label_plot(
         ax,
         title,
         xlab=xlab,
         ylab=ylab,
     )
@@ -94,16 +93,16 @@
     rc_context: dict = settings.rc_context,
     return_axes: bool = False,
     **kwargs,
 ) -> None:
     """
     Plot a confusion matrix for given targets and predictions within SeqData
 
-    Creates a confusion matrix from the given target and prediction keys held 
-    in the seqs_annot of the passed in SeqData. The 
+    Creates a confusion matrix from the given target and prediction keys held
+    in the seqs_annot of the passed in SeqData. The
 
     Parameters
     ----------
     sdata : SeqData
         SeqData object.
     target_key : str
         Key to use as target.
@@ -121,36 +120,34 @@
     Returns
     -------
         None
     """
     with plt.rc_context(rc_context):
         if kind == "binary":
             ax = _plot_binary_confusion_mtx(
-                sdata, 
-                target_key, 
-                prediction_key, 
-                threshold, 
-                **kwargs
+                sdata, target_key, prediction_key, threshold, **kwargs
             )
         else:
-            raise ValueError(f"Confusion matrix for '{kind}' classification not currently supported.")
+            raise ValueError(
+                f"Confusion matrix for '{kind}' classification not currently supported."
+            )
     if return_axes:
         return ax
 
 
 def auroc(
     sdata,
     target_keys: Union[Sequence[str], str],
     prediction_keys: Union[Sequence[str], str],
     labels: Union[Sequence[str], str] = "",
     xlab: str = "False Positive Rate",
     ylab: str = "True Positive Rate",
     figsize: tuple = (8, 8),
     save: str = None,
-    ax = None,
+    ax=None,
     **kwargs,
 ) -> None:
     """
     Plot the area under the receiver operating characteristic curve for one or more predictions against
     a one or more targets.
 
 
@@ -173,28 +170,26 @@
         Label for the y-axis.
     figsize : tuple
         Size of the figure.
     save : str
         Path to save the figure. If none, figure will not be saved.
     **kwargs
         Additional keyword arguments to pass to matplotlib plot function
-    """ 
+    """
     target_keys, prediction_keys, labels = _check_input(
-        sdata,
-        target_keys, 
-        prediction_keys, 
-        labels
+        sdata, target_keys, prediction_keys, labels
     )
     if ax is None:
         _, ax = plt.subplots(1, 1, figsize=figsize)
     for label, target_key, prediction_key in zip(labels, target_keys, prediction_keys):
-        ts = sdata.seqs_annot[target_key].values.reshape(-1, 1)
-        ps = sdata.seqs_annot[prediction_key].values.reshape(-1, 1)
+        ts = sdata[target_key].values.reshape(-1, 1)
+        ps = sdata[prediction_key].values.reshape(-1, 1)
         fpr, tpr, _ = roc_curve(ts, ps)
         roc_auc = auc(fpr, tpr)
+        print(roc_auc, label)
         ax.plot(fpr, tpr, label=f"{label} (AUC = {roc_auc:.3f})", **kwargs)
         ax.plot([0, 1], [0, 1], "k--")
         ax.set_xlabel(xlab, fontsize=20)
         ax.set_ylabel(ylab, fontsize=20)
         ax.legend(loc="lower right")
         plt.tight_layout()
     if save:
@@ -207,15 +202,15 @@
     target_keys: Union[Sequence[str], str],
     prediction_keys: Union[Sequence[str], str],
     labels: Union[Sequence[str], str] = "",
     xlab: str = "Recall",
     ylab: str = "Precision",
     figsize: tuple = (8, 8),
     save: str = None,
-    ax = None,
+    ax=None,
     **kwargs,
 ) -> None:
     """
     Plot the area under the precision recall curve for one or more predictions against
     a one or more targets.
 
 
@@ -238,23 +233,27 @@
         Label for the y-axis.
     figsize : tuple
         Size of the figure.
     save : str
         Path to save the figure. If none, figure will not be saved.
     **kwargs
         Additional keyword arguments to pass to matplotlib plot function
-    """ 
-    target_keys, prediction_keys, labels = _check_input(sdata, target_keys, prediction_keys, labels)
+    """
+    target_keys, prediction_keys, labels = _check_input(
+        sdata, target_keys, prediction_keys, labels
+    )
     _, ax = plt.subplots(1, 1, figsize=figsize)
     for label, target_key, prediction_key in zip(labels, target_keys, prediction_keys):
-        ts = sdata.seqs_annot[target_key].values.reshape(-1, 1)
-        ps = sdata.seqs_annot[prediction_key].values.reshape(-1, 1)
+        ts = sdata[target_key].values.reshape(-1, 1)
+        ps = sdata[prediction_key].values.reshape(-1, 1)
         precision, recall, _ = precision_recall_curve(ts, ps)
         average_precision = average_precision_score(ts, ps)
-        ax.plot(recall, precision, label=f"{label} (AP = {average_precision:.3f})", **kwargs)
+        ax.plot(
+            recall, precision, label=f"{label} (AP = {average_precision:.3f})", **kwargs
+        )
         ax.set_xlabel(xlab, fontsize=20)
         ax.set_ylabel(ylab, fontsize=20)
         ax.legend(loc="lower right")
         plt.tight_layout()
     if save:
         _save_fig(save)
     return ax
```

### Comparing `eugene-tools-0.0.6/eugene/plot/_dim_reduce.py` & `eugene_tools-0.1.0/eugene/plot/_dim_reduce.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,41 @@
-from matplotlib import offsetbox
-import numpy as np
 import matplotlib.pyplot as plt
-import seaborn as sns
 
 
 def pca(
-    sdata, 
-    seqsm_key, 
-    pc1=0, 
-    pc2=1, 
-    loadings=None, 
-    labels=None, 
+    sdata,
+    seqsm_key,
+    pc1=0,
+    pc2=1,
+    loadings=None,
+    labels=None,
     n=5,
     return_axes=False,
-    **kwargs):
+    **kwargs
+):
     """
     Plot the PCA of the data.
 
     Parameters
     ----------
-    sdata : 
+    sdata :
         SeqData The SeqData object.
-    seqsm_key : 
+    seqsm_key :
     str The key of the SeqSM object to use.
-    pc1 : int 
+    pc1 : int
         The first PC to plot.
-    pc2 : int 
+    pc2 : int
         The second PC to plot.
-    color : str 
+    color : str
         The color of the points.
-    loadings : 
+    loadings :
         list of floats The loadings of the PCs.
-    labels : 
+    labels :
         list of str The labels of the points.
-    n : 
+    n :
         int The number of points to plot.
 
     Returns
     -------
     None
     """
     pc_data = sdata.seqsm[seqsm_key]
@@ -46,79 +44,95 @@
     scalex = 1.0 / (xs.max() - xs.min())
     scaley = 1.0 / (ys.max() - ys.min())
     ax = plt.scatter(xs * scalex, ys * scaley, **kwargs)
     if loadings is not None:
         if n > loadings.shape[0]:
             n = loadings.shape[0]
         for i in range(n):
-            plt.arrow(0, 0, loadings[0, i], loadings[1, i], color='r', alpha=0.5, head_width=0.07, head_length=0.07, overhang=0.7)
+            plt.arrow(
+                0,
+                0,
+                loadings[0, i],
+                loadings[1, i],
+                color="r",
+                alpha=0.5,
+                head_width=0.07,
+                head_length=0.07,
+                overhang=0.7,
+            )
         if labels is None:
-            plt.text(loadings[0, i] * 1.2, loadings[1, i] * 1.2, "Var" + str(i + 1), color='g', ha='center', va='center')
+            plt.text(
+                loadings[0, i] * 1.2,
+                loadings[1, i] * 1.2,
+                "Var" + str(i + 1),
+                color="g",
+                ha="center",
+                va="center",
+            )
         else:
-            plt.text(loadings[0, i] * 1.2, loadings[1, i] * 1.2, labels[i], color='g', ha='center', va='center')
+            plt.text(
+                loadings[0, i] * 1.2,
+                loadings[1, i] * 1.2,
+                labels[i],
+                color="g",
+                ha="center",
+                va="center",
+            )
     plt.xlim(-1, 1)
     plt.ylim(-1, 1)
     plt.xlabel("PC{}".format(1))
     plt.ylabel("PC{}".format(2))
     if return_axes:
         return ax
 
 
-def skree(
-    sdata, 
-    uns_key, 
-    n_comp=30, 
-    return_variance=False):
+def skree(sdata, uns_key, n_comp=30, return_variance=False):
     """
     Function to generate and output a Skree plot using matplotlib barplot
     Parameters
     ----------
     pca_obj : scikit-learn pca object
     n_comp : number of components to show in the plot
 
     Returns
     -------
 
     """
-    variance={}
-    for i,val in enumerate(sdata.uns[uns_key].explained_variance_ratio_.tolist()):
-        key="PC"+str(i+1)
-        variance[key]=val*100
-    plt.bar(["PC"+str(i) for i in range(1,n_comp+1)],sdata.uns[uns_key].explained_variance_ratio_*100)
+    variance = {}
+    for i, val in enumerate(sdata.uns[uns_key].explained_variance_ratio_.tolist()):
+        key = "PC" + str(i + 1)
+        variance[key] = val * 100
+    plt.bar(
+        ["PC" + str(i) for i in range(1, n_comp + 1)],
+        sdata.uns[uns_key].explained_variance_ratio_ * 100,
+    )
     plt.xticks(rotation=90)
     plt.ylabel("Variance Explained")
     plt.xlabel("Principal Component")
     if return_variance:
         return variance
 
 
-def umap(
-    sdata, 
-    seqsm_key, 
-    umap1=0, 
-    umap2=1,  
-    n=5,
-    return_axes=False,
-    **kwargs):
+def umap(sdata, seqsm_key, umap1=0, umap2=1, n=5, return_axes=False, **kwargs):
     """
     Plot the UMAP of the data.
 
     Parameters
     ----------
-    sdata : SeqData 
+    sdata : SeqData
         The SeqData object.
-    seqsm_key : str 
+    seqsm_key : str
         The key of the SeqSM object to use.
-    umap1 : int 
+    umap1 : int
         The first UMAP to plot.
-    umap2 : int 
+    umap2 : int
         The second UMAP to plot.
-    color : str 
+    color : str
         The color of the points.
-    n : int 
+    n : int
         The number of points to plot.
 
     Returns
     -------
     None
     """
     umap_data = sdata.seqsm[seqsm_key]
@@ -127,8 +141,8 @@
     scalex = 1.0 / (xs.max() - xs.min())
     scaley = 1.0 / (ys.max() - ys.min())
     ax = plt.scatter(xs * scalex, ys * scaley, **kwargs)
     plt.xlabel("UMAP{}".format(1))
     plt.ylabel("UMAP{}".format(2))
     plt.show()
     if return_axes:
-        return ax
+        return ax
```

### Comparing `eugene-tools-0.0.6/eugene/plot/_regression.py` & `eugene_tools-0.1.0/eugene/plot/_regression.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from os import PathLike
 import numpy as np
+import xarray as xr
+from os import PathLike
 import matplotlib.pyplot as plt
 from typing import Union, Sequence
 from sklearn.metrics import r2_score, mean_squared_error
-from scipy.stats import spearmanr
-from ._utils import (
-    _create_matplotlib_axes,
-    _save_fig
-)
+from scipy.stats import spearmanr, pearsonr
+from ._utils import _create_matplotlib_axes, _save_fig
 from .. import settings
 
 
 def _plot_performance_scatter(
     sdata,
     target_key: str,
     prediction_key: str,
-    metrics: Union[str, Sequence[str]] = ["r2", "mse", "spearmanr"],
+    metrics: Union[str, Sequence[str]] = ["r2", "mse", "pearsonr", "spearmanr"],
     groupby=None,
     figsize: tuple = (8, 8),
     save: PathLike = None,
     ax: bool = None,
     **kwargs,
 ) -> None:
     """
@@ -44,69 +42,82 @@
     -------
     None
 
     Note
     ----
     This function uses Matplotlib as opposed to Seaborn.
     """
-    target = sdata.seqs_annot[target_key]
-    prediction = sdata.seqs_annot[prediction_key]
+    target = sdata[target_key].to_numpy()
+    prediction = sdata[prediction_key].to_numpy()
 
     nan_mask = ~np.isnan(target)
     target = target[nan_mask]
     prediction = prediction[nan_mask]
 
     r2 = r2_score(target, prediction) if "r2" in metrics else None
     mse = mean_squared_error(target, prediction) if "mse" in metrics else None
-    spearr = (spearmanr(target, prediction).correlation if "spearmanr" in metrics else None)
+    pearsr = pearsonr(target, prediction)[0] if "pearsonr" in metrics else None
+    spearr = (
+        spearmanr(target, prediction).correlation if "spearmanr" in metrics else None
+    )
     if "c" in kwargs:
-        if kwargs["c"] in sdata.seqs_annot.columns:
-            kwargs["c"] = sdata.seqs_annot[kwargs["c"]]
+        if kwargs["c"] in sdata.data_vars.keys():
+            kwargs["c"] = sdata[kwargs["c"]]
     ax = _create_matplotlib_axes(1, subplot_size=figsize) if ax is None else ax
     if groupby is not None:
         i = 0
-        print("Group", "R2", "MSE", "Spearmanr")
-        for group, data in sdata.seqs_annot.groupby(groupby):
+        print("Group", "R2", "MSE", "Pearsonr", "Spearmanr")
+        seqs_annot = sdata[[groupby, target_key, prediction_key]].to_dataframe()
+        for group, data in seqs_annot.groupby(groupby):
             target = data[target_key]
             prediction = data[prediction_key]
             group_r2 = r2_score(target, prediction) if "r2" in metrics else None
-            group_mse = mean_squared_error(target, prediction if "mse" in metrics else None)
-            group_spearr = spearmanr(target, prediction).correlation if "spearmanr" in metrics else None
-            im = ax.scatter(
-                target, 
-                prediction, 
-                label=group, 
-                color="bgrcm"[i], 
-                **kwargs
+            group_mse = mean_squared_error(
+                target, prediction if "mse" in metrics else None
+            )
+            group_pearsr = (
+                pearsonr(target, prediction)[0] if "pearsonr" in metrics else None
+            )
+            group_spearr = (
+                spearmanr(target, prediction).correlation
+                if "spearmanr" in metrics
+                else None
             )
+            im = ax.scatter(target, prediction, label=group, color="bgrcm"[i], **kwargs)
             print(group, group_r2, group_mse, group_spearr)
             i += 1
             ax.legend()
     else:
         im = ax.scatter(
-            target, 
-            prediction, 
-            edgecolor="black", 
-            linewidth=0.1, 
-            s=10, 
-            **kwargs
+            target, prediction, edgecolor="black", linewidth=0.1, s=10, **kwargs
         )
     if "c" in kwargs:
         plt.colorbar(im, location="bottom", label=kwargs["c"].name)
     ax.set_xlabel(target_key)
     ax.set_ylabel(prediction_key)
     ax.text(
         1.02, 0.95, f"$R^2$: {r2:.2f}", transform=plt.gca().transAxes, fontsize=16
     ) if r2 is not None else None
     ax.text(
         1.02, 0.90, f"MSE: {mse:.2f}", transform=plt.gca().transAxes, fontsize=16
     ) if mse is not None else None
     ax.text(
-        1.02, 0.85, rf"Spearman $\rho$: {spearr:.2f}", transform=plt.gca().transAxes, fontsize=16,
+        1.02,
+        0.85,
+        rf"Spearman $\rho$: {spearr:.2f}",
+        transform=plt.gca().transAxes,
+        fontsize=16,
     ) if spearr is not None else None
+    ax.text(
+        1.02,
+        0.80,
+        rf"Pearson $r$: {pearsr:.2f}",
+        transform=plt.gca().transAxes,
+        fontsize=16,
+    ) if pearsr is not None else None
     lims = [
         np.min([ax.get_xlim(), ax.get_ylim()]),  # min of both axes
         np.max([ax.get_xlim(), ax.get_ylim()]),  # max of both axes
     ]
     ax.plot(lims, lims, color="black", linestyle="--", zorder=0)
     ax.set_aspect("equal")
     ax.set_xlim(lims)
@@ -123,18 +134,18 @@
     seq_idx: Union[Sequence[int], np.ndarray] = None,
     rc_context: dict = settings.rc_context,
     return_axes: bool = False,
     **kwargs,
 ) -> None:
     """
     Plot a scatter plot of the performance of the model on a subset of the sequences.
-    
+
     Classic predicted vs observed scatterplot that will be annotated with r2, mse and spearman correlation.
     If a groupby key is passed, the scatterplot will be colored according to group.
-    
+
     Parameters
     ----------
     sdata : SeqData
         SeqData object.
     target_key : str
         Name of the target_key variable.
     prediction_key : str
@@ -154,18 +165,17 @@
         prediction_keys = [prediction_keys]
     if type(target_keys) is list and type(prediction_keys) is list:
         assert len(target_keys) == len(prediction_keys)
     else:
         target_keys = [target_keys]
         prediction_keys = [prediction_keys]
     with plt.rc_context(rc_context):
-        for (target_key, prediction_key) in zip(target_keys, prediction_keys):
-            nan_mask = ~np.isnan(sdata.seqs_annot[target_key])
-            sdata = sdata[nan_mask]
+        for target_key, prediction_key in zip(target_keys, prediction_keys):
+            targs = sdata[target_key].values
+            nan_mask = xr.DataArray(np.isnan(targs), dims=["_sequence"])
+            print(f"Dropping {int(nan_mask.sum().values)} sequences with NaN targets.")
+            sdata = sdata.where(~nan_mask, drop=True)
             ax = _plot_performance_scatter(
-                sdata, 
-                target_key=target_key, 
-                prediction_key=prediction_key, 
-                **kwargs
+                sdata, target_key=target_key, prediction_key=prediction_key, **kwargs
             )
     if return_axes:
         return ax
```

### Comparing `eugene-tools-0.0.6/eugene/plot/_seq.py` & `eugene_tools-0.1.0/eugene/plot/_seq.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-from typing import Union
-from os import PathLike
-import pandas as pd
 import numpy as np
+import pandas as pd
 import seaborn as sns
-import matplotlib as mpl
-import matplotlib.pyplot as plt
-from matplotlib.axes import Axes
-import seqlogo
 import logomaker as lm
-from vizsequence import viz_sequence
+from os import PathLike
+import matplotlib as mpl
+from typing import Union
 from tqdm.auto import tqdm
-from ..preprocess._utils import _collapse_pos
 from ._utils import _save_fig
-from .. import settings
+import matplotlib.pyplot as plt
+from matplotlib.axes import Axes
+from ._utils import _collapse_pos
 
 
-vocab_dict = {
-    "DNA": ["A", "C", "G", "T"], 
-    "RNA": ["A", "C", "G", "U"]
-}
+vocab_dict = {"DNA": ["A", "C", "G", "T"], "RNA": ["A", "C", "G", "U"]}
 
 
 def _plot_seq_features(
     ax: Axes,
     seq: str,
     annots: pd.DataFrame,
     additional_annots: list = [],
 ):
     """
     Plot sequence features using matplotlib.
 
     This uses basic matplotlib rectangles and lines to plot sequence features
-    as blocks. Can be used along with importance scores to give a visual of where the 
+    as blocks. Can be used along with importance scores to give a visual of where the
     a prior known features of a sequence are
 
     Parameters
     ----------
     ax : matplotlib.axes.Axes
         The axes object to plot on
     seq : str
@@ -103,15 +97,15 @@
                     va="bottom",
                 )
 
 
 def _plot_seq_logo(
     ax: Axes,
     seq: str,
-    imp_scores: np.ndarray = None,
+    attrs: np.ndarray = None,
     highlight: list = [],
     threshold: float = None,
     ylab="Importance Score",
     **kwargs,
 ):
     """
     Plot sequence logo using plot_weights_given_ax function from viz_sequence
@@ -120,15 +114,15 @@
 
     Parameters
     ----------
     ax : matplotlib.axes.Axes
         The axes object to plot on
     seq : str
         The sequence to plot
-    imp_scores : np.ndarray
+    attrs : np.ndarray
         The importance scores to plot
     highlight : list
         A list of positions to highlight
     threshold : float
         The threshold for importance scores to highlight
     **kwargs
         Additional keyword arguments to pass to plot_weights_given_ax
@@ -138,41 +132,42 @@
     None
 
     Note
     ----
     This was adapted from the viz_sequence package:
     https://github.com/kundajelab/vizsequence
     """
-    if imp_scores is None:
-        from ..preprocess import ohe_seq
+    if attrs is None:
+        from seqpro import ohe
+
         print("No importance scores given, outputting just sequence")
         ylab = "Sequence" if ylab is None else ylab
         ax.spines["left"].set_visible(False)
         ax.set_yticklabels([])
         ax.set_yticks([])
-        imp_scores = ohe_seq(seq)
+        attrs = ohe(seq)
     else:
         ylab = "Importance Score" if ylab is None else ylab
 
     # Plot the featue importance scores
     if len(highlight) > 0:
         to_highlight = {"red": _collapse_pos(highlight)}
         print(to_highlight)
         viz_sequence.plot_weights_given_ax(
             ax,
-            imp_scores,
+            attrs,
             subticks_frequency=10,
             highlight=to_highlight,
             height_padding_factor=1,
             **kwargs,
         )
     else:
         viz_sequence.plot_weights_given_ax(
             ax,
-            imp_scores,
+            attrs,
             subticks_frequency=int(len(seq) / 10),
             height_padding_factor=1,
             **kwargs,
         )
     ax.spines["right"].set_visible(False)
     ax.spines["top"].set_visible(False)
     ax.set_xlabel("Sequence Position")
@@ -194,15 +189,15 @@
     return_axes: bool = False,
     save: str = None,
     **kwargs,
 ):
     """
     Function to plot tracks from a SeqData object using matplotlib and function
     from viz_sequence package.
-    
+
     This function allows users to also add features from the pos_annot attribute,
     which is not currently available with seq_track function.
 
     This also allows users to just plot the sequences with no importance scores, which is
     currently not available with seq_track function.
 
 
@@ -240,15 +235,15 @@
     seq_idx = np.where(sdata.seqs_annot.index == seq_id)[0][0]
     seq = sdata.seqs[seq_idx]
     p_annot = (
         sdata.pos_annot.df[sdata.pos_annot.df["Chromosome"] == seq_id]
         if sdata.pos_annot is not None
         else None
     )
-    imp_scores = sdata.uns[uns_key][seq_idx] if uns_key in sdata.uns.keys() else None
+    attrs = sdata.uns[uns_key][seq_idx] if uns_key in sdata.uns.keys() else None
 
     # Define subplots
     _, ax = (
         plt.subplots(2, 1, figsize=(12, 4), sharex=True)
         if p_annot is not None
         else plt.subplots(1, 1, figsize=(12, 4))
     )
@@ -258,24 +253,24 @@
     if p_annot is not None:
         _plot_seq_features(
             ax[0], seq, p_annot, additional_annots=additional_annotations
         )
         _plot_seq_logo(
             ax[1],
             seq,
-            imp_scores=imp_scores,
+            attrs=attrs,
             highlight=highlight,
             threshold=threshold,
             **kwargs,
         )
     else:
         _plot_seq_logo(
             ax,
             seq,
-            imp_scores=imp_scores,
+            attrs=attrs,
             highlight=highlight,
             threshold=threshold,
             **kwargs,
         )
 
     # Add title
     title = seq_id
@@ -294,27 +289,27 @@
     if save is not None:
         _save_fig(save)
 
 
 def multiseq_track_features(
     sdata,
     seq_ids: list,
-    uns_keys: str = None,
+    attr_keys: str = None,
     ylabs: list = None,
     width=None,
     height=None,
     return_axes: bool = False,
     save: str = None,
     **kwargs,
 ):
     """
     Wrapper around seq_track_features function to plot multiple tracks from a SeqData object
-    using matplotlib and viz_sequence. This function allows users to also add features from the 
+    using matplotlib and viz_sequence. This function allows users to also add features from the
     pos_annot attribute
-    
+
     Parameters
     ----------
     sdata : SeqData object
         The SeqData object to plot
     seq_ids : list
         The IDs of the sequences to plot
     uns_key : str
@@ -337,130 +332,66 @@
     Returns
     -------
     ax : matplotlib.axes.Axes
         The axes object
     """
     if isinstance(seq_ids, str):
         seq_ids = [seq_ids]
-    if isinstance(uns_keys, str):
-        uns_keys = [uns_keys]
-    ylabs = ylabs if ylabs is not None else ["Importance Score"] * len(uns_keys)
+    if isinstance(attr_keys, str):
+        attr_keys = [attr_keys]
+    ylabs = ylabs if ylabs is not None else ["Importance Score"] * len(attr_keys)
     seq_idx = np.where(sdata.seqs_annot.index.isin(seq_ids))[0]
     seqs = sdata.seqs[seq_idx]
     fig_width = (
         len(seq_ids) * int(len(seqs[0]) / 20) if width is None else width
     )  # make each sequence width proportional to its length and multiply by the number of sequences
     fig_height = (
-        len(uns_keys) * 4 if height is None else height
-    )  # make each sequence height proportional to the number of uns_keys
-    _, ax = plt.subplots(len(uns_keys), len(seq_ids), figsize=(fig_width, fig_height))
-    for i, uns_key in tqdm(enumerate(uns_keys), desc="Importance values", position=0):
+        len(attr_keys) * 4 if height is None else height
+    )  # make each sequence height proportional to the number of attr_keys
+    _, ax = plt.subplots(len(attr_keys), len(seq_ids), figsize=(fig_width, fig_height))
+    for i, uns_key in tqdm(enumerate(attr_keys), desc="Importance values", position=0):
         for j, seq in enumerate(seqs):
-            imp_scores = (
+            attrs = (
                 sdata.uns[uns_key][seq_idx[j]] if uns_key in sdata.uns.keys() else None
             )
             _plot_seq_logo(
                 ax.flatten()[i * len(seq_ids) + j],
                 seq,
-                imp_scores=imp_scores,
+                attrs=attrs,
                 ylab=ylabs[i],
             )
             if i == 0:
                 ax.flatten()[i * len(seq_ids) + j].set_title(
                     seq_ids[j], fontsize=18, weight="bold"
                 )
     plt.tight_layout()
     if return_axes:
         return ax
     if save is not None:
         _save_fig(save)
 
 
-def _plot_logo_seqlogo(
-    matrix, 
-    **kwargs
-):
-    """
-    Plot a sequence logo of a position frequency matrix (PFM) using the SeqLogo package. 
-    
-    This function is deprecated because there is no easy way to save these as
-    figures because they are not matplotlib axes.
-
-    Parameters
-    ----------
-    matrix : numpy.ndarray
-        The position frequency matrix to plot
-    **kwargs : dict
-        Additional keyword arguments to pass to the SeqLogo object
-    """
-    cpm = seqlogo.CompletePm(pfm=matrix)
-    logo = seqlogo.seqlogo(
-        cpm, 
-        ic_scale=True, 
-        format="png", 
-        **kwargs
-    )
-    display(logo)
-    return logo
-
-
-def filter_viz_seqlogo(
-    sdata, 
-    filter_id: Union[str, list], 
-    uns_key: str = "pfms", 
-    return_logo: bool = False,
-    **kwargs
-):
-    """Plot the logo of the pfm generated for a passed in filter.  
-    
-    This function is deprecated because there is no easy way to save these as
-    figures because they are not matplotlib axes.
-    
-    If a filter_id is given, the logo will be filtered to only show the features that match the filter_id.
-    The uns_key is the key in the sdata.uns dictionary that contains the importance scores.
-    The kwargs are passed to the SeqLogo object. See the SeqLogo documentation for more details.
-
-    Parameters
-    ----------
-    sdata : SeqData
-        The SeqData object to plot the logo for
-    filter_id : str
-        The filter_id to use to filter the logo
-    uns_key : str
-        The key in the sdata.uns dictionary that contains the importance scores
-    **kwargs : dict
-        The keyword arguments to pass to the SeqLogo object
-
-    Returns
-    -------
-    ax : matplotlib.axes._subplots.AxesSubplot
-        The matplotlib axes object
-    """
-    logo = _plot_logo_seqlogo(sdata.uns[uns_key][filter_id], **kwargs)
-    if return_logo:
-        return logo
-
-
 def seq_track(
     sdata,
     seq_id: str,
-    uns_key: str,
+    attrs_key: str,
+    id_key="id",
     vocab: str = "DNA",
     highlights: list = [],
     highlight_colors: list = ["lavenderblush", "lightcyan", "honeydew"],
-    title: str ="",
+    title: str = "",
     ylab: str = "Saliency",
     xlab: str = "Position",
     return_ax: bool = False,
     save: PathLike = None,
     **kwargs,
 ):
     """
     Plot a track of the importance scores for a sequence using the logomaker package
-    
+
     This function is a wrapper around the logomaker Logo function. See the logomaker documentation
     for more details on the kwargs that can be passed to this function.
 
     Currently does no allow for features to be plotted (users must do them themselves on returned axes) or
     for sequence only plotting (i.e. importance scores must be passed in through the uns key)
 
     Parameters
@@ -471,94 +402,99 @@
         The ID of the sequence to plot
     uns_key : str
         The key in the sdata.uns dictionary that contains the importance scores
     vocab : str
         The vocabulary to use for the sequence
     highlights : list
         A list of positions to highlight in the sequence
-    highlight_colors : list 
+    highlight_colors : list
         A list of colors to use for the highlights
     title : str
         The title to use for the plot
     ylab : str
         The y-axis label to use for the plot
     xlab : str
         The x-axis label to use for the plot
     return_ax : bool
         Whether to return the axes object
 
     Returns
     -------
     ax : matplotlib.axes._subplots.AxesSubplot
         The matplotlib axes object
-    """ 
+    """
     if isinstance(highlights, tuple):
         highlights = [highlights]
     if isinstance(highlight_colors, str):
         highlight_colors = [highlight_colors] * len(highlights)
-    seq_idx = np.where(sdata.seqs_annot.index == seq_id)[0][0]
-    imp_scores = sdata.uns[uns_key][seq_idx] if uns_key in sdata.uns.keys() else None
-    viz_seq = pd.DataFrame(imp_scores.T, columns=vocab_dict[vocab])
+    seq_idx = np.where(sdata[id_key].to_numpy() == seq_id)[0]
+    attrs = sdata[attrs_key][seq_idx].squeeze()
+    viz_seq = pd.DataFrame(attrs.T, columns=vocab_dict[vocab])
     viz_seq.index.name = "pos"
     y_max = np.max(viz_seq.values)
     y_min = np.min(viz_seq.values)
     nn_logo = lm.Logo(viz_seq, **kwargs)
 
     # style using Logo methods
     nn_logo.style_spines(visible=False)
-    nn_logo.style_spines(spines=["left"], visible=True, bounds=[y_min, y_max])
+    if float(y_min) == 0 and float(y_max) == 0:
+        nn_logo.style_spines(spines=["left"], visible=False)
+    else:
+        nn_logo.style_spines(
+            spines=["left"], visible=True, bounds=[float(y_min), float(y_max)]
+        )
 
     # style using Axes methods
     nn_logo.ax.set_xlim([0, len(viz_seq)])
     nn_logo.ax.set_xticks([])
     nn_logo.ax.set_ylim([y_min, y_max])
     nn_logo.ax.set_ylabel(ylab)
     nn_logo.ax.set_xlabel(xlab)
     nn_logo.ax.set_title(title)
     for i, highlight in enumerate(highlights):
+        print(highlight)
         nn_logo.highlight_position_range(
-            pmin=highlight[0], 
-            pmax=highlight[1], 
-            color=highlight_colors[i]
+            pmin=int(highlight[0]), pmax=int(highlight[1]), color=highlight_colors[i]
         )
     if save is not None:
         _save_fig(save)
     if return_ax:
         return nn_logo.ax
 
 
 def multiseq_track(
     sdata,
     seq_ids: list,
-    uns_keys: str = None,
+    attrs_keys: str,
+    id_key="id",
     ylabs: list = None,
     width: int = None,
     height: int = None,
     return_axes: bool = False,
     save: str = None,
     **kwargs,
 ):
-    """ 
+    """
     Plot the saliency tracks for multiple sequences across multiple importance scores in one plot.
 
-    Wraps the seq_track function to plot multiple sequences at once across multiple importance scores. 
+    Wraps the seq_track function to plot multiple sequences at once across multiple importance scores.
 
     Attempts to make each sequence width proportional to its length and multiply by the number of sequences
     if no width is passed in.
 
-    Attempts to make each sequence height proportional to the number of uns_keys passed in (the number of different
+    Attempts to make each sequence height proportional to the number of attr_keys passed in (the number of different
     importance scores to plot) if no height is passed in.
 
     Parameters
     ----------
     sdata : SeqData
         The SeqData object with sequences and importances to plot a logo for
     seq_ids : list
         The sequence ids to plot
-    uns_keys : list
+    attr_keys : list
         The keys in the sdata.uns dictionary that contain the importance scores to plot
     ylabs : list
         The ylabs to use for each importance score
     width : int
         The width of the figure to plot
     height : int
         The height of the figure to plot
@@ -572,29 +508,36 @@
     Returns
     -------
     axes : list
         The axes objects if return_axes is True
     """
     if isinstance(seq_ids, str):
         seq_ids = [seq_ids]
-    if isinstance(uns_keys, str):
-        uns_keys = [uns_keys]
+    if isinstance(attrs_keys, str):
+        attrs_keys = [attrs_keys]
     if isinstance(ylabs, str):
         ylabs = [ylabs]
-    seq = sdata.seqs[0]
-    ylabs= ylabs if ylabs is not None else ["Importance Score"] * len(uns_keys)
-    fig_width = (len(seq_ids) * int(len(seq) / 20) if width is None else width)  
-    fig_height = (len(uns_keys) * 4 if height is None else height)
-    _, ax = plt.subplots(len(uns_keys), len(seq_ids), figsize=(fig_width, fig_height))
-    for i, uns_key in tqdm(enumerate(uns_keys), desc="Importance values", position=0, total=len(uns_keys)):
+    example_attr = sdata[attrs_keys[0]][0]
+    seq_len = example_attr.sizes["length"]
+    ylabs = ylabs if ylabs is not None else ["Importance Score"] * len(attrs_keys)
+    fig_width = len(seq_ids) * int(len(seq_len) / 20) if width is None else width
+    fig_height = len(attrs_keys) * 4 if height is None else height
+    _, ax = plt.subplots(len(attrs_keys), len(seq_ids), figsize=(fig_width, fig_height))
+    for i, attrs_key in tqdm(
+        enumerate(attrs_keys),
+        desc="Importance values",
+        position=0,
+        total=len(attrs_keys),
+    ):
         for j, seq_id in enumerate(seq_ids):
             seq_track(
                 sdata,
                 seq_id=seq_id,
-                uns_key=uns_key,
+                attrs_key=attrs_key,
+                id_key=id_key,
                 ax=ax.flatten()[i * len(seq_ids) + j],
                 ylab=ylabs[i],
                 title=seq_id,
                 save=None,
                 **kwargs,
             )
     plt.tight_layout()
@@ -602,33 +545,33 @@
         _save_fig(save)
     if return_axes:
         return ax
 
 
 def filter_viz(
     sdata,
-    filter_id: Union[str, int],
-    uns_key: str = "pfms",
+    filter_num: Union[str, int],
+    pfms_key: str,
     vocab: str = "DNA",
     title: str = None,
     return_ax: bool = False,
     save: str = None,
     **kwargs,
 ):
-    """ 
+    """
     Plot the PFM for a single filter in a SeqData object's uns dictionary as a PWM logo
 
     This function also uses logomaker to generate the PWM and plot it. Check out the logomaker documentation
     for more information on how to style the plot.
 
     Parameters
     ----------
     sdata : SeqData
         The SeqData object with sequences and pfms to plot a logo for
-    filter_id : str or int
+    filter_num : str or int
         The filter id to plot
     uns_key : str
         The key in the sdata.uns dictionary that contains the pfms to plot
     vocab : str
         The vocabulary to use for the logo
     title : str
         The title to use for the plot, defaults to the filter id if None
@@ -636,194 +579,93 @@
         Whether to return the matplotlib axes object
 
     Returns
     -------
     ax : matplotlib.axes.Axes
         The axes object if return_ax is True
     """
-    pfm = sdata.uns[uns_key][filter_id]
-    if isinstance(pfm, np.ndarray):
-        pfm = pd.DataFrame(pfm, columns=vocab_dict[vocab])
+    pfm = sdata[pfms_key][filter_num].squeeze()
+    pfm = pd.DataFrame(pfm, columns=vocab_dict[vocab])
     vocab = vocab_dict[vocab]
-    if pfm[vocab[0]].dtype == "float64":
-        pfm.fillna(0.25, inplace=True)
-        info_mat = lm.transform_matrix(
-            pfm, 
-            from_type="probability", 
-            to_type="information"
-        )
-    elif pfm[vocab.keys[0]].dtype == "int64":
-        pfm.fillna(1, inplace=True)
-        info_mat = lm.transform_matrix(
-            pfm, 
-            from_type="counts", 
-            to_type="information", 
-            allow_nan=True
-        )
+    pfm.fillna(1, inplace=True)
+    info_mat = lm.transform_matrix(
+        pfm,
+        from_type="counts",
+        to_type="information",
+    )
     if "N" in pfm.columns:
         info_mat = info_mat.drop("N", axis=1)
     logo = lm.Logo(info_mat, **kwargs)
     logo.style_xticks(spacing=5, anchor=25, rotation=45, fmt="%d", fontsize=14)
     logo.style_spines(visible=False)
     logo.style_spines(spines=["left", "bottom"], visible=True, linewidth=2)
     logo.ax.set_ylim([0, 2])
     logo.ax.set_yticks([0, 1, 2])
     logo.ax.set_yticklabels(["0", "1", "2"])
     logo.ax.set_ylabel("bits")
-    logo.ax.set_title(title if title is not None else filter_id)
+    logo.ax.set_title(title if title is not None else filter_num)
     if save is not None:
         _save_fig(save)
     if return_ax:
         return logo.ax
 
 
 def multifilter_viz(
     sdata,
-    filter_ids: list,
+    filter_nums: list,
+    pfms_key: str,
     num_rows: int = None,
     num_cols: int = None,
-    uns_key: str = "pfms",
     titles: list = None,
-    figsize=(12,10),
+    figsize=(12, 10),
     save: PathLike = None,
     **kwargs,
 ):
     """
     Plot multiple filters in a SeqData object's uns dictionary as PWM logos.
 
     This function wraps filter_viz. Getting the figure to look nice it more of an art
     than a science. In experimenting so far, I've found that a 8x4 grid with a (12, 10)
-    figure size works well. 
+    figure size works well.
 
-    Parameters 
+    Parameters
     ----------
     sdata : SeqData
         The SeqData object with sequences and pfms to plot a logo for
-    filter_ids : list
+    filter_nums : list
         The filter ids to plot
     num_rows : int
         The number of rows to use for the figure
     num_cols : int
         The number of columns to use for the figure
     uns_key : str
         The key in the sdata.uns dictionary that contains the pfms to plot
     titles : list
         The titles to use for the plots, defaults to the filter ids if None
     figsize : tuple
         The figure size to use for the plot
     save : PathLike
         The path to save the figure to
-    
+
     Returns
     -------
     axes : list
         The axes objects if return_axes is True
     """
 
     _, ax = plt.subplots(num_rows, num_cols, figsize=figsize)
     for i in range(num_rows):
         for j in range(num_cols):
-            filter_id = filter_ids[i * num_cols + j]
+            filter_num = filter_nums[i * num_cols + j]
             filter_viz(
                 sdata,
-                filter_id=filter_id,
-                uns_key=uns_key,
+                filter_num=filter_num,
+                pfms_key=pfms_key,
                 ax=ax.flatten()[i * num_cols + j],
-                title=titles[i * num_cols + j] if titles is not None else filter_id,
+                title=titles[i * num_cols + j] if titles is not None else filter_num,
                 save=None,
                 **kwargs,
             )
 
     plt.tight_layout()
     if save is not None:
         _save_fig(save)
-
-
-def kipoi_ism_heatmap(
-    sdata, 
-    seq_id: Union[str, int], 
-    uns_key: str = "NaiveISM_imps", 
-    figsize: tuple = (15, 2.5),
-    save: PathLike = None,
-    return_axes: bool = False
-):
-    """ 
-    Wrapper function around Kipoi's seqlogo_heatmap function that generates a really 
-    nice heatmap of the importance scores for a single sequence in a SeqData object's
-    uns dictionary.
-
-    Parameters
-    ----------
-    sdata : SeqData
-        The SeqData object with sequences and importance scores to plot a heatmap for
-    seq_id : str or int
-        The sequence id to plot
-    uns_key : str
-        The key in the sdata.uns dictionary that contains the importance scores to plot
-    figsize : tuple
-        The figure size to use for the plot
-    save : PathLike
-        The path to save the figure to
-    return_axes : bool
-        Whether to return the matplotlib axes object
-    
-    Returns
-    -------
-    ax : matplotlib.axes.Axes
-    """
-    from ..external.kipoi.kipoi_veff.plot import seqlogo_heatmap
-    seq_idx = np.where(sdata.seqs_annot.index == seq_id)[0][0]
-    val = sdata.uns[uns_key][seq_idx]
-    ax = plt.figure(figsize=figsize)
-    seqlogo_heatmap(val.T, val, ax=plt.subplot())
-    if save:
-        _save_fig(save)
-    if return_axes:
-        return ax
-
-
-def feature_implant_plot(
-    sdata, 
-    seqsm_keys: list, 
-    xlab: str = "Position",
-    ylab: str = "Predicted Score",
-    save: PathLike = None, 
-    return_axes: bool = False
-):
-    """ 
-    Plot a lineplot for each position of the sequence after implanting a feature.
-
-    Assumes that the value corresponding to each seqsm_key in the sdata.uns dictionary
-    has the same shape, namely (L, ) where L are the positions where a feature was implanted
-    and scores were calculated using a model. Plots the scores as a line plot with a 95% CI
-    corresponding to the number of sequences used to make the plot.
-
-    Parameters
-    ----------
-    sdata : SeqData
-        The SeqData object with sequences and scores to plot
-    seqsm_keys : list
-        The keys in the sdata.uns dictionary that contain the scores to plot
-    xlab : str
-        The x-axis label
-    ylab : str
-        The y-axis label
-    save : PathLike
-        The path to save the figure to
-    return_axes : bool
-        Whether to return the matplotlib axes object
-    """
-    concat_df = pd.DataFrame()
-    for seqsm_key in seqsm_keys:
-        df = pd.DataFrame(index=sdata.names, data=sdata.seqsm[seqsm_key]).melt(
-            var_name=xlab, 
-            value_name=ylab, 
-            ignore_index=False
-        )
-        df["feature"] = seqsm_key
-        concat_df = pd.concat([concat_df, df])
-    concat_df.reset_index(drop=True, inplace=True)
-    g = sns.lineplot(data=concat_df, x=xlab, y=ylab, hue="feature")
-    if save:
-        _save_fig(save)
-    if return_axes:
-        return g
```

### Comparing `eugene-tools-0.0.6/eugene/plot/_summary.py` & `eugene_tools-0.1.0/eugene/plot/_summary.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from os import PathLike
 from typing import Union
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 from sklearn.metrics import r2_score, mean_squared_error
-from sklearn.metrics import accuracy_score, roc_auc_score, average_precision_score, precision_score, recall_score, f1_score
+from sklearn.metrics import (
+    accuracy_score,
+    roc_auc_score,
+    average_precision_score,
+    precision_score,
+    recall_score,
+    f1_score,
+)
 from scipy.stats import spearmanr, pearsonr, kendalltau
 from ._utils import _plot_seaborn, _save_fig
 from .. import settings
 
 
 metric_dict = {
     "r2": r2_score,
@@ -17,15 +24,15 @@
     "pearson": pearsonr,
     "kendall": kendalltau,
     "accuracy": accuracy_score,
     "roc_auc": roc_auc_score,
     "average_precision": average_precision_score,
     "precision": precision_score,
     "recall": recall_score,
-    "f1": f1_score
+    "f1": f1_score,
 }
 
 
 def _model_performances_across_groups(
     sdataframe: pd.DataFrame,
     target_key: str,
     prediction_keys: list = None,
@@ -34,25 +41,25 @@
     metrics: str = "r2",
     clf_thresh: float = 0,
     **kwargs
 ):
     """
     Calculate model performance for a metric or set of metrics across groups.
 
-    Compares a target column to a set of prediction column in sdataframe 
+    Compares a target column to a set of prediction column in sdataframe
     and calculates the performance of the model for each group in groupby.
 
     Parameters
     ----------
     sdataframe : pd.DataFrame
         A dataframe containing the target and prediction columns in target_key and prediction_keys respectively.
     target_key : str
         The name of the column in sdataframe containing the target values.
     prediction_keys : list, optional
-        A list of the names of the columns in sdataframe containing the prediction values. 
+        A list of the names of the columns in sdataframe containing the prediction values.
         If None, all columns containing "predictions" in their name will be used.
     prediction_groups : list, optional
         A list of the names of the groups for each prediction column.
     groupby : str, optional
         The name of the column in sdataframe to group by. If None, the prediction_groups will be used.
     metrics : str, optional
         The name of the metric to calculate. If None, all metrics will be calculated.
@@ -66,72 +73,92 @@
         A dataframe containing the calculated metrics for each group.
     """
     if isinstance(metrics, str):
         metrics = [metrics]
     prediction_keys = (
         sdataframe.columns[sdataframe.columns.str.contains("predictions")]
         if prediction_keys is None
-        else prediction_keys 
+        else prediction_keys
     )
     conc = pd.DataFrame()
     for group, data in sdataframe.groupby(groupby):
         predicts = data[prediction_keys]
         bin_predicts = (predicts >= clf_thresh).astype(int)
         true = data[target_key]
         scores = pd.DataFrame()
         for metric in metrics:
             func = metric_dict[metric]
             if metric in ["r2", "mse"]:
                 scores = pd.concat(
-                    [scores, predicts.apply(lambda x: func(true, x), axis=0).to_frame(name=metric)],
+                    [
+                        scores,
+                        predicts.apply(lambda x: func(true, x), axis=0).to_frame(
+                            name=metric
+                        ),
+                    ],
                     axis=1,
                 )
             elif metric in ["spearman", "pearson", "kendall"]:
                 scores = pd.concat(
-                    [scores, predicts.apply(lambda x: func(true, x)[0], axis=0).to_frame(name=metric)],
+                    [
+                        scores,
+                        predicts.apply(lambda x: func(true, x)[0], axis=0).to_frame(
+                            name=metric
+                        ),
+                    ],
                     axis=1,
                 )
             elif metric in ["accuracy", "precision", "recall"]:
                 scores = pd.concat(
-                    [scores, bin_predicts.apply(lambda x: func(true, x), axis=0).to_frame(name=metric)],
+                    [
+                        scores,
+                        bin_predicts.apply(lambda x: func(true, x), axis=0).to_frame(
+                            name=metric
+                        ),
+                    ],
                     axis=1,
                 )
             elif metric in ["roc_auc", "average_precision"]:
                 scores = pd.concat(
-                    [scores, predicts.apply(lambda x: func(true, x), axis=0).to_frame(name=metric)],
+                    [
+                        scores,
+                        predicts.apply(lambda x: func(true, x), axis=0).to_frame(
+                            name=metric
+                        ),
+                    ],
                     axis=1,
                 )
         scores[groupby] = group
         if prediction_groups is not None:
             scores["prediction_groups"] = prediction_groups
         conc = pd.concat([conc, scores])
     return conc
 
 
 def _model_performances(
-    sdataframe: pd.DataFrame, 
+    sdataframe: pd.DataFrame,
     target_key: str,
-    prediction_keys: list = None, 
-    prediction_groups: list = None, 
-    metrics: str = "r2", 
-    clf_thresh: float = 0
+    prediction_keys: list = None,
+    prediction_groups: list = None,
+    metrics: str = "r2",
+    clf_thresh: float = 0,
 ):
-    """ 
+    """
     Calculate model performance for a metric or set of metrics.
 
     Uses columns from a passed in dataframe to calcuate a set of metrics.
 
     Parameters
     ----------
     sdataframe : pd.DataFrame
         A dataframe containing the target and prediction columns in target_key and prediction_keys respectively.
     target_key : str
         The name of the column in sdataframe containing the target values.
     prediction_keys : list, optional
-        A list of the names of the columns in sdataframe containing the prediction values. 
+        A list of the names of the columns in sdataframe containing the prediction values.
         If None, all columns containing "predictions" in their name will be used.
     prediction_groups : list, optional
         A list of the names of the groups for each prediction column.
     groupby : str, optional
         The name of the column in sdataframe to group by. If None, the prediction_groups will be used.
     metrics : str, optional
         The name of the metric to calculate. If None, all metrics will be calculated.
@@ -141,38 +168,57 @@
     -------
     pd.DataFrame
         A dataframe containing the calculated metrics.
     """
     if isinstance(metrics, str):
         metrics = [metrics]
     true = sdataframe[target_key]
-    prediction_keys = (
-        sdataframe.columns[sdataframe.columns.str.contains("predictions")]
-        if prediction_keys is None
-        else prediction_keys 
-    )
     predicts = sdataframe[prediction_keys]
     bin_predicts = (predicts >= clf_thresh).astype(int)
     scores = pd.DataFrame()
     for metric in metrics:
         func = metric_dict[metric]
         if metric in ["r2", "mse"]:
-            scores = pd.concat([scores, predicts.apply(lambda x: func(true, x), axis=0).to_frame(name=metric)],
+            scores = pd.concat(
+                [
+                    scores,
+                    predicts.apply(lambda x: func(true, x), axis=0).to_frame(
+                        name=metric
+                    ),
+                ],
                 axis=1,
             )
         elif metric in ["spearman", "pearson", "kendall"]:
-            scores = pd.concat([scores, predicts.apply(lambda x: func(true, x)[0], axis=0).to_frame(name=metric)],
+            scores = pd.concat(
+                [
+                    scores,
+                    predicts.apply(lambda x: func(true, x)[0], axis=0).to_frame(
+                        name=metric
+                    ),
+                ],
                 axis=1,
             )
         elif metric in ["accuracy", "precision", "recall", "f1"]:
-            scores = pd.concat([scores, bin_predicts.apply(lambda x: func(true, x), axis=0).to_frame(name=metric)],
+            scores = pd.concat(
+                [
+                    scores,
+                    bin_predicts.apply(lambda x: func(true, x), axis=0).to_frame(
+                        name=metric
+                    ),
+                ],
                 axis=1,
             )
         elif metric in ["roc_auc", "average_precision"]:
-            scores = pd.concat([scores, predicts.apply(lambda x: func(true, x), axis=0).to_frame(name=metric)],
+            scores = pd.concat(
+                [
+                    scores,
+                    predicts.apply(lambda x: func(true, x), axis=0).to_frame(
+                        name=metric
+                    ),
+                ],
                 axis=1,
             )
     if prediction_groups is not None:
         scores["prediction_groups"] = prediction_groups
     return scores
 
 
@@ -221,36 +267,34 @@
         A dictionary of rcParams to pass to matplotlib. Default is settings.rc_context.
     return_axes : bool, optional
         Whether to return the axes object. Default is False.
     save : PathLike, optional
         The path to save the figure to. Default is None.
     **kwargs
         Additional keyword arguments to pass to sns.violinplot.
-    
+
     Returns
     -------
     ax : matplotlib.axes.Axes
     """
-    sdataframe = sdata.seqs_annot
+    prediction_keys = prediction_keys = (
+        [k for k in sdata.keys() if "preds" in k]
+        if prediction_keys is None
+        else prediction_keys
+    )
+    sdataframe = (
+        sdata[["id"] + [target_key] + prediction_keys].to_dataframe().set_index("id")
+    )
     if groupby is None:
         scores = _model_performances(
-            sdataframe, 
-            target_key, 
-            prediction_keys, 
-            prediction_groups, 
-            metrics
+            sdataframe, target_key, prediction_keys, prediction_groups, metrics
         )
     else:
         scores = _model_performances_across_groups(
-            sdataframe, 
-            target_key, 
-            prediction_keys, 
-            prediction_groups, 
-            groupby, 
-            metrics
+            sdataframe, target_key, prediction_keys, prediction_groups, groupby, metrics
         )
     with plt.rc_context(rc_context):
         ax = _plot_seaborn(
             scores,
             keys=metrics,
             func=sns.boxplot,
             groupby="prediction_groups" if groupby is None else groupby,
```

### Comparing `eugene-tools-0.0.6/eugene/plot/_training.py` & `eugene_tools-0.1.0/eugene/plot/_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
-from os import PathLike
 import glob
-import matplotlib.pyplot as plt
 import seaborn as sns
+from os import PathLike
+import matplotlib.pyplot as plt
 from ._utils import (
     _plot_seaborn,
     many_logs2pandas,
     _save_fig,
 )
 from .. import settings
 
@@ -14,15 +14,15 @@
 def metric_curve(
     log_path: str = None,
     metric: str = None,
     hue: str = "metric",
     title: str = None,
     xlab: str = "minibatch step",
     ylab: str = None,
-    ax = None,
+    ax=None,
     return_axes: bool = False,
     **kwargs
 ) -> None:
     """
     Plots the loss curves from a PyTorch Lightning (PL) training run.
 
     Uses the tensorboard event file to extract the loss curves. The loss curves are extracted from the event file and
@@ -71,15 +71,15 @@
 
 
 def loss_curve(
     log_path: PathLike = None,
     title: str = None,
     xlab: str = "minibatch_step",
     ylab: str = "loss",
-    ax = None,
+    ax=None,
     return_axes: bool = False,
     **kwargs
 ) -> None:
     """
     Plots the loss curves from a PyTorch Lightning (PL) training run. Wraps metrics_curve function.
 
     Uses the tensorboard event file to extract the metric curves. The metric curves are extracted from the event file and
@@ -103,37 +103,31 @@
 
     Returns
     -------
     If return_axes is True, returns the axes object.
     """
     log_path = settings.logging_dir if log_path is None else log_path
     ax = metric_curve(
-        log_path, 
-        metric="loss", 
-        title=title, 
-        xlab=xlab, 
-        ylab=ylab, 
-        ax=ax,
-        **kwargs
+        log_path, metric="loss", title=title, xlab=xlab, ylab=ylab, ax=ax, **kwargs
     )
     if return_axes:
         return ax
 
 
 def training_summary(
-    log_path: PathLike = None, 
-    metric: str = "r2", 
+    log_path: PathLike = None,
+    metric: str = "r2",
     figsize=(12, 6),
-    save: str = None, 
+    save: str = None,
     return_axes: bool = False,
     **kwargs
 ) -> None:
     """
     Plots the training summary from a given training run
-    
+
     Convenience function to plot loss and metric together.
 
     Parameters
     ----------
     log_path : str
         Path to tensorboard log directory.
     metrics : str or list of str
```

### Comparing `eugene-tools-0.0.6/eugene/plot/_utils.py` & `eugene_tools-0.1.0/eugene/plot/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import os
-from os import PathLike
 import traceback
 import numpy as np
 import pandas as pd
-import matplotlib.pyplot as plt
 import seaborn as sns
+from .. import settings
+from os import PathLike
+import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
 from typing import List, Union, Sequence
 from tensorboard.backend.event_processing.event_accumulator import EventAccumulator
-from .. import settings
 
-def _create_matplotlib_axes(
-    num_axes, 
-    subplot_size=(4, 4)
-) -> List[Axes]:
+
+def _create_matplotlib_axes(num_axes, subplot_size=(4, 4)) -> List[Axes]:
     """
-    Creates and returns a list of matplotlib axes. 
-    
+    Creates and returns a list of matplotlib axes.
+
     Uses at most 3 columns before breaking into a new row.
     By default each subplot is 4x4.
 
     Parameters
     ----------
     num_axes : int
         Number of axes to create.
@@ -39,21 +37,15 @@
         num_cols,
         figsize=(num_cols * subplot_size[0], num_rows * subplot_size[1]),
     )
     ax = ax.flatten() if num_axes > 1 else ax
     return ax
 
 
-def _label_plot(
-    ax: Axes, 
-    title: str, 
-    xlab: str, 
-    ylab: str, 
-    xtick_rot: int = 0
-) -> None:
+def _label_plot(ax: Axes, title: str, xlab: str, ylab: str, xtick_rot: int = 0) -> None:
     """
     Labels a passed in axes with a title, x-axis label, and y-axis label.
 
     Optinally rotate the x-axis if you have long labels.
 
     Parameters
     ----------
@@ -74,19 +66,16 @@
     if xtick_rot != 0:
         ax.set_xticklabels(ax.get_xticklabels(), rotation=xtick_rot)
     ax.set_ylabel(ylab)
     ax.set_title(title)
     plt.tight_layout()
 
 
-def _save_fig(
-    file_path: PathLike,
-    dpi=settings.dpi
-):
-    """ 
+def _save_fig(file_path: PathLike, dpi=settings.dpi):
+    """
     Save a figure to a file path.
 
     Creates the filepath if it doesn't exist.
     Uses the dpi specified in package settings.
     """
     if "/" not in file_path:
         file_path = os.path.join(os.getcwd(), file_path)
@@ -137,15 +126,15 @@
         Label for y-axis.
     figsize : tuple of ints
         Size of figure to plot. By default, (10, 5).
     save : str
         Path to save figure. If None, then figure is not saved.
         Note that this will create a directory if it does not exist.
     **kwargs
-        Additional keyword arguments to pass to seaborn. This will be 
+        Additional keyword arguments to pass to seaborn. This will be
         dependent on func
 
     Returns
     -------
     matplotlib.axes.Axes
     """
     keys = [keys] if isinstance(keys, str) else keys
@@ -167,62 +156,62 @@
         _label_plot(
             curr_ax,
             title,
             xlab=key if xlab is None else xlab,
             xtick_rot=xtick_rot,
             ylab=ylab,
         )
-    #plt.show()
+    # plt.show()
     if save is not None:
         _save_fig(save)
     return ax
 
 
 def _violin_long(
-    sdata,
+    dataframe,
     groups: Union[str, Sequence[str]],
     title: str = None,
     xlab: str = "variable",
     xtick_rot: int = 0,
     ylab: str = "value",
     figsize: tuple = (8, 8),
     save: PathLike = None,
     ax: Axes = None,
-    **kwargs
+    **kwargs,
 ):
     """
-    Plots a violinplot using seaborn on an SeqData object.
-    The difference between this and the _plot_seaborn function is that
-    this function takes a list of groups and plots them on the same
-    plot (i.e. it takes in multiple columns and turns them into a single one
-    in long format. Then plots these as different groups)
-
-   Parameters
-    ----------
-    sdata : SeqData
-        SeqData object.
-    groups : str or list of str
-        Groups to plot.
-    xlabel : str
-        Label for x-axis.
-    ylabel : str
-        Label for y-axis.
-    figsize : tuple
-        Figure size.
-    save : str
-        Filepath to save figure to.
-    **kwargs
+     Plots a violinplot using seaborn on an SeqData object.
+     The difference between this and the _plot_seaborn function is that
+     this function takes a list of groups and plots them on the same
+     plot (i.e. it takes in multiple columns and turns them into a single one
+     in long format. Then plots these as different groups)
 
-    Returns
-    -------
-    None
+    Parameters
+     ----------
+     sdata : SeqData
+         SeqData object.
+     groups : str or list of str
+         Groups to plot.
+     xlabel : str
+         Label for x-axis.
+     ylabel : str
+         Label for y-axis.
+     figsize : tuple
+         Figure size.
+     save : str
+         Filepath to save figure to.
+     **kwargs
+
+     Returns
+     -------
+     None
     """
 
     groups = [groups] if isinstance(groups, str) else groups
-    long = sdata.seqs_annot.melt(value_vars=groups)
+    long = dataframe.melt(value_vars=groups)
     if ax is None:
         _, ax = plt.subplots(1, 1, figsize=figsize)
     sns.violinplot(data=long, x="variable", y="value", ax=ax, **kwargs)
     sns.stripplot(data=long, x="variable", y="value", ax=ax, color="black", alpha=0.75)
     _label_plot(
         ax,
         title,
@@ -239,16 +228,16 @@
     sdata,
     targets: Union[Sequence[str], str],
     predictions: Union[Sequence[str], str],
     labels: Union[Sequence[str], str],
 ):
     """
     Helper function to check input for plotting functions.
-    
-    Makes sure that the targets, predictions, and labels are all the same length.  
+
+    Makes sure that the targets, predictions, and labels are all the same length.
     """
     if isinstance(targets, str):
         targets = [targets]
     if isinstance(predictions, str):
         predictions = [predictions]
     if isinstance(labels, str):
         labels = [labels]
@@ -274,15 +263,15 @@
     Returns
     -------
     pd.DataFrame
         converted dataframe
 
     Note
     ----
-    Extraction function modified from 
+    Extraction function modified from
     https://github.com/theRealSuperMario/supermariopy/blob/master/scripts/tflogs2pandas.py
     """
     DEFAULT_SIZE_GUIDANCE = {
         "compressedHistograms": 1,
         "images": 1,
         "scalars": 0,  # 0 means load all
         "histograms": 1,
@@ -305,15 +294,15 @@
         traceback.print_exc()
     return runlog_data.reset_index(drop=True)
 
 
 def many_logs2pandas(event_paths):
     """
     Convert many tensorflow log files to pandas DataFrame.
-    
+
     Wraps around tflog2pandas to convert many tensorflow log files to a single
 
     Parameters
     ----------
     event_paths : list of str
         paths to tensorflow log files
 
@@ -329,16 +318,26 @@
             if all_logs.shape[0] == 0:
                 all_logs = log
             else:
                 all_logs = all_logs.append(log, ignore_index=True)
     return all_logs
 
 
-def _const_line(
-    *args, 
-    **kwargs
-):
+def _const_line(*args, **kwargs):
     """
     Plots a constant line on current axis
-    """ 
+    """
     x = np.arange(-1, 1.01, 0.01)
-    plt.plot(x, x, c='k', ls='--')
+    plt.plot(x, x, c="k", ls="--")
+
+def _collapse_pos(positions):
+    """Collapse neighbor positions of array to ranges"""
+    ranges = []
+    start = positions[0]
+    for i in range(1, len(positions)):
+        if positions[i - 1] == positions[i] - 1:
+            continue
+        else:
+            ranges.append((start, positions[i - 1] + 2))
+            start = positions[i]
+    ranges.append((start, positions[-1] + 2))
+    return ranges
```

### Comparing `eugene-tools-0.0.6/eugene/utils/_custom_callbacks.py` & `eugene_tools-0.1.0/eugene/evaluate/_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 import os
 import pandas as pd
 import numpy as np
-from pytorch_lightning.callbacks import Callback
 from pytorch_lightning.callbacks import BasePredictionWriter
-from pytorch_lightning.utilities.cli import CALLBACK_REGISTRY
 
 
 class PredictionWriter(BasePredictionWriter):
     def __init__(self, output_dir: str, file_label: str, write_interval="epoch"):
         super().__init__(write_interval)
         self.output_dir = output_dir
         if not os.path.exists(self.output_dir):
             os.makedirs(self.output_dir)
         self.file_label = file_label
 
     def write_on_epoch_end(self, trainer, pl_module, outputs, batch_indices):
-        outputs = np.concatenate(outputs[0], axis=0)
+        outputs = np.concatenate(outputs, axis=0)
         num_outputs = pl_module.output_dim
         pred_cols = [f"predictions_{i}" for i in range(num_outputs)]
         target_cols = [f"target_{i}" for i in range(num_outputs)]
-        pred_df = pd.DataFrame(
-            data=outputs, columns=["names"] + pred_cols + target_cols
-        )
+        pred_df = pd.DataFrame(data=outputs, columns=pred_cols + target_cols)
         pred_df.to_csv(
             os.path.join(self.output_dir, self.file_label) + "_predictions.tsv",
             sep="\t",
             index=False,
         )
-
```

