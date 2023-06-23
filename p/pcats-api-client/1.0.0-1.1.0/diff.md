# Comparing `tmp/pcats_api_client-1.0.0.tar.gz` & `tmp/pcats_api_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcats_api_client-1.0.0.tar", last modified: Tue Aug 17 17:18:31 2021, max compression
+gzip compressed data, was "pcats_api_client-1.1.0.tar", last modified: Fri Jun 23 17:33:06 2023, max compression
```

## Comparing `pcats_api_client-1.0.0.tar` & `pcats_api_client-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 michal     (501) staff       (20)        0 2021-08-17 17:18:31.688417 pcats_api_client-1.0.0/
--rw-r--r--   0 michal     (501) staff       (20)     1086 2021-08-17 17:18:31.688300 pcats_api_client-1.0.0/PKG-INFO
--rw-r--r--   0 michal     (501) staff       (20)      841 2021-08-17 17:16:42.000000 pcats_api_client-1.0.0/README.md
-drwxr-xr-x   0 michal     (501) staff       (20)        0 2021-08-17 17:18:31.687256 pcats_api_client-1.0.0/pcats_api_client/
--rw-r--r--   0 michal     (501) staff       (20)      992 2021-08-17 02:50:01.000000 pcats_api_client-1.0.0/pcats_api_client/__init__.py
--rw-r--r--   0 michal     (501) staff       (20)    24480 2021-08-17 16:35:25.000000 pcats_api_client-1.0.0/pcats_api_client/pcats_api.py
-drwxr-xr-x   0 michal     (501) staff       (20)        0 2021-08-17 17:18:31.688160 pcats_api_client-1.0.0/pcats_api_client.egg-info/
--rw-r--r--   0 michal     (501) staff       (20)     1086 2021-08-17 17:18:31.000000 pcats_api_client-1.0.0/pcats_api_client.egg-info/PKG-INFO
--rw-r--r--   0 michal     (501) staff       (20)      276 2021-08-17 17:18:31.000000 pcats_api_client-1.0.0/pcats_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 michal     (501) staff       (20)        1 2021-08-17 17:18:31.000000 pcats_api_client-1.0.0/pcats_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 michal     (501) staff       (20)        9 2021-08-17 17:18:31.000000 pcats_api_client-1.0.0/pcats_api_client.egg-info/requires.txt
--rw-r--r--   0 michal     (501) staff       (20)       17 2021-08-17 17:18:31.000000 pcats_api_client-1.0.0/pcats_api_client.egg-info/top_level.txt
--rw-r--r--   0 michal     (501) staff       (20)       38 2021-08-17 17:18:31.688507 pcats_api_client-1.0.0/setup.cfg
--rw-r--r--   0 michal     (501) staff       (20)      611 2021-08-17 17:16:57.000000 pcats_api_client-1.0.0/setup.py
+drwxr-xr-x   0 michal     (501) staff       (20)        0 2023-06-23 17:33:06.416243 pcats_api_client-1.1.0/
+-rw-r--r--   0 michal     (501) staff       (20)     1066 2023-06-23 17:33:06.416078 pcats_api_client-1.1.0/PKG-INFO
+-rw-r--r--   0 michal     (501) staff       (20)      841 2021-08-17 17:16:42.000000 pcats_api_client-1.1.0/README.md
+drwxr-xr-x   0 michal     (501) staff       (20)        0 2023-06-23 17:33:06.415092 pcats_api_client-1.1.0/pcats_api_client/
+-rw-r--r--   0 michal     (501) staff       (20)     1036 2021-08-31 20:09:32.000000 pcats_api_client-1.1.0/pcats_api_client/__init__.py
+-rw-r--r--   0 michal     (501) staff       (20)    24354 2023-06-23 02:41:17.000000 pcats_api_client-1.1.0/pcats_api_client/pcats_api.py
+-rw-r--r--   0 michal     (501) staff       (20)     7314 2021-08-31 20:12:05.000000 pcats_api_client-1.1.0/pcats_api_client/pcats_api_staticgp2.py
+drwxr-xr-x   0 michal     (501) staff       (20)        0 2023-06-23 17:33:06.415886 pcats_api_client-1.1.0/pcats_api_client.egg-info/
+-rw-r--r--   0 michal     (501) staff       (20)     1066 2023-06-23 17:33:06.000000 pcats_api_client-1.1.0/pcats_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 michal     (501) staff       (20)      316 2023-06-23 17:33:06.000000 pcats_api_client-1.1.0/pcats_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 michal     (501) staff       (20)        1 2023-06-23 17:33:06.000000 pcats_api_client-1.1.0/pcats_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 michal     (501) staff       (20)        9 2023-06-23 17:33:06.000000 pcats_api_client-1.1.0/pcats_api_client.egg-info/requires.txt
+-rw-r--r--   0 michal     (501) staff       (20)       17 2023-06-23 17:33:06.000000 pcats_api_client-1.1.0/pcats_api_client.egg-info/top_level.txt
+-rw-r--r--   0 michal     (501) staff       (20)       38 2023-06-23 17:33:06.416293 pcats_api_client-1.1.0/setup.cfg
+-rw-r--r--   0 michal     (501) staff       (20)      661 2023-06-23 02:27:26.000000 pcats_api_client-1.1.0/setup.py
```

### Comparing `pcats_api_client-1.0.0/PKG-INFO` & `pcats_api_client-1.1.0/pcats_api_client.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
-Name: pcats_api_client
-Version: 1.0.0
+Name: pcats-api-client
+Version: 1.1.0
 Summary: PCATS REST API Client
 Home-page: https://github.com/pcats-api/pcats_api_client_py
 Author: Michal Kouril
 Author-email: michal.kouril@cchmc.org
 License: MIT
