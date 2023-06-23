# Comparing `tmp/pyselector-0.0.8b0.tar.gz` & `tmp/pyselector-0.0.9.tar.gz`

## Comparing `pyselector-0.0.8b0.tar` & `pyselector-0.0.9.tar`

### file list

```diff
@@ -1,161 +1,161 @@
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.coverage
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.dmypy.json
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/mkdocs.yml
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/pa.py
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/pyproject.toml.bk
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/1586d67568282a40
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/160270c07008d21a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/1649e7152a516b02
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/1950c7571caa3c4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/1bf3a9feef6da7b4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/1e4e65c508ae2eb4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/240e03c8eca20b3b
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/2faf0f1a0ce67f90
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/30e95cfadd495118
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/3146b9ac234e7da3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/3a16f27e6fcb42d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/3e6529a91dd73754
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/3fa8094dd6d237f2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/48d29984b323bdc3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/4ed6e931c98abb83
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/4f73f0e8cb30ea2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/5218d43b5a17e9e4
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/5660809a5af94d5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/5dbe5b320ab74a2c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/668143f5f1847553
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/695870d8b84cc1df
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/6cb82af6df540b64
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/6d671464c22ea4ef
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/7152592b55eb5d34
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/760d6554a6900e87
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/76e9e2875da73d5f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/7f8954763a9666d9
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/855c110b65d23e74
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/87c6f3c429b29bad
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/8a393223eee50efd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/8ae83ca87493671d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/8c5be33a43c5ecaf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/9097067d3ee1fc7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/90bf583d9cf22efd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/93fea773ecf1a505
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/941b8c063a6fab52
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/9599bc2cf2cba1ec
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/a37dcb5c1ed3e3ce
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/ac44f5ed0c4189be
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/ad23de5dfb3bd182
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/adac83471c4f6964
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/b3c5732df5eb18f3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/b99e17733901818c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/bc1edf2b88b558c2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/bc9392902044c07f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/be40c467e313f25b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/becb3ba9082bc475
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/c4fe6e9a45d0c14e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/c5a8079d0cae3f81
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/cebd5672b707b4c3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/d7cd6258ea9d25e8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/de7ae2b3a0ecb97d
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/e80854fc5d62c800
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/ec5acb59db4f2a9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/f0248d0c57d75f
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/f196c1fe7be41aeb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/f402b8c7d9e687be
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.ruff_cache/content/fc10e3817ee99c4f
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/docs/index.md
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/docs/tutorials.md
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/examples/example.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/.gitignore
--rw-r--r--   0        0        0    20650 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_2d6ebab7310f0e1c___init___py.html
--rw-r--r--   0        0        0    25120 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_2d6ebab7310f0e1c_helpers_py.html
--rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_2d6ebab7310f0e1c_interfaces_py.html
--rw-r--r--   0        0        0    42430 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_2d6ebab7310f0e1c_key_manager_py.html
--rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_2d6ebab7310f0e1c_logger_py.html
--rw-r--r--   0        0        0    12223 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_2d6ebab7310f0e1c_selector_py.html
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_a44f0ac069e85531_test_dmenu_py.html
--rw-r--r--   0        0        0    28515 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_a44f0ac069e85531_test_fzf_py.html
--rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_a44f0ac069e85531_test_helpers_py.html
--rw-r--r--   0        0        0    40128 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_a44f0ac069e85531_test_key_manager_py.html
--rw-r--r--   0        0        0    43618 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_a44f0ac069e85531_test_rofi_py.html
--rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_a44f0ac069e85531_test_selector_py.html
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_c46c4fc7bbe4d838___init___py.html
--rw-r--r--   0        0        0    28909 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_c46c4fc7bbe4d838_dmenu_py.html
--rw-r--r--   0        0        0    29901 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_c46c4fc7bbe4d838_fzf_py.html
--rw-r--r--   0        0        0    52717 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/d_c46c4fc7bbe4d838_rofi_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/status.json
--rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/htmlcov/style.css
--rw-r--r--   0        0        0     8681 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/404.html
--rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/index.html
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/sitemap.xml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/sitemap.xml.gz
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/images/favicon.png
--rw-r--r--   0        0        0   115258 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/bundle.5a2dcb6a.min.js
--rw-r--r--   0        0        0   612394 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/bundle.5a2dcb6a.min.js.map
--rw-r--r--   0        0        0    34219 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/extra/bundle.5f09fbc3.min.js
--rw-r--r--   0        0        0    82551 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/extra/bundle.5f09fbc3.min.js.map
--rw-r--r--   0        0        0    22878 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0        0        0   677455 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/wordcut.js
--rw-r--r--   0        0        0    17074 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0        0        0    11499 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0        0        0    10669 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0        0        0    10171 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0        0        0    15009 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0        0        0    36472 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/workers/search.16e2a7d4.min.js
--rw-r--r--   0        0        0   182197 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/javascripts/workers/search.16e2a7d4.min.js.map
--rw-r--r--   0        0        0    18200 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/stylesheets/extra.0d2c79a8.min.css
--rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/stylesheets/extra.0d2c79a8.min.css.map
--rw-r--r--   0        0        0   135600 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/stylesheets/main.975780f9.min.css
--rw-r--r--   0        0        0    45210 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/stylesheets/main.975780f9.min.css.map
--rw-r--r--   0        0        0    12289 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/stylesheets/palette.2505c338.min.css
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/assets/stylesheets/palette.2505c338.min.css.map
--rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/search/search_index.json
--rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/site/tutorials/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/src/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/src/pyselector/__init__.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/src/pyselector/helpers.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/src/pyselector/interfaces.py
--rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/src/pyselector/key_manager.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/src/pyselector/logger.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/src/pyselector/selector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/src/pyselector/menus/__init__.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/src/pyselector/menus/dmenu.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/src/pyselector/menus/fzf.py
--rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/src/pyselector/menus/rofi.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/tests/test_dmenu.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/tests/test_fzf.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/tests/test_helpers.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/tests/test_key_manager.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/tests/test_rofi.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/tests/test_selector.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/.gitignore
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/README.md
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/pyproject.toml
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 pyselector-0.0.8b0/PKG-INFO
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 pyselector-0.0.9/.coverage
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pyselector-0.0.9/.dmypy.json
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pyselector-0.0.9/mkdocs.yml
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pyselector-0.0.9/pa.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 pyselector-0.0.9/pyproject.toml.bk
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/1586d67568282a40
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/160270c07008d21a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/1649e7152a516b02
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/1950c7571caa3c4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/1bf3a9feef6da7b4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/1e4e65c508ae2eb4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/240e03c8eca20b3b
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/2faf0f1a0ce67f90
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/30e95cfadd495118
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/3146b9ac234e7da3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/3a16f27e6fcb42d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/3e6529a91dd73754
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/3fa8094dd6d237f2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/48d29984b323bdc3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/4ed6e931c98abb83
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/4f73f0e8cb30ea2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/5218d43b5a17e9e4
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/5660809a5af94d5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/5dbe5b320ab74a2c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/668143f5f1847553
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/695870d8b84cc1df
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/6cb82af6df540b64
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/6d671464c22ea4ef
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/7152592b55eb5d34
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/760d6554a6900e87
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/76e9e2875da73d5f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/7f8954763a9666d9
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/855c110b65d23e74
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/87c6f3c429b29bad
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/8a393223eee50efd
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/8ae83ca87493671d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/8c5be33a43c5ecaf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/9097067d3ee1fc7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/90bf583d9cf22efd
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/93fea773ecf1a505
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/941b8c063a6fab52
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/9599bc2cf2cba1ec
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/a37dcb5c1ed3e3ce
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/ac44f5ed0c4189be
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/ad23de5dfb3bd182
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/adac83471c4f6964
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/b3c5732df5eb18f3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/b99e17733901818c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/bc1edf2b88b558c2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/bc9392902044c07f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/be40c467e313f25b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/becb3ba9082bc475
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/c4fe6e9a45d0c14e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/c5a8079d0cae3f81
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/cebd5672b707b4c3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/d7cd6258ea9d25e8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/de7ae2b3a0ecb97d
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/e80854fc5d62c800
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/ec5acb59db4f2a9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/f0248d0c57d75f
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/f196c1fe7be41aeb
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/f402b8c7d9e687be
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyselector-0.0.9/.ruff_cache/content/fc10e3817ee99c4f
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 pyselector-0.0.9/docs/index.md
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 pyselector-0.0.9/docs/tutorials.md
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 pyselector-0.0.9/examples/example.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/.gitignore
+-rw-r--r--   0        0        0    20650 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_2d6ebab7310f0e1c___init___py.html
+-rw-r--r--   0        0        0    25120 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_2d6ebab7310f0e1c_helpers_py.html
+-rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_2d6ebab7310f0e1c_interfaces_py.html
+-rw-r--r--   0        0        0    42430 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_2d6ebab7310f0e1c_key_manager_py.html
+-rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_2d6ebab7310f0e1c_logger_py.html
+-rw-r--r--   0        0        0    12223 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_2d6ebab7310f0e1c_selector_py.html
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_a44f0ac069e85531_test_dmenu_py.html
+-rw-r--r--   0        0        0    28515 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_a44f0ac069e85531_test_fzf_py.html
+-rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_a44f0ac069e85531_test_helpers_py.html
+-rw-r--r--   0        0        0    40128 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_a44f0ac069e85531_test_key_manager_py.html
+-rw-r--r--   0        0        0    43618 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_a44f0ac069e85531_test_rofi_py.html
+-rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_a44f0ac069e85531_test_selector_py.html
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_c46c4fc7bbe4d838___init___py.html
+-rw-r--r--   0        0        0    28909 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_c46c4fc7bbe4d838_dmenu_py.html
+-rw-r--r--   0        0        0    29901 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_c46c4fc7bbe4d838_fzf_py.html
+-rw-r--r--   0        0        0    52717 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/d_c46c4fc7bbe4d838_rofi_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/status.json
+-rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 pyselector-0.0.9/htmlcov/style.css
+-rw-r--r--   0        0        0     8681 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/404.html
+-rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/index.html
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/sitemap.xml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/sitemap.xml.gz
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/images/favicon.png
+-rw-r--r--   0        0        0   115258 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/bundle.5a2dcb6a.min.js
+-rw-r--r--   0        0        0   612394 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/bundle.5a2dcb6a.min.js.map
+-rw-r--r--   0        0        0    34219 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/extra/bundle.5f09fbc3.min.js
+-rw-r--r--   0        0        0    82551 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/extra/bundle.5f09fbc3.min.js.map
+-rw-r--r--   0        0        0    22878 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677455 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    17074 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    36472 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/workers/search.16e2a7d4.min.js
+-rw-r--r--   0        0        0   182197 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/javascripts/workers/search.16e2a7d4.min.js.map
+-rw-r--r--   0        0        0    18200 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/stylesheets/extra.0d2c79a8.min.css
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/stylesheets/extra.0d2c79a8.min.css.map
+-rw-r--r--   0        0        0   135600 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/stylesheets/main.975780f9.min.css
+-rw-r--r--   0        0        0    45210 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/stylesheets/main.975780f9.min.css.map
+-rw-r--r--   0        0        0    12289 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/stylesheets/palette.2505c338.min.css
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/assets/stylesheets/palette.2505c338.min.css.map
+-rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/search/search_index.json
+-rw-r--r--   0        0        0    11585 2020-02-02 00:00:00.000000 pyselector-0.0.9/site/tutorials/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyselector-0.0.9/src/__init__.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pyselector-0.0.9/src/pyselector/__init__.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 pyselector-0.0.9/src/pyselector/helpers.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pyselector-0.0.9/src/pyselector/interfaces.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyselector-0.0.9/src/pyselector/key_manager.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pyselector-0.0.9/src/pyselector/logger.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pyselector-0.0.9/src/pyselector/selector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyselector-0.0.9/src/pyselector/menus/__init__.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 pyselector-0.0.9/src/pyselector/menus/dmenu.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 pyselector-0.0.9/src/pyselector/menus/fzf.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 pyselector-0.0.9/src/pyselector/menus/rofi.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 pyselector-0.0.9/tests/test_dmenu.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 pyselector-0.0.9/tests/test_fzf.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 pyselector-0.0.9/tests/test_helpers.py
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 pyselector-0.0.9/tests/test_key_manager.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 pyselector-0.0.9/tests/test_rofi.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pyselector-0.0.9/tests/test_selector.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pyselector-0.0.9/.gitignore
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 pyselector-0.0.9/README.md
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 pyselector-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 pyselector-0.0.9/PKG-INFO
```

