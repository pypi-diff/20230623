# Comparing `tmp/openllm-0.1.8.tar.gz` & `tmp/openllm-0.1.9.tar.gz`

## Comparing `openllm-0.1.8.tar` & `openllm-0.1.9.tar`

### file list

```diff
@@ -1,149 +1,149 @@
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 openllm-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.1.8/ADDING_NEW_MODEL.md
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 openllm-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 openllm-0.1.8/DEVELOPMENT.md
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 openllm-0.1.8/nightly-requirements.generated.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.1.8/package.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.1.8/taplo.toml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/CODEOWNERS
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/SECURITY.md
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/dependabot.yml
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/ISSUE_TEMPLATE/feature_request.yml
--rwxr-xr-x   0        0        0     1428 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/actions/create_release_and_archive.sh
--rwxr-xr-x   0        0        0     1853 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/actions/release.sh
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/actions/setup-repo/action.yml
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/workflows/create-releases.yml
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/workflows/release-notes.yml
--rw-r--r--   0        0        0  1264669 2020-02-02 00:00:00.000000 openllm-0.1.8/assets/main-banner.png
--rw-r--r--   0        0        0 10631249 2020-02-02 00:00:00.000000 openllm-0.1.8/assets/output.gif
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 openllm-0.1.8/changelog.d/template.md.jinja
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/bentoml-demo/bentofile.yaml
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/bentoml-demo/service.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-chains-demo/README.md
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-chains-demo/bentofile.yaml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-chains-demo/download_model.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-chains-demo/service.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-tools-demo/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-tools-demo/bentofile.yaml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-tools-demo/bentoml_configuration.yaml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-tools-demo/download_model.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-tools-demo/requirements.txt
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-tools-demo/service.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/__about__.py
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/__main__.py
--rw-r--r--   0        0        0    54358 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_configuration.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_generation.py
--rw-r--r--   0        0        0    43521 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_llm.py
--rw-r--r--   0        0        0    13551 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_package.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_prompt.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_schema.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_service.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_types.py
--rw-r--r--   0        0        0    48388 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/cli.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/client.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/py.typed
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/auto/__init__.py
--rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/auto/configuration_auto.py
--rw-r--r--   0        0        0    12738 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/auto/factory.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/auto/modeling_auto.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/auto/modeling_flax_auto.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/auto/modeling_tf_auto.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/chatglm/__init__.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/chatglm/configuration_chatglm.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/chatglm/modeling_chatglm.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/dolly_v2/__init__.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/dolly_v2/configuration_dolly_v2.py
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/dolly_v2/modeling_dolly_v2.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/falcon/__init__.py
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/falcon/configuration_falcon.py
--rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/falcon/modeling_falcon.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/flan_t5/configuration_flan_t5.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/flan_t5/modeling_flan_t5.py
--rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/gpt_neox/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/llama/__init__.py
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/opt/__init__.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/opt/configuration_opt.py
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/opt/modeling_flax_opt.py
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/opt/modeling_opt.py
--rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/opt/modeling_tf_opt.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/roberta/__init__.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/stablelm/__init__.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/stablelm/configuration_stablelm.py
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/stablelm/modeling_stablelm.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/starcoder/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/starcoder/configuration_starcoder.py
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/starcoder/modeling_starcoder.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/playground/README
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/playground/__init__.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/playground/features.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/playground/ft_opt_lora.py
--rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/__init__.py
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/analytics.py
--rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/codegen.py
--rw-r--r--   0        0        0    15488 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/dantic.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/dummy_flax_objects.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/dummy_pt_and_einops_objects.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/dummy_pt_objects.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/dummy_tf_objects.py
--rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/import_utils.py
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/lazy.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_client/_prompt.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_client/runtimes/__init__.py
--rw-r--r--   0        0        0    11495 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_client/runtimes/base.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_client/runtimes/grpc.py
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_client/runtimes/http.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_js/package.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_js/tsconfig.cjs.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_js/tsconfig.json
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/test_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/_strategies/__init__.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/_strategies/_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/models/flan_t5/test_modeling_flan_t5.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/models/opt/__init__.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/models/opt/test_modeling_opt.py
--rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 openllm-0.1.8/tools/add-license-headers
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 openllm-0.1.8/tools/assert-license-headers
--rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 openllm-0.1.8/tools/assert-model-table-latest
--rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 openllm-0.1.8/tools/run-release-action
--rwxr-xr-x   0        0        0     5012 2020-02-02 00:00:00.000000 openllm-0.1.8/tools/update-optional-dependencies.py
--rwxr-xr-x   0        0        0     3575 2020-02-02 00:00:00.000000 openllm-0.1.8/tools/update-readme.py
--rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/__init__.pyi
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/_cmp.pyi
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/_compat.pyi
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/_typing_compat.pyi
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/_version_info.pyi
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/converters.pyi
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/exceptions.pyi
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/filters.pyi
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/setters.pyi
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/validators.pyi
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/click_option_group/__init__.pyi
--rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/click_option_group/_core.pyi
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/click_option_group/_decorators.pyi
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/click_option_group/_helpers.pyi
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/click_option_group/_version.pyi
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/deepmerge/__init__.pyi
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/deepmerge/merger.pyi
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/deepmerge/strategy/core.pyi
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/deepmerge/strategy/dict.pyi
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/deepmerge/strategy/list.pyi
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/deepmerge/strategy/set.pyi
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 openllm-0.1.8/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.1.8/LICENSE.md
--rw-r--r--   0        0        0    14995 2020-02-02 00:00:00.000000 openllm-0.1.8/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 openllm-0.1.8/hatch.toml
--rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 openllm-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    18257 2020-02-02 00:00:00.000000 openllm-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 openllm-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.1.9/ADDING_NEW_MODEL.md
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 openllm-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 openllm-0.1.9/DEVELOPMENT.md
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 openllm-0.1.9/nightly-requirements.generated.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.1.9/package.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.1.9/taplo.toml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 openllm-0.1.9/.github/CODEOWNERS
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 openllm-0.1.9/.github/SECURITY.md
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openllm-0.1.9/.github/dependabot.yml
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 openllm-0.1.9/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 openllm-0.1.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openllm-0.1.9/.github/ISSUE_TEMPLATE/feature_request.yml
+-rwxr-xr-x   0        0        0     1428 2020-02-02 00:00:00.000000 openllm-0.1.9/.github/actions/create_release_and_archive.sh
+-rwxr-xr-x   0        0        0     1853 2020-02-02 00:00:00.000000 openllm-0.1.9/.github/actions/release.sh
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 openllm-0.1.9/.github/actions/setup-repo/action.yml
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 openllm-0.1.9/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 openllm-0.1.9/.github/workflows/create-releases.yml
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 openllm-0.1.9/.github/workflows/release-notes.yml
+-rw-r--r--   0        0        0  1264669 2020-02-02 00:00:00.000000 openllm-0.1.9/assets/main-banner.png
+-rw-r--r--   0        0        0 10631249 2020-02-02 00:00:00.000000 openllm-0.1.9/assets/output.gif
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 openllm-0.1.9/changelog.d/template.md.jinja
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 openllm-0.1.9/examples/bentoml-demo/bentofile.yaml
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 openllm-0.1.9/examples/bentoml-demo/service.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 openllm-0.1.9/examples/langchain-chains-demo/README.md
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openllm-0.1.9/examples/langchain-chains-demo/bentofile.yaml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.9/examples/langchain-chains-demo/download_model.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 openllm-0.1.9/examples/langchain-chains-demo/service.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 openllm-0.1.9/examples/langchain-tools-demo/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 openllm-0.1.9/examples/langchain-tools-demo/bentofile.yaml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.1.9/examples/langchain-tools-demo/bentoml_configuration.yaml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.9/examples/langchain-tools-demo/download_model.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 openllm-0.1.9/examples/langchain-tools-demo/requirements.txt
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 openllm-0.1.9/examples/langchain-tools-demo/service.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/__about__.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/__main__.py
+-rw-r--r--   0        0        0    54358 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/_configuration.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/_generation.py
+-rw-r--r--   0        0        0    43524 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/_llm.py
+-rw-r--r--   0        0        0    13580 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/_package.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/_prompt.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/_schema.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/_service.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/_types.py
+-rw-r--r--   0        0        0    48288 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/cli.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/client.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/py.typed
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/auto/__init__.py
+-rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/auto/configuration_auto.py
+-rw-r--r--   0        0        0    12738 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/auto/factory.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/auto/modeling_auto.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/auto/modeling_flax_auto.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/auto/modeling_tf_auto.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/chatglm/__init__.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/dolly_v2/__init__.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/dolly_v2/configuration_dolly_v2.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/dolly_v2/modeling_dolly_v2.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/falcon/__init__.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/falcon/configuration_falcon.py
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/falcon/modeling_falcon.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/flan_t5/configuration_flan_t5.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/flan_t5/modeling_flan_t5.py
+-rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/gpt_neox/__init__.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/llama/__init__.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/opt/__init__.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/opt/configuration_opt.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/opt/modeling_flax_opt.py
+-rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/opt/modeling_opt.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/opt/modeling_tf_opt.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/roberta/__init__.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/stablelm/configuration_stablelm.py
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/stablelm/modeling_stablelm.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/starcoder/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/starcoder/configuration_starcoder.py
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/models/starcoder/modeling_starcoder.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/playground/README
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/playground/__init__.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/playground/features.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/playground/ft_opt_lora.py
+-rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/utils/__init__.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/utils/analytics.py
+-rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/utils/codegen.py
+-rw-r--r--   0        0        0    15488 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/utils/dantic.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/utils/dummy_flax_objects.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/utils/dummy_pt_and_einops_objects.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/utils/dummy_pt_objects.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/utils/dummy_tf_objects.py
+-rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/utils/import_utils.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm/utils/lazy.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm_client/_prompt.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm_client/runtimes/__init__.py
+-rw-r--r--   0        0        0    11495 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm_client/runtimes/base.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm_client/runtimes/grpc.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm_client/runtimes/http.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm_js/package.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm_js/tsconfig.cjs.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.1.9/src/openllm_js/tsconfig.json
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 openllm-0.1.9/tests/test_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.9/tests/_strategies/__init__.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 openllm-0.1.9/tests/_strategies/_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.9/tests/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 openllm-0.1.9/tests/models/flan_t5/test_modeling_flan_t5.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.9/tests/models/opt/__init__.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 openllm-0.1.9/tests/models/opt/test_modeling_opt.py
+-rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 openllm-0.1.9/tools/add-license-headers
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 openllm-0.1.9/tools/assert-license-headers
+-rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 openllm-0.1.9/tools/assert-model-table-latest
+-rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 openllm-0.1.9/tools/run-release-action
+-rwxr-xr-x   0        0        0     5012 2020-02-02 00:00:00.000000 openllm-0.1.9/tools/update-optional-dependencies.py
+-rwxr-xr-x   0        0        0     3575 2020-02-02 00:00:00.000000 openllm-0.1.9/tools/update-readme.py
+-rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/attr/__init__.pyi
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/attr/_cmp.pyi
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/attr/_compat.pyi
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/attr/_typing_compat.pyi
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/attr/_version_info.pyi
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/attr/converters.pyi
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/attr/exceptions.pyi
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/attr/filters.pyi
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/attr/setters.pyi
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/attr/validators.pyi
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/click_option_group/__init__.pyi
+-rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/click_option_group/_core.pyi
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/click_option_group/_decorators.pyi
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/click_option_group/_helpers.pyi
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/click_option_group/_version.pyi
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/deepmerge/__init__.pyi
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/deepmerge/merger.pyi
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/deepmerge/strategy/core.pyi
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/deepmerge/strategy/dict.pyi
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/deepmerge/strategy/list.pyi
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 openllm-0.1.9/typings/deepmerge/strategy/set.pyi
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 openllm-0.1.9/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0    15000 2020-02-02 00:00:00.000000 openllm-0.1.9/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 openllm-0.1.9/hatch.toml
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 openllm-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    18262 2020-02-02 00:00:00.000000 openllm-0.1.9/PKG-INFO
```