-Platform: UNKNOWN
 
 PCATS: Bayesian Causal Inference for General Type of Treatment
 
 The PCATS application programming interface (API) implements two Bayesian's non parametric causal inference modeling, Bayesian's Gaussian process regression and Bayesian additive regression tree, and provides estimates of averaged causal treatment (ATE) and conditional averaged causal treatment (CATE) for adaptive or non-adaptive treatment. The API is able to handle general types of treatment - binary, multilevel, continuous and their combinations, as well as general type of outcomes including bounded summary scores such as health related quality of life and survival outcomes. In addition, the API is able to deal with missing data using user supplied multiply imputed missing data. Summary tables and interactive figures of the results are generated and downloadable.
 
-
-
```

### Comparing `pcats_api_client-1.0.0/README.md` & `pcats_api_client-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pcats_api_client-1.0.0/pcats_api_client/__init__.py` & `pcats_api_client-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-"""
+Metadata-Version: 2.1
+Name: pcats_api_client
+Version: 1.1.0
+Summary: PCATS REST API Client
+Home-page: https://github.com/pcats-api/pcats_api_client_py
+Author: Michal Kouril
+Author-email: michal.kouril@cchmc.org
+License: MIT
+
 PCATS: Bayesian Causal Inference for General Type of Treatment
 
 The PCATS application programming interface (API) implements two Bayesian's non parametric causal inference modeling, Bayesian's Gaussian process regression and Bayesian additive regression tree, and provides estimates of averaged causal treatment (ATE) and conditional averaged causal treatment (CATE) for adaptive or non-adaptive treatment. The API is able to handle general types of treatment - binary, multilevel, continuous and their combinations, as well as general type of outcomes including bounded summary scores such as health related quality of life and survival outcomes. In addition, the API is able to deal with missing data using user supplied multiply imputed missing data. Summary tables and interactive figures of the results are generated and downloadable.
 
-"""
-
-from .pcats_api import job_status, staticgp, dynamicgp, uploadfile, wait_for_result, printgp, ploturl, staticgp_cate, dynamicgp_cate, results
```

### Comparing `pcats_api_client-1.0.0/pcats_api_client/pcats_api.py` & `pcats_api_client-1.1.0/pcats_api_client/pcats_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,20 +76,19 @@
              outcome_censor_lv=None,
              outcome_censor_uv=None,
              outcome_link="identity",
              treatment=None, 
              x_explanatory=None,
              x_confounding=None,
              tr_type="Discrete",
