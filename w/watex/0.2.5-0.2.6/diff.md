# Comparing `tmp/watex-0.2.5.tar.gz` & `tmp/watex-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watex-0.2.5.tar", last modified: Thu Jun 22 07:45:30 2023, max compression
+gzip compressed data, was "watex-0.2.6.tar", last modified: Fri Jun 23 03:30:49 2023, max compression
```

## Comparing `watex-0.2.5.tar` & `watex-0.2.6.tar`

### file list

```diff
@@ -1,372 +1,374 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.715684 watex-0.2.5/
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.319450 watex-0.2.5/.github/
--rw-rw-rw-   0        0        0      524 2023-02-19 15:19:16.000000 watex-0.2.5/.github/dependabot.yml
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.322368 watex-0.2.5/.github/workflows/
--rw-rw-rw-   0        0        0     1616 2023-02-21 12:32:38.000000 watex-0.2.5/.github/workflows/ci.yaml
--rw-rw-rw-   0        0        0     3025 2023-02-19 15:19:16.000000 watex-0.2.5/.github/workflows/codeql.yml
--rw-rw-rw-   0        0        0      905 2023-02-19 15:19:16.000000 watex-0.2.5/.github/workflows/dependency-review.yml
--rw-rw-rw-   0        0        0     1457 2023-03-02 12:14:24.000000 watex-0.2.5/.github/workflows/python-package.yml
--rw-rw-rw-   0        0        0     3118 2023-05-07 17:25:43.000000 watex-0.2.5/.gitignore
--rw-rw-rw-   0        0        0      553 2023-03-17 13:03:23.000000 watex-0.2.5/CITATION.cff
--rw-rw-rw-   0        0        0     1548 2023-01-08 08:20:47.000000 watex-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     1045 2023-05-14 08:24:24.000000 watex-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0    15816 2023-06-22 07:45:30.716661 watex-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    14379 2023-05-24 12:02:39.000000 watex-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.338766 watex-0.2.5/docs/
--rw-rw-rw-   0        0        0      139 2023-02-18 10:33:13.000000 watex-0.2.5/docs/.gitignore
--rw-rw-rw-   0        0        0      658 2023-01-08 08:20:47.000000 watex-0.2.5/docs/Makefile
--rw-rw-rw-   0        0        0      251 2023-03-20 12:42:04.000000 watex-0.2.5/docs/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.355477 watex-0.2.5/docs/_static/
--rw-rw-rw-   0        0        0     2711 2023-01-08 08:52:36.000000 watex-0.2.5/docs/_static/copybutton.js
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.357424 watex-0.2.5/docs/_static/css/
--rw-rw-rw-   0        0        0   155712 2023-01-28 12:21:35.000000 watex-0.2.5/docs/_static/css/bootstrap.min.css
--rw-rw-rw-   0        0        0     7607 2023-05-13 16:07:36.000000 watex-0.2.5/docs/_static/css/custom.css
--rw-rw-rw-   0        0        0    70782 2023-02-01 10:38:29.000000 watex-0.2.5/docs/_static/favicon.ico
--rw-rw-rw-   0        0        0     1150 2023-01-30 16:08:53.000000 watex-0.2.5/docs/_static/favicon0.ico
--rw-rw-rw-   0        0        0     8356 2023-01-08 08:52:36.000000 watex-0.2.5/docs/_static/favicon_old.ico
--rw-rw-rw-   0        0        0     3519 2023-01-30 11:43:04.000000 watex-0.2.5/docs/_static/index_api.svg
--rw-rw-rw-   0        0        0     2528 2023-01-30 11:43:05.000000 watex-0.2.5/docs/_static/index_contribute.svg
--rw-rw-rw-   0        0        0     3977 2023-01-30 11:43:04.000000 watex-0.2.5/docs/_static/index_getting_started.svg
--rw-rw-rw-   0        0        0     6429 2023-01-30 11:43:05.000000 watex-0.2.5/docs/_static/index_user_guide.svg
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.306263 watex-0.2.5/docs/_static/js/
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.359370 watex-0.2.5/docs/_static/js/vendor/
--rw-rw-rw-   0        0        0    58030 2023-01-28 12:21:35.000000 watex-0.2.5/docs/_static/js/vendor/bootstrap.min.js
--rw-rw-rw-   0        0        0    72818 2023-01-28 12:21:35.000000 watex-0.2.5/docs/_static/js/vendor/jquery-3.6.3.slim.min.js
--rw-rw-rw-   0        0        0     1738 2023-02-02 06:30:47.000000 watex-0.2.5/docs/_static/logo.svg
--rw-rw-rw-   0        0        0     2346 2023-01-08 08:52:36.000000 watex-0.2.5/docs/_static/logo_no_name.svg
--rw-rw-rw-   0        0        0     1916 2023-01-28 05:52:08.000000 watex-0.2.5/docs/_static/logo_small.svg
--rw-rw-rw-   0        0        0     2631 2023-01-08 08:52:36.000000 watex-0.2.5/docs/_static/logo_wide.svg
--rw-rw-rw-   0        0        0     1916 2023-01-28 05:52:08.000000 watex-0.2.5/docs/_static/logo_wide_rev.svg
--rw-rw-rw-   0        0        0     3052 2023-01-08 08:52:36.000000 watex-0.2.5/docs/_static/logo_wide_rev0.svg
--rw-rw-rw-   0        0        0     1132 2023-06-20 12:20:59.000000 watex-0.2.5/docs/_static/switcher.json
--rw-rw-rw-   0        0        0      166 2023-01-28 15:18:48.000000 watex-0.2.5/docs/_static/theme.conf
--rw-rw-rw-   0        0        0     1464 2023-01-30 16:00:33.000000 watex-0.2.5/docs/_static/to_favicon.svg
--rw-rw-rw-   0        0        0   125058 2023-01-30 14:23:50.000000 watex-0.2.5/docs/_static/watex_thumb_image.svg
--rw-rw-rw-   0        0        0    26516 2023-01-30 05:05:07.000000 watex-0.2.5/docs/_static/watex_workflow.svg
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.362321 watex-0.2.5/docs/_templates/
--rw-rw-rw-   0        0        0     5128 2023-01-28 12:21:35.000000 watex-0.2.5/docs/_templates/javascript.html
--rw-rw-rw-   0        0        0      867 2023-05-25 11:10:55.000000 watex-0.2.5/docs/_templates/layout.html
--rw-rw-rw-   0        0        0       87 2023-01-09 10:30:31.000000 watex-0.2.5/docs/_templates/version.html
--rw-rw-rw-   0        0        0    16686 2023-02-01 15:09:39.000000 watex-0.2.5/docs/analysis.rst
--rw-rw-rw-   0        0        0    23500 2023-06-21 11:42:13.000000 watex-0.2.5/docs/api_references.rst
--rw-rw-rw-   0        0        0    15873 2023-04-14 23:54:09.000000 watex-0.2.5/docs/base.rst
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.363604 watex-0.2.5/docs/binder/
--rw-rw-rw-   0        0        0      258 2023-01-08 08:52:36.000000 watex-0.2.5/docs/binder/requirements.txt
--rw-rw-rw-   0        0        0    11688 2023-01-30 11:20:05.000000 watex-0.2.5/docs/cases.rst
--rw-rw-rw-   0        0        0     2772 2023-03-17 13:03:23.000000 watex-0.2.5/docs/citing.rst
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.363604 watex-0.2.5/docs/community/
--rw-rw-rw-   0        0        0     2322 2023-02-19 15:58:54.000000 watex-0.2.5/docs/community/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    16384 2023-03-25 08:21:17.000000 watex-0.2.5/docs/conf.py
--rw-rw-rw-   0        0        0    18198 2023-02-01 09:06:05.000000 watex-0.2.5/docs/datasets.rst
--rw-rw-rw-   0        0        0    16155 2023-02-05 16:03:43.000000 watex-0.2.5/docs/development.rst
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.364962 watex-0.2.5/docs/example_thumbs/
--rw-rw-rw-   0        0        0        0 2023-01-08 08:52:36.000000 watex-0.2.5/docs/example_thumbs/.gitkeep
--rw-rw-rw-   0        0        0    69141 2023-01-30 05:05:07.000000 watex-0.2.5/docs/example_thumbs/watex_workflow.gif
--rw-rw-rw-   0        0        0   100537 2023-03-12 07:09:50.000000 watex-0.2.5/docs/glossary.rst
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.368494 watex-0.2.5/docs/history/
--rw-rw-rw-   0        0        0     5834 2023-02-18 16:26:08.000000 watex-0.2.5/docs/history/five_min_understanding.rst
--rw-rw-rw-   0        0        0      385 2023-02-18 15:40:51.000000 watex-0.2.5/docs/history/index.rst
--rw-rw-rw-   0        0        0     5454 2023-02-21 12:32:38.000000 watex-0.2.5/docs/history/project_goals.rst
--rw-rw-rw-   0        0        0     9463 2023-02-20 11:39:27.000000 watex-0.2.5/docs/history/project_story.rst
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.370444 watex-0.2.5/docs/includes/
--rw-rw-rw-   0        0        0      762 2023-01-10 10:17:54.000000 watex-0.2.5/docs/includes/big_toc_css.rst
--rw-rw-rw-   0        0        0     1087 2023-01-10 10:19:34.000000 watex-0.2.5/docs/includes/bigger_toc_css.rst
--rw-rw-rw-   0        0        0     1918 2023-02-19 16:15:09.000000 watex-0.2.5/docs/index.rst
--rw-rw-rw-   0        0        0    12622 2023-03-19 07:20:06.000000 watex-0.2.5/docs/installation.rst
--rwxrwxrwx   0        0        0      804 2023-01-08 08:20:47.000000 watex-0.2.5/docs/make.bat
--rw-rw-rw-   0        0        0       20 2023-01-08 08:52:36.000000 watex-0.2.5/docs/matplotlibrc.txt
--rw-rw-rw-   0        0        0    46356 2023-02-18 06:46:56.000000 watex-0.2.5/docs/methods.rst
--rw-rw-rw-   0        0        0      548 2023-03-24 16:49:23.000000 watex-0.2.5/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.371417 watex-0.2.5/docs/source/
--rw-rw-rw-   0        0        0    20241 2023-01-10 14:10:18.000000 watex-0.2.5/docs/source/index.html
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.374337 watex-0.2.5/docs/sphinxext/
--rw-rw-rw-   0        0        0       43 2023-01-12 12:03:56.000000 watex-0.2.5/docs/sphinxext/MANIFEST.in
--rw-rw-rw-   0        0        0     6182 2023-01-12 11:57:22.000000 watex-0.2.5/docs/sphinxext/add_toctree_functions.py
--rw-rw-rw-   0        0        0     1784 2023-01-12 12:03:00.000000 watex-0.2.5/docs/sphinxext/doi_role.py
--rw-rw-rw-   0        0        0     8329 2023-01-12 12:01:15.000000 watex-0.2.5/docs/sphinxext/sphinx_issues.py
--rw-rw-rw-   0        0        0    16329 2023-02-05 13:07:26.000000 watex-0.2.5/docs/structure.rst
--rw-rw-rw-   0        0        0     3807 2023-01-10 10:22:10.000000 watex-0.2.5/docs/tune_toc.rst
--rw-rw-rw-   0        0        0      391 2023-02-02 12:44:21.000000 watex-0.2.5/docs/user_guide.rst
--rw-rw-rw-   0        0        0    42796 2023-01-30 09:59:53.000000 watex-0.2.5/docs/utils.rst
--rw-rw-rw-   0        0        0    76837 2023-02-10 02:52:23.000000 watex-0.2.5/docs/view.rst
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.387964 watex-0.2.5/docs/whatsnew/
--rw-rw-rw-   0        0        0      560 2023-06-20 12:32:10.000000 watex-0.2.5/docs/whatsnew/index.rst
--rw-rw-rw-   0        0        0     1737 2023-03-19 09:38:32.000000 watex-0.2.5/docs/whatsnew/v0.1.0.rst
--rw-rw-rw-   0        0        0     2801 2023-03-19 09:37:06.000000 watex-0.2.5/docs/whatsnew/v0.1.1.rst
--rw-rw-rw-   0        0        0     2202 2023-03-19 09:44:19.000000 watex-0.2.5/docs/whatsnew/v0.1.2.rst
--rw-rw-rw-   0        0        0     2120 2023-03-19 09:42:28.000000 watex-0.2.5/docs/whatsnew/v0.1.3.rst
--rw-rw-rw-   0        0        0     3469 2023-03-19 09:27:50.000000 watex-0.2.5/docs/whatsnew/v0.1.4.rst
--rw-rw-rw-   0        0        0     4092 2023-03-19 10:54:01.000000 watex-0.2.5/docs/whatsnew/v0.1.5.rst
--rw-rw-rw-   0        0        0    21723 2023-03-07 14:39:00.000000 watex-0.2.5/docs/whatsnew/v0.1.6-alpha.rst
--rw-rw-rw-   0        0        0     5019 2023-03-19 09:20:02.000000 watex-0.2.5/docs/whatsnew/v0.1.6.rst
--rw-rw-rw-   0        0        0     1457 2023-03-19 10:17:51.000000 watex-0.2.5/docs/whatsnew/v0.1.7.rst
--rw-rw-rw-   0        0        0     2108 2023-03-20 12:42:04.000000 watex-0.2.5/docs/whatsnew/v0.1.8.rst
--rw-rw-rw-   0        0        0     2042 2023-04-14 23:54:09.000000 watex-0.2.5/docs/whatsnew/v0.1.9.rst
--rw-rw-rw-   0        0        0     5730 2023-04-20 04:00:41.000000 watex-0.2.5/docs/whatsnew/v0.2.0.rst
--rw-rw-rw-   0        0        0     4070 2023-04-22 11:36:08.000000 watex-0.2.5/docs/whatsnew/v0.2.1.rst
--rw-rw-rw-   0        0        0     1093 2023-04-22 07:50:27.000000 watex-0.2.5/docs/whatsnew/v0.2.2.rst
--rw-rw-rw-   0        0        0     2011 2023-05-25 12:52:32.000000 watex-0.2.5/docs/whatsnew/v0.2.3.rst
--rw-rw-rw-   0        0        0     4124 2023-05-27 00:28:54.000000 watex-0.2.5/docs/whatsnew/v0.2.4.rst
--rw-rw-rw-   0        0        0     3337 2023-06-22 04:55:18.000000 watex-0.2.5/docs/whatsnew/v0.2.5.rst
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.388937 watex-0.2.5/examples/
--rw-rw-rw-   0        0        0      427 2023-01-11 10:44:04.000000 watex-0.2.5/examples/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.391857 watex-0.2.5/examples/analysis/
--rw-rw-rw-   0        0        0      109 2023-01-18 16:53:37.000000 watex-0.2.5/examples/analysis/README.txt
--rw-rw-rw-   0        0        0     1031 2023-01-11 15:25:23.000000 watex-0.2.5/examples/analysis/plot_decision_regions.py
--rw-rw-rw-   0        0        0     1171 2023-01-11 15:25:54.000000 watex-0.2.5/examples/analysis/plot_explained_variance_ratio.py
--rw-rw-rw-   0        0        0      875 2023-01-11 15:26:26.000000 watex-0.2.5/examples/analysis/plot_linear_discriminant_analysis.py
--rw-rw-rw-   0        0        0      541 2023-01-11 15:26:56.000000 watex-0.2.5/examples/analysis/plot_pca_vs_factor_with_scedatic_noises.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.395750 watex-0.2.5/examples/applications/
--rw-rw-rw-   0        0        0      510 2023-01-18 17:34:21.000000 watex-0.2.5/examples/applications/README.txt
--rw-rw-rw-   0        0        0     3329 2023-03-05 22:27:58.000000 watex-0.2.5/examples/applications/plot_auto_detect_drilling_location.py
--rw-rw-rw-   0        0        0     8710 2023-01-11 16:26:30.000000 watex-0.2.5/examples/applications/plot_data_exploratory_quick_view.py
--rw-rw-rw-   0        0        0    10236 2023-02-15 12:36:42.000000 watex-0.2.5/examples/applications/plot_dc_em_parameters_computings.py
--rw-rw-rw-   0        0        0     8084 2023-01-20 17:43:45.000000 watex-0.2.5/examples/applications/plot_flow_rate_prediction.py
--rw-rw-rw-   0        0        0    10004 2023-06-17 08:36:57.000000 watex-0.2.5/examples/applications/plot_kmf.py
--rw-rw-rw-   0        0        0     3325 2023-02-16 17:12:25.000000 watex-0.2.5/examples/applications/plot_nsamt_tensor_recovery.py
--rw-rw-rw-   0        0        0     5719 2023-03-17 13:03:23.000000 watex-0.2.5/examples/applications/plot_tensor_restoring.py
--rw-rw-rw-   0        0        0    11379 2023-05-25 12:48:47.000000 watex-0.2.5/examples/applications/plot_ymxs_label_for_k_prediction.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.396724 watex-0.2.5/examples/auto_examples/
--rw-rw-rw-   0        0        0        0 2023-01-25 09:04:31.000000 watex-0.2.5/examples/auto_examples/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.399644 watex-0.2.5/examples/base/
--rw-rw-rw-   0        0        0      141 2023-01-18 16:52:30.000000 watex-0.2.5/examples/base/README.txt
--rw-rw-rw-   0        0        0     1002 2023-01-11 15:30:46.000000 watex-0.2.5/examples/base/plot_ada_gd.py
--rw-rw-rw-   0        0        0     1032 2023-01-11 15:31:27.000000 watex-0.2.5/examples/base/plot_ada_stochastic_gd.py
--rw-rw-rw-   0        0        0      902 2023-01-11 15:31:50.000000 watex-0.2.5/examples/base/plot_missing.py
--rw-rw-rw-   0        0        0     1392 2023-01-11 15:32:51.000000 watex-0.2.5/examples/base/plot_sbs_feature_selector.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.405989 watex-0.2.5/examples/methods/
--rw-rw-rw-   0        0        0      106 2023-01-08 08:52:36.000000 watex-0.2.5/examples/methods/README.txt
--rw-rw-rw-   0        0        0      874 2023-01-20 17:25:23.000000 watex-0.2.5/examples/methods/plot_2d_tensor_filtered.py
--rw-rw-rw-   0        0        0     1071 2023-01-11 15:40:37.000000 watex-0.2.5/examples/methods/plot_anomaly.py
--rw-rw-rw-   0        0        0     1852 2023-01-11 15:41:46.000000 watex-0.2.5/examples/methods/plot_filtered_tensors.py
--rw-rw-rw-   0        0        0     1007 2023-01-11 15:43:30.000000 watex-0.2.5/examples/methods/plot_logging_predictor_and_target.py
--rw-rw-rw-   0        0        0      884 2023-01-11 15:44:27.000000 watex-0.2.5/examples/methods/plot_logging_predictor_only.py
--rw-rw-rw-   0        0        0      638 2023-01-11 15:44:36.000000 watex-0.2.5/examples/methods/plot_multiple_sites_recovery_signal.py
--rw-rw-rw-   0        0        0     2423 2023-03-02 12:26:23.000000 watex-0.2.5/examples/methods/plot_phase_tensors.py
--rw-rw-rw-   0        0        0      806 2023-01-11 15:44:59.000000 watex-0.2.5/examples/methods/plot_raw_2d_tensor.py
--rw-rw-rw-   0        0        0      915 2023-01-11 15:45:48.000000 watex-0.2.5/examples/methods/plot_ves_fracture_zone.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.420589 watex-0.2.5/examples/utils/
--rw-rw-rw-   0        0        0      125 2023-01-08 08:52:36.000000 watex-0.2.5/examples/utils/README.txt
--rw-rw-rw-   0        0        0      788 2023-01-09 07:43:08.000000 watex-0.2.5/examples/utils/plot_clusters.py
--rw-rw-rw-   0        0        0     2373 2023-03-06 16:32:37.000000 watex-0.2.5/examples/utils/plot_confidence_in_data.py
--rw-rw-rw-   0        0        0     1489 2023-01-11 15:46:32.000000 watex-0.2.5/examples/utils/plot_confusion_matrices.py
--rw-rw-rw-   0        0        0     1124 2023-01-09 07:43:29.000000 watex-0.2.5/examples/utils/plot_confusion_matrix_sweet.py
--rw-rw-rw-   0        0        0      526 2023-01-11 15:46:56.000000 watex-0.2.5/examples/utils/plot_elbow.py
--rw-rw-rw-   0        0        0     1758 2023-01-25 03:02:32.000000 watex-0.2.5/examples/utils/plot_erp.py
--rw-rw-rw-   0        0        0      655 2023-01-11 15:48:44.000000 watex-0.2.5/examples/utils/plot_errors_vs_epochs.py
--rw-rw-rw-   0        0        0      631 2023-01-11 15:49:01.000000 watex-0.2.5/examples/utils/plot_ex_heatmap.py
--rw-rw-rw-   0        0        0      717 2023-01-11 15:50:15.000000 watex-0.2.5/examples/utils/plot_ex_matrix.py
--rw-rw-rw-   0        0        0     1094 2023-01-11 15:50:34.000000 watex-0.2.5/examples/utils/plot_learning_curves.py
--rw-rw-rw-   0        0        0     1787 2023-01-11 15:51:32.000000 watex-0.2.5/examples/utils/plot_log.py
--rw-rw-rw-   0        0        0     1053 2023-01-09 07:44:13.000000 watex-0.2.5/examples/utils/plot_model_confusion_matrix.py
--rw-rw-rw-   0        0        0      751 2023-01-11 15:53:36.000000 watex-0.2.5/examples/utils/plot_naive_dendrogram.py
--rw-rw-rw-   0        0        0      716 2023-01-11 15:53:51.000000 watex-0.2.5/examples/utils/plot_naive_silhouette.py
--rw-rw-rw-   0        0        0      678 2023-01-11 15:54:53.000000 watex-0.2.5/examples/utils/plot_ohmic_area.py
--rw-rw-rw-   0        0        0      814 2023-01-08 08:52:36.000000 watex-0.2.5/examples/utils/plot_pca_components.py
--rw-rw-rw-   0        0        0      611 2023-01-11 15:55:25.000000 watex-0.2.5/examples/utils/plot_regularization_path.py
--rw-rw-rw-   0        0        0      623 2023-01-11 15:55:45.000000 watex-0.2.5/examples/utils/plot_rf_feature_importances.py
--rw-rw-rw-   0        0        0      966 2023-01-24 10:29:45.000000 watex-0.2.5/examples/utils/plot_savitzky_golay1d.py
--rw-rw-rw-   0        0        0     1132 2023-01-08 08:52:36.000000 watex-0.2.5/examples/utils/plot_sbs_feature_selection.py
--rw-rw-rw-   0        0        0     1793 2023-01-25 04:57:49.000000 watex-0.2.5/examples/utils/plot_sfi.py
--rw-rw-rw-   0        0        0     3121 2023-03-04 11:47:12.000000 watex-0.2.5/examples/utils/plot_skew.py
--rw-rw-rw-   0        0        0      618 2023-06-21 11:42:13.000000 watex-0.2.5/examples/utils/plot_stratalog.py
--rw-rw-rw-   0        0        0     2236 2023-03-19 08:17:21.000000 watex-0.2.5/examples/utils/plot_strike.py
--rw-rw-rw-   0        0        0      693 2023-05-14 06:02:07.000000 watex-0.2.5/examples/utils/plot_voronoi.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.441816 watex-0.2.5/examples/view/
--rw-rw-rw-   0        0        0      113 2023-01-18 16:54:11.000000 watex-0.2.5/examples/view/README.txt
--rw-rw-rw-   0        0        0      915 2023-01-24 02:59:52.000000 watex-0.2.5/examples/view/plot_2d_filtered_tensors.py
--rw-rw-rw-   0        0        0      933 2023-01-11 15:58:16.000000 watex-0.2.5/examples/view/plot_base_distributions.py
--rw-rw-rw-   0        0        0     1101 2023-01-16 18:53:31.000000 watex-0.2.5/examples/view/plot_biplot.py
--rw-rw-rw-   0        0        0      553 2023-01-11 15:59:22.000000 watex-0.2.5/examples/view/plot_box.py
--rw-rw-rw-   0        0        0     1678 2023-01-11 16:00:02.000000 watex-0.2.5/examples/view/plot_confusion_matrix_metric.py
--rw-rw-rw-   0        0        0      852 2023-01-08 08:52:36.000000 watex-0.2.5/examples/view/plot_correlating_features.py
--rw-rw-rw-   0        0        0      449 2023-01-11 16:01:24.000000 watex-0.2.5/examples/view/plot_correlation_missing_data.py
--rw-rw-rw-   0        0        0      599 2023-01-11 16:00:47.000000 watex-0.2.5/examples/view/plot_cut_comparison.py
--rw-rw-rw-   0        0        0      453 2023-01-11 16:01:48.000000 watex-0.2.5/examples/view/plot_dendro_missing_data.py
--rw-rw-rw-   0        0        0      921 2023-01-16 17:55:57.000000 watex-0.2.5/examples/view/plot_dendrogram.py
--rw-rw-rw-   0        0        0      854 2023-01-16 17:19:14.000000 watex-0.2.5/examples/view/plot_dendroheat.py
--rw-rw-rw-   0        0        0      920 2023-01-11 16:05:35.000000 watex-0.2.5/examples/view/plot_discussing_features.py
--rw-rw-rw-   0        0        0      697 2023-01-11 16:06:18.000000 watex-0.2.5/examples/view/plot_grid.py
--rw-rw-rw-   0        0        0      676 2023-01-11 16:06:48.000000 watex-0.2.5/examples/view/plot_hist.py
--rw-rw-rw-   0        0        0      888 2023-01-08 08:52:36.000000 watex-0.2.5/examples/view/plot_jointing_features.py
--rw-rw-rw-   0        0        0      644 2023-01-11 16:07:06.000000 watex-0.2.5/examples/view/plot_learning_inspections.py
--rw-rw-rw-   0        0        0     1365 2023-01-11 16:08:38.000000 watex-0.2.5/examples/view/plot_matshow.py
--rw-rw-rw-   0        0        0     2370 2023-01-11 16:10:01.000000 watex-0.2.5/examples/view/plot_model.py
--rw-rw-rw-   0        0        0      588 2023-01-11 16:10:11.000000 watex-0.2.5/examples/view/plot_model_inspection.py
--rw-rw-rw-   0        0        0     1964 2023-01-18 15:28:17.000000 watex-0.2.5/examples/view/plot_model_scores.py
--rw-rw-rw-   0        0        0      725 2023-01-09 07:52:42.000000 watex-0.2.5/examples/view/plot_multiple_feature_distributions.py
--rw-rw-rw-   0        0        0     1226 2023-01-09 07:52:51.000000 watex-0.2.5/examples/view/plot_num_features.py
--rw-rw-rw-   0        0        0     1241 2023-01-11 16:11:17.000000 watex-0.2.5/examples/view/plot_pairwise_corr.py
--rw-rw-rw-   0        0        0      524 2023-01-11 16:11:59.000000 watex-0.2.5/examples/view/plot_pararell_corrdinates.py
--rw-rw-rw-   0        0        0     1372 2023-01-11 16:12:35.000000 watex-0.2.5/examples/view/plot_pca.py
--rw-rw-rw-   0        0        0     5274 2023-03-04 05:56:10.000000 watex-0.2.5/examples/view/plot_phase_sensistive_skew.py
--rw-rw-rw-   0        0        0      818 2023-01-20 17:26:34.000000 watex-0.2.5/examples/view/plot_phase_tensor_2d.py
--rw-rw-rw-   0        0        0      817 2023-01-11 16:12:58.000000 watex-0.2.5/examples/view/plot_pr.py
--rw-rw-rw-   0        0        0     1893 2023-01-16 18:57:53.000000 watex-0.2.5/examples/view/plot_projection.py
--rw-rw-rw-   0        0        0      883 2023-01-11 16:18:27.000000 watex-0.2.5/examples/view/plot_radviz.py
--rw-rw-rw-   0        0        0      929 2023-01-11 16:19:02.000000 watex-0.2.5/examples/view/plot_reg_scoring.py
--rw-rw-rw-   0        0        0      869 2023-01-11 16:19:28.000000 watex-0.2.5/examples/view/plot_res_tensor_2d.py
--rw-rw-rw-   0        0        0     1939 2023-04-20 03:25:59.000000 watex-0.2.5/examples/view/plot_rhoa.py
--rw-rw-rw-   0        0        0     1757 2023-01-11 16:19:47.000000 watex-0.2.5/examples/view/plot_roc.py
--rw-rw-rw-   0        0        0      794 2023-01-11 16:20:19.000000 watex-0.2.5/examples/view/plot_scatter.py
--rw-rw-rw-   0        0        0     1523 2023-01-11 16:20:37.000000 watex-0.2.5/examples/view/plot_scattering_features.py
--rw-rw-rw-   0        0        0      543 2023-01-08 08:52:36.000000 watex-0.2.5/examples/view/plot_silhouette.py
--rw-rw-rw-   0        0        0      759 2023-01-09 07:56:02.000000 watex-0.2.5/examples/view/plot_single_site_signal_recovery.py
--rw-rw-rw-   0        0        0      834 2023-01-11 16:21:15.000000 watex-0.2.5/examples/view/plot_target_inspection.py
--rw-rw-rw-   0        0        0     1615 2023-06-22 05:08:26.000000 watex-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0      901 2023-06-22 07:45:30.718607 watex-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     4646 2023-05-25 04:59:14.000000 watex-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.479707 watex-0.2.5/watex/
--rw-rw-rw-   0        0        0     8552 2023-06-20 12:24:38.000000 watex-0.2.5/watex/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.514360 watex-0.2.5/watex/_build/
--rw-rw-rw-   0        0        0       27 2023-03-11 03:28:02.000000 watex-0.2.5/watex/_build/__init__.py
--rw-rw-rw-   0        0        0       30 2023-01-08 08:20:47.000000 watex-0.2.5/watex/_build/_check_build.pyx
--rw-rw-rw-   0        0        0      333 2023-01-08 08:20:47.000000 watex-0.2.5/watex/_distributor_init.py
--rw-rw-rw-   0        0        0    32160 2023-06-17 08:36:57.000000 watex-0.2.5/watex/_docstring.py
--rw-rw-rw-   0        0        0     3852 2023-03-11 03:28:02.000000 watex-0.2.5/watex/_isotonic.pyx
--rw-rw-rw-   0        0        0    17770 2023-04-14 23:54:09.000000 watex-0.2.5/watex/_typing.py
--rw-rw-rw-   0        0        0      218 2023-06-22 07:45:29.000000 watex-0.2.5/watex/_version.py
--rw-rw-rw-   0        0        0     8798 2023-03-12 01:49:05.000000 watex-0.2.5/watex/_watexlog.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.516764 watex-0.2.5/watex/analysis/
--rw-rw-rw-   0        0        0     1242 2023-02-04 08:11:48.000000 watex-0.2.5/watex/analysis/__init__.py
--rw-rw-rw-   0        0        0    23341 2023-01-18 16:30:53.000000 watex-0.2.5/watex/analysis/decomposition.py
--rw-rw-rw-   0        0        0    25575 2023-02-05 12:23:26.000000 watex-0.2.5/watex/analysis/dimensionality.py
--rw-rw-rw-   0        0        0     9305 2023-02-04 08:20:23.000000 watex-0.2.5/watex/analysis/factor.py
--rw-rw-rw-   0        0        0    85025 2023-03-12 01:49:14.000000 watex-0.2.5/watex/base.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.519790 watex-0.2.5/watex/cases/
--rw-rw-rw-   0        0        0     1078 2023-01-12 16:27:24.000000 watex-0.2.5/watex/cases/__init__.py
--rw-rw-rw-   0        0        0    38684 2023-03-12 01:39:59.000000 watex-0.2.5/watex/cases/features.py
--rw-rw-rw-   0        0        0    31952 2023-03-12 01:40:49.000000 watex-0.2.5/watex/cases/modeling.py
--rw-rw-rw-   0        0        0    39022 2023-03-12 01:40:40.000000 watex-0.2.5/watex/cases/prepare.py
--rw-rw-rw-   0        0        0    49220 2023-03-12 01:41:33.000000 watex-0.2.5/watex/cases/processing.py
--rw-rw-rw-   0        0        0     1353 2023-03-15 12:48:58.000000 watex-0.2.5/watex/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.526982 watex-0.2.5/watex/datasets/
--rw-rw-rw-   0        0        0      911 2023-06-20 13:03:34.000000 watex-0.2.5/watex/datasets/__init__.py
--rw-rw-rw-   0        0        0     7785 2023-03-21 13:31:09.000000 watex-0.2.5/watex/datasets/_config.py
--rw-rw-rw-   0        0        0       29 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/_hongliu.py
--rw-rw-rw-   0        0        0     5677 2023-03-21 13:58:43.000000 watex-0.2.5/watex/datasets/_p.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.568114 watex-0.2.5/watex/datasets/data/
--rw-rw-rw-   0        0        0       27 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/data/__init__.py
--rw-rw-rw-   0        0        0   328758 2023-03-20 17:59:44.000000 watex-0.2.5/watex/datasets/data/b.pkl
--rw-rw-rw-   0        0        0    34993 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/data/bagoue.csv
--rw-rw-rw-   0        0        0    35250 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/data/boston_house_prices.csv
--rw-rw-rw-   0        0        0      638 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/data/boundiali_ves.csv
--rw-rw-rw-   0        0        0     1158 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/data/dcerp_gbalo.csv
--rw-rw-rw-   0        0        0      699 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/data/dcves_gbalo.csv
--rw-rw-rw-   0        0        0  2216584 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/data/e.h5
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.571481 watex-0.2.5/watex/datasets/data/edis/
--rw-rw-rw-   0        0        0        4 2023-02-24 10:23:34.000000 watex-0.2.5/watex/datasets/data/edis/__init__.py
--rw-rw-rw-   0        0        0   170380 2023-02-24 10:23:34.000000 watex-0.2.5/watex/datasets/data/edis/raw.E.zip
--rw-rw-rw-   0        0        0   184986 2023-02-24 10:23:34.000000 watex-0.2.5/watex/datasets/data/edis/s.E.zip
--rw-rw-rw-   0        0        0 11940145 2023-05-05 12:57:48.000000 watex-0.2.5/watex/datasets/data/h.h5
--rw-rw-rw-   0        0        0     2885 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/data/iris.csv
--rw-rw-rw-   0        0        0   731414 2023-05-05 12:57:48.000000 watex-0.2.5/watex/datasets/data/mxs.joblib
--rw-rw-rw-   0        0        0     6955 2023-06-20 12:17:20.000000 watex-0.2.5/watex/datasets/data/nlogs+.csv
--rw-rw-rw-   0        0        0    13993 2023-06-20 12:17:20.000000 watex-0.2.5/watex/datasets/data/nlogs.csv
--rw-rw-rw-   0        0        0      603 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/data/semien_ves.csv
--rw-rw-rw-   0        0        0     2230 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/data/tankesse.csv
--rw-rw-rw-   0        0        0    11336 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/data/wine_data.csv
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.582319 watex-0.2.5/watex/datasets/descr/
--rw-rw-rw-   0        0        0       29 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/descr/__init__.py
--rw-rw-rw-   0        0        0     2827 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/descr/bagoue.rst
--rw-rw-rw-   0        0        0     2397 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/descr/boston_house_prices.rst
--rw-rw-rw-   0        0        0     2844 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/descr/boundiali_ves.rst
--rw-rw-rw-   0        0        0     1822 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/descr/california_housing.rst
--rw-rw-rw-   0        0        0     2844 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/descr/gbalo_erp.rst
--rw-rw-rw-   0        0        0     2844 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/descr/gbalo_ves.rst
--rw-rw-rw-   0        0        0     2845 2023-06-20 12:17:20.000000 watex-0.2.5/watex/datasets/descr/huayuan_edis.rst
--rw-rw-rw-   0        0        0     2844 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/descr/iris.rst
--rw-rw-rw-   0        0        0     3381 2023-06-20 12:17:20.000000 watex-0.2.5/watex/datasets/descr/nanshang+.rst
--rw-rw-rw-   0        0        0     2332 2023-06-20 12:17:20.000000 watex-0.2.5/watex/datasets/descr/nanshang.rst
--rw-rw-rw-   0        0        0     3544 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/descr/wine_data.rst
--rw-rw-rw-   0        0        0    52573 2023-06-20 12:38:30.000000 watex-0.2.5/watex/datasets/dload.py
--rw-rw-rw-   0        0        0    17331 2023-05-05 12:57:48.000000 watex-0.2.5/watex/datasets/gdata.py
--rw-rw-rw-   0        0        0    13639 2023-03-24 15:43:33.000000 watex-0.2.5/watex/datasets/io.py
--rw-rw-rw-   0        0        0    34896 2023-03-12 01:42:57.000000 watex-0.2.5/watex/datasets/rload.py
--rw-rw-rw-   0        0        0     7180 2023-06-20 12:17:20.000000 watex-0.2.5/watex/datasets/sets.py
--rw-rw-rw-   0        0        0      822 2023-01-08 08:20:47.000000 watex-0.2.5/watex/datasets/setup.py
--rw-rw-rw-   0        0        0   101919 2023-06-21 11:42:13.000000 watex-0.2.5/watex/decorators.py
--rw-rw-rw-   0        0        0   115869 2023-03-23 14:01:07.000000 watex-0.2.5/watex/edi.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.592416 watex-0.2.5/watex/etc/
--rw-rw-rw-   0        0        0     5711 2023-01-08 08:20:47.000000 watex-0.2.5/watex/etc/AGSO.csv
--rw-rw-rw-   0        0        0      351 2023-01-08 08:20:47.000000 watex-0.2.5/watex/etc/AGSO_STCODES.csv
--rw-rw-rw-   0        0        0    14650 2023-03-20 14:32:57.000000 watex-0.2.5/watex/etc/__XTyT.pkl
--rw-rw-rw-   0        0        0    37763 2023-03-20 16:12:55.000000 watex-0.2.5/watex/etc/__Xy.pkl
--rw-rw-rw-   0        0        0       29 2023-01-08 08:20:47.000000 watex-0.2.5/watex/etc/__init__.py
--rw-rw-rw-   0        0        0   978190 2023-06-22 04:42:01.000000 watex-0.2.5/watex/etc/__memory.pkl
--rw-rw-rw-   0        0        0    28672 2023-01-08 08:20:47.000000 watex-0.2.5/watex/etc/memory.sq3
--rw-rw-rw-   0        0        0 52244397 2023-01-08 08:20:47.000000 watex-0.2.5/watex/etc/p.models.pkl
--rw-rw-rw-   0        0        0     9763 2023-06-21 11:42:13.000000 watex-0.2.5/watex/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.664181 watex-0.2.5/watex/exlib/
--rw-rw-rw-   0        0        0     4022 2023-03-27 14:03:16.000000 watex-0.2.5/watex/exlib/__init__.py
--rw-rw-rw-   0        0        0     2580 2023-03-15 12:48:58.000000 watex-0.2.5/watex/exlib/gbm.py
--rw-rw-rw-   0        0        0     7156 2023-03-12 01:43:33.000000 watex-0.2.5/watex/exlib/sklearn.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.669201 watex-0.2.5/watex/externals/
--rw-rw-rw-   0        0        0      313 2023-01-18 17:47:22.000000 watex-0.2.5/watex/externals/__init__.py
--rw-rw-rw-   0        0        0     4835 2023-01-08 08:20:47.000000 watex-0.2.5/watex/externals/_numpy_compiler_patch.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.671147 watex-0.2.5/watex/externals/_pkgs/
--rw-rw-rw-   0        0        0       29 2023-01-08 08:20:47.000000 watex-0.2.5/watex/externals/_pkgs/__init__.py
--rw-rw-rw-   0        0        0     3035 2023-01-08 08:20:47.000000 watex-0.2.5/watex/externals/_pkgs/_structures.py
--rw-rw-rw-   0        0        0    16762 2023-01-08 08:20:47.000000 watex-0.2.5/watex/externals/_pkgs/version.py
--rw-rw-rw-   0        0        0      273 2023-01-08 08:20:47.000000 watex-0.2.5/watex/externals/readme.md
--rw-rw-rw-   0        0        0    57854 2023-03-23 14:01:07.000000 watex-0.2.5/watex/externals/z.py
--rw-rw-rw-   0        0        0    24161 2023-03-12 01:43:53.000000 watex-0.2.5/watex/externals/zutils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.677223 watex-0.2.5/watex/geology/
--rw-rw-rw-   0        0        0     1067 2023-06-17 08:36:57.000000 watex-0.2.5/watex/geology/__init__.py
--rw-rw-rw-   0        0        0    12712 2023-06-22 04:42:01.000000 watex-0.2.5/watex/geology/core.py
--rw-rw-rw-   0        0        0    56354 2023-03-12 01:44:15.000000 watex-0.2.5/watex/geology/database.py
--rw-rw-rw-   0        0        0   130836 2023-06-22 07:24:02.000000 watex-0.2.5/watex/geology/drilling.py
--rw-rw-rw-   0        0        0    14488 2023-05-24 12:02:39.000000 watex-0.2.5/watex/geology/geology.py
--rw-rw-rw-   0        0        0    73452 2023-06-22 04:42:01.000000 watex-0.2.5/watex/geology/stratigraphic.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.684363 watex-0.2.5/watex/methods/
--rw-rw-rw-   0        0        0      867 2023-04-15 15:25:13.000000 watex-0.2.5/watex/methods/__init__.py
--rw-rw-rw-   0        0        0    82817 2023-04-22 06:56:19.000000 watex-0.2.5/watex/methods/electrical.py
--rw-rw-rw-   0        0        0   136679 2023-05-14 09:33:31.000000 watex-0.2.5/watex/methods/em.py
--rw-rw-rw-   0        0        0    86661 2023-04-22 06:56:19.000000 watex-0.2.5/watex/methods/erp.py
--rw-rw-rw-   0        0        0    43855 2023-03-12 01:45:26.000000 watex-0.2.5/watex/methods/hydro.py
--rw-rw-rw-   0        0        0    28992 2023-05-24 12:02:39.000000 watex-0.2.5/watex/metrics.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.687308 watex-0.2.5/watex/models/
--rw-rw-rw-   0        0        0     1064 2023-03-24 12:58:06.000000 watex-0.2.5/watex/models/__init__.py
--rw-rw-rw-   0        0        0     6889 2023-03-15 12:48:58.000000 watex-0.2.5/watex/models/_metapredictors.py
--rw-rw-rw-   0        0        0    18878 2023-03-15 12:48:58.000000 watex-0.2.5/watex/models/premodels.py
--rw-rw-rw-   0        0        0    44482 2023-03-28 11:58:09.000000 watex-0.2.5/watex/models/validation.py
--rw-rw-rw-   0        0        0    73934 2023-06-22 04:42:01.000000 watex-0.2.5/watex/property.py
--rw-rw-rw-   0        0        0    51498 2023-06-22 07:29:40.000000 watex-0.2.5/watex/site.py
--rw-rw-rw-   0        0        0    61886 2023-06-17 08:36:57.000000 watex-0.2.5/watex/transformers.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.710803 watex-0.2.5/watex/utils/
--rw-rw-rw-   0        0        0     6196 2023-06-21 11:42:13.000000 watex-0.2.5/watex/utils/__init__.py
--rw-rw-rw-   0        0        0     7140 2023-01-08 08:20:47.000000 watex-0.2.5/watex/utils/_array_api.py
--rw-rw-rw-   0        0        0     7730 2023-01-08 08:20:47.000000 watex-0.2.5/watex/utils/_arraytools.py
--rw-rw-rw-   0        0        0     5936 2023-02-01 06:46:13.000000 watex-0.2.5/watex/utils/_dependency.py
--rw-rw-rw-   0        0        0      222 2023-01-08 08:20:47.000000 watex-0.2.5/watex/utils/_openmp_helpers.pxd
--rw-rw-rw-   0        0        0     2674 2023-01-08 08:20:47.000000 watex-0.2.5/watex/utils/_openmp_helpers.pyx
--rw-rw-rw-   0        0        0    16659 2023-01-28 02:10:06.000000 watex-0.2.5/watex/utils/_packaging_version.py
--rw-rw-rw-   0        0        0     1616 2023-03-28 11:58:09.000000 watex-0.2.5/watex/utils/_set_gdal.py
--rw-rw-rw-   0        0        0     2583 2023-02-16 08:00:08.000000 watex-0.2.5/watex/utils/_show_versions.py
--rw-rw-rw-   0        0        0    13908 2023-05-26 13:32:06.000000 watex-0.2.5/watex/utils/box.py
--rw-rw-rw-   0        0        0    98080 2023-06-18 14:15:21.000000 watex-0.2.5/watex/utils/coreutils.py
--rw-rw-rw-   0        0        0   580618 2023-01-08 08:20:47.000000 watex-0.2.5/watex/utils/epsg.npy
--rw-rw-rw-   0        0        0   232345 2023-06-22 07:30:24.000000 watex-0.2.5/watex/utils/exmath.py
--rw-rw-rw-   0        0        0   252184 2023-06-21 11:42:13.000000 watex-0.2.5/watex/utils/funcutils.py
--rw-rw-rw-   0        0        0    82957 2023-06-22 07:00:16.000000 watex-0.2.5/watex/utils/geotools.py
--rw-rw-rw-   0        0        0    58698 2023-03-28 11:58:09.000000 watex-0.2.5/watex/utils/gistools.py
--rw-rw-rw-   0        0        0   139514 2023-06-22 04:42:01.000000 watex-0.2.5/watex/utils/hydroutils.py
--rw-rw-rw-   0        0        0   122844 2023-05-24 12:02:39.000000 watex-0.2.5/watex/utils/mlutils.py
--rw-rw-rw-   0        0        0   139113 2023-06-22 05:05:15.000000 watex-0.2.5/watex/utils/plotutils.py
--rw-rw-rw-   0        0        0      974 2023-01-08 08:20:47.000000 watex-0.2.5/watex/utils/setup.py
--rw-rw-rw-   0        0        0     3548 2023-01-08 08:20:47.000000 watex-0.2.5/watex/utils/thread.py
--rw-rw-rw-   0        0        0    86096 2023-06-17 08:36:57.000000 watex-0.2.5/watex/utils/validator.py
--rw-rw-rw-   0        0        0    16835 2023-01-28 01:30:49.000000 watex-0.2.5/watex/utils/version.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.714229 watex-0.2.5/watex/view/
--rw-rw-rw-   0        0        0     1008 2023-02-24 10:23:34.000000 watex-0.2.5/watex/view/__init__.py
--rw-rw-rw-   0        0        0   145840 2023-05-14 06:19:47.000000 watex-0.2.5/watex/view/mlplot.py
--rw-rw-rw-   0        0        0   190822 2023-04-22 06:56:19.000000 watex-0.2.5/watex/view/plot.py
--rw-rw-rw-   0        0        0     1222 2023-03-11 03:28:02.000000 watex-0.2.5/watex/wlog.yml
-drwxrwxrwx   0        0        0        0 2023-06-22 07:45:30.512398 watex-0.2.5/watex.egg-info/
--rw-rw-rw-   0        0        0    15816 2023-06-22 07:45:29.000000 watex-0.2.5/watex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9678 2023-06-22 07:45:30.000000 watex-0.2.5/watex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 07:45:29.000000 watex-0.2.5/watex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-06-22 07:45:29.000000 watex-0.2.5/watex.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      366 2023-06-22 07:45:29.000000 watex-0.2.5/watex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-22 07:45:29.000000 watex-0.2.5/watex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-22 07:44:19.000000 watex-0.2.5/watex.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:49.023674 watex-0.2.6/
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:46.808689 watex-0.2.6/.github/
+-rw-rw-rw-   0        0        0      524 2023-02-19 15:19:16.000000 watex-0.2.6/.github/dependabot.yml
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:46.840513 watex-0.2.6/.github/workflows/
+-rw-rw-rw-   0        0        0     1616 2023-02-21 12:32:38.000000 watex-0.2.6/.github/workflows/ci.yaml
+-rw-rw-rw-   0        0        0     3025 2023-02-19 15:19:16.000000 watex-0.2.6/.github/workflows/codeql.yml
+-rw-rw-rw-   0        0        0      905 2023-02-19 15:19:16.000000 watex-0.2.6/.github/workflows/dependency-review.yml
+-rw-rw-rw-   0        0        0     1457 2023-03-02 12:14:24.000000 watex-0.2.6/.github/workflows/python-package.yml
+-rw-rw-rw-   0        0        0     3118 2023-05-07 17:25:43.000000 watex-0.2.6/.gitignore
+-rw-rw-rw-   0        0        0      553 2023-03-17 13:03:23.000000 watex-0.2.6/CITATION.cff
+-rw-rw-rw-   0        0        0     1548 2023-01-08 08:20:47.000000 watex-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     1045 2023-05-14 08:24:24.000000 watex-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    15816 2023-06-23 03:30:49.023674 watex-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    14379 2023-05-24 12:02:39.000000 watex-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.021960 watex-0.2.6/docs/
+-rw-rw-rw-   0        0        0      139 2023-02-18 10:33:13.000000 watex-0.2.6/docs/.gitignore
+-rw-rw-rw-   0        0        0      658 2023-01-08 08:20:47.000000 watex-0.2.6/docs/Makefile
+-rw-rw-rw-   0        0        0      251 2023-03-20 12:42:04.000000 watex-0.2.6/docs/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.168037 watex-0.2.6/docs/_static/
+-rw-rw-rw-   0        0        0     2711 2023-01-08 08:52:36.000000 watex-0.2.6/docs/_static/copybutton.js
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.195647 watex-0.2.6/docs/_static/css/
+-rw-rw-rw-   0        0        0   155712 2023-01-28 12:21:35.000000 watex-0.2.6/docs/_static/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0     7607 2023-05-13 16:07:36.000000 watex-0.2.6/docs/_static/css/custom.css
+-rw-rw-rw-   0        0        0    70782 2023-02-01 10:38:29.000000 watex-0.2.6/docs/_static/favicon.ico
+-rw-rw-rw-   0        0        0     1150 2023-01-30 16:08:53.000000 watex-0.2.6/docs/_static/favicon0.ico
+-rw-rw-rw-   0        0        0     8356 2023-01-08 08:52:36.000000 watex-0.2.6/docs/_static/favicon_old.ico
+-rw-rw-rw-   0        0        0     3519 2023-01-30 11:43:04.000000 watex-0.2.6/docs/_static/index_api.svg
+-rw-rw-rw-   0        0        0     2528 2023-01-30 11:43:05.000000 watex-0.2.6/docs/_static/index_contribute.svg
+-rw-rw-rw-   0        0        0     3977 2023-01-30 11:43:04.000000 watex-0.2.6/docs/_static/index_getting_started.svg
+-rw-rw-rw-   0        0        0     6429 2023-01-30 11:43:05.000000 watex-0.2.6/docs/_static/index_user_guide.svg
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:46.769682 watex-0.2.6/docs/_static/js/
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.298803 watex-0.2.6/docs/_static/js/vendor/
+-rw-rw-rw-   0        0        0    58030 2023-01-28 12:21:35.000000 watex-0.2.6/docs/_static/js/vendor/bootstrap.min.js
+-rw-rw-rw-   0        0        0    72818 2023-01-28 12:21:35.000000 watex-0.2.6/docs/_static/js/vendor/jquery-3.6.3.slim.min.js
+-rw-rw-rw-   0        0        0     1738 2023-02-02 06:30:47.000000 watex-0.2.6/docs/_static/logo.svg
+-rw-rw-rw-   0        0        0     2346 2023-01-08 08:52:36.000000 watex-0.2.6/docs/_static/logo_no_name.svg
+-rw-rw-rw-   0        0        0     1916 2023-01-28 05:52:08.000000 watex-0.2.6/docs/_static/logo_small.svg
+-rw-rw-rw-   0        0        0     2631 2023-01-08 08:52:36.000000 watex-0.2.6/docs/_static/logo_wide.svg
+-rw-rw-rw-   0        0        0     1916 2023-01-28 05:52:08.000000 watex-0.2.6/docs/_static/logo_wide_rev.svg
+-rw-rw-rw-   0        0        0     3052 2023-01-08 08:52:36.000000 watex-0.2.6/docs/_static/logo_wide_rev0.svg
+-rw-rw-rw-   0        0        0     1244 2023-06-23 02:07:49.000000 watex-0.2.6/docs/_static/switcher.json
+-rw-rw-rw-   0        0        0      166 2023-01-28 15:18:48.000000 watex-0.2.6/docs/_static/theme.conf
+-rw-rw-rw-   0        0        0     1464 2023-01-30 16:00:33.000000 watex-0.2.6/docs/_static/to_favicon.svg
+-rw-rw-rw-   0        0        0   125058 2023-01-30 14:23:50.000000 watex-0.2.6/docs/_static/watex_thumb_image.svg
+-rw-rw-rw-   0        0        0    26516 2023-01-30 05:05:07.000000 watex-0.2.6/docs/_static/watex_workflow.svg
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.343753 watex-0.2.6/docs/_templates/
+-rw-rw-rw-   0        0        0     5128 2023-01-28 12:21:35.000000 watex-0.2.6/docs/_templates/javascript.html
+-rw-rw-rw-   0        0        0      867 2023-05-25 11:10:55.000000 watex-0.2.6/docs/_templates/layout.html
+-rw-rw-rw-   0        0        0       87 2023-01-09 10:30:31.000000 watex-0.2.6/docs/_templates/version.html
+-rw-rw-rw-   0        0        0    16686 2023-02-01 15:09:39.000000 watex-0.2.6/docs/analysis.rst
+-rw-rw-rw-   0        0        0    23500 2023-06-21 11:42:13.000000 watex-0.2.6/docs/api_references.rst
+-rw-rw-rw-   0        0        0    15873 2023-04-14 23:54:09.000000 watex-0.2.6/docs/base.rst
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.347656 watex-0.2.6/docs/binder/
+-rw-rw-rw-   0        0        0      258 2023-01-08 08:52:36.000000 watex-0.2.6/docs/binder/requirements.txt
+-rw-rw-rw-   0        0        0    11688 2023-01-30 11:20:05.000000 watex-0.2.6/docs/cases.rst
+-rw-rw-rw-   0        0        0     2772 2023-03-17 13:03:23.000000 watex-0.2.6/docs/citing.rst
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.357393 watex-0.2.6/docs/community/
+-rw-rw-rw-   0        0        0     2322 2023-02-19 15:58:54.000000 watex-0.2.6/docs/community/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    16384 2023-03-25 08:21:17.000000 watex-0.2.6/docs/conf.py
+-rw-rw-rw-   0        0        0    18198 2023-02-01 09:06:05.000000 watex-0.2.6/docs/datasets.rst
+-rw-rw-rw-   0        0        0    16155 2023-02-05 16:03:43.000000 watex-0.2.6/docs/development.rst
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.359338 watex-0.2.6/docs/example_thumbs/
+-rw-rw-rw-   0        0        0        0 2023-01-08 08:52:36.000000 watex-0.2.6/docs/example_thumbs/.gitkeep
+-rw-rw-rw-   0        0        0    69141 2023-01-30 05:05:07.000000 watex-0.2.6/docs/example_thumbs/watex_workflow.gif
+-rw-rw-rw-   0        0        0   100537 2023-03-12 07:09:50.000000 watex-0.2.6/docs/glossary.rst
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.387095 watex-0.2.6/docs/history/
+-rw-rw-rw-   0        0        0     5834 2023-02-18 16:26:08.000000 watex-0.2.6/docs/history/five_min_understanding.rst
+-rw-rw-rw-   0        0        0      385 2023-02-18 15:40:51.000000 watex-0.2.6/docs/history/index.rst
+-rw-rw-rw-   0        0        0     5454 2023-02-21 12:32:38.000000 watex-0.2.6/docs/history/project_goals.rst
+-rw-rw-rw-   0        0        0     9463 2023-02-20 11:39:27.000000 watex-0.2.6/docs/history/project_story.rst
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.398439 watex-0.2.6/docs/includes/
+-rw-rw-rw-   0        0        0      762 2023-01-10 10:17:54.000000 watex-0.2.6/docs/includes/big_toc_css.rst
+-rw-rw-rw-   0        0        0     1087 2023-01-10 10:19:34.000000 watex-0.2.6/docs/includes/bigger_toc_css.rst
+-rw-rw-rw-   0        0        0     1918 2023-02-19 16:15:09.000000 watex-0.2.6/docs/index.rst
+-rw-rw-rw-   0        0        0    12622 2023-03-19 07:20:06.000000 watex-0.2.6/docs/installation.rst
+-rwxrwxrwx   0        0        0      804 2023-01-08 08:20:47.000000 watex-0.2.6/docs/make.bat
+-rw-rw-rw-   0        0        0       20 2023-01-08 08:52:36.000000 watex-0.2.6/docs/matplotlibrc.txt
+-rw-rw-rw-   0        0        0    46356 2023-02-18 06:46:56.000000 watex-0.2.6/docs/methods.rst
+-rw-rw-rw-   0        0        0      548 2023-03-24 16:49:23.000000 watex-0.2.6/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.422879 watex-0.2.6/docs/source/
+-rw-rw-rw-   0        0        0    20241 2023-01-10 14:10:18.000000 watex-0.2.6/docs/source/index.html
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.463541 watex-0.2.6/docs/sphinxext/
+-rw-rw-rw-   0        0        0       43 2023-01-12 12:03:56.000000 watex-0.2.6/docs/sphinxext/MANIFEST.in
+-rw-rw-rw-   0        0        0     6182 2023-01-12 11:57:22.000000 watex-0.2.6/docs/sphinxext/add_toctree_functions.py
+-rw-rw-rw-   0        0        0     1784 2023-01-12 12:03:00.000000 watex-0.2.6/docs/sphinxext/doi_role.py
+-rw-rw-rw-   0        0        0     8329 2023-01-12 12:01:15.000000 watex-0.2.6/docs/sphinxext/sphinx_issues.py
+-rw-rw-rw-   0        0        0    16329 2023-02-05 13:07:26.000000 watex-0.2.6/docs/structure.rst
+-rw-rw-rw-   0        0        0     3807 2023-01-10 10:22:10.000000 watex-0.2.6/docs/tune_toc.rst
+-rw-rw-rw-   0        0        0      391 2023-02-02 12:44:21.000000 watex-0.2.6/docs/user_guide.rst
+-rw-rw-rw-   0        0        0    42796 2023-01-30 09:59:53.000000 watex-0.2.6/docs/utils.rst
+-rw-rw-rw-   0        0        0    76837 2023-02-10 02:52:23.000000 watex-0.2.6/docs/view.rst
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.603352 watex-0.2.6/docs/whatsnew/
+-rw-rw-rw-   0        0        0      571 2023-06-23 01:06:41.000000 watex-0.2.6/docs/whatsnew/index.rst
+-rw-rw-rw-   0        0        0     1737 2023-03-19 09:38:32.000000 watex-0.2.6/docs/whatsnew/v0.1.0.rst
+-rw-rw-rw-   0        0        0     2801 2023-03-19 09:37:06.000000 watex-0.2.6/docs/whatsnew/v0.1.1.rst
+-rw-rw-rw-   0        0        0     2202 2023-03-19 09:44:19.000000 watex-0.2.6/docs/whatsnew/v0.1.2.rst
+-rw-rw-rw-   0        0        0     2120 2023-03-19 09:42:28.000000 watex-0.2.6/docs/whatsnew/v0.1.3.rst
+-rw-rw-rw-   0        0        0     3469 2023-03-19 09:27:50.000000 watex-0.2.6/docs/whatsnew/v0.1.4.rst
+-rw-rw-rw-   0        0        0     4092 2023-03-19 10:54:01.000000 watex-0.2.6/docs/whatsnew/v0.1.5.rst
+-rw-rw-rw-   0        0        0    21723 2023-03-07 14:39:00.000000 watex-0.2.6/docs/whatsnew/v0.1.6-alpha.rst
+-rw-rw-rw-   0        0        0     5019 2023-03-19 09:20:02.000000 watex-0.2.6/docs/whatsnew/v0.1.6.rst
+-rw-rw-rw-   0        0        0     1457 2023-03-19 10:17:51.000000 watex-0.2.6/docs/whatsnew/v0.1.7.rst
+-rw-rw-rw-   0        0        0     2108 2023-03-20 12:42:04.000000 watex-0.2.6/docs/whatsnew/v0.1.8.rst
+-rw-rw-rw-   0        0        0     2042 2023-04-14 23:54:09.000000 watex-0.2.6/docs/whatsnew/v0.1.9.rst
+-rw-rw-rw-   0        0        0     5730 2023-04-20 04:00:41.000000 watex-0.2.6/docs/whatsnew/v0.2.0.rst
+-rw-rw-rw-   0        0        0     4070 2023-04-22 11:36:08.000000 watex-0.2.6/docs/whatsnew/v0.2.1.rst
+-rw-rw-rw-   0        0        0     1093 2023-04-22 07:50:27.000000 watex-0.2.6/docs/whatsnew/v0.2.2.rst
+-rw-rw-rw-   0        0        0     2011 2023-05-25 12:52:32.000000 watex-0.2.6/docs/whatsnew/v0.2.3.rst
+-rw-rw-rw-   0        0        0     4124 2023-05-27 00:28:54.000000 watex-0.2.6/docs/whatsnew/v0.2.4.rst
+-rw-rw-rw-   0        0        0     3337 2023-06-22 04:55:18.000000 watex-0.2.6/docs/whatsnew/v0.2.5.rst
+-rw-rw-rw-   0        0        0     1319 2023-06-23 02:16:28.000000 watex-0.2.6/docs/whatsnew/v0.2.6.rst
+-rw-rw-rw-   0        0        0    18951 2023-06-22 21:09:44.000000 watex-0.2.6/etc
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.610167 watex-0.2.6/examples/
+-rw-rw-rw-   0        0        0      427 2023-01-11 10:44:04.000000 watex-0.2.6/examples/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.642583 watex-0.2.6/examples/analysis/
+-rw-rw-rw-   0        0        0      109 2023-01-18 16:53:37.000000 watex-0.2.6/examples/analysis/README.txt
+-rw-rw-rw-   0        0        0     1031 2023-01-11 15:25:23.000000 watex-0.2.6/examples/analysis/plot_decision_regions.py
+-rw-rw-rw-   0        0        0     1171 2023-01-11 15:25:54.000000 watex-0.2.6/examples/analysis/plot_explained_variance_ratio.py
+-rw-rw-rw-   0        0        0      875 2023-01-11 15:26:26.000000 watex-0.2.6/examples/analysis/plot_linear_discriminant_analysis.py
+-rw-rw-rw-   0        0        0      541 2023-01-11 15:26:56.000000 watex-0.2.6/examples/analysis/plot_pca_vs_factor_with_scedatic_noises.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.709679 watex-0.2.6/examples/applications/
+-rw-rw-rw-   0        0        0      510 2023-01-18 17:34:21.000000 watex-0.2.6/examples/applications/README.txt
+-rw-rw-rw-   0        0        0     3329 2023-03-05 22:27:58.000000 watex-0.2.6/examples/applications/plot_auto_detect_drilling_location.py
+-rw-rw-rw-   0        0        0     8710 2023-01-11 16:26:30.000000 watex-0.2.6/examples/applications/plot_data_exploratory_quick_view.py
+-rw-rw-rw-   0        0        0    10236 2023-02-15 12:36:42.000000 watex-0.2.6/examples/applications/plot_dc_em_parameters_computings.py
+-rw-rw-rw-   0        0        0     8084 2023-01-20 17:43:45.000000 watex-0.2.6/examples/applications/plot_flow_rate_prediction.py
+-rw-rw-rw-   0        0        0    10004 2023-06-17 08:36:57.000000 watex-0.2.6/examples/applications/plot_kmf.py
+-rw-rw-rw-   0        0        0     3325 2023-02-16 17:12:25.000000 watex-0.2.6/examples/applications/plot_nsamt_tensor_recovery.py
+-rw-rw-rw-   0        0        0     5719 2023-03-17 13:03:23.000000 watex-0.2.6/examples/applications/plot_tensor_restoring.py
+-rw-rw-rw-   0        0        0    11379 2023-05-25 12:48:47.000000 watex-0.2.6/examples/applications/plot_ymxs_label_for_k_prediction.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.710572 watex-0.2.6/examples/auto_examples/
+-rw-rw-rw-   0        0        0        0 2023-01-25 09:04:31.000000 watex-0.2.6/examples/auto_examples/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.739825 watex-0.2.6/examples/base/
+-rw-rw-rw-   0        0        0      141 2023-01-18 16:52:30.000000 watex-0.2.6/examples/base/README.txt
+-rw-rw-rw-   0        0        0     1002 2023-01-11 15:30:46.000000 watex-0.2.6/examples/base/plot_ada_gd.py
+-rw-rw-rw-   0        0        0     1032 2023-01-11 15:31:27.000000 watex-0.2.6/examples/base/plot_ada_stochastic_gd.py
+-rw-rw-rw-   0        0        0      902 2023-01-11 15:31:50.000000 watex-0.2.6/examples/base/plot_missing.py
+-rw-rw-rw-   0        0        0     1392 2023-01-11 15:32:51.000000 watex-0.2.6/examples/base/plot_sbs_feature_selector.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.804445 watex-0.2.6/examples/methods/
+-rw-rw-rw-   0        0        0      106 2023-01-08 08:52:36.000000 watex-0.2.6/examples/methods/README.txt
+-rw-rw-rw-   0        0        0      874 2023-01-20 17:25:23.000000 watex-0.2.6/examples/methods/plot_2d_tensor_filtered.py
+-rw-rw-rw-   0        0        0     1071 2023-01-11 15:40:37.000000 watex-0.2.6/examples/methods/plot_anomaly.py
+-rw-rw-rw-   0        0        0     1852 2023-01-11 15:41:46.000000 watex-0.2.6/examples/methods/plot_filtered_tensors.py
+-rw-rw-rw-   0        0        0     1007 2023-01-11 15:43:30.000000 watex-0.2.6/examples/methods/plot_logging_predictor_and_target.py
+-rw-rw-rw-   0        0        0      884 2023-01-11 15:44:27.000000 watex-0.2.6/examples/methods/plot_logging_predictor_only.py
+-rw-rw-rw-   0        0        0      638 2023-01-11 15:44:36.000000 watex-0.2.6/examples/methods/plot_multiple_sites_recovery_signal.py
+-rw-rw-rw-   0        0        0     2423 2023-03-02 12:26:23.000000 watex-0.2.6/examples/methods/plot_phase_tensors.py
+-rw-rw-rw-   0        0        0      806 2023-01-11 15:44:59.000000 watex-0.2.6/examples/methods/plot_raw_2d_tensor.py
+-rw-rw-rw-   0        0        0      915 2023-01-11 15:45:48.000000 watex-0.2.6/examples/methods/plot_ves_fracture_zone.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:47.962659 watex-0.2.6/examples/utils/
+-rw-rw-rw-   0        0        0      125 2023-01-08 08:52:36.000000 watex-0.2.6/examples/utils/README.txt
+-rw-rw-rw-   0        0        0      788 2023-01-09 07:43:08.000000 watex-0.2.6/examples/utils/plot_clusters.py
+-rw-rw-rw-   0        0        0     2373 2023-03-06 16:32:37.000000 watex-0.2.6/examples/utils/plot_confidence_in_data.py
+-rw-rw-rw-   0        0        0     1489 2023-01-11 15:46:32.000000 watex-0.2.6/examples/utils/plot_confusion_matrices.py
+-rw-rw-rw-   0        0        0     1124 2023-01-09 07:43:29.000000 watex-0.2.6/examples/utils/plot_confusion_matrix_sweet.py
+-rw-rw-rw-   0        0        0      526 2023-01-11 15:46:56.000000 watex-0.2.6/examples/utils/plot_elbow.py
+-rw-rw-rw-   0        0        0     1758 2023-01-25 03:02:32.000000 watex-0.2.6/examples/utils/plot_erp.py
+-rw-rw-rw-   0        0        0      655 2023-01-11 15:48:44.000000 watex-0.2.6/examples/utils/plot_errors_vs_epochs.py
+-rw-rw-rw-   0        0        0      631 2023-01-11 15:49:01.000000 watex-0.2.6/examples/utils/plot_ex_heatmap.py
+-rw-rw-rw-   0        0        0      717 2023-01-11 15:50:15.000000 watex-0.2.6/examples/utils/plot_ex_matrix.py
+-rw-rw-rw-   0        0        0     1094 2023-01-11 15:50:34.000000 watex-0.2.6/examples/utils/plot_learning_curves.py
+-rw-rw-rw-   0        0        0     1787 2023-01-11 15:51:32.000000 watex-0.2.6/examples/utils/plot_log.py
+-rw-rw-rw-   0        0        0     1053 2023-01-09 07:44:13.000000 watex-0.2.6/examples/utils/plot_model_confusion_matrix.py
+-rw-rw-rw-   0        0        0      751 2023-01-11 15:53:36.000000 watex-0.2.6/examples/utils/plot_naive_dendrogram.py
+-rw-rw-rw-   0        0        0      716 2023-01-11 15:53:51.000000 watex-0.2.6/examples/utils/plot_naive_silhouette.py
+-rw-rw-rw-   0        0        0      678 2023-01-11 15:54:53.000000 watex-0.2.6/examples/utils/plot_ohmic_area.py
+-rw-rw-rw-   0        0        0      814 2023-01-08 08:52:36.000000 watex-0.2.6/examples/utils/plot_pca_components.py
+-rw-rw-rw-   0        0        0      611 2023-01-11 15:55:25.000000 watex-0.2.6/examples/utils/plot_regularization_path.py
+-rw-rw-rw-   0        0        0      623 2023-01-11 15:55:45.000000 watex-0.2.6/examples/utils/plot_rf_feature_importances.py
+-rw-rw-rw-   0        0        0      966 2023-01-24 10:29:45.000000 watex-0.2.6/examples/utils/plot_savitzky_golay1d.py
+-rw-rw-rw-   0        0        0     1132 2023-01-08 08:52:36.000000 watex-0.2.6/examples/utils/plot_sbs_feature_selection.py
+-rw-rw-rw-   0        0        0     1793 2023-01-25 04:57:49.000000 watex-0.2.6/examples/utils/plot_sfi.py
+-rw-rw-rw-   0        0        0     3121 2023-03-04 11:47:12.000000 watex-0.2.6/examples/utils/plot_skew.py
+-rw-rw-rw-   0        0        0      618 2023-06-21 11:42:13.000000 watex-0.2.6/examples/utils/plot_stratalog.py
+-rw-rw-rw-   0        0        0     2236 2023-03-19 08:17:21.000000 watex-0.2.6/examples/utils/plot_strike.py
+-rw-rw-rw-   0        0        0      693 2023-05-14 06:02:07.000000 watex-0.2.6/examples/utils/plot_voronoi.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.248057 watex-0.2.6/examples/view/
+-rw-rw-rw-   0        0        0      113 2023-01-18 16:54:11.000000 watex-0.2.6/examples/view/README.txt
+-rw-rw-rw-   0        0        0      915 2023-01-24 02:59:52.000000 watex-0.2.6/examples/view/plot_2d_filtered_tensors.py
+-rw-rw-rw-   0        0        0      933 2023-01-11 15:58:16.000000 watex-0.2.6/examples/view/plot_base_distributions.py
+-rw-rw-rw-   0        0        0     1101 2023-01-16 18:53:31.000000 watex-0.2.6/examples/view/plot_biplot.py
+-rw-rw-rw-   0        0        0      553 2023-01-11 15:59:22.000000 watex-0.2.6/examples/view/plot_box.py
+-rw-rw-rw-   0        0        0     1678 2023-01-11 16:00:02.000000 watex-0.2.6/examples/view/plot_confusion_matrix_metric.py
+-rw-rw-rw-   0        0        0      852 2023-01-08 08:52:36.000000 watex-0.2.6/examples/view/plot_correlating_features.py
+-rw-rw-rw-   0        0        0      449 2023-01-11 16:01:24.000000 watex-0.2.6/examples/view/plot_correlation_missing_data.py
+-rw-rw-rw-   0        0        0      599 2023-01-11 16:00:47.000000 watex-0.2.6/examples/view/plot_cut_comparison.py
+-rw-rw-rw-   0        0        0      453 2023-01-11 16:01:48.000000 watex-0.2.6/examples/view/plot_dendro_missing_data.py
+-rw-rw-rw-   0        0        0      921 2023-01-16 17:55:57.000000 watex-0.2.6/examples/view/plot_dendrogram.py
+-rw-rw-rw-   0        0        0      854 2023-01-16 17:19:14.000000 watex-0.2.6/examples/view/plot_dendroheat.py
+-rw-rw-rw-   0        0        0      920 2023-01-11 16:05:35.000000 watex-0.2.6/examples/view/plot_discussing_features.py
+-rw-rw-rw-   0        0        0      697 2023-01-11 16:06:18.000000 watex-0.2.6/examples/view/plot_grid.py
+-rw-rw-rw-   0        0        0      676 2023-01-11 16:06:48.000000 watex-0.2.6/examples/view/plot_hist.py
+-rw-rw-rw-   0        0        0      888 2023-01-08 08:52:36.000000 watex-0.2.6/examples/view/plot_jointing_features.py
+-rw-rw-rw-   0        0        0      644 2023-01-11 16:07:06.000000 watex-0.2.6/examples/view/plot_learning_inspections.py
+-rw-rw-rw-   0        0        0     1365 2023-01-11 16:08:38.000000 watex-0.2.6/examples/view/plot_matshow.py
+-rw-rw-rw-   0        0        0     2370 2023-01-11 16:10:01.000000 watex-0.2.6/examples/view/plot_model.py
+-rw-rw-rw-   0        0        0      588 2023-01-11 16:10:11.000000 watex-0.2.6/examples/view/plot_model_inspection.py
+-rw-rw-rw-   0        0        0     1964 2023-01-18 15:28:17.000000 watex-0.2.6/examples/view/plot_model_scores.py
+-rw-rw-rw-   0        0        0      725 2023-01-09 07:52:42.000000 watex-0.2.6/examples/view/plot_multiple_feature_distributions.py
+-rw-rw-rw-   0        0        0     1226 2023-01-09 07:52:51.000000 watex-0.2.6/examples/view/plot_num_features.py
+-rw-rw-rw-   0        0        0     1241 2023-01-11 16:11:17.000000 watex-0.2.6/examples/view/plot_pairwise_corr.py
+-rw-rw-rw-   0        0        0      524 2023-01-11 16:11:59.000000 watex-0.2.6/examples/view/plot_pararell_corrdinates.py
+-rw-rw-rw-   0        0        0     1372 2023-01-11 16:12:35.000000 watex-0.2.6/examples/view/plot_pca.py
+-rw-rw-rw-   0        0        0     5274 2023-03-04 05:56:10.000000 watex-0.2.6/examples/view/plot_phase_sensistive_skew.py
+-rw-rw-rw-   0        0        0      818 2023-01-20 17:26:34.000000 watex-0.2.6/examples/view/plot_phase_tensor_2d.py
+-rw-rw-rw-   0        0        0      817 2023-01-11 16:12:58.000000 watex-0.2.6/examples/view/plot_pr.py
+-rw-rw-rw-   0        0        0     1893 2023-01-16 18:57:53.000000 watex-0.2.6/examples/view/plot_projection.py
+-rw-rw-rw-   0        0        0      883 2023-01-11 16:18:27.000000 watex-0.2.6/examples/view/plot_radviz.py
+-rw-rw-rw-   0        0        0      929 2023-01-11 16:19:02.000000 watex-0.2.6/examples/view/plot_reg_scoring.py
+-rw-rw-rw-   0        0        0      869 2023-01-11 16:19:28.000000 watex-0.2.6/examples/view/plot_res_tensor_2d.py
+-rw-rw-rw-   0        0        0     1939 2023-04-20 03:25:59.000000 watex-0.2.6/examples/view/plot_rhoa.py
+-rw-rw-rw-   0        0        0     1757 2023-01-11 16:19:47.000000 watex-0.2.6/examples/view/plot_roc.py
+-rw-rw-rw-   0        0        0      794 2023-01-11 16:20:19.000000 watex-0.2.6/examples/view/plot_scatter.py
+-rw-rw-rw-   0        0        0     1523 2023-01-11 16:20:37.000000 watex-0.2.6/examples/view/plot_scattering_features.py
+-rw-rw-rw-   0        0        0      543 2023-01-08 08:52:36.000000 watex-0.2.6/examples/view/plot_silhouette.py
+-rw-rw-rw-   0        0        0      759 2023-01-09 07:56:02.000000 watex-0.2.6/examples/view/plot_single_site_signal_recovery.py
+-rw-rw-rw-   0        0        0      834 2023-01-11 16:21:15.000000 watex-0.2.6/examples/view/plot_target_inspection.py
+-rw-rw-rw-   0        0        0     1615 2023-06-23 02:52:44.000000 watex-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0      901 2023-06-23 03:30:49.029728 watex-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     4646 2023-06-23 02:53:38.000000 watex-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.337363 watex-0.2.6/watex/
+-rw-rw-rw-   0        0        0     8552 2023-06-23 02:53:18.000000 watex-0.2.6/watex/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.391889 watex-0.2.6/watex/_build/
+-rw-rw-rw-   0        0        0       27 2023-03-11 03:28:02.000000 watex-0.2.6/watex/_build/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-01-08 08:20:47.000000 watex-0.2.6/watex/_build/_check_build.pyx
+-rw-rw-rw-   0        0        0      333 2023-01-08 08:20:47.000000 watex-0.2.6/watex/_distributor_init.py
+-rw-rw-rw-   0        0        0    32160 2023-06-17 08:36:57.000000 watex-0.2.6/watex/_docstring.py
+-rw-rw-rw-   0        0        0     3852 2023-03-11 03:28:02.000000 watex-0.2.6/watex/_isotonic.pyx
+-rw-rw-rw-   0        0        0    17770 2023-04-14 23:54:09.000000 watex-0.2.6/watex/_typing.py
+-rw-rw-rw-   0        0        0      218 2023-06-23 03:30:45.000000 watex-0.2.6/watex/_version.py
+-rw-rw-rw-   0        0        0     8798 2023-03-12 01:49:05.000000 watex-0.2.6/watex/_watexlog.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.416828 watex-0.2.6/watex/analysis/
+-rw-rw-rw-   0        0        0     1242 2023-02-04 08:11:48.000000 watex-0.2.6/watex/analysis/__init__.py
+-rw-rw-rw-   0        0        0    23341 2023-01-18 16:30:53.000000 watex-0.2.6/watex/analysis/decomposition.py
+-rw-rw-rw-   0        0        0    25575 2023-02-05 12:23:26.000000 watex-0.2.6/watex/analysis/dimensionality.py
+-rw-rw-rw-   0        0        0     9305 2023-02-04 08:20:23.000000 watex-0.2.6/watex/analysis/factor.py
+-rw-rw-rw-   0        0        0    85025 2023-03-12 01:49:14.000000 watex-0.2.6/watex/base.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.420897 watex-0.2.6/watex/cases/
+-rw-rw-rw-   0        0        0     1078 2023-01-12 16:27:24.000000 watex-0.2.6/watex/cases/__init__.py
+-rw-rw-rw-   0        0        0    38684 2023-03-12 01:39:59.000000 watex-0.2.6/watex/cases/features.py
+-rw-rw-rw-   0        0        0    31952 2023-03-12 01:40:49.000000 watex-0.2.6/watex/cases/modeling.py
+-rw-rw-rw-   0        0        0    39022 2023-03-12 01:40:40.000000 watex-0.2.6/watex/cases/prepare.py
+-rw-rw-rw-   0        0        0    49220 2023-03-12 01:41:33.000000 watex-0.2.6/watex/cases/processing.py
+-rw-rw-rw-   0        0        0     1353 2023-03-15 12:48:58.000000 watex-0.2.6/watex/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.477547 watex-0.2.6/watex/datasets/
+-rw-rw-rw-   0        0        0      911 2023-06-20 13:03:34.000000 watex-0.2.6/watex/datasets/__init__.py
+-rw-rw-rw-   0        0        0     7785 2023-03-21 13:31:09.000000 watex-0.2.6/watex/datasets/_config.py
+-rw-rw-rw-   0        0        0       29 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/_hongliu.py
+-rw-rw-rw-   0        0        0     5677 2023-03-21 13:58:43.000000 watex-0.2.6/watex/datasets/_p.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.604062 watex-0.2.6/watex/datasets/data/
+-rw-rw-rw-   0        0        0       27 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/data/__init__.py
+-rw-rw-rw-   0        0        0   328758 2023-03-20 17:59:44.000000 watex-0.2.6/watex/datasets/data/b.pkl
+-rw-rw-rw-   0        0        0    34993 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/data/bagoue.csv
+-rw-rw-rw-   0        0        0    35250 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/data/boston_house_prices.csv
+-rw-rw-rw-   0        0        0      638 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/data/boundiali_ves.csv
+-rw-rw-rw-   0        0        0     1158 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/data/dcerp_gbalo.csv
+-rw-rw-rw-   0        0        0      699 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/data/dcves_gbalo.csv
+-rw-rw-rw-   0        0        0  2216584 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/data/e.h5
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.619261 watex-0.2.6/watex/datasets/data/edis/
+-rw-rw-rw-   0        0        0        4 2023-02-24 10:23:34.000000 watex-0.2.6/watex/datasets/data/edis/__init__.py
+-rw-rw-rw-   0        0        0   170380 2023-02-24 10:23:34.000000 watex-0.2.6/watex/datasets/data/edis/raw.E.zip
+-rw-rw-rw-   0        0        0   184986 2023-02-24 10:23:34.000000 watex-0.2.6/watex/datasets/data/edis/s.E.zip
+-rw-rw-rw-   0        0        0 11940145 2023-05-05 12:57:48.000000 watex-0.2.6/watex/datasets/data/h.h5
+-rw-rw-rw-   0        0        0     2885 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/data/iris.csv
+-rw-rw-rw-   0        0        0   731414 2023-05-05 12:57:48.000000 watex-0.2.6/watex/datasets/data/mxs.joblib
+-rw-rw-rw-   0        0        0     6955 2023-06-20 12:17:20.000000 watex-0.2.6/watex/datasets/data/nlogs+.csv
+-rw-rw-rw-   0        0        0    13993 2023-06-20 12:17:20.000000 watex-0.2.6/watex/datasets/data/nlogs.csv
+-rw-rw-rw-   0        0        0      603 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/data/semien_ves.csv
+-rw-rw-rw-   0        0        0     2230 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/data/tankesse.csv
+-rw-rw-rw-   0        0        0    11336 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/data/wine_data.csv
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.676581 watex-0.2.6/watex/datasets/descr/
+-rw-rw-rw-   0        0        0       29 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/descr/__init__.py
+-rw-rw-rw-   0        0        0     2827 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/descr/bagoue.rst
+-rw-rw-rw-   0        0        0     2397 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/descr/boston_house_prices.rst
+-rw-rw-rw-   0        0        0     2844 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/descr/boundiali_ves.rst
+-rw-rw-rw-   0        0        0     1822 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/descr/california_housing.rst
+-rw-rw-rw-   0        0        0     2844 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/descr/gbalo_erp.rst
+-rw-rw-rw-   0        0        0     2844 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/descr/gbalo_ves.rst
+-rw-rw-rw-   0        0        0     2845 2023-06-20 12:17:20.000000 watex-0.2.6/watex/datasets/descr/huayuan_edis.rst
+-rw-rw-rw-   0        0        0     2844 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/descr/iris.rst
+-rw-rw-rw-   0        0        0     3381 2023-06-20 12:17:20.000000 watex-0.2.6/watex/datasets/descr/nanshang+.rst
+-rw-rw-rw-   0        0        0     2332 2023-06-20 12:17:20.000000 watex-0.2.6/watex/datasets/descr/nanshang.rst
+-rw-rw-rw-   0        0        0     3544 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/descr/wine_data.rst
+-rw-rw-rw-   0        0        0    52573 2023-06-20 12:38:30.000000 watex-0.2.6/watex/datasets/dload.py
+-rw-rw-rw-   0        0        0    17331 2023-05-05 12:57:48.000000 watex-0.2.6/watex/datasets/gdata.py
+-rw-rw-rw-   0        0        0    13639 2023-03-24 15:43:33.000000 watex-0.2.6/watex/datasets/io.py
+-rw-rw-rw-   0        0        0    34896 2023-03-12 01:42:57.000000 watex-0.2.6/watex/datasets/rload.py
+-rw-rw-rw-   0        0        0     7180 2023-06-20 12:17:20.000000 watex-0.2.6/watex/datasets/sets.py
+-rw-rw-rw-   0        0        0      822 2023-01-08 08:20:47.000000 watex-0.2.6/watex/datasets/setup.py
+-rw-rw-rw-   0        0        0   101919 2023-06-21 11:42:13.000000 watex-0.2.6/watex/decorators.py
+-rw-rw-rw-   0        0        0   115869 2023-03-23 14:01:07.000000 watex-0.2.6/watex/edi.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.728093 watex-0.2.6/watex/etc/
+-rw-rw-rw-   0        0        0     5711 2023-01-08 08:20:47.000000 watex-0.2.6/watex/etc/AGSO.csv
+-rw-rw-rw-   0        0        0      351 2023-01-08 08:20:47.000000 watex-0.2.6/watex/etc/AGSO_STCODES.csv
+-rw-rw-rw-   0        0        0    14650 2023-03-20 14:32:57.000000 watex-0.2.6/watex/etc/__XTyT.pkl
+-rw-rw-rw-   0        0        0    37763 2023-03-20 16:12:55.000000 watex-0.2.6/watex/etc/__Xy.pkl
+-rw-rw-rw-   0        0        0       29 2023-01-08 08:20:47.000000 watex-0.2.6/watex/etc/__init__.py
+-rw-rw-rw-   0        0        0    18951 2023-06-23 01:36:31.000000 watex-0.2.6/watex/etc/__memory.pkl
+-rw-rw-rw-   0        0        0    28672 2023-01-08 08:20:47.000000 watex-0.2.6/watex/etc/memory.sq3
+-rw-rw-rw-   0        0        0 52244397 2023-01-08 08:20:47.000000 watex-0.2.6/watex/etc/p.models.pkl
+-rw-rw-rw-   0        0        0     9763 2023-06-21 11:42:13.000000 watex-0.2.6/watex/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.827264 watex-0.2.6/watex/exlib/
+-rw-rw-rw-   0        0        0     4022 2023-03-27 14:03:16.000000 watex-0.2.6/watex/exlib/__init__.py
+-rw-rw-rw-   0        0        0     2580 2023-03-15 12:48:58.000000 watex-0.2.6/watex/exlib/gbm.py
+-rw-rw-rw-   0        0        0     7156 2023-03-12 01:43:33.000000 watex-0.2.6/watex/exlib/sklearn.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.862549 watex-0.2.6/watex/externals/
+-rw-rw-rw-   0        0        0      313 2023-01-18 17:47:22.000000 watex-0.2.6/watex/externals/__init__.py
+-rw-rw-rw-   0        0        0     4835 2023-01-08 08:20:47.000000 watex-0.2.6/watex/externals/_numpy_compiler_patch.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.877740 watex-0.2.6/watex/externals/_pkgs/
+-rw-rw-rw-   0        0        0       29 2023-01-08 08:20:47.000000 watex-0.2.6/watex/externals/_pkgs/__init__.py
+-rw-rw-rw-   0        0        0     3035 2023-01-08 08:20:47.000000 watex-0.2.6/watex/externals/_pkgs/_structures.py
+-rw-rw-rw-   0        0        0    16762 2023-01-08 08:20:47.000000 watex-0.2.6/watex/externals/_pkgs/version.py
+-rw-rw-rw-   0        0        0      273 2023-01-08 08:20:47.000000 watex-0.2.6/watex/externals/readme.md
+-rw-rw-rw-   0        0        0    57854 2023-03-23 14:01:07.000000 watex-0.2.6/watex/externals/z.py
+-rw-rw-rw-   0        0        0    24161 2023-03-12 01:43:53.000000 watex-0.2.6/watex/externals/zutils.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.889716 watex-0.2.6/watex/geology/
+-rw-rw-rw-   0        0        0     1067 2023-06-17 08:36:57.000000 watex-0.2.6/watex/geology/__init__.py
+-rw-rw-rw-   0        0        0    12889 2023-06-23 01:35:29.000000 watex-0.2.6/watex/geology/core.py
+-rw-rw-rw-   0        0        0    56362 2023-06-23 01:02:33.000000 watex-0.2.6/watex/geology/database.py
+-rw-rw-rw-   0        0        0   130836 2023-06-22 07:24:02.000000 watex-0.2.6/watex/geology/drilling.py
+-rw-rw-rw-   0        0        0    14488 2023-05-24 12:02:39.000000 watex-0.2.6/watex/geology/geology.py
+-rw-rw-rw-   0        0        0    73222 2023-06-23 01:29:17.000000 watex-0.2.6/watex/geology/stratigraphic.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.903946 watex-0.2.6/watex/methods/
+-rw-rw-rw-   0        0        0      867 2023-04-15 15:25:13.000000 watex-0.2.6/watex/methods/__init__.py
+-rw-rw-rw-   0        0        0    82817 2023-04-22 06:56:19.000000 watex-0.2.6/watex/methods/electrical.py
+-rw-rw-rw-   0        0        0   136679 2023-05-14 09:33:31.000000 watex-0.2.6/watex/methods/em.py
+-rw-rw-rw-   0        0        0    86661 2023-04-22 06:56:19.000000 watex-0.2.6/watex/methods/erp.py
+-rw-rw-rw-   0        0        0    43855 2023-03-12 01:45:26.000000 watex-0.2.6/watex/methods/hydro.py
+-rw-rw-rw-   0        0        0    28992 2023-05-24 12:02:39.000000 watex-0.2.6/watex/metrics.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.912641 watex-0.2.6/watex/models/
+-rw-rw-rw-   0        0        0     1064 2023-03-24 12:58:06.000000 watex-0.2.6/watex/models/__init__.py
+-rw-rw-rw-   0        0        0     6889 2023-03-15 12:48:58.000000 watex-0.2.6/watex/models/_metapredictors.py
+-rw-rw-rw-   0        0        0    18878 2023-03-15 12:48:58.000000 watex-0.2.6/watex/models/premodels.py
+-rw-rw-rw-   0        0        0    44482 2023-03-28 11:58:09.000000 watex-0.2.6/watex/models/validation.py
+-rw-rw-rw-   0        0        0    73934 2023-06-22 04:42:01.000000 watex-0.2.6/watex/property.py
+-rw-rw-rw-   0        0        0    51498 2023-06-22 07:29:40.000000 watex-0.2.6/watex/site.py
+-rw-rw-rw-   0        0        0    61886 2023-06-17 08:36:57.000000 watex-0.2.6/watex/transformers.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:49.020031 watex-0.2.6/watex/utils/
+-rw-rw-rw-   0        0        0     6196 2023-06-21 11:42:13.000000 watex-0.2.6/watex/utils/__init__.py
+-rw-rw-rw-   0        0        0     7140 2023-01-08 08:20:47.000000 watex-0.2.6/watex/utils/_array_api.py
+-rw-rw-rw-   0        0        0     7730 2023-01-08 08:20:47.000000 watex-0.2.6/watex/utils/_arraytools.py
+-rw-rw-rw-   0        0        0     5936 2023-02-01 06:46:13.000000 watex-0.2.6/watex/utils/_dependency.py
+-rw-rw-rw-   0        0        0      222 2023-01-08 08:20:47.000000 watex-0.2.6/watex/utils/_openmp_helpers.pxd
+-rw-rw-rw-   0        0        0     2674 2023-01-08 08:20:47.000000 watex-0.2.6/watex/utils/_openmp_helpers.pyx
+-rw-rw-rw-   0        0        0    16659 2023-01-28 02:10:06.000000 watex-0.2.6/watex/utils/_packaging_version.py
+-rw-rw-rw-   0        0        0     1616 2023-03-28 11:58:09.000000 watex-0.2.6/watex/utils/_set_gdal.py
+-rw-rw-rw-   0        0        0     2583 2023-02-16 08:00:08.000000 watex-0.2.6/watex/utils/_show_versions.py
+-rw-rw-rw-   0        0        0    13908 2023-05-26 13:32:06.000000 watex-0.2.6/watex/utils/box.py
+-rw-rw-rw-   0        0        0    98080 2023-06-18 14:15:21.000000 watex-0.2.6/watex/utils/coreutils.py
+-rw-rw-rw-   0        0        0   580618 2023-01-08 08:20:47.000000 watex-0.2.6/watex/utils/epsg.npy
+-rw-rw-rw-   0        0        0   232345 2023-06-22 07:30:24.000000 watex-0.2.6/watex/utils/exmath.py
+-rw-rw-rw-   0        0        0   252184 2023-06-21 11:42:13.000000 watex-0.2.6/watex/utils/funcutils.py
+-rw-rw-rw-   0        0        0    82957 2023-06-22 07:00:16.000000 watex-0.2.6/watex/utils/geotools.py
+-rw-rw-rw-   0        0        0    58698 2023-03-28 11:58:09.000000 watex-0.2.6/watex/utils/gistools.py
+-rw-rw-rw-   0        0        0   139514 2023-06-22 04:42:01.000000 watex-0.2.6/watex/utils/hydroutils.py
+-rw-rw-rw-   0        0        0   122844 2023-05-24 12:02:39.000000 watex-0.2.6/watex/utils/mlutils.py
+-rw-rw-rw-   0        0        0   139113 2023-06-22 05:05:15.000000 watex-0.2.6/watex/utils/plotutils.py
+-rw-rw-rw-   0        0        0      974 2023-01-08 08:20:47.000000 watex-0.2.6/watex/utils/setup.py
+-rw-rw-rw-   0        0        0     3548 2023-01-08 08:20:47.000000 watex-0.2.6/watex/utils/thread.py
+-rw-rw-rw-   0        0        0    86096 2023-06-17 08:36:57.000000 watex-0.2.6/watex/utils/validator.py
+-rw-rw-rw-   0        0        0    16835 2023-01-28 01:30:49.000000 watex-0.2.6/watex/utils/version.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:49.022298 watex-0.2.6/watex/view/
+-rw-rw-rw-   0        0        0     1008 2023-02-24 10:23:34.000000 watex-0.2.6/watex/view/__init__.py
+-rw-rw-rw-   0        0        0   145840 2023-05-14 06:19:47.000000 watex-0.2.6/watex/view/mlplot.py
+-rw-rw-rw-   0        0        0   190822 2023-04-22 06:56:19.000000 watex-0.2.6/watex/view/plot.py
+-rw-rw-rw-   0        0        0     1222 2023-03-11 03:28:02.000000 watex-0.2.6/watex/wlog.yml
+drwxrwxrwx   0        0        0        0 2023-06-23 03:30:48.379443 watex-0.2.6/watex.egg-info/
+-rw-rw-rw-   0        0        0    15816 2023-06-23 03:30:45.000000 watex-0.2.6/watex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9707 2023-06-23 03:30:46.000000 watex-0.2.6/watex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 03:30:45.000000 watex-0.2.6/watex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-06-23 03:30:45.000000 watex-0.2.6/watex.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      366 2023-06-23 03:30:45.000000 watex-0.2.6/watex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-23 03:30:45.000000 watex-0.2.6/watex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-23 03:29:00.000000 watex-0.2.6/watex.egg-info/zip-safe
```

### Comparing `watex-0.2.5/.github/dependabot.yml` & `watex-0.2.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/.github/workflows/ci.yaml` & `watex-0.2.6/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/.github/workflows/codeql.yml` & `watex-0.2.6/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/.github/workflows/dependency-review.yml` & `watex-0.2.6/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/.github/workflows/python-package.yml` & `watex-0.2.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/.gitignore` & `watex-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/CITATION.cff` & `watex-0.2.6/CITATION.cff`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/LICENSE` & `watex-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/MANIFEST.in` & `watex-0.2.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/PKG-INFO` & `watex-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watex
-Version: 0.2.5
+Version: 0.2.6
 Summary: Machine learning research in water exploration
 Home-page: https://github.com/WEgeophysics/watex
 Download-URL: https://pypi.org/project/watex/#files
 Author: Laurent Kouadio
 Author-email: etanoyau@gmail.com
 Maintainer: Laurent Kouadio
 Maintainer-email: etanoyau@gmail.com
```

