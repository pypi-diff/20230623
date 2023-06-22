# Comparing `tmp/vocab-coverage-0.4.tar.gz` & `tmp/vocab-coverage-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocab-coverage-0.4.tar", last modified: Fri Jun 16 08:04:58 2023, max compression
+gzip compressed data, was "vocab-coverage-0.5.tar", last modified: Thu Jun 22 22:38:47 2023, max compression
```

## Comparing `vocab-coverage-0.4.tar` & `vocab-coverage-0.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 08:04:58.017979 vocab-coverage-0.4/
--rw-r--r--   0 tao        (502) staff       (20)    11357 2023-06-15 09:34:29.000000 vocab-coverage-0.4/LICENSE
--rw-r--r--   0 tao        (502) staff       (20)     9038 2023-06-16 08:04:58.017828 vocab-coverage-0.4/PKG-INFO
--rw-r--r--   0 tao        (502) staff       (20)     8149 2023-06-15 08:53:12.000000 vocab-coverage-0.4/README.md
--rw-r--r--   0 tao        (502) staff       (20)       38 2023-06-16 08:04:58.018039 vocab-coverage-0.4/setup.cfg
--rw-r--r--   0 tao        (502) staff       (20)     1401 2023-06-16 07:49:50.000000 vocab-coverage-0.4/setup.py
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 08:04:58.016943 vocab-coverage-0.4/vocab_coverage/
--rw-r--r--   0 tao        (502) staff       (20)      128 2023-06-16 07:49:46.000000 vocab-coverage-0.4/vocab_coverage/__init__.py
--rw-r--r--   0 tao        (502) staff       (20)     4166 2023-06-16 07:57:21.000000 vocab-coverage-0.4/vocab_coverage/charsets.py
--rw-r--r--   0 tao        (502) staff       (20)     3002 2023-06-16 05:34:42.000000 vocab-coverage-0.4/vocab_coverage/draw.py
--rw-r--r--   0 tao        (502) staff       (20)     1645 2023-06-16 07:57:38.000000 vocab-coverage-0.4/vocab_coverage/main.py
--rw-r--r--   0 tao        (502) staff       (20)     5196 2023-06-16 07:57:33.000000 vocab-coverage-0.4/vocab_coverage/model.py
-drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-16 08:04:58.017632 vocab-coverage-0.4/vocab_coverage.egg-info/
--rw-r--r--   0 tao        (502) staff       (20)     9038 2023-06-16 08:04:57.000000 vocab-coverage-0.4/vocab_coverage.egg-info/PKG-INFO
--rw-r--r--   0 tao        (502) staff       (20)      380 2023-06-16 08:04:57.000000 vocab-coverage-0.4/vocab_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 tao        (502) staff       (20)        1 2023-06-16 08:04:57.000000 vocab-coverage-0.4/vocab_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 tao        (502) staff       (20)       55 2023-06-16 08:04:57.000000 vocab-coverage-0.4/vocab_coverage.egg-info/entry_points.txt
--rw-r--r--   0 tao        (502) staff       (20)      101 2023-06-16 08:04:57.000000 vocab-coverage-0.4/vocab_coverage.egg-info/requires.txt
--rw-r--r--   0 tao        (502) staff       (20)       15 2023-06-16 08:04:57.000000 vocab-coverage-0.4/vocab_coverage.egg-info/top_level.txt
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-22 22:38:47.066887 vocab-coverage-0.5/
+-rw-r--r--   0 tao        (502) staff       (20)    11357 2023-06-15 09:34:29.000000 vocab-coverage-0.5/LICENSE
+-rw-r--r--   0 tao        (502) staff       (20)    24281 2023-06-22 22:38:47.066715 vocab-coverage-0.5/PKG-INFO
+-rw-r--r--   0 tao        (502) staff       (20)    23456 2023-06-22 06:23:03.000000 vocab-coverage-0.5/README.md
+-rw-r--r--   0 tao        (502) staff       (20)       38 2023-06-22 22:38:47.066928 vocab-coverage-0.5/setup.cfg
+-rw-r--r--   0 tao        (502) staff       (20)     1482 2023-06-22 22:35:32.000000 vocab-coverage-0.5/setup.py
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-22 22:38:47.065398 vocab-coverage-0.5/vocab_coverage/
+-rw-r--r--   0 tao        (502) staff       (20)      170 2023-06-19 22:57:11.000000 vocab-coverage-0.5/vocab_coverage/__init__.py
+-rw-r--r--   0 tao        (502) staff       (20)    11667 2023-06-22 18:50:50.000000 vocab-coverage-0.5/vocab_coverage/charsets.py
+-rw-r--r--   0 tao        (502) staff       (20)     7331 2023-06-21 19:52:17.000000 vocab-coverage-0.5/vocab_coverage/draw.py
+-rw-r--r--   0 tao        (502) staff       (20)     8296 2023-06-22 18:56:13.000000 vocab-coverage-0.5/vocab_coverage/embedding.py
+-rw-r--r--   0 tao        (502) staff       (20)     2714 2023-06-19 23:08:26.000000 vocab-coverage-0.5/vocab_coverage/main.py
+-rw-r--r--   0 tao        (502) staff       (20)     5285 2023-06-20 04:53:16.000000 vocab-coverage-0.5/vocab_coverage/model.py
+drwxr-xr-x   0 tao        (502) staff       (20)        0 2023-06-22 22:38:47.066470 vocab-coverage-0.5/vocab_coverage.egg-info/
+-rw-r--r--   0 tao        (502) staff       (20)    24281 2023-06-22 22:38:47.000000 vocab-coverage-0.5/vocab_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 tao        (502) staff       (20)      408 2023-06-22 22:38:47.000000 vocab-coverage-0.5/vocab_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 tao        (502) staff       (20)        1 2023-06-22 22:38:47.000000 vocab-coverage-0.5/vocab_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 tao        (502) staff       (20)       55 2023-06-22 22:38:47.000000 vocab-coverage-0.5/vocab_coverage.egg-info/entry_points.txt
+-rw-r--r--   0 tao        (502) staff       (20)      125 2023-06-22 22:38:47.000000 vocab-coverage-0.5/vocab_coverage.egg-info/requires.txt
+-rw-r--r--   0 tao        (502) staff       (20)       15 2023-06-22 22:38:47.000000 vocab-coverage-0.5/vocab_coverage.egg-info/top_level.txt
```

### Comparing `vocab-coverage-0.4/LICENSE` & `vocab-coverage-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vocab-coverage-0.4/setup.py` & `vocab-coverage-0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vocab-coverage',
-    version='0.4',
+    version='0.5',
     packages=find_packages(),
     install_requires=[
         'Pillow',
         'protobuf==3.20.0',
         'sentencepiece',
         'tiktoken',
         'torch',
         'transformers',
         'beautifulsoup4',
         'bs4',
         'pandas',
         'requests',
+        'scikit-learn',
+        'accelerate',
     ],