### Comparing `openllm-0.1.8/.pre-commit-config.yaml` & `openllm-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/ADDING_NEW_MODEL.md` & `openllm-0.1.9/ADDING_NEW_MODEL.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/CHANGELOG.md` & `openllm-0.1.9/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,22 @@
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 -->
 
 <!-- towncrier release notes start -->
 
+## [0.1.9](https://github.com/bentoml/openllm/tree/v0.1.9)
+
+### Changes
+
+- Fixes setting logs for agents to info instead of logger object.
+  [#37](https://github.com/bentoml/openllm/issues/37)
+
+
 ## [0.1.8](https://github.com/bentoml/openllm/tree/v0.1.8)
 No significant changes.
 
 
 ## [0.1.7](https://github.com/bentoml/openllm/tree/v0.1.7)
 
 ### Features
```

### Comparing `openllm-0.1.8/DEVELOPMENT.md` & `openllm-0.1.9/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/nightly-requirements.generated.txt` & `openllm-0.1.9/nightly-requirements.generated.txt`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/package.json` & `openllm-0.1.9/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.1.9'"}*

```diff
@@ -11,12 +11,12 @@
     "engines": {
         "node": ">=16"
     },
     "license": "Apache 2.0",
     "name": "openllm",
     "private": true,
     "repository": "git@github.com:llmsys/OpenLLM.git",
-    "version": "0.1.8",
+    "version": "0.1.9",
     "workspaces": [
         "src/openllm_js"
     ]
 }