### Comparing `watex-0.2.5/README.md` & `watex-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/Makefile` & `watex-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/copybutton.js` & `watex-0.2.6/docs/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/css/bootstrap.min.css` & `watex-0.2.6/docs/_static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/css/custom.css` & `watex-0.2.6/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/favicon.ico` & `watex-0.2.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/favicon0.ico` & `watex-0.2.6/docs/_static/favicon0.ico`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/favicon_old.ico` & `watex-0.2.6/docs/_static/favicon_old.ico`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/index_api.svg` & `watex-0.2.6/docs/_static/index_api.svg`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/index_contribute.svg` & `watex-0.2.6/docs/_static/index_contribute.svg`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/index_getting_started.svg` & `watex-0.2.6/docs/_static/index_getting_started.svg`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/index_user_guide.svg` & `watex-0.2.6/docs/_static/index_user_guide.svg`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/js/vendor/bootstrap.min.js` & `watex-0.2.6/docs/_static/js/vendor/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/js/vendor/jquery-3.6.3.slim.min.js` & `watex-0.2.6/docs/_static/js/vendor/jquery-3.6.3.slim.min.js`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/logo.svg` & `watex-0.2.6/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/logo_no_name.svg` & `watex-0.2.6/docs/_static/logo_no_name.svg`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/logo_small.svg` & `watex-0.2.6/docs/_static/logo_small.svg`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/logo_wide.svg` & `watex-0.2.6/docs/_static/logo_wide.svg`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/logo_wide_rev.svg` & `watex-0.2.6/docs/_static/logo_wide_rev.svg`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/logo_wide_rev0.svg` & `watex-0.2.6/docs/_static/logo_wide_rev0.svg`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/switcher.json` & `watex-0.2.6/docs/_static/switcher.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8636363636363636%*

 * *Differences: {'0': "{'version': 'v0.2.7'}",*

 * * '1': "{'name': '0.2.6 (stable)', 'url': 'https://watex.readthedocs.io/en/0.2.6/'}",*

 * * 'insert': "[(2, OrderedDict([('name', '0.2.5'), ('version', 'v0.2.5'), ('url', "*

 * *           "'https://watex.readthedocs.io/en/0.2.5/')]))]"}*