### Comparing `pyselector-0.0.8b0/.coverage` & `pyselector-0.0.9/.coverage`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/pyproject.toml.bk` & `pyselector-0.0.9/pyproject.toml.bk`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/.ruff_cache/content/2faf0f1a0ce67f90` & `pyselector-0.0.9/.ruff_cache/content/2faf0f1a0ce67f90`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/.ruff_cache/content/5660809a5af94d5` & `pyselector-0.0.9/.ruff_cache/content/5660809a5af94d5`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/.ruff_cache/content/6d671464c22ea4ef` & `pyselector-0.0.9/.ruff_cache/content/6d671464c22ea4ef`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/docs/index.md` & `pyselector-0.0.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/docs/tutorials.md` & `pyselector-0.0.9/docs/tutorials.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 def sort_by_key(key: str, items: list[dict[str, str]]) -> list[dict[str, str]]:
     return sorted(items, key=lambda x: x[key])
 
 
 def parse_selection(menu: Menu, keycode: int, **kwargs) -> Optional[Keybind]:
-    for key in menu.keybind.all_registered:
+    for key in menu.keybind.registered_keys:
         if key.code == keycode:
             logging.info("keybind: %s", key)
             return key
     return None
 
 
 def main() -> int:
```

### Comparing `pyselector-0.0.8b0/examples/example.py` & `pyselector-0.0.9/examples/example.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 def sort_by_key(key: str, items: list[dict[str, str]]) -> list[dict[str, str]]:
     return sorted(items, key=lambda x: x[key])
 
 
 def parse_selection(menu: Menu, keycode: int, **kwargs) -> Optional[Keybind]:
-    for key in menu.keybind.all_registered:
+    for key in menu.keybind.registered_keys:
         if key.code == keycode:
             logging.info("keybind: %s", key)
             return key
     return None
 
 
 def main() -> int:
```

### Comparing `pyselector-0.0.8b0/htmlcov/coverage_html.js` & `pyselector-0.0.9/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_2d6ebab7310f0e1c___init___py.html` & `pyselector-0.0.9/htmlcov/d_2d6ebab7310f0e1c___init___py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_2d6ebab7310f0e1c_helpers_py.html` & `pyselector-0.0.9/htmlcov/d_2d6ebab7310f0e1c_helpers_py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_2d6ebab7310f0e1c_interfaces_py.html` & `pyselector-0.0.9/htmlcov/d_2d6ebab7310f0e1c_interfaces_py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_2d6ebab7310f0e1c_key_manager_py.html` & `pyselector-0.0.9/htmlcov/d_2d6ebab7310f0e1c_key_manager_py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_2d6ebab7310f0e1c_logger_py.html` & `pyselector-0.0.9/htmlcov/d_2d6ebab7310f0e1c_logger_py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_2d6ebab7310f0e1c_selector_py.html` & `pyselector-0.0.9/htmlcov/d_2d6ebab7310f0e1c_selector_py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_a44f0ac069e85531___init___py.html` & `pyselector-0.0.9/htmlcov/d_a44f0ac069e85531___init___py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_a44f0ac069e85531_test_dmenu_py.html` & `pyselector-0.0.9/htmlcov/d_a44f0ac069e85531_test_dmenu_py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_a44f0ac069e85531_test_fzf_py.html` & `pyselector-0.0.9/htmlcov/d_a44f0ac069e85531_test_fzf_py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_a44f0ac069e85531_test_helpers_py.html` & `pyselector-0.0.9/htmlcov/d_a44f0ac069e85531_test_helpers_py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_a44f0ac069e85531_test_key_manager_py.html` & `pyselector-0.0.9/htmlcov/d_a44f0ac069e85531_test_key_manager_py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_a44f0ac069e85531_test_rofi_py.html` & `pyselector-0.0.9/htmlcov/d_a44f0ac069e85531_test_rofi_py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_a44f0ac069e85531_test_selector_py.html` & `pyselector-0.0.9/htmlcov/d_a44f0ac069e85531_test_selector_py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_c46c4fc7bbe4d838___init___py.html` & `pyselector-0.0.9/htmlcov/d_c46c4fc7bbe4d838___init___py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_c46c4fc7bbe4d838_dmenu_py.html` & `pyselector-0.0.9/htmlcov/d_c46c4fc7bbe4d838_dmenu_py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_c46c4fc7bbe4d838_fzf_py.html` & `pyselector-0.0.9/htmlcov/d_c46c4fc7bbe4d838_fzf_py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/d_c46c4fc7bbe4d838_rofi_py.html` & `pyselector-0.0.9/htmlcov/d_c46c4fc7bbe4d838_rofi_py.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/favicon_32.png` & `pyselector-0.0.9/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/index.html` & `pyselector-0.0.9/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/keybd_closed.png` & `pyselector-0.0.9/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/keybd_open.png` & `pyselector-0.0.9/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/status.json` & `pyselector-0.0.9/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/htmlcov/style.css` & `pyselector-0.0.9/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/404.html` & `pyselector-0.0.9/site/404.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/index.html` & `pyselector-0.0.9/site/index.html`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/images/favicon.png` & `pyselector-0.0.9/site/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/bundle.5a2dcb6a.min.js` & `pyselector-0.0.9/site/assets/javascripts/bundle.5a2dcb6a.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/bundle.5a2dcb6a.min.js.map` & `pyselector-0.0.9/site/assets/javascripts/bundle.5a2dcb6a.min.js.map`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/extra/bundle.5f09fbc3.min.js` & `pyselector-0.0.9/site/assets/javascripts/extra/bundle.5f09fbc3.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/extra/bundle.5f09fbc3.min.js.map` & `pyselector-0.0.9/site/assets/javascripts/extra/bundle.5f09fbc3.min.js.map`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/tinyseg.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/wordcut.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.ar.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.da.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.de.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.du.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.es.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.fi.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.fr.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.hi.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.hi.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.hu.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.it.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.ja.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.ko.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.ko.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.multi.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.nl.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.no.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.pt.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.ro.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.ru.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.sv.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.ta.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.ta.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.th.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.th.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.tr.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.vi.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/lunr/min/lunr.zh.min.js` & `pyselector-0.0.9/site/assets/javascripts/lunr/min/lunr.zh.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/workers/search.16e2a7d4.min.js` & `pyselector-0.0.9/site/assets/javascripts/workers/search.16e2a7d4.min.js`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/javascripts/workers/search.16e2a7d4.min.js.map` & `pyselector-0.0.9/site/assets/javascripts/workers/search.16e2a7d4.min.js.map`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/stylesheets/extra.0d2c79a8.min.css` & `pyselector-0.0.9/site/assets/stylesheets/extra.0d2c79a8.min.css`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/stylesheets/extra.0d2c79a8.min.css.map` & `pyselector-0.0.9/site/assets/stylesheets/extra.0d2c79a8.min.css.map`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/stylesheets/main.975780f9.min.css` & `pyselector-0.0.9/site/assets/stylesheets/main.975780f9.min.css`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/stylesheets/main.975780f9.min.css.map` & `pyselector-0.0.9/site/assets/stylesheets/main.975780f9.min.css.map`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/stylesheets/palette.2505c338.min.css` & `pyselector-0.0.9/site/assets/stylesheets/palette.2505c338.min.css`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/assets/stylesheets/palette.2505c338.min.css.map` & `pyselector-0.0.9/site/assets/stylesheets/palette.2505c338.min.css.map`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/site/search/search_index.json` & `pyselector-0.0.9/site/search/search_index.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940476190476191%*

 * *Differences: {"'docs'": "{5: {'text': 'PySelector Example # example.py from __future__ import annotations "*

 * *           'import functools import logging from typing import TYPE_CHECKING from typing import '*

 * *           'Optional from pyselector import Menu if TYPE_CHECKING: from pyselector.key_manager '*

 * *           'import Keybind items = [ {"name": "item0", "date": "2022-02-10", "category": "A"}, '*

 * *           '{"name": "item1", "date": "2022-03-20", "category": "A"}, {"name": "item2", "date": '*

 * *           '"2022-03-19", " […]*

```diff
@@ -32,15 +32,15 @@
         {
             "location": "#usage",
             "text": "This is a simple example from pyselector import Menu rofi = Menu.rofi() items = [ {\"name\": \"item0\", \"date\": \"2022-02-10\", \"category\": \"A\"}, {\"name\": \"item1\", \"date\": \"2022-03-20\", \"category\": \"A\"}, {\"name\": \"item2\", \"date\": \"2022-03-19\", \"category\": \"B\"}, {\"name\": \"item3\", \"date\": \"2022-03-18\", \"category\": \"A\"}, ] selection, code = rofi.prompt( items=items, case_sensitive=False, multi_select=False, prompt=\"PyExample> \", ) print(\">Selected:\", selection)",
             "title": "\ud83d\ude80 Usage"
         },
         {
             "location": "tutorials/",
-            "text": "PySelector Example # example.py from __future__ import annotations import functools import logging from typing import TYPE_CHECKING from typing import Optional from pyselector import Menu if TYPE_CHECKING: from pyselector.key_manager import Keybind items = [ {\"name\": \"item0\", \"date\": \"2022-02-10\", \"category\": \"A\"}, {\"name\": \"item1\", \"date\": \"2022-03-20\", \"category\": \"A\"}, {\"name\": \"item2\", \"date\": \"2022-03-19\", \"category\": \"B\"}, {\"name\": \"item3\", \"date\": \"2022-03-18\", \"category\": \"A\"}, {\"name\": \"item4\", \"date\": \"2022-03-21\", \"category\": \"C\"}, {\"name\": \"item5\", \"date\": \"2022-03-20\", \"category\": \"B\"}, ] def sort_by_key(key: str, items: list[dict[str, str]]) -> list[dict[str, str]]: return sorted(items, key=lambda x: x[key]) def parse_selection(menu: Menu, keycode: int, **kwargs) -> Optional[Keybind]: for key in menu.keybind.all_registered: if key.code == keycode: logging.info(\"keybind: %s\", key) return key return None def main() -> int: Menu.logging_debug(verbose=True) menu = Menu.rofi() menu.keybind.add( key=\"alt-d\", description=\"sort by date\", callback=lambda: \"date\", ) menu.keybind.add( key=\"alt-t\", description=\"sort by category\", callback=lambda: \"category\", ) menu.keybind.add( key=\"alt-n\", description=\"sort by name\", callback=lambda: \"name\", ) prompt = functools.partial( menu.prompt, prompt=\"PyExample>\", width=\"40%\", height=\"40%\" ) # Enter always returns 0 item, keycode = prompt(items=items) while keycode != 0: keybind = parse_selection(menu, keycode, item=item) sorted_items = sort_by_key(keybind.callback(), items=items) item, keycode = prompt(items=sorted_items) logging.info(\"selected: %s\", item) return 0 if __name__ == \"__main__\": raise SystemExit(main())",
+            "text": "PySelector Example # example.py from __future__ import annotations import functools import logging from typing import TYPE_CHECKING from typing import Optional from pyselector import Menu if TYPE_CHECKING: from pyselector.key_manager import Keybind items = [ {\"name\": \"item0\", \"date\": \"2022-02-10\", \"category\": \"A\"}, {\"name\": \"item1\", \"date\": \"2022-03-20\", \"category\": \"A\"}, {\"name\": \"item2\", \"date\": \"2022-03-19\", \"category\": \"B\"}, {\"name\": \"item3\", \"date\": \"2022-03-18\", \"category\": \"A\"}, {\"name\": \"item4\", \"date\": \"2022-03-21\", \"category\": \"C\"}, {\"name\": \"item5\", \"date\": \"2022-03-20\", \"category\": \"B\"}, ] def sort_by_key(key: str, items: list[dict[str, str]]) -> list[dict[str, str]]: return sorted(items, key=lambda x: x[key]) def parse_selection(menu: Menu, keycode: int, **kwargs) -> Optional[Keybind]: for key in menu.keybind.registered_keys: if key.code == keycode: logging.info(\"keybind: %s\", key) return key return None def main() -> int: Menu.logging_debug(verbose=True) menu = Menu.rofi() menu.keybind.add( key=\"alt-d\", description=\"sort by date\", callback=lambda: \"date\", ) menu.keybind.add( key=\"alt-t\", description=\"sort by category\", callback=lambda: \"category\", ) menu.keybind.add( key=\"alt-n\", description=\"sort by name\", callback=lambda: \"name\", ) prompt = functools.partial( menu.prompt, prompt=\"PyExample>\", width=\"40%\", height=\"40%\" ) # Enter always returns 0 item, keycode = prompt(items=items) while keycode != 0: keybind = parse_selection(menu, keycode, item=item) sorted_items = sort_by_key(keybind.callback(), items=items) item, keycode = prompt(items=sorted_items) logging.info(\"selected: %s\", item) return 0 if __name__ == \"__main__\": raise SystemExit(main())",
             "title": "Examples"
         },
         {
             "location": "tutorials/#pyselector-example",
             "text": "# example.py from __future__ import annotations import functools import logging from typing import TYPE_CHECKING from typing import Optional from pyselector import Menu if TYPE_CHECKING: from pyselector.key_manager import Keybind items = [ {\"name\": \"item0\", \"date\": \"2022-02-10\", \"category\": \"A\"}, {\"name\": \"item1\", \"date\": \"2022-03-20\", \"category\": \"A\"}, {\"name\": \"item2\", \"date\": \"2022-03-19\", \"category\": \"B\"}, {\"name\": \"item3\", \"date\": \"2022-03-18\", \"category\": \"A\"}, {\"name\": \"item4\", \"date\": \"2022-03-21\", \"category\": \"C\"}, {\"name\": \"item5\", \"date\": \"2022-03-20\", \"category\": \"B\"}, ] def sort_by_key(key: str, items: list[dict[str, str]]) -> list[dict[str, str]]: return sorted(items, key=lambda x: x[key]) def parse_selection(menu: Menu, keycode: int, **kwargs) -> Optional[Keybind]: for key in menu.keybind.all_registered: if key.code == keycode: logging.info(\"keybind: %s\", key) return key return None def main() -> int: Menu.logging_debug(verbose=True) menu = Menu.rofi() menu.keybind.add( key=\"alt-d\", description=\"sort by date\", callback=lambda: \"date\", ) menu.keybind.add( key=\"alt-t\", description=\"sort by category\", callback=lambda: \"category\", ) menu.keybind.add( key=\"alt-n\", description=\"sort by name\", callback=lambda: \"name\", ) prompt = functools.partial( menu.prompt, prompt=\"PyExample>\", width=\"40%\", height=\"40%\" ) # Enter always returns 0 item, keycode = prompt(items=items) while keycode != 0: keybind = parse_selection(menu, keycode, item=item) sorted_items = sort_by_key(keybind.callback(), items=items) item, keycode = prompt(items=sorted_items) logging.info(\"selected: %s\", item) return 0 if __name__ == \"__main__\": raise SystemExit(main())",
             "title": "PySelector Example"
         }