```

### Comparing `openllm-0.1.8/.github/SECURITY.md` & `openllm-0.1.9/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/.github/dependabot.yml` & `openllm-0.1.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/.github/ISSUE_TEMPLATE/bug_report.yml` & `openllm-0.1.9/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files 10% similar despite different names*

```diff
@@ -26,34 +26,34 @@
   - type: textarea
     id: describe-the-bug
     validations:
       required: true
     attributes:
       label: Describe the bug
       description: |
-        Please provide a clear and concise description about the problem you ran into.
+        Please provide a clear and concise description of the problem you ran into.
       placeholder: This happened when I...
   - type: textarea
     id: to-reproduce
     validations:
       required: false
     attributes:
       label: To reproduce
       description: |
-        Please provide a code sample or a code snipet to reproduce said problem. If you have code snippets, error messages, stack trace please also provide them here.
+        Please provide a code sample or a code snippet to reproduce said problem. If you have code snippets, error messages, stack trace please also provide them here.
 
         **IMPORTANT**: make sure to use [code tag](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-and-highlighting-code-blocks#syntax-highlighting) to correctly format your code. Screenshot is helpful but don't use it for code snippets as it doesn't allow others to copy-and-paste your code.
 
         To give us more information for diagnosing the issue, it would be great if you can provide a minimal reproducible!
       placeholder: |
         Steps to reproduce the bug:
 
           1. Provide '...'
           2. Run '...'
-          3. See error
+          3. See the error
   - type: textarea
     id: logs
     attributes:
       label: Logs
       description: 'Please include the Python logs if you can.'
       render: shell
   - type: textarea
@@ -65,7 +65,19 @@
       placeholder: |
         bentoml: ...
         transformers: ...
         python: ...
         platform: ...
     validations:
       required: true
+  - type: textarea
+    id: system-info
+    attributes:
+      label: System information (Optional)
+      description: |
+        Please share your system information with us.
+      placeholder: |
+        memory: ...
+        platform: ...
+        architecture: ...
+        CPU: ...
+        GPU: ...
```