-             tr2_type="Discrete",             
              tr_values=None,
-             tr2_values=None,
-             pr_values=None,
+             c_margin=None,
              tr_hte=None,
-             tr2_hte=None,
+	         time=None,
+	         time_value=None,
              burn_num=500,
              mcmc_num=500,
              x_categorical=None,
              mi_datafile=None,
              mi_dataref=None,
              sheet=None,
              mi_sheet=None,
@@ -121,61 +120,60 @@
           "identity" if no transformation needed.
           "log" for log transformation.
           "logit" for logit transformation.
     treatment The vector of the name of the treatment variables. Users can input at most two treatment variables.
     x.explanatory The vector of the name of the explanatory variables.
     x.confounding The vector of the name of the confounding variables.
     tr.type The type of the first treatment. "Continuous" for continuous treatment and "Discrete" for categorical treatment. The default value is "Discrete".
-    tr2.type The type of the second treatment if available. "Continuous" for continuous treatment and "Discrete" for categorical treatment. The default value is "Discrete".
     tr.values user-defined values for the calculation of ATE if the first treatment variable is continuous
-    tr2.values user-defined values for the calculation of ATE if the second treatment variable is continuous
-    pr.values An optional vector of user-defined values of c for PrTE.
+    c.margin An optional vector of user-defined values of c for PrTE.
     tr.hte An optional vector specifying variables which may have heterogeneous treatment effect with the first treatment variable
-    tr2.hte An optional vector specifying variables which may have heterogeneous treatment effect with the second treatment variable
+    time
+    time.value
     burn.num numeric; the number of MCMC 'burn-in' samples, i.e. number of MCMC to be discarded. The default value is 500.
     mcmc.num numeric; the number of MCMC samples after 'burn-in'. The default value is 500.
     x.categorical A vector of the name of categorical variables in data.
     mi.datafile File to upload (.csv or .xls) that contains the imputed data in the model.
     mi.dataref Reference to already uploaded file that contains the imputed data in the model.
     sheet If \code{datafile} or \code{dataref} points to an Excel file this variable specifies which sheet to load.
     mi.sheet If \code{mi.datafile} or \code{mi.dataurl} points to an Excel file this variable specifies which sheet to load.
     seed Sets the seed. The default value is 5000.
     token Authentication token.
     use_cache Use cached results (default True).
 
+
     Returns
     -------
     UUID
         jobid
     """
 
     data={
         'data': (datafile, open(datafile, 'rb') if datafile!=None else None ),
         'dataref': (None, dataref),
         'outcome': (None, outcome),
         'treatment': (None, treatment),
         'x.explanatory': (None, x_explanatory),
         'x.confounding': (None, x_confounding),
         'tr.hte': (None, tr_hte),
-        'tr2.values': (None, tr2_values),
+        'time': (None, time),
+        'time.value': (None, time_value),
         'burn.num': (None, burn_num),
         'mcmc.num': (None, mcmc_num),
         'outcome.lb': (None, outcome_lb),
         'outcome.ub': (None, outcome_ub),
         'outcome.bound_censor': (None, outcome_bound_censor),
         'outcome.type': (None, outcome_type),
         'outcome.censor.lv': (None, outcome_censor_lv),
         'outcome.censor.uv': (None, outcome_censor_uv),
         'outcome.censor.yn': (None, outcome_censor_yn),
         'outcome.link': (None, outcome_link),
         'tr.type': (None, tr_type),
-        'tr2.type': (None, tr2_type),
         'tr.values': (None, tr_values),
-        'tr2.values': (None, tr2_values),
-        'pr.values': (None, pr_values),
+        'c.margin': (None, c_margin),
         'x.categorical': (None, x_categorical),
         'method': (None, method),
         'mi.data':  (mi_datafile, open(mi_datafile, 'rb')
                      if mi_datafile!=None else None ),
         'mi.dataref': (None, mi_dataref),
         'sheet': (None, sheet),
         'mi.sheet': (None, mi_sheet),
@@ -206,15 +204,15 @@
    Return formatted string with job results
 
     Parameters
     ----------
     jobid : UUID
             Job ID of the previously submitted job
     token : string
-             Authentication token.
+            Authentication token.
             
     Returns
     -------
     string
         formatted text
 
     """