```

### Comparing `pyselector-0.0.8b0/site/tutorials/index.html` & `pyselector-0.0.9/site/tutorials/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
 
 
 def sort_by_key(key: str, items: list[dict[str, str]]) -&gt; list[dict[str, str]]:
     return sorted(items, key=lambda x: x[key])
 
 
 def parse_selection(menu: Menu, keycode: int, **kwargs) -&gt; Optional[Keybind]:
-    for key in menu.keybind.all_registered:
+    for key in menu.keybind.registered_keys:
         if key.code == keycode:
             logging.info(&quot;keybind: %s&quot;, key)
             return key
     return None
 
 
 def main() -&gt; int:
@@ -348,8 +348,8 @@
     
     
       <script src="../assets/javascripts/bundle.5a2dcb6a.min.js"></script>
       
     
     
   </body>
-</html>
+</html>
```

#### html2text {}

```diff
@@ -42,15 +42,15 @@
 
 
 def sort_by_key(key: str, items: list[dict[str, str]]) -> list[dict[str, str]]:
     return sorted(items, key=lambda x: x[key])
 
 
 def parse_selection(menu: Menu, keycode: int, **kwargs) -> Optional[Keybind]:
-    for key in menu.keybind.all_registered:
+    for key in menu.keybind.registered_keys:
         if key.code == keycode:
             logging.info("keybind: %s", key)
             return key
     return None
 
 
 def main() -> int:
```

### Comparing `pyselector-0.0.8b0/src/pyselector/helpers.py` & `pyselector-0.0.9/src/pyselector/helpers.py`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/src/pyselector/interfaces.py` & `pyselector-0.0.9/src/pyselector/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/src/pyselector/key_manager.py` & `pyselector-0.0.9/src/pyselector/key_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # keybinds.py
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Any
 from typing import Callable
 from typing import Optional
 
@@ -37,32 +38,36 @@
     action: Optional[str] = ""
     hidden: bool = True
     callback: Optional[Callable[..., Any]] = None
 
     def toggle_hidden(self) -> None:
         self.hidden = not self.hidden
 
+    def __hash__(self):
+        return hash((self.code, self.description))
+
 
 class KeyManager:
     """
     A class for managing keybinds, which are associations between key combinations
     and callback functions.
 
     Attributes:
         keys        (dict[str, Keybind]): A dictionary mapping keybinds to their corresponding `Keybind` objects.
         key_count   (int): A counter for assigning unique IDs to newly added keybinds.
         code_count  (int): A counter for assigning unique codes to newly added keybinds.
         temp_hidden (list[Keybind]): A list of temporarily hidden keybinds.
     """
 
     def __init__(self) -> None:
-        self.keys: dict[str, Keybind] = {}
+        self.keys: dict[int, Keybind] = {}
         self.key_count = 1
         self.code_count = 1
         self.temp_hidden: list[Keybind] = []
+        self.original_states: dict[Keybind, bool] = {}
 
     def add(
         self,
         key: str,
         description: str,
         callback: Callable[..., Any],
         hidden: bool = False,
@@ -87,67 +92,99 @@
                 description=description,
                 hidden=hidden,
                 callback=callback,
             ),
             exist_ok=exist_ok,
         )
 
-    def unregister(self, bind: str) -> None:
+    def unregister(self, code: int) -> None:
         """Removes the keybind with the specified bind."""
-        if not self.keys.get(bind):
-            raise KeybindError(f"{bind=} not found")
-        self.keys.pop(bind)
+        if not self.keys.get(code):
+            raise KeybindError(f"No keybind found with {code=}")
+        self.keys.pop(code)
+
+    def unregister_all(self) -> None:
+        """Removes all registered keybinds."""
+        self.keys.clear()
 
     def register(self, key: Keybind, exist_ok: bool = False) -> Keybind:
         """
         Args:
             key     (Keybind): The keybind to register.
             exist_ok (bool): Whether to overwrite an existing keybind with the same bind. Defaults to False.
 
         Returns:
             Keybind: The registered keybind.
 
         Raises:
             KeybindError: If `exist_ok` is False and a keybind with the same bind is already registered.
         """
-        if exist_ok and self.keys.get(key.bind):
-            self.unregister(key.bind)
+        if exist_ok and self.keys.get(key.code):
+            self.unregister(key.code)
 
-        if self.keys.get(key.bind):
+        if self.keys.get(key.code):
             raise KeybindError(f"{key.bind=} already registered")
 
         self.key_count += 1
         self.code_count += 1
-        self.keys[key.bind] = key
-        return key
-
-    def patch(self, bind: str) -> Keybind:
-        # FIX: delete me
-        key = self.keys.get(bind)
-        if not key:
-            raise KeybindError(f"{bind=} not found")
+        self.keys[key.code] = key
         return key
 
     @property
-    def all_registered(self) -> list[Keybind]:
+    def registered_keys(self) -> list[Keybind]:
         return list(self.keys.values())
 
     def toggle_all(self) -> None:
         """Toggles the "hidden" property of all non-hidden keybinds."""
-        for key in self.all_registered:
+        for key in self.registered_keys:
             if not key.hidden:
                 key.hidden = True
 
     def toggle_hidden(self, restore: bool = False) -> None:
         """
         Toggles the "hidden" property of all non-hidden keybinds, and
         temporarily stores the original "hidden" state of each keybind.
         If `restore` is True, restores the original "hidden" state of each keybind.
         """
-        for key in self.all_registered:
+        for key in self.registered_keys:
             if not key.hidden:
                 key.toggle_hidden()
                 self.temp_hidden.append(key)
         if restore:
             for key in self.temp_hidden:
                 key.toggle_hidden()
             self.temp_hidden = []
+
+    def toggle_nonhidden_keys(self, restore: bool = False) -> None:
+        """
+        Toggles the "hidden" property of all non-hidden keybinds, and temporarily
+        stores the original "hidden" state of each keybind. If `restore` is True,
+        restores the original "hidden" state of each keybind.
+        """
+        if not restore:
+            self.original_states = {
+                key: key.hidden for key in self.registered_keys if not key.hidden
+            }
+
+        for key in self.registered_keys:
+            if not key.hidden:
+                key.toggle_hidden()
+
+        if restore:
+            try:
+                for key, state in self.original_states.items():
+                    if state:
+                        key.toggle_hidden()
+            finally:
+                self.original_states.clear()
+
+    def get_keybind_by_code(self, code: int) -> Keybind:
+        """
+        Returns the keybind with the specified code.
+
+        Raises:
+            KeybindError: If no keybind is found with the specified code.
+        """
+        try:
+            return self.keys[code]
+        except KeyError:
+            raise KeybindError(f"No keybind found with {code=}") from None
```