```diff
@@ -1,19 +1,24 @@
 [
     {
         "name": "dev",
         "url": "https://watex.readthedocs.io/en/latest/",
-        "version": "v0.2.6"
+        "version": "v0.2.7"
     },
     {
-        "name": "0.2.5 (stable)",
-        "url": "https://watex.readthedocs.io/en/stable/",
+        "name": "0.2.6 (stable)",
+        "url": "https://watex.readthedocs.io/en/0.2.6/",
         "version": "stable"
     },
     {
+        "name": "0.2.5",
+        "url": "https://watex.readthedocs.io/en/0.2.5/",
+        "version": "v0.2.5"
+    },
+    {
         "name": "0.2.4",
         "url": "https://watex.readthedocs.io/en/0.2.4/",
         "version": "v0.2.4"
     },
     {
         "name": "0.2.3",
         "url": "https://watex.readthedocs.io/en/0.2.3/",
```

### Comparing `watex-0.2.5/docs/_static/to_favicon.svg` & `watex-0.2.6/docs/_static/to_favicon.svg`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/watex_thumb_image.svg` & `watex-0.2.6/docs/_static/watex_thumb_image.svg`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_static/watex_workflow.svg` & `watex-0.2.6/docs/_static/watex_workflow.svg`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_templates/javascript.html` & `watex-0.2.6/docs/_templates/javascript.html`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/_templates/layout.html` & `watex-0.2.6/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/analysis.rst` & `watex-0.2.6/docs/analysis.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/api_references.rst` & `watex-0.2.6/docs/api_references.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/base.rst` & `watex-0.2.6/docs/base.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/cases.rst` & `watex-0.2.6/docs/cases.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/citing.rst` & `watex-0.2.6/docs/citing.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/community/CONTRIBUTING.md` & `watex-0.2.6/docs/community/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/conf.py` & `watex-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/datasets.rst` & `watex-0.2.6/docs/datasets.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/development.rst` & `watex-0.2.6/docs/development.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/example_thumbs/watex_workflow.gif` & `watex-0.2.6/docs/example_thumbs/watex_workflow.gif`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/glossary.rst` & `watex-0.2.6/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/history/five_min_understanding.rst` & `watex-0.2.6/docs/history/five_min_understanding.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/history/project_goals.rst` & `watex-0.2.6/docs/history/project_goals.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/history/project_story.rst` & `watex-0.2.6/docs/history/project_story.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/includes/big_toc_css.rst` & `watex-0.2.6/docs/includes/big_toc_css.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/includes/bigger_toc_css.rst` & `watex-0.2.6/docs/includes/bigger_toc_css.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/index.rst` & `watex-0.2.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/installation.rst` & `watex-0.2.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/make.bat` & `watex-0.2.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/methods.rst` & `watex-0.2.6/docs/methods.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/requirements.txt` & `watex-0.2.6/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/source/index.html` & `watex-0.2.6/docs/source/index.html`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/sphinxext/add_toctree_functions.py` & `watex-0.2.6/docs/sphinxext/add_toctree_functions.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/sphinxext/doi_role.py` & `watex-0.2.6/docs/sphinxext/doi_role.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/sphinxext/sphinx_issues.py` & `watex-0.2.6/docs/sphinxext/sphinx_issues.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/structure.rst` & `watex-0.2.6/docs/structure.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/tune_toc.rst` & `watex-0.2.6/docs/tune_toc.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/utils.rst` & `watex-0.2.6/docs/utils.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/view.rst` & `watex-0.2.6/docs/view.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/index.rst` & `watex-0.2.6/docs/whatsnew/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 Version 0.2
 -------------
 
 .. toctree::
    :maxdepth: 2
    