@@ -234,15 +232,15 @@
     Return job results
 
     Parameters
     ----------
     jobid : UUID
             Job ID of the previously submitted job
     token : string
-             Authentication token.
+            Authentication token.
             
     Returns
     -------
     json
         results
 
     """
@@ -255,15 +253,15 @@
         '/api/job/{}/results'.format(jobid)),
         headers=headers).content.decode("utf-8") 
 
 def staticgp_cate(jobid, 
               x, 
               control_tr, 
               treat_tr, 
-              pr_values=None,
+              c_margin=None,
               token=None,
               use_cache=None,
               reuse_cached_jobid=None):
     """Get conditional average treatment effect
 
     Estimate the conditional average treatment effect of user-specified treatment groups.
 
@@ -273,35 +271,36 @@
 
     Parameters
     ----------
     jobid job id of the "staticGP".
     x The name of a categorical variable which may have the heterogeneous treatment effect.
     control.tr The value of the treatment variable as the reference group.
     treat.tr The value of the treatment variable compared to the reference group.
-    pr.values An optional vector of user-defined values of c for PrCTE.
+    c.margin An optional vector of user-defined values of c for PrCTE.
     token Authentication token.
     use_cache Use cached results (default True).
 
     Returns
     -------
     UUID
         jobid
 
     """
     data={
         'x': (None, x),
         'control.tr': (None, control_tr),
         'treat.tr': (None, treat_tr),
-        'pr.values': (None, pr_values)}
+        'c.margin': (None, c_margin)}
 
     headers=dict()
     if (str(use_cache)=="1"):
         headers["X-API-Cache"]="1"
     if (str(reuse_cached_jobid)=="1"):
         headers["X-API-Reuse-Cached-Jobid"]="1"
+
     if token is not None:
         headers["Authorization"]="Bearer {}".format(token)
 
     res=requests.post(_url(
         '/api/job/{}/staticgp.cate'.format(jobid)), files=data, headers=headers);
     return ret_jobid(res)
 
@@ -317,41 +316,45 @@
               stg1_outcome=None,
               stg1_treatment=None, 
               stg1_x_explanatory=None,
               stg1_x_confounding=None,
               stg1_tr_hte=None,
               stg1_tr_values=None,
               stg1_tr_type="Discrete",
+              stg1_time=None,
+              stg1_time_value=None,
               stg1_outcome_type="Continuous",
               stg1_outcome_bound_censor="neither",
               stg1_outcome_lb=None,
               stg1_outcome_ub=None,
               stg1_outcome_censor_lv=None,
               stg1_outcome_censor_uv=None,
               stg1_outcome_censor_yn=None,
               stg1_outcome_link="identity",
-              stg1_pr_values=None,
+              stg1_c_margin=None,
 
               stg2_outcome=None,
               stg2_treatment=None,
               stg2_x_explanatory=None,
               stg2_x_confounding=None,
               stg2_tr1_hte=None,
               stg2_tr2_hte=None,
               stg2_tr_values=None,
               stg2_tr_type="Discrete",
+              stg2_time=None,
+              stg2_time_value=None,
               stg2_outcome_type="Continuous",
               stg2_outcome_bound_censor="neither",
               stg2_outcome_lb=None,
               stg2_outcome_ub=None,
               stg2_outcome_censor_lv=None,
               stg2_outcome_censor_uv=None,
               stg2_outcome_censor_yn=None,
               stg2_outcome_link="identity",
-              stg2_pr_values=None,
+              stg2_c_margin=None,
 
               burn_num=500,
               mcmc_num=500,
               x_categorical=None,
               mi_datafile=None,
               mi_dataref=None,
               sheet=None,
@@ -370,14 +373,16 @@
     dataref Reference to already uploaded file.
     method The method to be used. "GP" for GP method and "BART" for BART method. The default value is "BART".
     stg1.outcome The name of the intermediate outcome variable for stage 1.
     stg1.treatment The name of the treatment variable for stage 1.
     stg1.x.explanatory A vector of the name of the explanatory variables for stage 1.
     stg1.x.confounding A vector of the name of the confounding variables for stage 1.
     stg1.tr.hte An optional vector specifying categorical variables which may have heterogeneous treatment effect with the treatment variable for stage 1.
+    stg1.time
+    stg1.time.value
     stg1.outcome.bound_censor The default value is "neither".
         "neither" if the intermediate outcome is not bounded or censored.
         "bounded" if the intermediate outcome is bounded.
         "censored" if the intermediate outcome is censored.
     stg1.outcome.lb Stage 1 lower bound if the intermediate outcome is bounded.
     stg1.outcome.ub Stage 1 upper bound if the intermediate outcome is bounded.
     stg1.outcome.type Intermediate outcome type ("Continuous" or "Discrete") for stage 1.
@@ -386,21 +391,23 @@
     stg1.outcome.censor.uv upper variable of censored interval if the intermediate outcome is censored.
     stg1.outcome.link function for the intermediate outcome; the default value is ``identity''.
         "identity" if no transformation needed.
         "log" for log transformation.
         "logit" for logit transformation.
     stg1.tr.values User-defined values for the calculation of ATE if the treatment variable is continuous for stage 1.
     stg1.tr.type The type of treatment at stage 1. "Continuous" for continuous treatment and "Discrete" for categorical treatment. The default value is "Discrete".
-    stg1.pr.values An optional vector of user-defined values of c for PrTE at stage 1.
+    stg1.c.margin An optional vector of user-defined values of c for PrTE at stage 1.
     stg2.outcome The name of the outcome variable for stage 2.
     stg2.treatment The name of the treatment variable for stage 2.
     stg2.x.explanatory A vector of the name of the explanatory variables for stage 2.
     stg2.x.confounding A vector of the name of the confounding variables for stage 2.
     stg2.tr1.hte At stage 2, an optional vector specifying cate-gorical variables which may have heterogeneoustreatment effect with the stage 1 treatment variable
     stg2.tr2.hte At stage 2, an optional vector specifying cate-gorical variables which may have heterogeneoustreatment effect with the stage 2 treatment variable
+    stg2.time
+    stg2.time.value
     stg2.outcome.bound_censor The default value is "neither".
         "neither" if the intermediate outcome is not bounded or censored.
         "bounded" if the intermediate outcome is bounded.
         "censored" if the intermediate outcome is censored.
     stg2.outcome.lb Stage 2 lower bound if the outcome is bounded.
     stg2.outcome.ub Stage 2 upper bound if the outcome is bounded.
     stg2.outcome.type Outcome type ("Continuous" or "Discrete") for stage 2.
@@ -409,15 +416,15 @@
     stg2.outcome.censor.uv upper variable of censored interval if the outcome is censored.
     stg2.outcome.link function for the outcome; the default value is ``identity''.
         "identity" if no transformation needed.
         "log" for log transformation.
         "logit" for logit transformation.
     stg2.tr.values User-defined values for the calculation of ATE if the treatment variable is continuous for stage 2.
     stg2.tr.type The type of treatment at stage 2. "Continuous" for continuous treatment and "Discrete" for categorical treatment. The default value is "Discrete".
-    stg2.pr.values An optional vector of user-defined values of c for PrTE at stage 2.
+    stg2.c.margin An optional vector of user-defined values of c for PrTE at stage 2.
     burn.num numeric; the number of MCMC 'burn-in' samples, i.e. number of MCMC to be discarded. The default value is 500.
     mcmc.num numeric; the number of MCMC samples after 'burn-in'. The default value is 500.
     x.categorical A vector of the name of categorical variables in data.
     mi.datafile File to upload (.csv or .xls) that contains the imputed data in the model.
     mi.dataref Reference to already uploaded file that contains the imputed data in the model.
     sheet If \code{datafile} or \code{dataref} points to an Excel file this variable specifies which sheet to load.
     mi.sheet If \code{mi.datafile} or \code{mi.dataurl} points to an Excel file this variable specifies which sheet to load.
@@ -438,40 +445,44 @@
         'stg1.outcome': (None, stg1_outcome),
         'stg1.treatment': (None, stg1_treatment),
         'stg1.x.explanatory': (None, stg1_x_explanatory),
         'stg1.x.confounding': (None, stg1_x_confounding),
         'stg1.tr.hte': (None, stg1_tr_hte),
         'stg1.tr.values': (None, stg1_tr_values),
         'stg1.tr.type': (None, stg1_tr_type),
+        'stg1.time': (None, stg1_time),
+        'stg1.time.value': (None, stg1_time_value),
         'stg1.outcome.type': (None, stg1_outcome_type),
         'stg1.outcome.bound_censor': (None, stg1_outcome_bound_censor),
         'stg1.outcome.lb': (None, stg1_outcome_lb),
         'stg1.outcome.ub': (None, stg1_outcome_ub),
         'stg1.outcome.censor.lv': (None, stg1_outcome_censor_lv),
         'stg1.outcome.censor.uv': (None, stg1_outcome_censor_uv),
         'stg1.outcome.censor.yn': (None, stg1_outcome_censor_yn),
         'stg1.outcome.link': (None, stg1_outcome_link),
-        'stg1.pr.values': (None, stg1_pr_values),
+        'stg1.c.margin': (None, stg1_c_margin),
         'stg2.outcome': (None, stg2_outcome),
         'stg2.treatment': (None, stg2_treatment),
         'stg2.x.explanatory': (None, stg2_x_explanatory),
         'stg2.x.confounding': (None, stg2_x_confounding),
         'stg2.tr1.hte': (None, stg2_tr1_hte),
         'stg2.tr2.hte': (None, stg2_tr2_hte),
         'stg2.tr.values': (None, stg2_tr_values),
         'stg2.tr.type': (None, stg2_tr_type),
+        'stg2.time': (None, stg2_time),
+        'stg2.time.value': (None, stg2_time_value),
         'stg2.outcome.type': (None, stg2_outcome_type),
         'stg2.outcome.bound_censor': (None, stg2_outcome_bound_censor),
         'stg2.outcome.lb': (None, stg2_outcome_lb),
         'stg2.outcome.ub': (None, stg2_outcome_ub),
         'stg2.outcome.censor.lv': (None, stg2_outcome_censor_lv),
         'stg2.outcome.censor.uv': (None, stg2_outcome_censor_uv),
         'stg2.outcome.censor.yn': (None, stg2_outcome_censor_yn),
         'stg2.outcome.link': (None, stg2_outcome_link),
-        'stg2.pr.values': (None, stg2_pr_values),
+        'stg2.c.margin': (None, stg2_c_margin),
         'burn.num': (None, burn_num),
         'mcmc.num': (None, mcmc_num),
         'x.categorical': (None, x_categorical),
         'method': (None, method),
         'mi.data':  (mi_datafile, open(mi_datafile, 'rb') if mi_datafile!=None else None ),
         'mi.dataref': (None, mi_dataref),
         'sheet': (None, sheet),
@@ -485,26 +496,25 @@
     elif (str(use_cache)=="0"):
         headers["X-API-Cache"]="0"
 
     if (str(reuse_cached_jobid)=="1"):
         headers["X-API-Reuse-Cached-Jobid"]="1"
     elif (str(reuse_cached_jobid)=="0"):
         headers["X-API-Reuse-Cached-Jobid"]="0"
-
     if token is not None:
         headers["Authorization"]="Bearer {}".format(token)
 
     res=requests.post(_url('/api/dynamicgp'), files=data, headers=headers);
     return ret_jobid(res)
 
 def dynamicgp_cate(jobid, 
               x, 
               control_tr, 
               treat_tr, 
-              pr_values=None,
+              c_margin=None,
               token=None,
               use_cache=None,
               reuse_cached_jobid=None):
     """Get conditional average treatment effect for data with two time points.
 
     Estimate the conditional average treatment effect of user-specified treatment groups.
 