### Comparing `pyselector-0.0.8b0/src/pyselector/logger.py` & `pyselector-0.0.9/src/pyselector/logger.py`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/src/pyselector/selector.py` & `pyselector-0.0.9/src/pyselector/selector.py`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/src/pyselector/menus/dmenu.py` & `pyselector-0.0.9/src/pyselector/menus/dmenu.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,26 +42,29 @@
         if prompt:
             args.extend(["-p", prompt])
 
         if kwargs.get("bottom"):
             kwargs.pop("bottom")
             args.append("-b")
 
-        if case_sensitive:
+        if not case_sensitive:
             args.append("-i")
 
         if kwargs.get("font"):
             args.extend(["-fn", kwargs.pop("font")])
 
         if multi_select:
             log.warning("not supported in dmenu: %s", "multi-select")
 
+        for key in self.keybind.registered_keys:
+            log.warning("key=%s not supported in dmenu", key)
+
         if kwargs:
             for arg, value in kwargs.items():
-                log.debug("'%s=%s' not supported", arg, value)
+                log.warning("'%s=%s' not supported", arg, value)
         return args
 
     def prompt(
         self,
         items: Optional[Iterable[Union[str, int]]] = None,
         case_sensitive: bool = False,
         multi_select: bool = False,
```

### Comparing `pyselector-0.0.8b0/src/pyselector/menus/fzf.py` & `pyselector-0.0.9/src/pyselector/menus/fzf.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,23 +52,24 @@
         if prompt:
             args.extend(["--prompt", prompt])
 
         if multi_select:
             args.append("--multi")
 
         # FIX: rethink keybinds for FZF
-        log.debug("keybinds are disabled")
-        for key in self.keybind.all_registered:
-            args.extend(shlex.split(f"--bind='{key.bind}:{key.action}'"))
-            if not key.hidden:
-                header.append(f"Use {key.bind} {key.description}")
+        # log.warning("keybinds are disabled")
+        for key in self.keybind.registered_keys:
+            log.warning("key=%s not supported in fzf", key)
+            # args.extend(shlex.split(f"--bind='{key.bind}:{key.action}'"))
+            # if not key.hidden:
+            #     header.append(f"Use {key.bind} {key.description}")
 
         if kwargs:
             for arg, value in kwargs.items():
-                log.debug("'%s=%s' not supported", arg, value)
+                log.warning("'%s=%s' not supported", arg, value)
 
         if header:
             mesg = "\n".join(msg.replace("\n", " ") for msg in header)
             args.extend(shlex.split(f"--header '{mesg}'"))
 
         return args
```

### Comparing `pyselector-0.0.8b0/src/pyselector/menus/rofi.py` & `pyselector-0.0.9/src/pyselector/menus/rofi.py`

 * *Files 20% similar despite different names*

```diff
@@ -57,24 +57,29 @@
     ) -> list[str]:
         messages: list[str] = []
         dimensions_args: list[str] = []
         args = []
 
         args.extend(shlex.split(self.command))
         args.append("-dmenu")