+   v0.2.6
    v0.2.5
    v0.2.4
    v0.2.3
    v0.2.2
    v0.2.1
    v0.2.0
```

### Comparing `watex-0.2.5/docs/whatsnew/v0.1.0.rst` & `watex-0.2.6/docs/whatsnew/v0.1.0.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.1.1.rst` & `watex-0.2.6/docs/whatsnew/v0.1.1.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.1.2.rst` & `watex-0.2.6/docs/whatsnew/v0.1.2.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.1.3.rst` & `watex-0.2.6/docs/whatsnew/v0.1.3.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.1.4.rst` & `watex-0.2.6/docs/whatsnew/v0.1.4.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.1.5.rst` & `watex-0.2.6/docs/whatsnew/v0.1.5.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.1.6-alpha.rst` & `watex-0.2.6/docs/whatsnew/v0.1.6-alpha.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.1.6.rst` & `watex-0.2.6/docs/whatsnew/v0.1.6.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.1.7.rst` & `watex-0.2.6/docs/whatsnew/v0.1.7.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.1.8.rst` & `watex-0.2.6/docs/whatsnew/v0.1.8.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.1.9.rst` & `watex-0.2.6/docs/whatsnew/v0.1.9.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.2.0.rst` & `watex-0.2.6/docs/whatsnew/v0.2.0.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.2.1.rst` & `watex-0.2.6/docs/whatsnew/v0.2.1.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.2.2.rst` & `watex-0.2.6/docs/whatsnew/v0.2.2.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.2.3.rst` & `watex-0.2.6/docs/whatsnew/v0.2.3.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.2.4.rst` & `watex-0.2.6/docs/whatsnew/v0.2.4.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/docs/whatsnew/v0.2.5.rst` & `watex-0.2.6/docs/whatsnew/v0.2.5.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/analysis/plot_decision_regions.py` & `watex-0.2.6/examples/analysis/plot_decision_regions.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/analysis/plot_explained_variance_ratio.py` & `watex-0.2.6/examples/analysis/plot_explained_variance_ratio.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/analysis/plot_linear_discriminant_analysis.py` & `watex-0.2.6/examples/analysis/plot_linear_discriminant_analysis.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/analysis/plot_pca_vs_factor_with_scedatic_noises.py` & `watex-0.2.6/examples/analysis/plot_pca_vs_factor_with_scedatic_noises.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/applications/plot_auto_detect_drilling_location.py` & `watex-0.2.6/examples/applications/plot_auto_detect_drilling_location.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/applications/plot_data_exploratory_quick_view.py` & `watex-0.2.6/examples/applications/plot_data_exploratory_quick_view.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/applications/plot_dc_em_parameters_computings.py` & `watex-0.2.6/examples/applications/plot_dc_em_parameters_computings.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/applications/plot_flow_rate_prediction.py` & `watex-0.2.6/examples/applications/plot_flow_rate_prediction.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/applications/plot_kmf.py` & `watex-0.2.6/examples/applications/plot_kmf.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/applications/plot_nsamt_tensor_recovery.py` & `watex-0.2.6/examples/applications/plot_nsamt_tensor_recovery.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/applications/plot_tensor_restoring.py` & `watex-0.2.6/examples/applications/plot_tensor_restoring.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/applications/plot_ymxs_label_for_k_prediction.py` & `watex-0.2.6/examples/applications/plot_ymxs_label_for_k_prediction.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/base/plot_ada_gd.py` & `watex-0.2.6/examples/base/plot_ada_gd.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/base/plot_ada_stochastic_gd.py` & `watex-0.2.6/examples/base/plot_ada_stochastic_gd.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/base/plot_missing.py` & `watex-0.2.6/examples/base/plot_missing.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/base/plot_sbs_feature_selector.py` & `watex-0.2.6/examples/base/plot_sbs_feature_selector.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/methods/plot_2d_tensor_filtered.py` & `watex-0.2.6/examples/methods/plot_2d_tensor_filtered.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/methods/plot_anomaly.py` & `watex-0.2.6/examples/methods/plot_anomaly.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/methods/plot_filtered_tensors.py` & `watex-0.2.6/examples/methods/plot_filtered_tensors.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/methods/plot_logging_predictor_and_target.py` & `watex-0.2.6/examples/methods/plot_logging_predictor_and_target.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/methods/plot_logging_predictor_only.py` & `watex-0.2.6/examples/methods/plot_logging_predictor_only.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/methods/plot_multiple_sites_recovery_signal.py` & `watex-0.2.6/examples/methods/plot_multiple_sites_recovery_signal.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/methods/plot_phase_tensors.py` & `watex-0.2.6/examples/methods/plot_phase_tensors.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/methods/plot_raw_2d_tensor.py` & `watex-0.2.6/examples/methods/plot_raw_2d_tensor.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/methods/plot_ves_fracture_zone.py` & `watex-0.2.6/examples/methods/plot_ves_fracture_zone.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_clusters.py` & `watex-0.2.6/examples/utils/plot_clusters.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_confidence_in_data.py` & `watex-0.2.6/examples/utils/plot_confidence_in_data.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_confusion_matrices.py` & `watex-0.2.6/examples/utils/plot_confusion_matrices.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_confusion_matrix_sweet.py` & `watex-0.2.6/examples/utils/plot_confusion_matrix_sweet.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_elbow.py` & `watex-0.2.6/examples/utils/plot_elbow.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_erp.py` & `watex-0.2.6/examples/utils/plot_erp.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_errors_vs_epochs.py` & `watex-0.2.6/examples/utils/plot_errors_vs_epochs.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_ex_heatmap.py` & `watex-0.2.6/examples/utils/plot_ex_heatmap.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_ex_matrix.py` & `watex-0.2.6/examples/utils/plot_ex_matrix.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_learning_curves.py` & `watex-0.2.6/examples/utils/plot_learning_curves.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_log.py` & `watex-0.2.6/examples/utils/plot_log.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_model_confusion_matrix.py` & `watex-0.2.6/examples/utils/plot_model_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_naive_dendrogram.py` & `watex-0.2.6/examples/utils/plot_naive_dendrogram.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_naive_silhouette.py` & `watex-0.2.6/examples/utils/plot_naive_silhouette.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_ohmic_area.py` & `watex-0.2.6/examples/utils/plot_ohmic_area.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_pca_components.py` & `watex-0.2.6/examples/utils/plot_pca_components.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_regularization_path.py` & `watex-0.2.6/examples/utils/plot_regularization_path.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_rf_feature_importances.py` & `watex-0.2.6/examples/utils/plot_rf_feature_importances.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_savitzky_golay1d.py` & `watex-0.2.6/examples/utils/plot_savitzky_golay1d.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_sbs_feature_selection.py` & `watex-0.2.6/examples/utils/plot_sbs_feature_selection.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_sfi.py` & `watex-0.2.6/examples/utils/plot_sfi.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_skew.py` & `watex-0.2.6/examples/utils/plot_skew.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_stratalog.py` & `watex-0.2.6/examples/utils/plot_stratalog.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_strike.py` & `watex-0.2.6/examples/utils/plot_strike.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/utils/plot_voronoi.py` & `watex-0.2.6/examples/utils/plot_voronoi.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_2d_filtered_tensors.py` & `watex-0.2.6/examples/view/plot_2d_filtered_tensors.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_base_distributions.py` & `watex-0.2.6/examples/view/plot_base_distributions.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_biplot.py` & `watex-0.2.6/examples/view/plot_biplot.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_box.py` & `watex-0.2.6/examples/view/plot_box.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_confusion_matrix_metric.py` & `watex-0.2.6/examples/view/plot_confusion_matrix_metric.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_correlating_features.py` & `watex-0.2.6/examples/view/plot_correlating_features.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_cut_comparison.py` & `watex-0.2.6/examples/view/plot_cut_comparison.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_dendrogram.py` & `watex-0.2.6/examples/view/plot_dendrogram.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_dendroheat.py` & `watex-0.2.6/examples/view/plot_dendroheat.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_discussing_features.py` & `watex-0.2.6/examples/view/plot_discussing_features.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_grid.py` & `watex-0.2.6/examples/view/plot_grid.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_hist.py` & `watex-0.2.6/examples/view/plot_hist.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_jointing_features.py` & `watex-0.2.6/examples/view/plot_jointing_features.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_learning_inspections.py` & `watex-0.2.6/examples/view/plot_learning_inspections.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_matshow.py` & `watex-0.2.6/examples/view/plot_matshow.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_model.py` & `watex-0.2.6/examples/view/plot_model.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_model_inspection.py` & `watex-0.2.6/examples/view/plot_model_inspection.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_model_scores.py` & `watex-0.2.6/examples/view/plot_model_scores.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_multiple_feature_distributions.py` & `watex-0.2.6/examples/view/plot_multiple_feature_distributions.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_num_features.py` & `watex-0.2.6/examples/view/plot_num_features.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_pairwise_corr.py` & `watex-0.2.6/examples/view/plot_pairwise_corr.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_pararell_corrdinates.py` & `watex-0.2.6/examples/view/plot_pararell_corrdinates.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_pca.py` & `watex-0.2.6/examples/view/plot_pca.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_phase_sensistive_skew.py` & `watex-0.2.6/examples/view/plot_phase_sensistive_skew.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_phase_tensor_2d.py` & `watex-0.2.6/examples/view/plot_phase_tensor_2d.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_pr.py` & `watex-0.2.6/examples/view/plot_pr.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_projection.py` & `watex-0.2.6/examples/view/plot_projection.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_radviz.py` & `watex-0.2.6/examples/view/plot_radviz.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_reg_scoring.py` & `watex-0.2.6/examples/view/plot_reg_scoring.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_res_tensor_2d.py` & `watex-0.2.6/examples/view/plot_res_tensor_2d.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_rhoa.py` & `watex-0.2.6/examples/view/plot_rhoa.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_roc.py` & `watex-0.2.6/examples/view/plot_roc.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_scatter.py` & `watex-0.2.6/examples/view/plot_scatter.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_scattering_features.py` & `watex-0.2.6/examples/view/plot_scattering_features.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_silhouette.py` & `watex-0.2.6/examples/view/plot_silhouette.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_single_site_signal_recovery.py` & `watex-0.2.6/examples/view/plot_single_site_signal_recovery.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/examples/view/plot_target_inspection.py` & `watex-0.2.6/examples/view/plot_target_inspection.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/pyproject.toml` & `watex-0.2.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 00000080: 2243 7974 686f 6e3e 3d30 2e32 392e 3333  "Cython>=0.29.33
 00000090: 222c 0d0a 2020 2020 2020 2020 5d0d 0a62  ",..        ]..b
 000000a0: 7569 6c64 2d62 6163 6b65 6e64 203d 2022  uild-backend = "
 000000b0: 7365 7475 7074 6f6f 6c73 2e62 7569 6c64  setuptools.build
 000000c0: 5f6d 6574 6122 0d0a 0d0a 5b70 726f 6a65  _meta"....[proje
 000000d0: 6374 5d0d 0a6e 616d 6520 3d20 2277 6174  ct]..name = "wat
 000000e0: 6578 220d 0a76 6572 7369 6f6e 3d22 302e  ex"..version="0.