@@ -514,45 +524,44 @@
 
     Parameters
     ----------
     jobid job id of the "dynamicGP".
     x The name of variable which may have the heterogeneous treatment effect. x should be a categorical variable.
     control.tr A vector of the values of the treatment variables at all stages as the reference group.
     treat.tr A vector of the values of the treatment variables at all stages compared to the reference group.
-    pr.values An optional vector of user-defined values of c for PrCTE.
+    c.margin An optional vector of user-defined values of c for PrCTE.
     token Authentication token.
     use_cache Use cached results (default True).
 
     Returns
     -------
     UUID
         jobid
 
     """
     data={
         'x': (None, x),
         'control.tr': (None, control_tr),
         'treat.tr': (None, treat_tr),
-        'pr.values': (None, pr_values)}
+        'c.margin': (None, c_margin)}
 
     headers=dict()
     if (str(use_cache)=="1"):
         headers["X-API-Cache"]="1"
     if (str(reuse_cached_jobid)=="1"):
         headers["X-API-Reuse-Cached-Jobid"]="1"
-
     if token is not None:
         headers["Authorization"]="Bearer {}".format(token)
 
     res=requests.post(_url(
         '/api/job/{}/dynamicgp.cate'.format(jobid)), files=data, headers=headers);
     return ret_jobid(res)
 
 def uploadfile(datafile,
-               token=NULL):
+               token=None):
     """Upload a file
 
     Upload a file
 
     Parameters
     ----------
     filename Filename of a file to upload