### Comparing `openllm-0.1.8/.github/ISSUE_TEMPLATE/config.yml` & `openllm-0.1.9/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/.github/ISSUE_TEMPLATE/feature_request.yml` & `openllm-0.1.9/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/.github/actions/create_release_and_archive.sh` & `openllm-0.1.9/.github/actions/create_release_and_archive.sh`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/.github/actions/release.sh` & `openllm-0.1.9/.github/actions/release.sh`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/.github/actions/setup-repo/action.yml` & `openllm-0.1.9/.github/actions/setup-repo/action.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/.github/workflows/ci.yml` & `openllm-0.1.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/.github/workflows/create-releases.yml` & `openllm-0.1.9/.github/workflows/create-releases.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/.github/workflows/release-notes.yml` & `openllm-0.1.9/.github/workflows/release-notes.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/assets/main-banner.png` & `openllm-0.1.9/assets/main-banner.png`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/assets/output.gif` & `openllm-0.1.9/assets/output.gif`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/changelog.d/template.md.jinja` & `openllm-0.1.9/changelog.d/template.md.jinja`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/examples/bentoml-demo/bentofile.yaml` & `openllm-0.1.9/examples/bentoml-demo/bentofile.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/examples/bentoml-demo/service.py` & `openllm-0.1.9/examples/bentoml-demo/service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/examples/langchain-chains-demo/bentofile.yaml` & `openllm-0.1.9/examples/langchain-chains-demo/bentofile.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/examples/langchain-chains-demo/download_model.py` & `openllm-0.1.9/examples/langchain-chains-demo/download_model.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/examples/langchain-chains-demo/service.py` & `openllm-0.1.9/examples/langchain-chains-demo/service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/examples/langchain-tools-demo/bentofile.yaml` & `openllm-0.1.9/examples/langchain-tools-demo/bentofile.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/examples/langchain-tools-demo/bentoml_configuration.yaml` & `openllm-0.1.9/examples/langchain-tools-demo/bentoml_configuration.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/examples/langchain-tools-demo/download_model.py` & `openllm-0.1.9/examples/langchain-tools-demo/download_model.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/examples/langchain-tools-demo/service.py` & `openllm-0.1.9/examples/langchain-tools-demo/service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/__about__.py` & `openllm-0.1.9/src/openllm/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

### Comparing `openllm-0.1.8/src/openllm/__init__.py` & `openllm-0.1.9/src/openllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/__main__.py` & `openllm-0.1.9/src/openllm/__main__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/_configuration.py` & `openllm-0.1.9/src/openllm/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/_generation.py` & `openllm-0.1.9/src/openllm/_generation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/_llm.py` & `openllm-0.1.9/src/openllm/_llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,15 +464,15 @@
         int8_has_fp16_weight = attrs.pop("llm_int8_has_fp16_weight", False)
         # 4 bit configuration
         int4_compute_dtype = attrs.pop("llm_bnb_4bit_compute_dtype", torch.bfloat16)
         int4_quant_type = attrs.pop("llm_bnb_4bit_quant_type", "nf4")
         int4_use_double_quant = attrs.pop("llm_bnb_4bit_use_double_quant", True)
 
         if llm_config is not None:
-            logger.debug("Using provided LLMConfig to initialize LLM instead of from default.", llm_config)
+            logger.debug("Using provided LLMConfig to initialize LLM instead of from default: %r", llm_config)
             self.config = llm_config
         else:
             self.config = self.config_class.model_construct_env(**attrs)
             # The rests of the kwargs that is not used by the config class should be stored into __openllm_extras__.
             attrs = self.config["extras"]
 
         if quantization_config and quantize:
```

### Comparing `openllm-0.1.8/src/openllm/_package.py` & `openllm-0.1.9/src/openllm/_package.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         f'runners."llm-{llm.config["start_name"]}-runner".workers_per_resource={workers_per_resource}',
     ]
     _bentoml_config_options += " " if _bentoml_config_options else "" + " ".join(_bentoml_config_options_opts)
     env: ModelEnv = llm.config["env"]
 
     env_dict = {
         env.framework: env.framework_value,
-        env.config: llm.config.model_dump_json().decode(),
+        env.config: f"'{llm.config.model_dump_json().decode()}'",
         "OPENLLM_MODEL": llm.config["model_name"],
         "OPENLLM_MODEL_ID": llm.model_id,
         "BENTOML_DEBUG": str(get_debug_mode()),
         "BENTOML_CONFIG_OPTIONS": _bentoml_config_options,
     }
 
     # We need to handle None separately here, as env from subprocess doesn't
@@ -229,15 +229,17 @@
     labels.update({"_type": llm.llm_type, "_framework": framework_envvar})
     logger.info("Building Bento for LLM '%s'", llm.config["start_name"])
     return bentoml.bentos.build(
         f"{service_name}:svc",
         name=bento_tag.name,
         labels=labels,
         description=f"OpenLLM service for {llm.config['start_name']}",
-        include=list(llm_fs.walk.files(filter=["*.py"])),  # NOTE: By default, we are using _service.py as the default service, for now.
+        include=list(
+            llm_fs.walk.files(filter=["*.py"])
+        ),  # NOTE: By default, we are using _service.py as the default service, for now.
         exclude=["/venv", "__pycache__/", "*.py[cod]", "*$py.class"],
         python=construct_python_options(llm, llm_fs, extra_dependencies),
         docker=construct_docker_options(llm, llm_fs, workers_per_resource, quantize, bettertransformer),
         version=bento_tag.version,
         build_ctx=llm_fs.getsyspath("/"),
     )
```

### Comparing `openllm-0.1.8/src/openllm/_prompt.py` & `openllm-0.1.9/src/openllm/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/_schema.py` & `openllm-0.1.9/src/openllm/_schema.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/_service.py` & `openllm-0.1.9/src/openllm/_service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/_types.py` & `openllm-0.1.9/src/openllm/_types.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/cli.py` & `openllm-0.1.9/src/openllm/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,21 +184,21 @@
     help="Showing output type.",
     show_default=True,
     envvar="OPENLLM_OUTPUT",
     show_envvar=True,
 )
 
 