-000000f0: 322e 3522 0d0a 6479 6e61 6d69 6320 3d20  2.5"..dynamic = 
+000000f0: 322e 3622 0d0a 6479 6e61 6d69 6320 3d20  2.6"..dynamic = 
 00000100: 5b20 226b 6579 776f 7264 7322 5d0d 0a0d  [ "keywords"]...
 00000110: 0a64 6570 656e 6465 6e63 6965 733d 5b0d  .dependencies=[.
 00000120: 0a20 2020 2022 7365 6162 6f72 6e20 3e3d  .    "seaborn >=
 00000130: 302e 3132 2e30 222c 200d 0a20 2020 2022  0.12.0", ..    "
 00000140: 7061 6e64 6173 203e 3d31 2e34 2e30 222c  pandas >=1.4.0",
 00000150: 0d0a 2020 2020 2263 7974 686f 6e20 3e3d  ..    "cython >=
 00000160: 302e 3239 2e33 3322 2c0d 0a20 2020 2022  0.29.33",..    "
```

### Comparing `watex-0.2.5/setup.cfg` & `watex-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/setup.py` & `watex-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 builtins.__WATEX_SETUP__ = True
 
 # We can actually import watex version from 
 # in editable mode :$ python -m pip install -e .
 try: 
     import watex  # noqa
     VERSION = watex.__version__
-except: VERSION ='0.2.4'
+except: VERSION ='0.2.6'
 # set global variables 
 DISTNAME = "watex"
 DESCRIPTION= "Machine learning research in water exploration"
 with open('README.md', 'r', encoding ='utf8') as fm:
     LONG_DESCRIPTION =fm.read()
 MAINTAINER = "Laurent Kouadio"
 MAINTAINER_EMAIL = 'etanoyau@gmail.com'
```

### Comparing `watex-0.2.5/watex/__init__.py` & `watex-0.2.6/watex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         os.path.dirname(__file__), "wlog.yml")
 
 # generated version by setuptools_scm 
 try:
     from . import _version
     __version__ = _version.version.split('.dev')[0]
 except ImportError:
-    __version__ = '0.2.5' 
+    __version__ = '0.2.6' 
 
 # # set loging Level
 logging.getLogger(__name__)#.setLevel(logging.WARNING)
 # disable the matplotlib font manager logger.
 logging.getLogger('matplotlib.font_manager').disabled = True
 # or ust suppress the DEBUG messages but not the others from that logger.
 # logging.getLogger('matplotlib.font_manager').setLevel(logging.ERROR)
```

### Comparing `watex-0.2.5/watex/_docstring.py` & `watex-0.2.6/watex/_docstring.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/_isotonic.pyx` & `watex-0.2.6/watex/_isotonic.pyx`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/_typing.py` & `watex-0.2.6/watex/_typing.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/_watexlog.py` & `watex-0.2.6/watex/_watexlog.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/analysis/__init__.py` & `watex-0.2.6/watex/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/analysis/decomposition.py` & `watex-0.2.6/watex/analysis/decomposition.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/analysis/dimensionality.py` & `watex-0.2.6/watex/analysis/dimensionality.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/analysis/factor.py` & `watex-0.2.6/watex/analysis/factor.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/base.py` & `watex-0.2.6/watex/base.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/cases/__init__.py` & `watex-0.2.6/watex/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/cases/features.py` & `watex-0.2.6/watex/cases/features.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/cases/modeling.py` & `watex-0.2.6/watex/cases/modeling.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/cases/prepare.py` & `watex-0.2.6/watex/cases/prepare.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/cases/processing.py` & `watex-0.2.6/watex/cases/processing.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/cli.py` & `watex-0.2.6/watex/cli.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/__init__.py` & `watex-0.2.6/watex/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/_config.py` & `watex-0.2.6/watex/datasets/_config.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/_p.py` & `watex-0.2.6/watex/datasets/_p.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/b.pkl` & `watex-0.2.6/watex/datasets/data/b.pkl`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/bagoue.csv` & `watex-0.2.6/watex/datasets/data/bagoue.csv`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/boston_house_prices.csv` & `watex-0.2.6/watex/datasets/data/boston_house_prices.csv`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/boundiali_ves.csv` & `watex-0.2.6/watex/datasets/data/boundiali_ves.csv`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/dcerp_gbalo.csv` & `watex-0.2.6/watex/datasets/data/dcerp_gbalo.csv`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/dcves_gbalo.csv` & `watex-0.2.6/watex/datasets/data/dcves_gbalo.csv`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/e.h5` & `watex-0.2.6/watex/datasets/data/e.h5`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/edis/raw.E.zip` & `watex-0.2.6/watex/datasets/data/edis/raw.E.zip`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/edis/s.E.zip` & `watex-0.2.6/watex/datasets/data/edis/s.E.zip`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/h.h5` & `watex-0.2.6/watex/datasets/data/h.h5`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/iris.csv` & `watex-0.2.6/watex/datasets/data/iris.csv`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/mxs.joblib` & `watex-0.2.6/watex/datasets/data/mxs.joblib`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/nlogs+.csv` & `watex-0.2.6/watex/datasets/data/nlogs+.csv`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/nlogs.csv` & `watex-0.2.6/watex/datasets/data/nlogs.csv`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/semien_ves.csv` & `watex-0.2.6/watex/datasets/data/semien_ves.csv`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/tankesse.csv` & `watex-0.2.6/watex/datasets/data/tankesse.csv`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/data/wine_data.csv` & `watex-0.2.6/watex/datasets/data/wine_data.csv`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/descr/bagoue.rst` & `watex-0.2.6/watex/datasets/descr/bagoue.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/descr/boston_house_prices.rst` & `watex-0.2.6/watex/datasets/descr/boston_house_prices.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/descr/boundiali_ves.rst` & `watex-0.2.6/watex/datasets/descr/boundiali_ves.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/descr/california_housing.rst` & `watex-0.2.6/watex/datasets/descr/california_housing.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/descr/gbalo_erp.rst` & `watex-0.2.6/watex/datasets/descr/gbalo_erp.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/descr/gbalo_ves.rst` & `watex-0.2.6/watex/datasets/descr/gbalo_ves.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/descr/huayuan_edis.rst` & `watex-0.2.6/watex/datasets/descr/huayuan_edis.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/descr/iris.rst` & `watex-0.2.6/watex/datasets/descr/iris.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/descr/nanshang+.rst` & `watex-0.2.6/watex/datasets/descr/nanshang+.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/descr/nanshang.rst` & `watex-0.2.6/watex/datasets/descr/nanshang.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/descr/wine_data.rst` & `watex-0.2.6/watex/datasets/descr/wine_data.rst`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/dload.py` & `watex-0.2.6/watex/datasets/dload.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/gdata.py` & `watex-0.2.6/watex/datasets/gdata.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/io.py` & `watex-0.2.6/watex/datasets/io.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/rload.py` & `watex-0.2.6/watex/datasets/rload.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/sets.py` & `watex-0.2.6/watex/datasets/sets.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/datasets/setup.py` & `watex-0.2.6/watex/datasets/setup.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/decorators.py` & `watex-0.2.6/watex/decorators.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/edi.py` & `watex-0.2.6/watex/edi.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/etc/AGSO.csv` & `watex-0.2.6/watex/etc/AGSO.csv`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/etc/__XTyT.pkl` & `watex-0.2.6/watex/etc/__XTyT.pkl`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/etc/__Xy.pkl` & `watex-0.2.6/watex/etc/__Xy.pkl`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/etc/memory.sq3` & `watex-0.2.6/watex/etc/memory.sq3`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/etc/p.models.pkl` & `watex-0.2.6/watex/etc/p.models.pkl`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/exceptions.py` & `watex-0.2.6/watex/exceptions.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/exlib/__init__.py` & `watex-0.2.6/watex/exlib/__init__.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/exlib/gbm.py` & `watex-0.2.6/watex/exlib/gbm.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/exlib/sklearn.py` & `watex-0.2.6/watex/exlib/sklearn.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/externals/_numpy_compiler_patch.py` & `watex-0.2.6/watex/externals/_numpy_compiler_patch.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/externals/_pkgs/_structures.py` & `watex-0.2.6/watex/externals/_pkgs/_structures.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/externals/_pkgs/version.py` & `watex-0.2.6/watex/externals/_pkgs/version.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/externals/z.py` & `watex-0.2.6/watex/externals/z.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/externals/zutils.py` & `watex-0.2.6/watex/externals/zutils.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/geology/__init__.py` & `watex-0.2.6/watex/geology/__init__.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/geology/core.py` & `watex-0.2.6/watex/geology/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 """
 
 import os
 import warnings
 import shutil 
 from six.moves import urllib 
 from pprint import pprint 
+from importlib import resources
 
 from ..utils.funcutils import ( 
     smart_format, 
     sPath,
     )
 from ..utils._dependency import ( 
     import_optional_dependency )
@@ -80,18 +81,21 @@
         self._logging = watexlog.get_watex_logger(self.__class__.__name__)
         self.verbose= verbose 
         
         for key in list(kwargs.keys()): 
             setattr(self, key, kwargs[key])
             
 #++++ configure the geological rocks from files:AGSO & AGSO.STCODES +++++++++++
+EMOD = 'watex.etc' ; buffer_file = 'AGSO.csv'
+with resources.path (EMOD, buffer_file) as buff : 
+     props_buf  = str(buff) 
 __agso_properties =dict(
     GIT_REPO = 'https://github.com/WEgeophysics/watex', 
     GIT_ROOT ='https://raw.githubusercontent.com/WEgeophysics/watex/master/',
-    props_dir = 'watex/etc/',
+    props_dir = os.path.dirname (props_buf),
     props_files = ['AGSO.csv', 'AGSO_STCODES.csv'], 
     props_codes = ['code', 'label', 'name', 'pattern','size',
             'density', 'thickness', 'color']
     )
 
 def set_agso_properties (download_files = True ): 
     """ Set the rocks and their properties from inner files located in