+        args.append("-sync")
 
         if kwargs.get("theme"):
             args.extend(["-theme", kwargs.pop("theme")])
 
         if kwargs.get("lines"):
             args.extend(["-l", str(kwargs.pop("lines"))])
 
         if prompt:
             args.extend(["-p", prompt])
 
+        if kwargs.get("markup"):
+            del kwargs["markup"]
+            args.append("-markup-rows")
+
         if kwargs.get("mesg"):
             messages.extend(shlex.split(f"'{kwargs.pop('mesg')}'"))
 
         if kwargs.get("filter"):
             args.extend(["-filter", kwargs.pop("filter")])
 
         if kwargs.get("location"):
@@ -95,28 +100,36 @@
         if multi_select:
             args.append("-multi-select")
 
         if dimensions_args:
             formated_string = " ".join(dimensions_args)
             args.extend(shlex.split("-theme-str 'window {" + formated_string + "}'"))
 
-        for key in self.keybind.all_registered:
+        for key in self.keybind.registered_keys:
             args.extend(shlex.split(f"-kb-custom-{key.id} {key.bind}"))
             if not key.hidden:
                 messages.append(f"{BULLET} Use <{key.bind}> {key.description}")
 
         if messages:
             mesg = "\n".join(messages)
             args.extend(shlex.split(f"-mesg '{mesg}'"))
 
         if kwargs:
             for arg, value in kwargs.items():
                 log.debug("'%s=%s' not supported", arg, value)
 