-    description='A Python package designed to perform coverage analysis on Chinese vocabulary for language models.',
+    description='语言模型中文识字率分析\nA Python package designed to perform coverage analysis on Chinese vocabulary for language models.',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     author='Tao Wang',
     author_email='twang2218@gmail.com',
     url='https://github.com/twang2218/vocab-coverage',
     license='Apache License 2.0',
     classifiers=[
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vocab-coverage-0.4/vocab_coverage/main.py` & `vocab-coverage-0.5/vocab_coverage/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,39 +2,49 @@
 import sys
 import argparse
 import json
 
 if __name__ == "__main__":
     sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
-from vocab_coverage import model_check
+from vocab_coverage import model_check, embedding_analysis
 
 def main():
     parser = argparse.ArgumentParser()
 
     subcommands = parser.add_subparsers(dest='command')
 
     cmdModel = subcommands.add_parser('model', help='模型汉字识字率分析')
     cmdModel.add_argument("--model_name", type=str, default="shibing624/text2vec-base-chinese", help="模型在 HuggingFace Hub 上的名称（默认为 shibing624/text2vec-base-chinese）")
     cmdModel.add_argument("--charset_file", type=str, default="charset.json", help="用以统计识字率的字表文件（默认为 charset.json）")
     cmdModel.add_argument("--output_dir", type=str, default="images", help="生成的图像文件的输出目录（默认为 images）")
     cmdModel.add_argument("--debug", action='store_true', help="是否打印调试信息")
 
+    cmdEmbedding = subcommands.add_parser('embedding', help='词向量可视化分析')
+    cmdEmbedding.add_argument("--model_name", type=str, default="shibing624/text2vec-base-chinese", help="模型在 HuggingFace Hub 上的名称（默认为 shibing624/text2vec-base-chinese）")
+    cmdEmbedding.add_argument("--charset_file", type=str, default="charset.json", help="用以统计识字率的字表文件（默认为 charset.json）")
+    cmdEmbedding.add_argument("--output_dir", type=str, default="images", help="生成的图像文件的输出目录（默认为 images）")
+    cmdEmbedding.add_argument("--is_detail", action='store_true', help="是否对汉字进行详细分类（默认为 False）")
+    cmdEmbedding.add_argument("--debug", action='store_true', help="是否打印调试信息（默认为 False）")
+
     cmdCharset = subcommands.add_parser('charset', help='生成用以统计识字率的字表文件')
-    cmdCharset.add_argument("--charset_file", type=str, default="charset.json", help="用以统计识字率的字表文件")
+    cmdCharset.add_argument("--charset_file", type=str, default="charset.json", help="用以统计识字率的字表文件（默认为 charset.json）")
 
     args = parser.parse_args()
 
     if args.command == 'charset':
         from vocab_coverage import generate_charsets
         generate_charsets(args.charset_file)
         return
     elif args.command == 'model':
         charsets = json.load(open(args.charset_file, 'r'))
-        model_check(charsets, args.model_name, args.output_dir, args.debug)
+        model_check(args.model_name, charsets, args.output_dir, args.debug)
         return
+    elif args.command == 'embedding':
+        charsets = json.load(open(args.charset_file, 'r'))
+        embedding_analysis(args.model_name, charsets, args.output_dir, args.is_detail, args.debug)
     else:
         parser.print_help()
         return
 
 if __name__ == "__main__":
     main()
```

### Comparing `vocab-coverage-0.4/vocab_coverage/model.py` & `vocab-coverage-0.5/vocab_coverage/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import sys
 
 from transformers import AutoTokenizer
 
 from vocab_coverage.draw import draw_vocab_graph
 
-def model_check(charsets, model_name:str, output_dir:str, debug=False):
+def model_check(model_name:str, charsets, output_dir:str, debug=False):
     print("检查模型 {} 的字表".format(model_name))
     try:
         tokenizer = AutoTokenizer.from_pretrained(model_name, trust_remote_code=True)
     except Exception as e:
         if "LLaMATokenizer" in e.args[0]:
             from transformers import LlamaTokenizer
             tokenizer = LlamaTokenizer.from_pretrained(model_name, trust_remote_code=True)
@@ -105,12 +105,16 @@
                 if debug:
                     print("[{}] 汉字({})被拆分了，编码为{}".format(tn, c, tokens_ids))
 
     # 统计显示
     for name, stats in charset_stats.items():
         print("字表{}：{}/{} ({:.2%})".format(name, stats['known'], stats['total'], float(stats['known'])/stats['total']))
 
-    # 生成字表图
-    filename = model_name.replace("/", "_") + ".png"
-    os.mkdir(output_dir) if not os.path.exists(output_dir) else None
+    # 生成文件名
+    filename = model_name.replace('/', '_') + '.png'
+    filename = 'coverage_' + filename
+    output_dir = os.path.join(output_dir, 'coverage')
+    os.makedirs(output_dir, exist_ok=True)
     filename = os.path.join(output_dir, filename)
+
+    # 生成字表图
     draw_vocab_graph(model_name, charset_stats, tokenizer.vocab_size, filename, width=150)
```