```

### Comparing `watex-0.2.5/watex/geology/database.py` & `watex-0.2.6/watex/geology/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,30 +18,29 @@
 import sys
 import numpy as np  
 import pandas as pd 
 import warnings
 import datetime
 import shutil 
 import sqlite3 as sq3 
+from importlib import resources
 # from pg8000 import DBAPI
 from ..exceptions import ( 
     GeoDatabaseError, 
     SQLError, 
     SQLManagerError
     )
 from .geology import ( 
     Structures
     )
 from .._watexlog import watexlog 
 _logger = watexlog().get_watex_logger(__name__ )
-
-# let set the systeme path find memory dataBase
-for p in ('.', '..', '../..', 'watex/etc'): 
-    # for consistency, force system to find the database path.
-    sys.path.insert(0, os.path.abspath(p))  
+#for consistency, force system to find the database path
+# from absolute path 
+sys.path.insert(0, "..") 
 
 class GeoDataBase (object): 
     """
     Core geological database class. 
     
     Currently we do not create the specific pattern for each geostructures. 
     DataBase is built is built following  structure or property code 
@@ -60,23 +59,23 @@
     
     """
     #  FGDC is not set yet , we use the  matplotlib pattern symbol makers 
     make_pattern_symbol =["/", "\\", "|", '-', '+', 'x', 'o', 'O', '.', 
                           '*', '\-', '\+', '\o', '\O', '\.', '\*'] 
     #use '\\' rather than '\'.
     # latter , it will be deprecated to FGDC geological map symbolization. 
