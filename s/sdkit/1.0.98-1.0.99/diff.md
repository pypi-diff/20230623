# Comparing `tmp/sdkit-1.0.98.tar.gz` & `tmp/sdkit-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkit-1.0.98.tar", last modified: Thu May 25 10:04:23 2023, max compression
+gzip compressed data, was "sdkit-1.0.99.tar", last modified: Tue May 30 11:18:06 2023, max compression
```

## Comparing `sdkit-1.0.98.tar` & `sdkit-1.0.99.tar`

### file list

```diff
@@ -1,82 +1,88 @@
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:23.779315 sdkit-1.0.98/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4121 2022-12-23 10:54:05.000000 sdkit-1.0.98/LICENSE
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       84 2023-02-06 11:28:37.000000 sdkit-1.0.98/MANIFEST.in
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-25 10:04:23.779315 sdkit-1.0.98/PKG-INFO
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9349 2023-04-10 11:16:32.000000 sdkit-1.0.98/README.md
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1441 2023-05-25 10:03:47.000000 sdkit-1.0.98/pyproject.toml
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:21.221645 sdkit-1.0.98/sdkit/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3719 2023-05-19 11:22:44.000000 sdkit-1.0.98/sdkit/__init__.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:21.497653 sdkit-1.0.98/sdkit/filter/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       41 2023-04-29 09:00:56.000000 sdkit-1.0.98/sdkit/filter/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1197 2023-05-19 11:22:44.000000 sdkit-1.0.98/sdkit/filter/apply_filters.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      998 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/filter/gfpgan.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      870 2023-05-22 11:11:30.000000 sdkit-1.0.98/sdkit/filter/latent_upscaler.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      614 2023-04-28 10:50:58.000000 sdkit-1.0.98/sdkit/filter/nsfw_checker.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      378 2023-04-10 12:49:03.000000 sdkit-1.0.98/sdkit/filter/realesrgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:21.585014 sdkit-1.0.98/sdkit/generate/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       45 2023-04-29 09:01:13.000000 sdkit-1.0.98/sdkit/generate/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11798 2023-05-25 10:03:04.000000 sdkit-1.0.98/sdkit/generate/image_generator.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2479 2023-02-17 07:20:50.000000 sdkit-1.0.98/sdkit/generate/prompt_parser.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:21.819646 sdkit-1.0.98/sdkit/generate/sampler/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:07.000000 sdkit-1.0.98/sdkit/generate/sampler/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3168 2023-04-10 11:16:32.000000 sdkit-1.0.98/sdkit/generate/sampler/default_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3396 2023-05-19 11:28:03.000000 sdkit-1.0.98/sdkit/generate/sampler/diffusers_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2589 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/generate/sampler/k_samplers.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2132 2023-02-16 16:27:22.000000 sdkit-1.0.98/sdkit/generate/sampler/sampler_main.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:21.985572 sdkit-1.0.98/sdkit/generate/sampler/unipc_samplers/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2737 2023-04-28 10:50:59.000000 sdkit-1.0.98/sdkit/generate/sampler/unipc_samplers/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    40444 2023-04-29 08:59:42.000000 sdkit-1.0.98/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:22.116434 sdkit-1.0.98/sdkit/models/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      258 2023-04-29 09:01:22.000000 sdkit-1.0.98/sdkit/models/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     5475 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/models/model_downloader.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:22.446139 sdkit-1.0.98/sdkit/models/model_loader/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1747 2023-05-19 11:22:44.000000 sdkit-1.0.98/sdkit/models/model_loader/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      609 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/models/model_loader/gfpgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:22.536377 sdkit-1.0.98/sdkit/models/model_loader/hypernetwork/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2337 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/models/model_loader/hypernetwork/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4414 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/models/model_loader/hypernetwork/hypernetwork.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      686 2023-05-22 10:50:46.000000 sdkit-1.0.98/sdkit/models/model_loader/latent_upscaler.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3945 2023-05-24 10:30:04.000000 sdkit-1.0.98/sdkit/models/model_loader/lora.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      513 2023-02-18 08:34:10.000000 sdkit-1.0.98/sdkit/models/model_loader/nsfw_checker.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1117 2023-04-20 10:42:08.000000 sdkit-1.0.98/sdkit/models/model_loader/realesrgan.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:22.680603 sdkit-1.0.98/sdkit/models/model_loader/stable_diffusion/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11522 2023-05-24 10:12:27.000000 sdkit-1.0.98/sdkit/models/model_loader/stable_diffusion/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    62271 2023-04-29 08:58:14.000000 sdkit-1.0.98/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    13171 2023-05-19 13:05:06.000000 sdkit-1.0.98/sdkit/models/model_loader/stable_diffusion/optimizations.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2501 2023-04-10 11:16:32.000000 sdkit-1.0.98/sdkit/models/model_loader/vae.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:22.894082 sdkit-1.0.98/sdkit/models/models_db/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1174 2023-04-28 10:50:59.000000 sdkit-1.0.98/sdkit/models/models_db/__init__.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:23.466527 sdkit-1.0.98/sdkit/models/models_db/configs/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1873 2022-12-25 10:25:54.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v1-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1991 2022-12-25 10:26:03.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v1-inpainting-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1815 2022-12-25 10:26:48.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v2-inference-v.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1789 2022-12-25 10:26:58.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v2-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4450 2022-12-25 10:26:26.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v2-inpainting-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1869 2022-12-25 10:26:35.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v2-midas-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1847 2023-04-17 10:06:16.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v2.1-inference-v.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1821 2023-04-17 10:06:49.000000 sdkit-1.0.98/sdkit/models/models_db/configs/v2.1-inference.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2251 2022-12-25 10:26:13.000000 sdkit-1.0.98/sdkit/models/models_db/configs/x4-upscaling.yaml
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      720 2023-04-22 10:11:26.000000 sdkit-1.0.98/sdkit/models/models_db/gfpgan.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      534 2022-12-26 07:39:49.000000 sdkit-1.0.98/sdkit/models/models_db/realesrgan.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10084 2023-02-06 10:52:19.000000 sdkit-1.0.98/sdkit/models/models_db/stable_diffusion.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      308 2023-04-19 09:15:54.000000 sdkit-1.0.98/sdkit/models/models_db/vae.json
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      206 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/models/scan_models.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:23.533247 sdkit-1.0.98/sdkit/train/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:28.000000 sdkit-1.0.98/sdkit/train/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2581 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/train/merge_models.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:23.750604 sdkit-1.0.98/sdkit/utils/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      984 2023-05-19 11:17:19.000000 sdkit-1.0.98/sdkit/utils/__init__.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4005 2023-04-28 10:35:29.000000 sdkit-1.0.98/sdkit/utils/file_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2189 2023-04-28 10:35:29.000000 sdkit-1.0.98/sdkit/utils/hash_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1113 2023-02-16 16:25:27.000000 sdkit-1.0.98/sdkit/utils/http_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2252 2023-05-19 11:18:10.000000 sdkit-1.0.98/sdkit/utils/image_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3962 2023-04-28 10:51:01.000000 sdkit-1.0.98/sdkit/utils/latent_utils.py
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     6889 2023-05-08 11:11:42.000000 sdkit-1.0.98/sdkit/utils/memory_utils.py
-drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-25 10:04:21.327643 sdkit-1.0.98/sdkit.egg-info/
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10532 2023-05-25 10:04:20.000000 sdkit-1.0.98/sdkit.egg-info/PKG-INFO
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2317 2023-05-25 10:04:21.000000 sdkit-1.0.98/sdkit.egg-info/SOURCES.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        1 2023-05-25 10:04:20.000000 sdkit-1.0.98/sdkit.egg-info/dependency_links.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      150 2023-05-25 10:04:20.000000 sdkit-1.0.98/sdkit.egg-info/requires.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        6 2023-05-25 10:04:20.000000 sdkit-1.0.98/sdkit.egg-info/top_level.txt
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       38 2023-05-25 10:04:23.779315 sdkit-1.0.98/setup.cfg
--rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      397 2023-05-19 11:22:44.000000 sdkit-1.0.98/setup.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:06.508744 sdkit-1.0.99/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4121 2022-12-23 10:54:05.000000 sdkit-1.0.99/LICENSE
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       84 2023-02-06 11:28:37.000000 sdkit-1.0.99/MANIFEST.in
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10633 2023-05-30 11:18:06.505742 sdkit-1.0.99/PKG-INFO
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     9450 2023-05-30 11:14:29.000000 sdkit-1.0.99/README.md
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1441 2023-05-30 11:17:34.000000 sdkit-1.0.99/pyproject.toml
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:04.162822 sdkit-1.0.99/sdkit/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3719 2023-05-19 11:22:44.000000 sdkit-1.0.99/sdkit/__init__.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:04.479991 sdkit-1.0.99/sdkit/filter/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       41 2023-04-29 09:00:56.000000 sdkit-1.0.99/sdkit/filter/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1239 2023-05-25 10:22:13.000000 sdkit-1.0.99/sdkit/filter/apply_filters.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3147 2023-05-30 11:08:26.000000 sdkit-1.0.99/sdkit/filter/codeformer.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      998 2023-02-16 16:25:27.000000 sdkit-1.0.99/sdkit/filter/gfpgan.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      870 2023-05-22 11:11:30.000000 sdkit-1.0.99/sdkit/filter/latent_upscaler.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      614 2023-04-28 10:50:58.000000 sdkit-1.0.99/sdkit/filter/nsfw_checker.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      378 2023-04-10 12:49:03.000000 sdkit-1.0.99/sdkit/filter/realesrgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:04.571992 sdkit-1.0.99/sdkit/generate/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       45 2023-04-29 09:01:13.000000 sdkit-1.0.99/sdkit/generate/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11798 2023-05-25 10:03:04.000000 sdkit-1.0.99/sdkit/generate/image_generator.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2479 2023-02-17 07:20:50.000000 sdkit-1.0.99/sdkit/generate/prompt_parser.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:04.747005 sdkit-1.0.99/sdkit/generate/sampler/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:07.000000 sdkit-1.0.99/sdkit/generate/sampler/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3168 2023-04-10 11:16:32.000000 sdkit-1.0.99/sdkit/generate/sampler/default_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3396 2023-05-19 11:28:03.000000 sdkit-1.0.99/sdkit/generate/sampler/diffusers_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2589 2023-02-16 16:25:27.000000 sdkit-1.0.99/sdkit/generate/sampler/k_samplers.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2132 2023-02-16 16:27:22.000000 sdkit-1.0.99/sdkit/generate/sampler/sampler_main.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:04.831093 sdkit-1.0.99/sdkit/generate/sampler/unipc_samplers/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2737 2023-04-28 10:50:59.000000 sdkit-1.0.99/sdkit/generate/sampler/unipc_samplers/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    40444 2023-04-29 08:59:42.000000 sdkit-1.0.99/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:04.927728 sdkit-1.0.99/sdkit/models/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      258 2023-04-29 09:01:22.000000 sdkit-1.0.99/sdkit/models/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     5475 2023-02-16 16:25:27.000000 sdkit-1.0.99/sdkit/models/model_downloader.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:05.179039 sdkit-1.0.99/sdkit/models/model_loader/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1794 2023-05-30 11:07:27.000000 sdkit-1.0.99/sdkit/models/model_loader/__init__.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:05.312065 sdkit-1.0.99/sdkit/models/model_loader/codeformer/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      560 2023-05-30 11:07:00.000000 sdkit-1.0.99/sdkit/models/model_loader/codeformer/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11004 2023-05-30 11:06:45.000000 sdkit-1.0.99/sdkit/models/model_loader/codeformer/codeformer_arch.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    15271 2023-05-30 11:06:54.000000 sdkit-1.0.99/sdkit/models/model_loader/codeformer/vqgan_arch.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      609 2023-02-16 16:25:27.000000 sdkit-1.0.99/sdkit/models/model_loader/gfpgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:05.399331 sdkit-1.0.99/sdkit/models/model_loader/hypernetwork/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2337 2023-02-16 16:25:27.000000 sdkit-1.0.99/sdkit/models/model_loader/hypernetwork/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4414 2023-02-16 16:25:27.000000 sdkit-1.0.99/sdkit/models/model_loader/hypernetwork/hypernetwork.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      686 2023-05-22 10:50:46.000000 sdkit-1.0.99/sdkit/models/model_loader/latent_upscaler.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3945 2023-05-24 10:30:04.000000 sdkit-1.0.99/sdkit/models/model_loader/lora.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      513 2023-02-18 08:34:10.000000 sdkit-1.0.99/sdkit/models/model_loader/nsfw_checker.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1117 2023-04-20 10:42:08.000000 sdkit-1.0.99/sdkit/models/model_loader/realesrgan.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:05.512635 sdkit-1.0.99/sdkit/models/model_loader/stable_diffusion/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    11522 2023-05-29 11:26:27.000000 sdkit-1.0.99/sdkit/models/model_loader/stable_diffusion/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    62271 2023-04-29 08:58:14.000000 sdkit-1.0.99/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    13171 2023-05-19 13:05:06.000000 sdkit-1.0.99/sdkit/models/model_loader/stable_diffusion/optimizations.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2501 2023-04-10 11:16:32.000000 sdkit-1.0.99/sdkit/models/model_loader/vae.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:05.755423 sdkit-1.0.99/sdkit/models/models_db/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1263 2023-05-29 11:06:57.000000 sdkit-1.0.99/sdkit/models/models_db/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      256 2023-05-29 11:06:44.000000 sdkit-1.0.99/sdkit/models/models_db/codeformer.json
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:06.177743 sdkit-1.0.99/sdkit/models/models_db/configs/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1873 2022-12-25 10:25:54.000000 sdkit-1.0.99/sdkit/models/models_db/configs/v1-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1991 2022-12-25 10:26:03.000000 sdkit-1.0.99/sdkit/models/models_db/configs/v1-inpainting-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1815 2022-12-25 10:26:48.000000 sdkit-1.0.99/sdkit/models/models_db/configs/v2-inference-v.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1789 2022-12-25 10:26:58.000000 sdkit-1.0.99/sdkit/models/models_db/configs/v2-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4450 2022-12-25 10:26:26.000000 sdkit-1.0.99/sdkit/models/models_db/configs/v2-inpainting-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1869 2022-12-25 10:26:35.000000 sdkit-1.0.99/sdkit/models/models_db/configs/v2-midas-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1847 2023-04-17 10:06:16.000000 sdkit-1.0.99/sdkit/models/models_db/configs/v2.1-inference-v.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1821 2023-04-17 10:06:49.000000 sdkit-1.0.99/sdkit/models/models_db/configs/v2.1-inference.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2251 2022-12-25 10:26:13.000000 sdkit-1.0.99/sdkit/models/models_db/configs/x4-upscaling.yaml
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      720 2023-04-22 10:11:26.000000 sdkit-1.0.99/sdkit/models/models_db/gfpgan.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      534 2023-05-29 11:07:36.000000 sdkit-1.0.99/sdkit/models/models_db/realesrgan.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10084 2023-02-06 10:52:19.000000 sdkit-1.0.99/sdkit/models/models_db/stable_diffusion.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      308 2023-04-19 09:15:54.000000 sdkit-1.0.99/sdkit/models/models_db/vae.json
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      206 2023-02-16 16:25:27.000000 sdkit-1.0.99/sdkit/models/scan_models.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:06.239750 sdkit-1.0.99/sdkit/train/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       39 2023-04-29 09:01:28.000000 sdkit-1.0.99/sdkit/train/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2581 2023-02-16 16:25:27.000000 sdkit-1.0.99/sdkit/train/merge_models.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:06.473741 sdkit-1.0.99/sdkit/utils/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      984 2023-05-19 11:17:19.000000 sdkit-1.0.99/sdkit/utils/__init__.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     4005 2023-04-28 10:35:29.000000 sdkit-1.0.99/sdkit/utils/file_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2189 2023-04-28 10:35:29.000000 sdkit-1.0.99/sdkit/utils/hash_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     1113 2023-02-16 16:25:27.000000 sdkit-1.0.99/sdkit/utils/http_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2252 2023-05-19 11:18:10.000000 sdkit-1.0.99/sdkit/utils/image_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     3962 2023-04-28 10:51:01.000000 sdkit-1.0.99/sdkit/utils/latent_utils.py
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     6889 2023-05-08 11:11:42.000000 sdkit-1.0.99/sdkit/utils/memory_utils.py
+drwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        0 2023-05-30 11:18:04.276633 sdkit-1.0.99/sdkit.egg-info/
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)    10633 2023-05-30 11:18:03.000000 sdkit-1.0.99/sdkit.egg-info/PKG-INFO
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)     2539 2023-05-30 11:18:03.000000 sdkit-1.0.99/sdkit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        1 2023-05-30 11:18:03.000000 sdkit-1.0.99/sdkit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      150 2023-05-30 11:18:03.000000 sdkit-1.0.99/sdkit.egg-info/requires.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)        6 2023-05-30 11:18:03.000000 sdkit-1.0.99/sdkit.egg-info/top_level.txt
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)       38 2023-05-30 11:18:06.510743 sdkit-1.0.99/setup.cfg
+-rwxrwxrwx   0 sshekhar  (1000) sshekhar  (1000)      397 2023-05-19 11:22:44.000000 sdkit-1.0.99/setup.py
```

### Comparing `sdkit-1.0.98/LICENSE` & `sdkit-1.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/PKG-INFO` & `sdkit-1.0.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkit
-Version: 1.0.98
+Version: 1.0.99
 Summary: sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like GFPGAN, RealESRGAN, k-samplers, custom VAE, hypernetworks etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc. Supports Stable Diffusion 2.1!
 Author-email: cmdr2 <secondary.cmdr2@gmail.com>
 Project-URL: Homepage, https://github.com/easydiffusion/sdkit
 Project-URL: Bug Tracker, https://github.com/easydiffusion/sdkit/issues
 Keywords: stable diffusion,ai,art
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,15 +24,15 @@
 *New: Stable Diffusion 2.1 is now supported!*
 
 This is a community project, so please feel free to contribute (and use in your project)!
 
 ![t2i](https://raw.githubusercontent.com/Stability-AI/stablediffusion/main/assets/stable-samples/txt2img/768/merged-0006.png)
 
 # Why?
-The goal is to let you be productive quickly (at your AI art project), so it bundles Stable Diffusion along with commonly-used features (like GFPGAN for face restoration, RealESRGAN for upscaling, k-samplers, support for loading custom VAEs and hypernetworks, NSFW filter etc).
+The goal is to let you be productive quickly (at your AI art project), so it bundles Stable Diffusion along with commonly-used features (like GFPGAN and CodeFormer for face restoration, RealESRGAN for upscaling, k-samplers, support for loading custom VAEs and hypernetworks, NSFW filter etc).
 
 Advanced features include a model-downloader (with a database of commonly used models), support for running in parallel on multiple GPUs, auto-scanning for malicious models etc. [Full list of features](https://github.com/easydiffusion/sdkit/wiki/Features)
 
 # Installation
 Tested with Python 3.8. Supports Windows, Linux and Mac.
 
 **Windows/Linux:**
@@ -110,17 +110,17 @@
 
 For models that don't match a known hash (e.g. custom models), or if you want to override the config file, you can set the path to the config file in `context.model_paths`. e.g. `context.model_paths['stable-diffusion'] = 'path/to/config.yaml'`
 
 # FAQ
 ## Does it have all the cool features?
 It has a lot of features! It was born out of a popular Stable Diffusion UI, splitting out the battle-tested core engine into `sdkit`.
 
-**Features include:** SD 2.1, txt2img, img2img, inpainting, NSFW filter, multiple GPU support, Mac Support, gfpgan (fix faces), realesrgan (upscale), 19 samplers (including k-samplers and UniPC), custom VAE, custom hypernetworks, low-memory optimizations, model merging, safetensor support, picklescan, etc. [Click here to see the full list of features](https://github.com/easydiffusion/sdkit/wiki/Features).
+**Features include:** SD 2.1, txt2img, img2img, inpainting, NSFW filter, multiple GPU support, Mac Support, GFPGAN and CodeFormer (fix faces), RealESRGAN (upscale), 19 samplers (including k-samplers and UniPC), custom VAE, custom hypernetworks, low-memory optimizations, model merging, safetensor support, picklescan, etc. [Click here to see the full list of features](https://github.com/easydiffusion/sdkit/wiki/Features).
 
-📢 We're looking to add support for *textual inversion embeddings*, *codeformer*, *seamless tiling*, and *outpainting*. We'd love code contributions for these!
+📢 We're looking to add support for *textual inversion embeddings*, *AMD support*, *ControlNet*, *Pix2Pix*, and *outpainting*. We'd love code contributions for these!
 
 ## Is it fast?
 It is pretty fast, and close to the fastest. For the same image, `sdkit` took 5.5 seconds, while `automatic1111` webui took 4.95 seconds. 📢 We're looking for code contributions to make `sdkit` even faster!
 
 `xformers` is supported experimentally, which will make `sdkit` even faster.
 
 **Details of the benchmark:**
@@ -131,24 +131,24 @@
 
 | | Time taken | Iterations/sec | Peak VRAM usage |
 | --- | --- | --- | --- |
 | `sdkit` | 5.5 sec | 6.0 it/s | 5.1 GB |
 | `automatic1111` webui | 4.95 sec | 6.15 it/s | 5.1 GB |
 
 ## Does it work on lower-end GPUs, or without GPUs?
-Yes. It works on NVIDIA/Mac GPUs with atleast 3GB of VRAM. For PCs without a compatible GPU, it can run entirely on the CPU. Running on the CPU will be *very* slow, but atleast you'll be able to try it out!
+Yes. It works on NVIDIA/Mac GPUs with atleast 2GB of VRAM. For PCs without a compatible GPU, it can run entirely on the CPU. Running on the CPU will be *very* slow, but atleast you'll be able to try it out!
 
 📢 We don't support AMD yet (it'll run in CPU-mode), but we're looking for code contributions for AMD support!
 
 ## Why not just use diffusers?
 You can certainly use diffusers. `sdkit` is infact using `diffusers` internally (currently in beta), so you can think of `sdkit` as a convenient API and a collection of tools, focused on Stable Diffusion projects.
 
 `sdkit`:
 1. is a simple, lightweight toolkit for Stable Diffusion projects.
-2. natively includes frequently-used projects like GFPGAN and RealESRGAN.
+2. natively includes frequently-used projects like GFPGAN, CodeFormer and RealESRGAN.
 3. works with the popular `.ckpt` and `.safetensors` model format.
 4. includes memory optimizations for low-end GPUs.
 5. built-in support for running on multiple GPUs.
 6. can download models from any server.
 7. auto-scans for malicious models.
 8. includes 19 samplers (including k-samplers).
 9. born out of the needs of the new Stable Diffusion AI Art scene, starting Aug 2022.
@@ -159,24 +159,25 @@
 
 If your project is using sdkit, you can add it to this list. Please feel free to open a pull request (or let us know at our [Discord community](https://discord.com/invite/u9yhsFmEkB)).
 
 # Contributing
 We'd love to accept code contributions. Please feel free to drop by our [Discord community](https://discord.com/invite/u9yhsFmEkB)!
 
 📢 We're looking for code contributions for these features (or anything else you'd like to work on):
-- CodeFormer upscaling (please maintain the required copyright notices).
 - Using custom Textual Inversion embeddings.
-- Seamless tiling.
 - Outpainting.
+- ControlNet.
+- Pix2Pix.
 - AMD support.
 
 If you'd like to set up a developer version on your PC (to contribute code changes), please follow [these instructions](https://github.com/easydiffusion/sdkit/blob/main/CONTRIBUTING.md).
 
 # Credits
 * Stable Diffusion: https://github.com/Stability-AI/stablediffusion
+* CodeFormer: https://github.com/sczhou/CodeFormer (license: https://github.com/sczhou/CodeFormer/blob/master/LICENSE)
 * GFPGAN: https://github.com/TencentARC/GFPGAN
 * RealESRGAN: https://github.com/xinntao/Real-ESRGAN
 * k-diffusion: https://github.com/crowsonkb/k-diffusion
 * Code contributors and artists on the cmdr2 UI: https://github.com/cmdr2/stable-diffusion-ui and Discord (https://discord.com/invite/u9yhsFmEkB)
 * Lots of contributors on the internet
 
 # Disclaimer
```

### Comparing `sdkit-1.0.98/README.md` & `sdkit-1.0.99/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 *New: Stable Diffusion 2.1 is now supported!*
 
 This is a community project, so please feel free to contribute (and use in your project)!
 
 ![t2i](https://raw.githubusercontent.com/Stability-AI/stablediffusion/main/assets/stable-samples/txt2img/768/merged-0006.png)
 
 # Why?
-The goal is to let you be productive quickly (at your AI art project), so it bundles Stable Diffusion along with commonly-used features (like GFPGAN for face restoration, RealESRGAN for upscaling, k-samplers, support for loading custom VAEs and hypernetworks, NSFW filter etc).
+The goal is to let you be productive quickly (at your AI art project), so it bundles Stable Diffusion along with commonly-used features (like GFPGAN and CodeFormer for face restoration, RealESRGAN for upscaling, k-samplers, support for loading custom VAEs and hypernetworks, NSFW filter etc).
 
 Advanced features include a model-downloader (with a database of commonly used models), support for running in parallel on multiple GPUs, auto-scanning for malicious models etc. [Full list of features](https://github.com/easydiffusion/sdkit/wiki/Features)
 
 # Installation
 Tested with Python 3.8. Supports Windows, Linux and Mac.
 
 **Windows/Linux:**
@@ -92,17 +92,17 @@
 
 For models that don't match a known hash (e.g. custom models), or if you want to override the config file, you can set the path to the config file in `context.model_paths`. e.g. `context.model_paths['stable-diffusion'] = 'path/to/config.yaml'`
 
 # FAQ
 ## Does it have all the cool features?
 It has a lot of features! It was born out of a popular Stable Diffusion UI, splitting out the battle-tested core engine into `sdkit`.
 
-**Features include:** SD 2.1, txt2img, img2img, inpainting, NSFW filter, multiple GPU support, Mac Support, gfpgan (fix faces), realesrgan (upscale), 19 samplers (including k-samplers and UniPC), custom VAE, custom hypernetworks, low-memory optimizations, model merging, safetensor support, picklescan, etc. [Click here to see the full list of features](https://github.com/easydiffusion/sdkit/wiki/Features).
+**Features include:** SD 2.1, txt2img, img2img, inpainting, NSFW filter, multiple GPU support, Mac Support, GFPGAN and CodeFormer (fix faces), RealESRGAN (upscale), 19 samplers (including k-samplers and UniPC), custom VAE, custom hypernetworks, low-memory optimizations, model merging, safetensor support, picklescan, etc. [Click here to see the full list of features](https://github.com/easydiffusion/sdkit/wiki/Features).
 
-📢 We're looking to add support for *textual inversion embeddings*, *codeformer*, *seamless tiling*, and *outpainting*. We'd love code contributions for these!
+📢 We're looking to add support for *textual inversion embeddings*, *AMD support*, *ControlNet*, *Pix2Pix*, and *outpainting*. We'd love code contributions for these!
 
 ## Is it fast?
 It is pretty fast, and close to the fastest. For the same image, `sdkit` took 5.5 seconds, while `automatic1111` webui took 4.95 seconds. 📢 We're looking for code contributions to make `sdkit` even faster!
 
 `xformers` is supported experimentally, which will make `sdkit` even faster.
 
 **Details of the benchmark:**
@@ -113,24 +113,24 @@
 
 | | Time taken | Iterations/sec | Peak VRAM usage |
 | --- | --- | --- | --- |
 | `sdkit` | 5.5 sec | 6.0 it/s | 5.1 GB |
 | `automatic1111` webui | 4.95 sec | 6.15 it/s | 5.1 GB |
 
 ## Does it work on lower-end GPUs, or without GPUs?
-Yes. It works on NVIDIA/Mac GPUs with atleast 3GB of VRAM. For PCs without a compatible GPU, it can run entirely on the CPU. Running on the CPU will be *very* slow, but atleast you'll be able to try it out!
+Yes. It works on NVIDIA/Mac GPUs with atleast 2GB of VRAM. For PCs without a compatible GPU, it can run entirely on the CPU. Running on the CPU will be *very* slow, but atleast you'll be able to try it out!
 
 📢 We don't support AMD yet (it'll run in CPU-mode), but we're looking for code contributions for AMD support!
 
 ## Why not just use diffusers?
 You can certainly use diffusers. `sdkit` is infact using `diffusers` internally (currently in beta), so you can think of `sdkit` as a convenient API and a collection of tools, focused on Stable Diffusion projects.
 
 `sdkit`:
 1. is a simple, lightweight toolkit for Stable Diffusion projects.
-2. natively includes frequently-used projects like GFPGAN and RealESRGAN.
+2. natively includes frequently-used projects like GFPGAN, CodeFormer and RealESRGAN.
 3. works with the popular `.ckpt` and `.safetensors` model format.
 4. includes memory optimizations for low-end GPUs.
 5. built-in support for running on multiple GPUs.
 6. can download models from any server.
 7. auto-scans for malicious models.
 8. includes 19 samplers (including k-samplers).
 9. born out of the needs of the new Stable Diffusion AI Art scene, starting Aug 2022.
@@ -141,24 +141,25 @@
 
 If your project is using sdkit, you can add it to this list. Please feel free to open a pull request (or let us know at our [Discord community](https://discord.com/invite/u9yhsFmEkB)).
 
 # Contributing
 We'd love to accept code contributions. Please feel free to drop by our [Discord community](https://discord.com/invite/u9yhsFmEkB)!
 
 📢 We're looking for code contributions for these features (or anything else you'd like to work on):
-- CodeFormer upscaling (please maintain the required copyright notices).
 - Using custom Textual Inversion embeddings.
-- Seamless tiling.
 - Outpainting.
+- ControlNet.
+- Pix2Pix.
 - AMD support.
 
 If you'd like to set up a developer version on your PC (to contribute code changes), please follow [these instructions](https://github.com/easydiffusion/sdkit/blob/main/CONTRIBUTING.md).
 
 # Credits
 * Stable Diffusion: https://github.com/Stability-AI/stablediffusion
+* CodeFormer: https://github.com/sczhou/CodeFormer (license: https://github.com/sczhou/CodeFormer/blob/master/LICENSE)
 * GFPGAN: https://github.com/TencentARC/GFPGAN
 * RealESRGAN: https://github.com/xinntao/Real-ESRGAN
 * k-diffusion: https://github.com/crowsonkb/k-diffusion
 * Code contributors and artists on the cmdr2 UI: https://github.com/cmdr2/stable-diffusion-ui and Discord (https://discord.com/invite/u9yhsFmEkB)
 * Lots of contributors on the internet
 
 # Disclaimer
```

### Comparing `sdkit-1.0.98/pyproject.toml` & `sdkit-1.0.99/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdkit"
-version = "1.0.98"
+version = "1.0.99"
 authors = [
   {name="cmdr2", email="secondary.cmdr2@gmail.com"},
 ]
 description = "sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like GFPGAN, RealESRGAN, k-samplers, custom VAE, hypernetworks etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc. Supports Stable Diffusion 2.1!"
 readme = "README.md"
 requires-python = ">=3.8.5"
 classifiers = [
```

### Comparing `sdkit-1.0.98/sdkit/__init__.py` & `sdkit-1.0.99/sdkit/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/filter/apply_filters.py` & `sdkit-1.0.99/sdkit/filter/apply_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from sdkit import Context
 from sdkit.utils import base64_str_to_img, gc, log
 
-from . import gfpgan, nsfw_checker, realesrgan, latent_upscaler
+from . import gfpgan, nsfw_checker, realesrgan, latent_upscaler, codeformer
 
 filter_modules = {
     "gfpgan": gfpgan,
     "realesrgan": realesrgan,
     "nsfw_checker": nsfw_checker,
+    "codeformer": codeformer,
     "latent_upscaler": latent_upscaler
 }
 
 
 def apply_filters(context: Context, filters, images, **kwargs):
     """
     * context: Context
```

### Comparing `sdkit-1.0.98/sdkit/filter/gfpgan.py` & `sdkit-1.0.99/sdkit/filter/gfpgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/filter/latent_upscaler.py` & `sdkit-1.0.99/sdkit/filter/latent_upscaler.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/filter/nsfw_checker.py` & `sdkit-1.0.99/sdkit/filter/nsfw_checker.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/generate/image_generator.py` & `sdkit-1.0.99/sdkit/generate/image_generator.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/generate/prompt_parser.py` & `sdkit-1.0.99/sdkit/generate/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/generate/sampler/default_samplers.py` & `sdkit-1.0.99/sdkit/generate/sampler/default_samplers.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/generate/sampler/diffusers_samplers.py` & `sdkit-1.0.99/sdkit/generate/sampler/diffusers_samplers.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/generate/sampler/k_samplers.py` & `sdkit-1.0.99/sdkit/generate/sampler/k_samplers.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/generate/sampler/sampler_main.py` & `sdkit-1.0.99/sdkit/generate/sampler/sampler_main.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/generate/sampler/unipc_samplers/__init__.py` & `sdkit-1.0.99/sdkit/generate/sampler/unipc_samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py` & `sdkit-1.0.99/sdkit/generate/sampler/unipc_samplers/unipc_sampler.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/model_downloader.py` & `sdkit-1.0.99/sdkit/models/model_downloader.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/model_loader/__init__.py` & `sdkit-1.0.99/sdkit/models/model_loader/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,27 @@
     hypernetwork,
     latent_upscaler,
     lora,
     nsfw_checker,
     realesrgan,
     stable_diffusion,
     vae,
+    codeformer,
 )
 
 models = {
     "stable-diffusion": stable_diffusion,
+    "codeformer": codeformer,
     "gfpgan": gfpgan,
     "realesrgan": realesrgan,
     "vae": vae,
     "hypernetwork": hypernetwork,
     "nsfw_checker": nsfw_checker,
     "lora": lora,
-    "latent_upscaler": latent_upscaler
+    "latent_upscaler": latent_upscaler,
 }
 
 
 def load_model(context: Context, model_type: str, **kwargs):
     if context.model_paths.get(model_type) is None and model_type != "nsfw_checker":
         return
```

### Comparing `sdkit-1.0.98/sdkit/models/model_loader/gfpgan.py` & `sdkit-1.0.99/sdkit/models/model_loader/gfpgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/model_loader/hypernetwork/__init__.py` & `sdkit-1.0.99/sdkit/models/model_loader/hypernetwork/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/model_loader/hypernetwork/hypernetwork.py` & `sdkit-1.0.99/sdkit/models/model_loader/hypernetwork/hypernetwork.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/model_loader/latent_upscaler.py` & `sdkit-1.0.99/sdkit/models/model_loader/latent_upscaler.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/model_loader/lora.py` & `sdkit-1.0.99/sdkit/models/model_loader/lora.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/model_loader/nsfw_checker.py` & `sdkit-1.0.99/sdkit/models/model_loader/nsfw_checker.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/model_loader/realesrgan.py` & `sdkit-1.0.99/sdkit/models/model_loader/realesrgan.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/model_loader/stable_diffusion/__init__.py` & `sdkit-1.0.99/sdkit/models/model_loader/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py` & `sdkit-1.0.99/sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/model_loader/stable_diffusion/optimizations.py` & `sdkit-1.0.99/sdkit/models/model_loader/stable_diffusion/optimizations.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/model_loader/vae.py` & `sdkit-1.0.99/sdkit/models/model_loader/vae.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/models_db/__init__.py` & `sdkit-1.0.99/sdkit/models/models_db/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,16 @@
         db["stable-diffusion"] = json.load(f)
     with open(db_path / "gfpgan.json") as f:
         db["gfpgan"] = json.load(f)
     with open(db_path / "realesrgan.json") as f:
         db["realesrgan"] = json.load(f)
     with open(db_path / "vae.json") as f:
         db["vae"] = json.load(f)
+    with open(db_path / "codeformer.json") as f:
+        db["codeformer"] = json.load(f)
     return db
 
 
 def get_model_info_from_db(quick_hash=None, model_type=None, model_id=None):
     db = get_models_db()
 
     if quick_hash:
```

### Comparing `sdkit-1.0.98/sdkit/models/models_db/configs/v1-inference.yaml` & `sdkit-1.0.99/sdkit/models/models_db/configs/v1-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/models_db/configs/v1-inpainting-inference.yaml` & `sdkit-1.0.99/sdkit/models/models_db/configs/v1-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/models_db/configs/v2-inference-v.yaml` & `sdkit-1.0.99/sdkit/models/models_db/configs/v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/models_db/configs/v2-inference.yaml` & `sdkit-1.0.99/sdkit/models/models_db/configs/v2-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/models_db/configs/v2-inpainting-inference.yaml` & `sdkit-1.0.99/sdkit/models/models_db/configs/v2-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/models_db/configs/v2-midas-inference.yaml` & `sdkit-1.0.99/sdkit/models/models_db/configs/v2-midas-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/models_db/configs/v2.1-inference-v.yaml` & `sdkit-1.0.99/sdkit/models/models_db/configs/v2.1-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/models_db/configs/v2.1-inference.yaml` & `sdkit-1.0.99/sdkit/models/models_db/configs/v2.1-inference.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/models_db/configs/x4-upscaling.yaml` & `sdkit-1.0.99/sdkit/models/models_db/configs/x4-upscaling.yaml`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/models_db/gfpgan.json` & `sdkit-1.0.99/sdkit/models/models_db/gfpgan.json`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/models_db/realesrgan.json` & `sdkit-1.0.99/sdkit/models/models_db/realesrgan.json`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/models/models_db/stable_diffusion.json` & `sdkit-1.0.99/sdkit/models/models_db/stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/train/merge_models.py` & `sdkit-1.0.99/sdkit/train/merge_models.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/utils/__init__.py` & `sdkit-1.0.99/sdkit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/utils/file_utils.py` & `sdkit-1.0.99/sdkit/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/utils/hash_utils.py` & `sdkit-1.0.99/sdkit/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/utils/http_utils.py` & `sdkit-1.0.99/sdkit/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/utils/image_utils.py` & `sdkit-1.0.99/sdkit/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/utils/latent_utils.py` & `sdkit-1.0.99/sdkit/utils/latent_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit/utils/memory_utils.py` & `sdkit-1.0.99/sdkit/utils/memory_utils.py`

 * *Files identical despite different names*

### Comparing `sdkit-1.0.98/sdkit.egg-info/PKG-INFO` & `sdkit-1.0.99/sdkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkit
-Version: 1.0.98
+Version: 1.0.99
 Summary: sdkit (stable diffusion kit) is an easy-to-use library for using Stable Diffusion in your AI Art projects. It is fast, feature-packed, and memory-efficient. It bundles Stable Diffusion along with commonly-used features (like GFPGAN, RealESRGAN, k-samplers, custom VAE, hypernetworks etc). It also includes a model-downloader with a database of commonly used models, and advanced features like running in parallel on multiple GPUs, auto-scanning for malicious models etc. Supports Stable Diffusion 2.1!
 Author-email: cmdr2 <secondary.cmdr2@gmail.com>
 Project-URL: Homepage, https://github.com/easydiffusion/sdkit
 Project-URL: Bug Tracker, https://github.com/easydiffusion/sdkit/issues
 Keywords: stable diffusion,ai,art
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,15 +24,15 @@
 *New: Stable Diffusion 2.1 is now supported!*
 
 This is a community project, so please feel free to contribute (and use in your project)!
 
 ![t2i](https://raw.githubusercontent.com/Stability-AI/stablediffusion/main/assets/stable-samples/txt2img/768/merged-0006.png)
 
 # Why?
-The goal is to let you be productive quickly (at your AI art project), so it bundles Stable Diffusion along with commonly-used features (like GFPGAN for face restoration, RealESRGAN for upscaling, k-samplers, support for loading custom VAEs and hypernetworks, NSFW filter etc).
+The goal is to let you be productive quickly (at your AI art project), so it bundles Stable Diffusion along with commonly-used features (like GFPGAN and CodeFormer for face restoration, RealESRGAN for upscaling, k-samplers, support for loading custom VAEs and hypernetworks, NSFW filter etc).
 
 Advanced features include a model-downloader (with a database of commonly used models), support for running in parallel on multiple GPUs, auto-scanning for malicious models etc. [Full list of features](https://github.com/easydiffusion/sdkit/wiki/Features)
 
 # Installation
 Tested with Python 3.8. Supports Windows, Linux and Mac.
 
 **Windows/Linux:**
@@ -110,17 +110,17 @@
 
 For models that don't match a known hash (e.g. custom models), or if you want to override the config file, you can set the path to the config file in `context.model_paths`. e.g. `context.model_paths['stable-diffusion'] = 'path/to/config.yaml'`
 
 # FAQ
 ## Does it have all the cool features?
 It has a lot of features! It was born out of a popular Stable Diffusion UI, splitting out the battle-tested core engine into `sdkit`.
 
-**Features include:** SD 2.1, txt2img, img2img, inpainting, NSFW filter, multiple GPU support, Mac Support, gfpgan (fix faces), realesrgan (upscale), 19 samplers (including k-samplers and UniPC), custom VAE, custom hypernetworks, low-memory optimizations, model merging, safetensor support, picklescan, etc. [Click here to see the full list of features](https://github.com/easydiffusion/sdkit/wiki/Features).
+**Features include:** SD 2.1, txt2img, img2img, inpainting, NSFW filter, multiple GPU support, Mac Support, GFPGAN and CodeFormer (fix faces), RealESRGAN (upscale), 19 samplers (including k-samplers and UniPC), custom VAE, custom hypernetworks, low-memory optimizations, model merging, safetensor support, picklescan, etc. [Click here to see the full list of features](https://github.com/easydiffusion/sdkit/wiki/Features).
 
-📢 We're looking to add support for *textual inversion embeddings*, *codeformer*, *seamless tiling*, and *outpainting*. We'd love code contributions for these!
+📢 We're looking to add support for *textual inversion embeddings*, *AMD support*, *ControlNet*, *Pix2Pix*, and *outpainting*. We'd love code contributions for these!
 
 ## Is it fast?
 It is pretty fast, and close to the fastest. For the same image, `sdkit` took 5.5 seconds, while `automatic1111` webui took 4.95 seconds. 📢 We're looking for code contributions to make `sdkit` even faster!
 
 `xformers` is supported experimentally, which will make `sdkit` even faster.
 
 **Details of the benchmark:**
@@ -131,24 +131,24 @@
 
 | | Time taken | Iterations/sec | Peak VRAM usage |
 | --- | --- | --- | --- |
 | `sdkit` | 5.5 sec | 6.0 it/s | 5.1 GB |
 | `automatic1111` webui | 4.95 sec | 6.15 it/s | 5.1 GB |
 
 ## Does it work on lower-end GPUs, or without GPUs?
-Yes. It works on NVIDIA/Mac GPUs with atleast 3GB of VRAM. For PCs without a compatible GPU, it can run entirely on the CPU. Running on the CPU will be *very* slow, but atleast you'll be able to try it out!
+Yes. It works on NVIDIA/Mac GPUs with atleast 2GB of VRAM. For PCs without a compatible GPU, it can run entirely on the CPU. Running on the CPU will be *very* slow, but atleast you'll be able to try it out!
 
 📢 We don't support AMD yet (it'll run in CPU-mode), but we're looking for code contributions for AMD support!
 
 ## Why not just use diffusers?
 You can certainly use diffusers. `sdkit` is infact using `diffusers` internally (currently in beta), so you can think of `sdkit` as a convenient API and a collection of tools, focused on Stable Diffusion projects.
 
 `sdkit`:
 1. is a simple, lightweight toolkit for Stable Diffusion projects.
-2. natively includes frequently-used projects like GFPGAN and RealESRGAN.
+2. natively includes frequently-used projects like GFPGAN, CodeFormer and RealESRGAN.
 3. works with the popular `.ckpt` and `.safetensors` model format.
 4. includes memory optimizations for low-end GPUs.
 5. built-in support for running on multiple GPUs.
 6. can download models from any server.
 7. auto-scans for malicious models.
 8. includes 19 samplers (including k-samplers).
 9. born out of the needs of the new Stable Diffusion AI Art scene, starting Aug 2022.
@@ -159,24 +159,25 @@
 
 If your project is using sdkit, you can add it to this list. Please feel free to open a pull request (or let us know at our [Discord community](https://discord.com/invite/u9yhsFmEkB)).
 
 # Contributing
 We'd love to accept code contributions. Please feel free to drop by our [Discord community](https://discord.com/invite/u9yhsFmEkB)!
 
 📢 We're looking for code contributions for these features (or anything else you'd like to work on):
-- CodeFormer upscaling (please maintain the required copyright notices).
 - Using custom Textual Inversion embeddings.
-- Seamless tiling.
 - Outpainting.
+- ControlNet.
+- Pix2Pix.
 - AMD support.
 
 If you'd like to set up a developer version on your PC (to contribute code changes), please follow [these instructions](https://github.com/easydiffusion/sdkit/blob/main/CONTRIBUTING.md).
 
 # Credits
 * Stable Diffusion: https://github.com/Stability-AI/stablediffusion
+* CodeFormer: https://github.com/sczhou/CodeFormer (license: https://github.com/sczhou/CodeFormer/blob/master/LICENSE)
 * GFPGAN: https://github.com/TencentARC/GFPGAN
 * RealESRGAN: https://github.com/xinntao/Real-ESRGAN
 * k-diffusion: https://github.com/crowsonkb/k-diffusion
 * Code contributors and artists on the cmdr2 UI: https://github.com/cmdr2/stable-diffusion-ui and Discord (https://discord.com/invite/u9yhsFmEkB)
 * Lots of contributors on the internet
 
 # Disclaimer
```

### Comparing `sdkit-1.0.98/sdkit.egg-info/SOURCES.txt` & `sdkit-1.0.99/sdkit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 sdkit.egg-info/PKG-INFO
 sdkit.egg-info/SOURCES.txt
 sdkit.egg-info/dependency_links.txt
 sdkit.egg-info/requires.txt
 sdkit.egg-info/top_level.txt
 sdkit/filter/__init__.py
 sdkit/filter/apply_filters.py
+sdkit/filter/codeformer.py
 sdkit/filter/gfpgan.py
 sdkit/filter/latent_upscaler.py
 sdkit/filter/nsfw_checker.py
 sdkit/filter/realesrgan.py
 sdkit/generate/__init__.py
 sdkit/generate/image_generator.py
 sdkit/generate/prompt_parser.py
@@ -31,20 +32,24 @@
 sdkit/models/model_loader/__init__.py
 sdkit/models/model_loader/gfpgan.py
 sdkit/models/model_loader/latent_upscaler.py
 sdkit/models/model_loader/lora.py
 sdkit/models/model_loader/nsfw_checker.py
 sdkit/models/model_loader/realesrgan.py
 sdkit/models/model_loader/vae.py
+sdkit/models/model_loader/codeformer/__init__.py
+sdkit/models/model_loader/codeformer/codeformer_arch.py
+sdkit/models/model_loader/codeformer/vqgan_arch.py
 sdkit/models/model_loader/hypernetwork/__init__.py
 sdkit/models/model_loader/hypernetwork/hypernetwork.py
 sdkit/models/model_loader/stable_diffusion/__init__.py
 sdkit/models/model_loader/stable_diffusion/convert_from_ckpt.py
 sdkit/models/model_loader/stable_diffusion/optimizations.py
 sdkit/models/models_db/__init__.py
+sdkit/models/models_db/codeformer.json
 sdkit/models/models_db/gfpgan.json
 sdkit/models/models_db/realesrgan.json
 sdkit/models/models_db/stable_diffusion.json
 sdkit/models/models_db/vae.json
 sdkit/models/models_db/configs/v1-inference.yaml
 sdkit/models/models_db/configs/v1-inpainting-inference.yaml
 sdkit/models/models_db/configs/v2-inference-v.yaml
```