-def model_id_option(factory: t.Any, model_env: ModelEnv | None = None, click_type: click.ParamType | None = None):
+def model_id_option(factory: t.Any, model_env: ModelEnv | None = None):
     envvar = None
     if model_env is not None:
         envvar = model_env.model_id
     return factory.option(
         "--model-id",
-        type=click_type if click_type else click.STRING,
+        type=click.STRING,
         default=None,
         help="Optional model_id name or path for (fine-tune) weight.",
         envvar=envvar,
         show_envvar=True if envvar is not None else False,
     )
 
 
@@ -580,15 +580,15 @@
     @cog.optgroup.option(
         "--server-timeout",
         type=int,
         default=None,
         help="Server timeout in seconds",
     )
     @workers_per_resource_option(cog.optgroup)
-    @model_id_option(cog.optgroup, model_env=env, click_type=click.Choice(llm_config["model_ids"]))
+    @model_id_option(cog.optgroup, model_env=env)
     @cog.optgroup.option(
         "--fast",
         is_flag=True,
         default=False,
         help="Bypass auto model checks and setup. This option is ahead-of-serving time.",
     )
     @cog.optgroup.group("LLM Optimization Options.")
@@ -836,15 +836,15 @@
     )
 
     if output == "pretty":
         if not get_quiet_mode():
             _echo("\n" + OPENLLM_FIGLET, fg="white")
             if not _previously_built:
                 _echo(f"Successfully built {bento}.", fg="green")