-    
     codef = ['code','label','__description','pattern', 'pat_size',	
              'pat_density','pat_thickness','rgb','electrical_props', 
-                 'hatch', 'colorMPL', 'FGDC' ]
+              'hatch', 'colorMPL', 'FGDC' ]
+
+    # let set the systeme path find memory dataBase
+    DMOD = 'watex.etc' ; memory='memory.sq3'
+    with resources.path (DMOD, memory) as p : 
+         geoDataBase = str(p) # for consistency
 
-    # locate the geodataBase
-    geoDataBase = os.path.join(
-        os.path.abspath('watex/etc'),'memory.sq3')
- 
     # :memory: is faster but we chose the static option :~.sq3 
     # in sql_DB contains drill holes and wells Tables 
 
     def __init__(
             self, 
             geo_structure_name=None
             ):
@@ -92,17 +91,18 @@
 
         try : 
         # to connect geodataBse 
             self.manage_geoDataBase =DBSetting(
                 db_host=os.path.dirname(self.geoDataBase), 
                                       db_name ='memory.sq3')
         except : 
-            mess =''.join(['Connection to geoDataBase failed! Sorry we can ',
-                           'not give a suitable reply for your request!', 
-                    'It would  be process with "geological structural class." !'])
+            mess =''.join([
+                'Connection to geoDataBase failed. Sorry, we can',
+                ' not give a suitable reply for your request', 
+                'It would  be process with "geological structural class." !'])
             
             warnings.warn(mess)
             self.success= 0
  
         else: 
             self.success = 1
```

### Comparing `watex-0.2.5/watex/geology/drilling.py` & `watex-0.2.6/watex/geology/drilling.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/geology/geology.py` & `watex-0.2.6/watex/geology/geology.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/geology/stratigraphic.py` & `watex-0.2.6/watex/geology/stratigraphic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1350,57 +1350,46 @@
             for k in _t]) + '>' 
             
         return  outm.format(self.__class__.__name__)
     
 def _ps_memory_management(obj=None, option='set'): 
     """ Manage the running times for stratigraphic model construction.
     
-    The script allows to avoid running several times the GeoStrataModel model
-    construction to retrieve the pseudostratigraphic (PS) log at each station.  
+    The script allows to avoid running several times the GeoStrataModel
+     model construction to retrieve the stratigraphic log at each station.  
     It memorizes the model data for the first run and used it when calling it
-    to  visualize the PS log at each station. Be aware to edit this script.
+    to  visualize the strata log at each station. Be aware to edit this script.
     """
-    DMOD = 'watex.etc'
-    memory, memorypath='__memory.pkl', 'watex/etc'
-    with resources.path (DMOD, memory) as p : 
-         memory_file = str(p) # for consistency
+    MMOD = 'watex.etc'; memory='__memory.pkl'
+    with resources.path (MMOD, memory) as mfile : 
+         memory_file = str(mfile) # for consistency
          
     mkeys= ('set', 'get', 'recover', 'fetch', set)
     if option not in mkeys: 
         raise ValueError('Wrong `option` argument. Acceptable '
                          f'values are  {smart_format(mkeys[:-1])}.')
         
     if option in ('set', set): 
         if obj is None: 
-            raise TypeError('NoneType object can not be set.') 
+            raise TypeError('NoneType object cannot be set. Provide the'
+                            " model object to 'obj' parameter.") 
         psobj_token = __build_ps__token(obj)
         data = (psobj_token, list(obj.__dict__.items()))
-        serialize_data ( data, memory, savepath= memorypath )
+        serialize_data ( data, memory, savepath= os.path.dirname (memory_file))
         return 
-    
     elif option in ('get', 'recover', 'fetch'): 
-        try: 
-            memory_exists =  os.path.isfile(os.path.join(memorypath, memory))
-        except: 
-            memory_exists =  os.path.isfile(memory_file)
-            
+        memory_exists =  os.path.isfile(memory_file)
         if not memory_exists: 
-            _logger.error('No memory found. Run the GeoStrataModel class '
-                          'beforehand to create your first model.')
-
-            warnings.warn("No memory found. You need to build your "
+            _logger.error('No memory found. Run the GeoStrataModel class'
+                          ' beforehand to create your first model.')
+            warnings.warn("No memory found. You need to build your"
                           " GeoStrataModel model by running the class first.")
             raise  MemoryError("Memory not found. Run the `buildNM` method"
                                " to create your model first.")
-        try: 
-            psobj_token, data_ = load_serialized_data(
-                os.path.join(memorypath, memory))
-        except: 
-            psobj_token, data_ = load_serialized_data(memory_file )
-            
+        psobj_token, data_ = load_serialized_data(memory_file )
         data = dict(data_)
         # create PseudoStratigraphicObj from metaclass and inherits from 
         # dictattributes of GeoStrataModel class
         psobj = type ('PseudoStratigraphic', (), { 
             k:v for k, v in data.items()})
         psobj.__token = psobj_token
```

### Comparing `watex-0.2.5/watex/methods/__init__.py` & `watex-0.2.6/watex/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/methods/electrical.py` & `watex-0.2.6/watex/methods/electrical.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/methods/em.py` & `watex-0.2.6/watex/methods/em.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/methods/erp.py` & `watex-0.2.6/watex/methods/erp.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/methods/hydro.py` & `watex-0.2.6/watex/methods/hydro.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/metrics.py` & `watex-0.2.6/watex/metrics.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/models/__init__.py` & `watex-0.2.6/watex/models/__init__.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/models/_metapredictors.py` & `watex-0.2.6/watex/models/_metapredictors.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/models/premodels.py` & `watex-0.2.6/watex/models/premodels.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/models/validation.py` & `watex-0.2.6/watex/models/validation.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/property.py` & `watex-0.2.6/watex/property.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/site.py` & `watex-0.2.6/watex/site.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/transformers.py` & `watex-0.2.6/watex/transformers.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/__init__.py` & `watex-0.2.6/watex/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/_array_api.py` & `watex-0.2.6/watex/utils/_array_api.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/_arraytools.py` & `watex-0.2.6/watex/utils/_arraytools.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/_dependency.py` & `watex-0.2.6/watex/utils/_dependency.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/_openmp_helpers.pyx` & `watex-0.2.6/watex/utils/_openmp_helpers.pyx`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/_packaging_version.py` & `watex-0.2.6/watex/utils/_packaging_version.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/_set_gdal.py` & `watex-0.2.6/watex/utils/_set_gdal.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/_show_versions.py` & `watex-0.2.6/watex/utils/_show_versions.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/box.py` & `watex-0.2.6/watex/utils/box.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/coreutils.py` & `watex-0.2.6/watex/utils/coreutils.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/epsg.npy` & `watex-0.2.6/watex/utils/epsg.npy`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/exmath.py` & `watex-0.2.6/watex/utils/exmath.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/funcutils.py` & `watex-0.2.6/watex/utils/funcutils.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/geotools.py` & `watex-0.2.6/watex/utils/geotools.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/gistools.py` & `watex-0.2.6/watex/utils/gistools.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/hydroutils.py` & `watex-0.2.6/watex/utils/hydroutils.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/mlutils.py` & `watex-0.2.6/watex/utils/mlutils.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/plotutils.py` & `watex-0.2.6/watex/utils/plotutils.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/setup.py` & `watex-0.2.6/watex/utils/setup.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/thread.py` & `watex-0.2.6/watex/utils/thread.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/validator.py` & `watex-0.2.6/watex/utils/validator.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/utils/version.py` & `watex-0.2.6/watex/utils/version.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/view/__init__.py` & `watex-0.2.6/watex/view/__init__.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/view/mlplot.py` & `watex-0.2.6/watex/view/mlplot.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/view/plot.py` & `watex-0.2.6/watex/view/plot.py`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex/wlog.yml` & `watex-0.2.6/watex/wlog.yml`

 * *Files identical despite different names*

### Comparing `watex-0.2.5/watex.egg-info/PKG-INFO` & `watex-0.2.6/watex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watex
-Version: 0.2.5
+Version: 0.2.6
 Summary: Machine learning research in water exploration
 Home-page: https://github.com/WEgeophysics/watex
 Download-URL: https://pypi.org/project/watex/#files
 Author: Laurent Kouadio
 Author-email: etanoyau@gmail.com
 Maintainer: Laurent Kouadio
 Maintainer-email: etanoyau@gmail.com
```

### Comparing `watex-0.2.5/watex.egg-info/SOURCES.txt` & `watex-0.2.6/watex.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 CITATION.cff
 LICENSE
 MANIFEST.in
 README.md
+etc
 pyproject.toml
 setup.cfg
 setup.py
 .github/dependabot.yml
 .github/workflows/ci.yaml
 .github/workflows/codeql.yml
 .github/workflows/dependency-review.yml
@@ -89,14 +90,15 @@
 docs/whatsnew/v0.1.9.rst
 docs/whatsnew/v0.2.0.rst
 docs/whatsnew/v0.2.1.rst
 docs/whatsnew/v0.2.2.rst
 docs/whatsnew/v0.2.3.rst
 docs/whatsnew/v0.2.4.rst
 docs/whatsnew/v0.2.5.rst
+docs/whatsnew/v0.2.6.rst
 examples/README.txt
 examples/analysis/README.txt
 examples/analysis/plot_decision_regions.py
 examples/analysis/plot_explained_variance_ratio.py
 examples/analysis/plot_linear_discriminant_analysis.py
 examples/analysis/plot_pca_vs_factor_with_scedatic_noises.py
 examples/applications/README.txt
```