-        args.extend(shlex.split("-theme-str 'textbox { markup: false;}'"))
+        # FIX:
+        # if kwargs.get("title_markup"):
+        #     log.error(kwargs.get("title_markup"))
+        #     args.extend(shlex.split("-theme-str 'textbox { markup: true;}'"))
+        # else:
+        #     args.extend(shlex.split("-theme-str 'textbox { markup: false;}'"))
+        title_markup = "true" if kwargs.pop("title_markup", False) else "false"
+        args.extend(shlex.split(f"-theme-str 'textbox {{ markup: {title_markup};}}'"))
+
         return args
 
     def prompt(
         self,
         items: Optional[Iterable[Union[str, int]]] = None,
         case_sensitive: bool = False,
         multi_select: bool = False,
@@ -139,15 +152,20 @@
             filter   (str): Filter the list by setting text in input bar to filter.
             location (str): The location of the selection window (e.g. "upper-left", "center" or "bottom-right").
             width    (str): The width of the selection window (e.g. 60%).
             height   (str): The height of the selection window (e.g. 50%).
             theme    (str): The path of the rofi theme to use.
 
         Returns:
-            A tuple containing the selected item (str or list of str if `multi_select` activated) and the return code (int).
+            A tuple containing the selected item (str or list of str if `multi_select` enabled) and the return code (int).
+
+        Return Code Value
+            0: Row has been selected accepted by user.
+            1: User cancelled the selection.
+            10-28: Row accepted by custom keybinding.
         """
         if items is None:
             items = []
 
         args = self._build_command(case_sensitive, multi_select, prompt, **kwargs)
         selection, code = helpers._execute(args, items)
```

### Comparing `pyselector-0.0.8b0/tests/test_dmenu.py` & `pyselector-0.0.9/tests/test_dmenu.py`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/tests/test_fzf.py` & `pyselector-0.0.9/tests/test_fzf.py`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/tests/test_helpers.py` & `pyselector-0.0.9/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/tests/test_key_manager.py` & `pyselector-0.0.9/tests/test_key_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,28 +88,28 @@
         code=10,
         description=description,
         hidden=hidden,
         callback=lambda: None,
     )
     key_manager.register(keybind)
     key_manager.unregister(bind)
-    assert key_manager.all_registered == []
+    assert key_manager.registered_keys == []
 
 
 def test_unregister_keybind_error(key_manager: KeyManager) -> None:
     with pytest.raises(KeybindError):
         key_manager.unregister("CTRL+XX")
 
 
 def test_toggle_all_keybinds(key_manager: KeyManager) -> None:
     key_manager.add("CTRL+S", "Save file", lambda: None)
     key_manager.add("CTRL+Z", "Undo last action", lambda: None)
     key_manager.add("CTRL+X", "Cut selected text", lambda: None)
     key_manager.toggle_all()
-    for keybind in key_manager.all_registered:
+    for keybind in key_manager.registered_keys:
         assert keybind.hidden
 
 
 def test_toggle_hidden_keybinds(key_manager: KeyManager) -> None:
     key_manager.add("CTRL+S", "Save file", lambda: None, hidden=False)
     key_manager.add("CTRL+Z", "Undo last action", lambda: None, hidden=False)
     key_manager.add("CTRL+X", "Cut selected text", lambda: None, hidden=False)
```

### Comparing `pyselector-0.0.8b0/tests/test_rofi.py` & `pyselector-0.0.9/tests/test_rofi.py`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/pyproject.toml` & `pyselector-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyselector-0.0.8b0/PKG-INFO` & `pyselector-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyselector
-Version: 0.0.8b0
+Version: 0.0.9
 Summary: WIP
 Author-email: haaag <git.haaag@gmail.com>
 License-Expression: MIT
 Keywords: cli,dmenu,fzf,menu,rofi,utility
 Requires-Python: >=3.7
 Provides-Extra: dev
 Requires-Dist: mypy==1.0.1; extra == 'dev'
```