-            else:
+            elif not overwrite:
                 _echo(
                     f"'{model_name}' already has a Bento built [{bento}]. To overwrite it pass '--overwrite'.",
                     fg="yellow",
                 )
 
             _echo(
                 "\nPossible next steps:\n\n"
@@ -1149,19 +1149,19 @@
             raise click.UsageError(
                 "Transformers version should be at least 4.29 to support HfAgent. "
                 "Upgrade with 'pip install -U transformers'"
             )
 
         _memoized = {k: v[0] for k, v in _memoized.items() if v}
 
-        client._hf_agent.set_stream(logger)
+        client._hf_agent.set_stream(logger.info)
         if output != "porcelain":
             _echo(f"Sending the following prompt ('{task}') with the following vars: {_memoized}", fg="magenta")
 
-        result = client.agent(task, agent_type=agent, return_code=False, remote=remote, **_memoized)
+        result = client.ask_agent(task, agent_type=agent, return_code=False, remote=remote, **_memoized)
         if output == "json":
             _echo(orjson.dumps(result, option=orjson.OPT_INDENT_2).decode(), fg="white")
         else:
             _echo(result, fg="white")
         return result
     else:
         raise click.BadOptionUsage("agent", f"Unknown agent type {agent}")
```

### Comparing `openllm-0.1.8/src/openllm/client.py` & `openllm-0.1.9/src/openllm/client.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/exceptions.py` & `openllm-0.1.9/src/openllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/__init__.py` & `openllm-0.1.9/src/openllm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/auto/__init__.py` & `openllm-0.1.9/src/openllm/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/auto/configuration_auto.py` & `openllm-0.1.9/src/openllm/models/auto/configuration_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/auto/factory.py` & `openllm-0.1.9/src/openllm/models/auto/factory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/auto/modeling_auto.py` & `openllm-0.1.9/src/openllm/models/auto/modeling_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/auto/modeling_flax_auto.py` & `openllm-0.1.9/src/openllm/models/auto/modeling_flax_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/auto/modeling_tf_auto.py` & `openllm-0.1.9/src/openllm/models/auto/modeling_tf_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/chatglm/__init__.py` & `openllm-0.1.9/src/openllm/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/chatglm/configuration_chatglm.py` & `openllm-0.1.9/src/openllm/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/chatglm/modeling_chatglm.py` & `openllm-0.1.9/src/openllm/models/chatglm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/dolly_v2/__init__.py` & `openllm-0.1.9/src/openllm/models/dolly_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/dolly_v2/configuration_dolly_v2.py` & `openllm-0.1.9/src/openllm/models/dolly_v2/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/dolly_v2/modeling_dolly_v2.py` & `openllm-0.1.9/src/openllm/models/dolly_v2/modeling_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/falcon/__init__.py` & `openllm-0.1.9/src/openllm/models/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/falcon/configuration_falcon.py` & `openllm-0.1.9/src/openllm/models/falcon/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/falcon/modeling_falcon.py` & `openllm-0.1.9/src/openllm/models/falcon/modeling_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/flan_t5/__init__.py` & `openllm-0.1.9/src/openllm/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/flan_t5/configuration_flan_t5.py` & `openllm-0.1.9/src/openllm/models/flan_t5/configuration_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/flan_t5/modeling_flan_t5.py` & `openllm-0.1.9/src/openllm/models/flan_t5/modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/flan_t5/modeling_flax_flan_t5.py` & `openllm-0.1.9/src/openllm/models/flan_t5/modeling_flax_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/flan_t5/modeling_tf_flan_t5.py` & `openllm-0.1.9/src/openllm/models/flan_t5/modeling_tf_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/gpt_neox/__init__.py` & `openllm-0.1.9/src/openllm/models/gpt_neox/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/llama/__init__.py` & `openllm-0.1.9/src/openllm/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/opt/__init__.py` & `openllm-0.1.9/src/openllm/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/opt/configuration_opt.py` & `openllm-0.1.9/src/openllm/models/opt/configuration_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/opt/modeling_flax_opt.py` & `openllm-0.1.9/src/openllm/models/opt/modeling_flax_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/opt/modeling_opt.py` & `openllm-0.1.9/src/openllm/models/opt/modeling_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/opt/modeling_tf_opt.py` & `openllm-0.1.9/src/openllm/models/opt/modeling_tf_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/roberta/__init__.py` & `openllm-0.1.9/src/openllm/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/stablelm/__init__.py` & `openllm-0.1.9/src/openllm/models/stablelm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/stablelm/configuration_stablelm.py` & `openllm-0.1.9/src/openllm/models/stablelm/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/stablelm/modeling_stablelm.py` & `openllm-0.1.9/src/openllm/models/stablelm/modeling_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/starcoder/__init__.py` & `openllm-0.1.9/src/openllm/models/starcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/starcoder/configuration_starcoder.py` & `openllm-0.1.9/src/openllm/models/starcoder/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/models/starcoder/modeling_starcoder.py` & `openllm-0.1.9/src/openllm/models/starcoder/modeling_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/playground/__init__.py` & `openllm-0.1.9/src/openllm/playground/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/playground/features.py` & `openllm-0.1.9/src/openllm/playground/features.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/playground/ft_opt_lora.py` & `openllm-0.1.9/src/openllm/playground/ft_opt_lora.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/utils/__init__.py` & `openllm-0.1.9/src/openllm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/utils/analytics.py` & `openllm-0.1.9/src/openllm/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/utils/codegen.py` & `openllm-0.1.9/src/openllm/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/utils/dantic.py` & `openllm-0.1.9/src/openllm/utils/dantic.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/utils/dummy_flax_objects.py` & `openllm-0.1.9/src/openllm/utils/dummy_flax_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py` & `openllm-0.1.9/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/utils/dummy_pt_and_einops_objects.py` & `openllm-0.1.9/src/openllm/utils/dummy_pt_and_einops_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/utils/dummy_pt_objects.py` & `openllm-0.1.9/src/openllm/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/utils/dummy_tf_objects.py` & `openllm-0.1.9/src/openllm/utils/dummy_tf_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/utils/import_utils.py` & `openllm-0.1.9/src/openllm/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm/utils/lazy.py` & `openllm-0.1.9/src/openllm/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm_client/__init__.py` & `openllm-0.1.9/src/openllm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm_client/_prompt.py` & `openllm-0.1.9/src/openllm_client/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm_client/runtimes/__init__.py` & `openllm-0.1.9/src/openllm_client/runtimes/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm_client/runtimes/base.py` & `openllm-0.1.9/src/openllm_client/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm_client/runtimes/grpc.py` & `openllm-0.1.9/src/openllm_client/runtimes/grpc.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/src/openllm_client/runtimes/http.py` & `openllm-0.1.9/src/openllm_client/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/tests/__init__.py` & `openllm-0.1.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/tests/test_configuration.py` & `openllm-0.1.9/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/tests/_strategies/__init__.py` & `openllm-0.1.9/tests/_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/tests/_strategies/_configuration.py` & `openllm-0.1.9/tests/_strategies/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/tests/models/flan_t5/__init__.py` & `openllm-0.1.9/tests/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/tests/models/flan_t5/test_modeling_flan_t5.py` & `openllm-0.1.9/tests/models/flan_t5/test_modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/tests/models/opt/__init__.py` & `openllm-0.1.9/tests/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/tests/models/opt/test_modeling_opt.py` & `openllm-0.1.9/tests/models/opt/test_modeling_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/tools/assert-model-table-latest` & `openllm-0.1.9/tools/assert-model-table-latest`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/tools/run-release-action` & `openllm-0.1.9/tools/run-release-action`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/tools/update-optional-dependencies.py` & `openllm-0.1.9/tools/update-optional-dependencies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/tools/update-readme.py` & `openllm-0.1.9/tools/update-readme.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/typings/attr/__init__.pyi` & `openllm-0.1.9/typings/attr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/typings/attr/exceptions.pyi` & `openllm-0.1.9/typings/attr/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/typings/attr/setters.pyi` & `openllm-0.1.9/typings/attr/setters.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/typings/attr/validators.pyi` & `openllm-0.1.9/typings/attr/validators.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/typings/click_option_group/__init__.pyi` & `openllm-0.1.9/typings/click_option_group/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/typings/click_option_group/_core.pyi` & `openllm-0.1.9/typings/click_option_group/_core.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/typings/click_option_group/_decorators.pyi` & `openllm-0.1.9/typings/click_option_group/_decorators.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/typings/click_option_group/_helpers.pyi` & `openllm-0.1.9/typings/click_option_group/_helpers.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/typings/deepmerge/merger.pyi` & `openllm-0.1.9/typings/deepmerge/merger.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/typings/deepmerge/strategy/core.pyi` & `openllm-0.1.9/typings/deepmerge/strategy/core.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/typings/deepmerge/strategy/set.pyi` & `openllm-0.1.9/typings/deepmerge/strategy/set.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/.gitignore` & `openllm-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/LICENSE.md` & `openllm-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/README.md` & `openllm-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 and model runtime, including StableLM, Falcon, Dolly, Flan-T5, ChatGLM,
 StarCoder and more.
 
 🔥 **Flexible APIs**: serve LLMs over RESTful API or gRPC with one command,
 query via WebUI, CLI, our Python/Javascript client, or any HTTP client.
 
 ⛓️ **Freedom To Build**: First-class support for LangChain, BentoML and
-HuggingFace that allows you to easily create your own AI apps by composing LLMs
+Hugging Face that allows you to easily create your own AI apps by composing LLMs
 with other models and services.
 
 🎯 **Streamline Deployment**: Automatically generate your LLM server Docker
 Images or deploy as serverless endpoint via
 [☁️ BentoCloud](https://l.bentoml.com/bento-cloud).
 
 🤖️ **Bring your own LLM**: Fine-tune any LLM to suit your needs with
@@ -338,22 +338,22 @@
 
 @svc.api(input=Text(), output=Text())
 async def prompt(input_text: str) -> str:
     answer = await llm_runner.generate(input_text)
     return answer
 ```
 
-### HuggingFace Agents
+### Hugging Face Agents
 
-OpenLLM seamlessly integrates with HuggingFace Agents.
+OpenLLM seamlessly integrates with Hugging Face Agents.
 
-> **Warning** The HuggingFace Agent is still at experimental stage. It is
+> **Warning** The Hugging Face Agent is still at experimental stage. It is
 > recommended to OpenLLM with
 > `pip install -r nightly-requirements.generated.txt` to get the latest API
-> update for HuggingFace agent.
+> update for Hugging Face agent.
 
 ```python
 import transformers
 
 agent = transformers.HfAgent("http://localhost:3000/hf/agent")  # URL that runs the OpenLLM server
 
 agent.run("Is the following `text` positive or negative?", text="I don't like how this models is generate inputs")
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 ## ð Introduction With OpenLLM, you can run inference with any open-source
 large-language models, deploy to the cloud or on-premises, and build powerful
 AI apps. ð **State-of-the-art LLMs**: built-in supports a wide range of
 open-source LLMs and model runtime, including StableLM, Falcon, Dolly, Flan-T5,
 ChatGLM, StarCoder and more. ð¥ **Flexible APIs**: serve LLMs over RESTful
 API or gRPC with one command, query via WebUI, CLI, our Python/Javascript
 client, or any HTTP client. âï¸ **Freedom To Build**: First-class support
-for LangChain, BentoML and HuggingFace that allows you to easily create your
+for LangChain, BentoML and Hugging Face that allows you to easily create your
 own AI apps by composing LLMs with other models and services. ð¯ **Streamline
 Deployment**: Automatically generate your LLM server Docker Images or deploy as
 serverless endpoint via [âï¸ BentoCloud](https://l.bentoml.com/bento-cloud).
 ð¤ï¸ **Bring your own LLM**: Fine-tune any LLM to suit your needs with
 `LLM.tuning()`. (Coming soon) ![Gif showing OpenLLM Intro](/assets/output.gif)
 ## ðâ Getting Started To use OpenLLM, you need to have Python 3.8 (or
 newer) and `pip` installed on your system. We highly recommend using a Virtual
@@ -114,19 +114,19 @@
 `generate` method that takes a string as a prompt and returns a corresponding
 output string. This will allow you to plug and play any OpenLLM models with
 your existing ML workflow. ```python import bentoml import openllm model =
 "opt" llm_config = openllm.AutoConfig.for_model(model) llm_runner =
 openllm.Runner(model, llm_config=llm_config) svc = bentoml.Service( name=f"llm-
 opt-service", runners=[llm_runner] ) @svc.api(input=Text(), output=Text())
 async def prompt(input_text: str) -> str: answer = await llm_runner.generate
-(input_text) return answer ``` ### HuggingFace Agents OpenLLM seamlessly
-integrates with HuggingFace Agents. > **Warning** The HuggingFace Agent is
+(input_text) return answer ``` ### Hugging Face Agents OpenLLM seamlessly
+integrates with Hugging Face Agents. > **Warning** The Hugging Face Agent is
 still at experimental stage. It is > recommended to OpenLLM with > `pip install
 -r nightly-requirements.generated.txt` to get the latest API > update for
-HuggingFace agent. ```python import transformers agent = transformers.HfAgent
+Hugging Face agent. ```python import transformers agent = transformers.HfAgent
 ("http://localhost:3000/hf/agent") # URL that runs the OpenLLM server agent.run
 ("Is the following `text` positive or negative?", text="I don't like how this
 models is generate inputs") ``` > **Note** Only `starcoder` is currently
 supported with Agent integration. The > example aboved was also ran with four
 T4s on EC2 `g4dn.12xlarge` If you want to use OpenLLM client to ask questions
 to the running agent, you can also do so: ```python import openllm client =
 openllm.client.HTTPClient("http://localhost:3000") client.ask_agent( task="Is
```

### Comparing `openllm-0.1.8/hatch.toml` & `openllm-0.1.9/hatch.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/pyproject.toml` & `openllm-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.8/PKG-INFO` & `openllm-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.1.8
+Version: 0.1.9
 Summary: OpenLLM: REST/gRPC API server for running any open Large-Language Model - StableLM, Llama, Alpaca, Dolly, Flan-T5, Custom
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: Issues, https://github.com/bentoml/openllm/issues
 Project-URL: Source, https://github.com/bentoml/openllm
 Author-email: Aaron Pham <aarnphm@bentoml.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
@@ -99,15 +99,15 @@
 and model runtime, including StableLM, Falcon, Dolly, Flan-T5, ChatGLM,
 StarCoder and more.
 
 🔥 **Flexible APIs**: serve LLMs over RESTful API or gRPC with one command,
 query via WebUI, CLI, our Python/Javascript client, or any HTTP client.
 
 ⛓️ **Freedom To Build**: First-class support for LangChain, BentoML and
-HuggingFace that allows you to easily create your own AI apps by composing LLMs
+Hugging Face that allows you to easily create your own AI apps by composing LLMs
 with other models and services.
 
 🎯 **Streamline Deployment**: Automatically generate your LLM server Docker
 Images or deploy as serverless endpoint via
 [☁️ BentoCloud](https://l.bentoml.com/bento-cloud).
 
 🤖️ **Bring your own LLM**: Fine-tune any LLM to suit your needs with
@@ -412,22 +412,22 @@
 
 @svc.api(input=Text(), output=Text())
 async def prompt(input_text: str) -> str:
     answer = await llm_runner.generate(input_text)
     return answer
 ```
 
-### HuggingFace Agents
+### Hugging Face Agents
 
-OpenLLM seamlessly integrates with HuggingFace Agents.
+OpenLLM seamlessly integrates with Hugging Face Agents.
 
-> **Warning** The HuggingFace Agent is still at experimental stage. It is
+> **Warning** The Hugging Face Agent is still at experimental stage. It is
 > recommended to OpenLLM with
 > `pip install -r nightly-requirements.generated.txt` to get the latest API
-> update for HuggingFace agent.
+> update for Hugging Face agent.
 
 ```python
 import transformers
 
 agent = transformers.HfAgent("http://localhost:3000/hf/agent")  # URL that runs the OpenLLM server
 
 agent.run("Is the following `text` positive or negative?", text="I don't like how this models is generate inputs")
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openllm Version: 0.1.8 Summary: OpenLLM: REST/gRPC
+Metadata-Version: 2.1 Name: openllm Version: 0.1.9 Summary: OpenLLM: REST/gRPC
 API server for running any open Large-Language Model - StableLM, Llama, Alpaca,
 Dolly, Flan-T5, Custom Project-URL: Documentation, https://github.com/bentoml/
 openllm#readme Project-URL: Issues, https://github.com/bentoml/openllm/issues
 Project-URL: Source, https://github.com/bentoml/openllm Author-email: Aaron
 Pham
 bentoml.com> License-Expression: Apache-2.0 License-File: LICENSE.md Keywords:
 AI,Alpaca,BentoML,Generative AI,LLMOps,Large Language Model,MLOps,Model
@@ -50,15 +50,15 @@
 ## ð Introduction With OpenLLM, you can run inference with any open-source
 large-language models, deploy to the cloud or on-premises, and build powerful
 AI apps. ð **State-of-the-art LLMs**: built-in supports a wide range of
 open-source LLMs and model runtime, including StableLM, Falcon, Dolly, Flan-T5,
 ChatGLM, StarCoder and more. ð¥ **Flexible APIs**: serve LLMs over RESTful
 API or gRPC with one command, query via WebUI, CLI, our Python/Javascript
 client, or any HTTP client. âï¸ **Freedom To Build**: First-class support
-for LangChain, BentoML and HuggingFace that allows you to easily create your
+for LangChain, BentoML and Hugging Face that allows you to easily create your
 own AI apps by composing LLMs with other models and services. ð¯ **Streamline
 Deployment**: Automatically generate your LLM server Docker Images or deploy as
 serverless endpoint via [âï¸ BentoCloud](https://l.bentoml.com/bento-cloud).
 ð¤ï¸ **Bring your own LLM**: Fine-tune any LLM to suit your needs with
 `LLM.tuning()`. (Coming soon) ![Gif showing OpenLLM Intro](/assets/output.gif)
 ## ðâ Getting Started To use OpenLLM, you need to have Python 3.8 (or
 newer) and `pip` installed on your system. We highly recommend using a Virtual
@@ -158,19 +158,19 @@
 `generate` method that takes a string as a prompt and returns a corresponding
 output string. This will allow you to plug and play any OpenLLM models with
 your existing ML workflow. ```python import bentoml import openllm model =
 "opt" llm_config = openllm.AutoConfig.for_model(model) llm_runner =
 openllm.Runner(model, llm_config=llm_config) svc = bentoml.Service( name=f"llm-
 opt-service", runners=[llm_runner] ) @svc.api(input=Text(), output=Text())
 async def prompt(input_text: str) -> str: answer = await llm_runner.generate
-(input_text) return answer ``` ### HuggingFace Agents OpenLLM seamlessly
-integrates with HuggingFace Agents. > **Warning** The HuggingFace Agent is
+(input_text) return answer ``` ### Hugging Face Agents OpenLLM seamlessly
+integrates with Hugging Face Agents. > **Warning** The Hugging Face Agent is
 still at experimental stage. It is > recommended to OpenLLM with > `pip install
 -r nightly-requirements.generated.txt` to get the latest API > update for
-HuggingFace agent. ```python import transformers agent = transformers.HfAgent
+Hugging Face agent. ```python import transformers agent = transformers.HfAgent
 ("http://localhost:3000/hf/agent") # URL that runs the OpenLLM server agent.run
 ("Is the following `text` positive or negative?", text="I don't like how this
 models is generate inputs") ``` > **Note** Only `starcoder` is currently
 supported with Agent integration. The > example aboved was also ran with four
 T4s on EC2 `g4dn.12xlarge` If you want to use OpenLLM client to ask questions
 to the running agent, you can also do so: ```python import openllm client =
 openllm.client.HTTPClient("http://localhost:3000") client.ask_agent( task="Is
```