```

### Comparing `pcats_api_client-1.0.0/pcats_api_client.egg-info/PKG-INFO` & `pcats_api_client-1.1.0/pcats_api_client/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,10 @@
-Metadata-Version: 2.1
-Name: pcats-api-client
-Version: 1.0.0
-Summary: PCATS REST API Client
-Home-page: https://github.com/pcats-api/pcats_api_client_py
-Author: Michal Kouril
-Author-email: michal.kouril@cchmc.org
-License: MIT
-Platform: UNKNOWN
-
+"""
 PCATS: Bayesian Causal Inference for General Type of Treatment
 
 The PCATS application programming interface (API) implements two Bayesian's non parametric causal inference modeling, Bayesian's Gaussian process regression and Bayesian additive regression tree, and provides estimates of averaged causal treatment (ATE) and conditional averaged causal treatment (CATE) for adaptive or non-adaptive treatment. The API is able to handle general types of treatment - binary, multilevel, continuous and their combinations, as well as general type of outcomes including bounded summary scores such as health related quality of life and survival outcomes. In addition, the API is able to deal with missing data using user supplied multiply imputed missing data. Summary tables and interactive figures of the results are generated and downloadable.
 
+"""
 
+from .pcats_api import job_status, staticgp, dynamicgp, uploadfile, wait_for_result, printgp, ploturl, staticgp_cate, dynamicgp_cate, results
 
+from .pcats_api_staticgp2 import staticgp2
```

### Comparing `pcats_api_client-1.0.0/setup.py` & `pcats_api_client-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,16 @@
     url='https://github.com/pcats-api/pcats_api_client_py',
     author='Michal Kouril',
     author_email='michal.kouril@cchmc.org',
     packages=['pcats_api_client'],
     # Needed for dependencies
     install_requires=['requests'],
     # *strongly* suggested for sharing
-    version='1.0.0',
+    version='1.1.0',
     # The license can be anything you like
     license='MIT',
     description='PCATS REST API Client',
     # We will also need a readme eventually (there will be a warning)
+    # long_description=open('README.txt').read(),
     long_description=open('README.md').read(),
     include_package_data=True,
 )
```

